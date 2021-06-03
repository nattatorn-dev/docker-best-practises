FROM node:10-slim

WORKDIR /nodeapp

COPY package.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD [ "node", "index.js" ]

# 1 Ignore files & Directories which are not needed to be part of the image which will be built.
# 2 Avoid accidentally copying Sensitive data.