docker build -t docker13:1.0.0 -f ./Dockerfile .
docker run -d -p 3013:3000 --name docker13 docker13:1.0.0

http://localhost:3013

docker build -t docker13:1.0.0 -f ./Dockerfile.better .
docker run -d -p 3013:3000 --name docker13 docker13:1.0.0

http://localhost:3013