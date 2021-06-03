docker build -t docker2:1.0.0 -f ./Dockerfile .
docker run -d -p 3002:3000 --name docker2 docker2:1.0.0

http://localhost:3002

docker build -t docker2:1.0.0 -f ./Dockerfile.better .
docker run -d -p 3002:3000 --name docker2 docker2:1.0.0

http://localhost:3002