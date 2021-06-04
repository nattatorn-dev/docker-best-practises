FROM alpine

RUN apk add nginx

COPY index.html /var/www/html/

EXPOSE 80

CMD ["nginx","-g","daemon off;"]

# After installing packages, often at times cache package files that were downloaded get stored and consume additional unnecessary space