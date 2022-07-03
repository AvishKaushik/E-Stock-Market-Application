# E-Stock-Market-Application
A Stock Market Full Stack Application to register and check all the company details and related stocks to it.

This repository contains 3 different folders in order to explain in depth and technologies in application.
The given repositories are mentioned below:
1. Screenshot of working application
2. Frontend - Angular
3. Backend - Spring Boot Microservices

## Frontend :
Frontend contains the Angular developed part which performs all the basic functions as asked in the problem.


## Backend :
Backend contains 2 spring microservices which are deployed in AWS EC2 and there respective files have been uploaded to AWS S3. These backend applications are deployed as background services using docker on the AWS Cloud Platform.
Above that, Swagger UI latest version is used in order to interact with API without trobuling User to understand the functionalities by going through the code. Also, to confirm the working of the code, Junit tests have been implemented.
Company Service Link - http://ec2-18-236-208-88.us-west-2.compute.amazonaws.com:8080/swagger-ui/
Stock Service Link - http://ec2-18-236-113-219.us-west-2.compute.amazonaws.com:8080/swagger-ui/

For management and storing the data, MongoDB is used on AWS server to provide its features & services 24x7.
MongoDB URL - mongodb://ec2-18-236-208-88.us-west-2.compute.amazonaws.com:27017/
It contains database service which eventually contains 2 tables, i.e., company and stock for their respective purposes.

To run the application, run both the company-service and stock-service in the backend. To do that,either open the links provided above or follow the given steps:
1. Open cmd in respective service folder.
2. Type `mvn clean package` to create a jar file in target class
3. Type `cd target` in cmd to move to target folder
4. Type `java -jar <filename>.jar` where <filename> is the name of the .jar file [NOTE: There will be only one .jar file in target folder]
These steps will run the microservices in your localhost through which you can check the Springboot project functionalities.

To run the angular project in your respective machine, follow the steps :
1. Go to e-stock-market folder present in Frontend.
2. Open cmd in the same folder.
3. Type `npm install` to install the dependencies for the project
4. After completing installation, type `ng serve --open` to run the Angular project.


