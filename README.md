### spring-boot-experiments-
how to change port number? <br/>
if you change port number, write (server.port=3132) command on application.properties in src/main/resources/application.properties. you can change port number in applicaton.properties. 
``` 
server.port=8182
``` 
#### 1 - spring-boot-HelloWorld
how to run project. Look at application.properties where Port number is there. 
``` 
Links: 
    http://localhost:3092/    http://localhost:3092/welcome
```
#### 2 - spring-boot-view-JSP-File-1
How to use and view jsp file on spring boot
``` 
Links: 
http://localhost:8182/    http://localhost:8182/personels
```
#### 3 - spring-boot-view-Error-Page
How to use and view Error page on spring boot<br/>
you can writer anylink  except bottom links. you have to add to src/main/resources/public/error 404.html (error page)<br/>
if you write one of bottom links, you can't see error page as error.html
``` 
http://localhost:8182/    http://localhost:8182/personels
``` 
if you write one of bottom links, you can see error page as error.html
``` 
http://localhost:8182/deneme                           http://localhost:8182/asd        
http://localhost:8182/asdqwe/121243dqwe?c=asldkwqe     http://localhost:8182/deneme.jsp
```
#### 4 - springboot-(REST_API_QUERY) 
###### (Static)
how to use RequestMethod.POST, RequestMethod.PUT, RequestMethod.DELETE and RequestMethod.GET<br/>
you can experiment with JUNİT on PersonelClinicRestControllerTest.java  (src/test/java/com/javaegitimleri/app/web/) 
```   
You can try runnuing the methods with run as -> Junit Test in src/test/java/com/javaegitimleri/app/web/PersonelClinicRestControllerTest.java. 
Then you can look at changing data on localhost:8182/rest/personels
``` 
#### 5 - springboot-with-h2-database (REST_API_QUERY)  (jdbc with h2 database)
how to create schema, table and add data with jdbc in table. you can look src/main/resources/ data.sql & schema.sql.<br/>
how to use h2 database with jdbc.
``` 
Also You can try runnuing createPersonelTest, deletePersonelTest methods with run as -> Junit Test 
in src/test/java/com/javaegitimleri/app/web/PersonelClinicRestControllerTest.java.
``` 
#### 6 - springboot-jpa-with-h2-database (REST_API_QUERY)
how to use jpa with h2 database<br/>
how to use @Transactional, @Id, @GeneratedValue, @Entity, @Table @Column
#### 7 - springboot-simple-security-example
how to use login and logout procedure<br/>
how to use specific login page <br/>
how to use remember me for security login<br/>
First you have to add spring-boot-starter-security dependency file in pom.xml. <br/>
look at application.properties file in src/main/resources/...
``` 
#you can change username and password. then you can try login proccessing
spring.security.user.name=celal
spring.security.user.password=123456
``` 
#### 8 - SpringJPA-PostgreSQL-Example

first step
Open pdAdmin 4, use SQL Editor and make a query to create customer table in database called Personels
Also you can create any database called diffrent name.
``` 
CREATE TABLE customer(
    id BIGINT PRIMARY KEY     NOT NULL,
    firstname VARCHAR(20),
    lastname VARCHAR(20)
);
``` 
second step
``` 
you need to write localhost:8182/save.
you can try writing bottom any link
localhost:8182/findall
localhost:8182/findbyid?id=3  
localhost:8182/findbylastname?lastname=Terim
``` 
