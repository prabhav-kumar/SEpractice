docker ps -a
docker image ls
docker build -t eduassess-tomcat .
docker run -d -p 8080:8080 --name eduassess-container eduassess-tomcat
docker logs eduassess-container
docker run -d -p 8080:8080 -m 512m --name eduassess-container eduassess-tomcat
docker login
docker tag eduassess-tomcat myuser/eduassess-tomcat:latest
docker push myuser/eduassess-tomcat:latest
docker top eduassess-container
docker images
docker tag abc123def456 myuser/eduassess-tomcat:latest
docker pull python
docker run -it python bash

docker run -d --name my-nginx -p 8080:80 nginx
docker ps
