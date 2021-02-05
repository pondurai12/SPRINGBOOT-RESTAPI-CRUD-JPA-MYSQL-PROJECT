# SPRINGBOOT-RESTAPI-CRUD-JPA-MYSQL-PROJECT
SPRINGBOOT REST CRUD OPERATION 

Technologies: JAVA,SPRINGBOOT,MYSQL
Tools Used: SPRING STS ,Xampp server,MySQL Db,POSTMAN.
Description: Web service for interview candidates ,we can create,read,update,delete candidates with name,skills,qualification.when  POST request candidate will save candidate table on interview database.on GET request retrieve all candidates.on PUT request update the particular candidate field data and on DELETE request delete candidate by id.CRUD operations done by JPA repository.


URLS:

GET http://localhost:8988/interview/candidates/

GET http://localhost:8988/interview/candidates/1

POST http://localhost:8988/interview/candidates/
 {
        "name": "pondurai",
        "emailid": "pdurai31@gmail.com",
        "skills": "corejava,spring,spring boot",
        "qualification": "BE"
    }

PUT http://localhost:8988/interview/candidates/4

 {
        "name": "pondurai",
        "emailid": "pdurai31@gmail.com",
        "skills": "corejava,spring,spring boot,spring mvc",
        "qualification": "BE-CSE"
    }

DELETE http://localhost:8988/interview/candidates/4


MYSQL QUERIES;

CREATE DATABASE interview;

CREATE TABLE candidate(
   ID INT PRIMARY KEY AUTO_INCREMENT,
   name VARCHAR (20) NOT NULL,
   emailid VARCHAR (20) NOT NULL,
   skills VARCHAR (20) NOT NULL,
   qualification VARCHAR (20) NOT NULL
);
