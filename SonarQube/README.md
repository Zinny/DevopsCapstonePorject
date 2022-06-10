https://hub.docker.com/_/sonarqube/




docker pull sonarqube:lts-community

Run below command to create the docker container for sonarqube:

-h, --hostname string Container host name -d, --detach Run container in background and print container ID

docker run --name sanarqube -h sonarqube -p 8084:9000 -d sonarqube

search sonarqube UI in your favourite browser

http://YOUR-IP:8084/

Then to stop the conatiner

docker stop sonarqube

Then to start the conatiner

docker start sonarqube

## TEST WEBHOOK 
