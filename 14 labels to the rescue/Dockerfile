FROM node:16-slim
LABEL maintainer="nattatorn.dev@gmail.com"
LABEL project="docker-best-practice"
LABEL com.example.version="0.0.1-beta"
LABEL vendor1="ACME Incorporated"
LABEL vendor2=ZENITH\ Incorporated
LABEL com.example.release-date="2015-02-12"
WORKDIR /usr/src/app

COPY package.json package-lock.json ./

RUN npm ci --production && npm cache clean --force

COPY ./src ./src

EXPOSE 3000

CMD [ "node", "src/index.js" ]
