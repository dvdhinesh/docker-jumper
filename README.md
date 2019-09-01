# docker-jumper
A jumper from LB on Nginx to Web App on Apache


# Commands
##Single Image from Dockerfile
```
$ docker build -t php-on-apache .
$ docker run -d -p 80:80 -t --name web1 php-on-apache
$ docker ps
$ docker ps -a

$ docker stop web1
$ docker start web1

$ docker login
$ docker tag <IMAGE ID> dvdhinesh/php-on-apache:latest
$ docker push dvdhinesh/php-on-apache

$ docker images
$ docker rm web1
$ docker rmi <IMAGE ID>
```

##Multi Image from Docker Compose file
```
$ docker-compose up --build
$ docker-compose up -d
$ docker-compose stop
$ docker-compose rm
```

## Utility
```
$ docker exec -it <CONTAINER_ID> /bin/bash
```
