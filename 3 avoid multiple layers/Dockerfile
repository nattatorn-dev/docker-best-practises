FROM alpine

RUN apk update

RUN apk add curl

RUN apk add nodejs

RUN apk add nginx-1.16.1-r6

RUN apk add nginx-mod-http-geoip2-1.16.1-r6

COPY index.html /var/www/html/

EXPOSE 80

CMD ["nginx","-g","daemon off;"]

# Below is a Dockerfile that contains instruction where we install Nginx along with other utilities that are needed. 
# In the case of Dockerfile, each new line of instruction forms a separate layer.