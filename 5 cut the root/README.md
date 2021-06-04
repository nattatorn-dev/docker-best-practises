Only copy what's needed. Avoid "COPY ." if possible

docker build -t docker5:1.0.0 -f ./Dockerfile .
docker run -d -p 3005:3000 --name docker5 docker5:1.0.0

http://localhost:3005

docker build -t docker5:1.0.0 -f ./Dockerfile.better .
docker run -d -p 3005:3000 --name docker5 docker5:1.0.0

http://localhost:3005