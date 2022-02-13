# Spring-Boot-Admin

Project created to monitor a Spring Boot application [Forum-Alura-Application](https://github.com/brunaellen/forum-project-springBoot-API-REST).

## Steps I followed to create the application:

1. Setup a simple boot project (using start.spring.io);
2. Added Spring Boot Admin Server starter and spring boot starter web to my dependencies within pom.xml;
3. Pulled in the Spring Boot Admin Server configuration via adding @EnableAdminServer to my configuration within SpringBootAdminApplication class;
4. Added the server port in which the application runs within aplication.properties file;

5. Added configurations to the client application to enable to monitoring it:
* Added Spring Boot Actuator to my client application;
* Added spring-boot-admin-starter-client to the dependencies within pom.xml;
* Enabled the SBA Client by configuring the URL of the Spring Boot Admin Server within aplication.properties file;