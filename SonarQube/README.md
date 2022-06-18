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


Run Sonarqube Manually form locally 

download the sonarqube-jacoco-code-coverage repo and cd to sonarqube-jacoco-code-coverage directory

cinnyabraham06@instance-1:~/sonarqube-jacoco-code-coverage$ ls
README.md  build.gradle  docker-compose.yml  gradle  gradlew  gradlew.bat  settings.gradle  src

Run ./gradlew command 
./gradlew sonarqube   -Dsonar.projectKey=sonarqubetest   -Dsonar.host.url=http://34.105.75.10:8084   -Dsonar.login=XXXXXXXXXXXXXXXXXXXXXXXXXX



Download Sonar-scanner tool: 

wget https://binaries.sonarsource.com/Distribution/sonar-scanner-cli/sonar-scanner-cli-4.7.0.2747-linux.zip
   unzip sonar-scanner-cli-4.7.0.2747-linux.zip 
   cd sonar-scanner-4.7.0.2747-linux/
   d bin/
   ./sonar-scanner   -Dsonar.projectKey=sonar   -Dsonar.sources=.   -Dsonar.host.url=http://34.105.75.10:8084   -Dsonar.login=XXXXXXXXXXXXXXXXXXXX
   validate sonar UI and see if project executed and passed
