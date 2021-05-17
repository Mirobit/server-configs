Alpine
docker exec -it cotainerID /bin/sh
Ubuntu
docker exec -it containerID /bin/bash

Listen netcap
netcat -l -p 8337

Send tcp per netcap
echo hello | nc ip port
nc ip port < file.txt
nc ip port -> next line enter

host.docker.internal -> host ip windows/mac
172.17.0.1 -> host ip linux

CTRL+P + CTRL+Q -> exit docker

docker scan --file Dockerfile topf-test

docker run -dit --name image-name -p 8081:8d000 containerid
docker run -dit --name bnm2 -p 8082:8000 .
docker run -ti tg /bin/sh -> replace CMD in Dockerfile with /bin/sh
docker run -d nameOfimage
docker start containerid
docker build -t getting-started . -> build from local dockerfile
docker run -dit -p 8080:8001 bnm2
docker run -d -p 8003:80 -v ${PWD}:/var/www/html php:7.4-apache -> ${PWD} or $(pwd)

docker rm containerid

docker stop $(docker ps -a -q) --> stop all container
FROM php:7.4-apache
COPY . /var/www/html
EXPOSE 80

