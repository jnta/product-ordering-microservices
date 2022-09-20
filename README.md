# product-ordering-microservices

This is a sample Java / Maven / Spring Boot application, built with microservice-based architecture,
for control product ordering.

## Tech Stack

- Spring Boot
- Spring Cloud
- Spring Data JPA
- Spring WebFlux
- MySQL
- MongoDB
- Resilience4J

## About the Application

The application is a set of REST microservices and the system consists of the following modules:  

* **ms-api-gateway**: using Spring Cloud Gateway, that provides a simple way to route to APIs.
* **ms-discovery-server**:  a module that uses Spring Cloud Netflix Eureka as an embedded discovery server.
* **product-service**: a microservice that allows to perform CRUD operation on MongoDB repository of products.
* **order-service**: a microservice to perform CRUD operation on MySQL repository, that communicates with inventory-service.
* **inventory-service**: an inventory microservice that communicates with order-service, allowing or not the ordering.
It uses MySQL repository.





