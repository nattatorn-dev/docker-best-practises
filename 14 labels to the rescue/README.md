### There’s lots of different use case for labels, including, but not limited to the following:

- you can label an image with git commit from which it was built;
- labels can be used for organizing your images: you can label images from different projects using their project name as the label value;
- you can label images containing different components (Java application, tools, database, proxy server, etc.) — also, for organizing stuff;
- you can label containers, created from the same image, with different labels, e.g. primary and secondary nodes.

ref: 
- https://docs.docker.com/develop/develop-images/dockerfile_best-practices/#label


docker build docker14:1.0.0 -f ./Dockerfile .

docker run -d -p 3014:3000 --name docker14 docker14:1.0.0

http://localhost:3014

docker inspect --format='{{.Config.Labels.maintainer}}' docker14
docker ps --all --filter label=project=docker-best-practice
