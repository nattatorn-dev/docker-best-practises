Only copy what's needed. Avoid "COPY ." if possible

docker build -t docker6:1.0.0 -f ./Dockerfile .
docker run -d -p 3006:3000 --name docker6 docker6:1.0.0

http://localhost:3006

docker build -t docker6:1.0.0 -f ./Dockerfile.better .
docker run -d -p 3006:3000 --name docker6 docker6:1.0.0

http://localhost:3006