# DevopsCapstonePorject# This is Demo Project post Advanced Devops Bootcamp - Nathan
 docker run --rm --group-add 0 -v //var/run/docker.sock:/var/run/docker.sock -v jenkins_docker_data:/var  -p 8080:8080 --name jenkins docker-in-docker-jenkins


docker run --rm --group-add 0 -v //var/run/docker.sock:/var/run/docker.sock --volume jenkins-data:/var  -p 8080:8080 --name jenkins docker-in-docker-jenkins
docker ps -a 
docker stop  ConatinerID
docker start ConatinerID


docker commit ConatinerID cinnyabraham06/NAME:TAG

docker rm ConatinerID
