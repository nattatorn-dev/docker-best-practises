docker build -t docker4:1.0.0 -f ./Dockerfile .
docker run -d -p 3000:3000 --name docker4 docker4:1.0.0
