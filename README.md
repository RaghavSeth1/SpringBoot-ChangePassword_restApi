# SpringBoot-ChangePassword_restApi
********CHANGE PASSWORD REST API using SPRING BOOT , AWS , Tomcat Server**************************

RestAPI has been developed using Spring Boot and deployed on AWS Tomcat Server.

GIT Repo for Spring Boot basic GET project: https://github.com/RaghavSeth1/SpringBoot-ChangePassword_restApi 

URL to access the API deployed on AWS.Please note ,as this is public IP , Cant keep it on git , So I will share the IP on separate email.Please replace that below for <IP>
http://IP:8080/changePassword?oldPassword=Asdf1234@%23qwerttyy&newPassword=Blkh9876!@uirqrewq


- Please note that I have developed this API as GET API instead of POST as I would have to setup SQL DB on AWS which could have taken a little longer.

- I have created few of the test cases in POSTMAN for functionally validating the API. Please import below URL in your POSTMAN to run few of the GET request. Please note the test cases on POSTMAN are similar to JUNIT test.

- To IMPORT : Open POSTMAN--> Collection--> Import --> Link and paste below link.

- Postman: https://www.getpostman.com/collections/f3dc558ad280aed2e74a
- Please note this API code does not have logic to validate 80% similar password logic. That logic can be checked in other Junit project.

Please let me know in case of any issues.

Please find the attached test approach document for this requirement.
  
**How to Deploy on AWS:**
  - Build your jar in eclipse : mvn clean install --> Jar will be created in target foler.
  - Create t2.micro EC2 instance , Login using ssh key -->  Copy jar to EC2 instance (Ubuntu t2.micro) 
  - Login to Ubuntu Box --> Go to path where you have copied .jar
  - Run command: java -jar "Yourjarname".jar or to run in background: **nohup java -jar "Yourjarname".jar &**
