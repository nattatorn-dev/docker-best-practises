docker build -t docker12:1.0.0 -f ./Dockerfile .
docker run -d -p 3012:3000 --name docker12 docker12:1.0.0

http://localhost:3012

docker build -t docker12:1.0.0 -f ./Dockerfile.better .
docker run -d -p 3012:3000 --name docker12 docker12:1.0.0

http://localhost:3012