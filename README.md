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


docker-compose up -d
docker network inspect edu_network
docker exec -it mysql-db bash
mysql -u edu_user -p

USE edu_assess_db;

CREATE TABLE ExamResults (
    id INT AUTO_INCREMENT PRIMARY KEY,
    student_id INT NOT NULL,
    exam_date DATE NOT NULL,
    score DECIMAL(5, 2) NOT NULL,
    subject VARCHAR(255) NOT NULL
);

EXIT;
exit
