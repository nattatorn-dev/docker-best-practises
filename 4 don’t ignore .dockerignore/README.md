docker build -t docker4:1.0.0 -f ./Dockerfile .
docker run -d -p 3004:3000 --name docker4 docker4:1.0.0

http://localhost:3004
