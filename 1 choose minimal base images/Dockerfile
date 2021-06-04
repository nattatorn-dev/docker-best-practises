FROM alpine

WORKDIR /app

COPY package.json /app

RUN npm install

CMD ["node","index.js"]

# As some time you might also come across issues where choosing a lightweight image involves a trade-off with compatibility with the application and not having the needed dependencies or libraries need to run the application.
