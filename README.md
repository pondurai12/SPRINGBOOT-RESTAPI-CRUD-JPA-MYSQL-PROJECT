# SPRINGBOOT-RESTAPI-CRUD-JPA-MYSQL-PROJECT
SPRINGBOOT REST CRUD OPERATION 

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
