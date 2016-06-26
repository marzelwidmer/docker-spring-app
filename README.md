**OSX**

***Create docker image***

`$ DOCKER_HOST=unix:///var/run/docker.sock mvn package docker:build `

***Show docker iamges***

`$ docker images`

***Start container***

`$ docker run -d -p 8080:8080 --name app1 spring-app/docker-spring-app`

***Test application***

http://http://localhost:8080/

***Start a second container***

`docker run -d --name app2 -p 8084:8080 keepcalm.ch/docker-spring-app`

***Test second application***

http://localhost:8084/


_docker run option_ :

`-d`
start background

`-p`
binding address

`--name`
set name

`{image prefix name}/{image name}`



***Show running docker processes***

`$ docker ps`

***Show stoped docker processes***

`$ docker ps -a`

***Start app1***

`$ docker start app1`

***Stop app1***

`$ docker stop app1`

***Delete all containers***

`$  docker rm $(docker ps -a -q)`

***Delete all images***

`$ docker rmi $(docker images -q)`