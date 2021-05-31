FROM node:10-slim

WORKDIR /app

COPY package.json ./

RUN npm install

COPY . .

EXPOSE 8888

CMD [ “node”, “index.js” ]

# Every image that we built using docker has default user as root well that is a security evil 
# we don’t need the user for the images to be root, as we can specify a default user with all the minimal permission needed for the application to function inside of the container