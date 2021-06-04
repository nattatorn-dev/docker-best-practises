FROM alpine

RUN apk add --no-cache nginx ssh emacs

COPY index.html /var/www/html/

EXPOSE 80

CMD ["nginx","-g","daemon off;"]
