FROM node:10

WORKDIR /nodeapp

COPY package.json ./

RUN npm install

COPY . .

EXPOSE 8888

CMD [ "node", "index.js" ]
