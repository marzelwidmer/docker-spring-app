**OSX**

Create Docker Image
`$ DOCKER_HOST=unix:///var/run/docker.sock mvn package docker:build `

Show Docker Iamges
`$ docker images`

Start Container
`$ docker run -d -p 8080:8080 --name app1 spring-app/docker-spring-app`

run option :
`-d start background
-p binding address
--name set name`

Show running Docker processes
`$ docker ps`

Show stoped Docker processes
`$ docker ps -a`

Start app1
`$ docker start app1`

Stop app1
`$ docker stop app1`

Delete all containers
`$  docker rm $(docker ps -a -q)`

Delete all images
`$ docker rmi $(docker images -q)`