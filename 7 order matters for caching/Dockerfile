FROM alpine

COPY index.html /var/www/html/

RUN apk add --no-cache nginx ssh emacs

EXPOSE 80

CMD ["nginx","-g","daemon off;"]
