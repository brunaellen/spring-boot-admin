# Spring-Boot-Admin

Project created to monitor the Spring Boot application [Forum-Alura-Application](https://github.com/brunaellen/forum-project-springBoot-API-REST).

### Application was made using:

* Spring Boot 2.6.1
* Java 11
* maven

## Endpoint

* GET /applications/

## Steps I followed to create the application: 
[Check Spring Boot Admin Reference Guide Here](https://codecentric.github.io/spring-boot-admin/2.4.3/)

1. Setup a simple boot project (using start.spring.io);
2. Added Spring Boot Admin Server starter and spring boot starter web to my dependencies within pom.xml; [check this step here](https://github.com/brunaellen/spring-boot-admin/blob/master/pom.xml)

3. Pulled in the Spring Boot Admin Server configuration via adding @EnableAdminServer to my configuration within SpringBootAdminApplication class; [check this step here](https://github.com/brunaellen/spring-boot-admin/commit/79e7c2d383528529b7be7aabd9459a69e8d65055)


4. Added the server port in which the application runs within aplication.properties file; [check this step here](https://github.com/brunaellen/spring-boot-admin/commit/f577c184b8cbce84dc208d3101cb524f767faf83)

5. Added configurations to the client application to enable to monitoring it:
[Check Client Application here](https://github.com/brunaellen/forum-project-springBoot-API-REST)

* Added Spring Boot Actuator to my client application;
<br/>

5.1. Added spring-boot-starter-actuator to dependencies and made the /actuator/ endpoint accessible; [check this step here](https://github.com/brunaellen/forum-project-springBoot-API-REST/commit/415d62e0f549749094bea8b2a05f6141e13ae96c)<br/> 

5.2. Added actuator configuration [check this step here](https://github.com/brunaellen/forum-project-springBoot-API-REST/commit/83f6add3731fc60ce16063c8ef2f92f029d116e4)<br/>

5.3. Added spring-boot-admin-starter-client to the dependencies within pom.xml; [check this step here](https://github.com/brunaellen/forum-project-springBoot-API-REST/commit/0456b26a6b2a97df3e108e526dc74f39f7291019)

5.4. Enabled the SBA Client by configuring the URL of the Spring Boot Admin Server within aplication.properties file; [check this step here](https://github.com/brunaellen/forum-project-springBoot-API-REST/commit/7c9c2b118a4ccf967b60c0388a097d8062796d87)