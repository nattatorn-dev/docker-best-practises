FROM node:16-slim

WORKDIR /nodeapp

COPY package.json package-lock.json ./

RUN npm ci --production && npm cache clean --force

COPY ./src ./src

EXPOSE 3000

CMD [ "node", "src/index.js" ]
