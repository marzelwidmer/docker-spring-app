**OSX**

Create Docker Image
`$ DOCKER_HOST=unix:///var/run/docker.sock mvn package docker:build `

Show Docker Iamges
`$ docker images`

Push to Cloud https://cloud.docker.com/
`$ docker push spring-app/docker-spring-app         `




Delete all containers
`$  docker rm $(docker ps -a -q)`

Delete all images
`$ docker rmi $(docker images -q)`