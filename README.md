﻿# property-management-system
# property-management

## Project Design

![project-design](property-management.png)

### DTO
Data transition object, an object that carries data between processes.

Ref: https://en.wikipedia.org/wiki/Data_transfer_object

### controller
In this design, works as a listener/server to wait and accept API calls from externals. When a call is received, controller will pass the DTO to the corresponding service.

### service
Service is responsible for handling the request from the controller. It is the logics that does the actual work of fetching data.

### repository
Data access layer in Spring boot to connect to DB for reading and writing data.

Ref: https://docs.spring.io/spring-data/data-commons/docs/1.6.1.RELEASE/reference/html/repositories.html

### DB
Data storage.
In this project, used h2 DB for local environment and SQL for other environments.

## Project management
### Maven
Used Maven as the project management for this project. Dependencies are defined in pom.xml file.

Ref: https://maven.apache.org/

### Dependencies
Spring boot
Swagger
H2 DB
SQL DB
