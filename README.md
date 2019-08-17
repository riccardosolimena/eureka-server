# Getting Started
This repo is part of teaching presented on Udemy Platform by [Udemy.com/riccardo-solimena](https://www.udemy.com/user/riccardo-solimena/).
For info and question contact me on [riccardo.solimena@gmail.com](mailto:riccardo.solimena@gmail.com).

### What this project does
This is an application that works as a simple eureka-server using Spring Cloud Eureka

### How to use it
Download the project and run the application. The application is configured The default port is 8761 as designed for Eureka Server applications.
In the application.properties file is possible to configure the port and the application name. For multiple instances is important to change on true the registration and add the replicas' names as follows 
```
eureka.client.fetch-registry=true
eureka.client.register-with-eureka=true
eureka.client.service-url.defaultZone=http://server1:port1/eureka/,http://server1:port2/eureka/
```
where "serverN" means the DNS name or ip and "portN" respectively the port number of the replicas' servers.

### Reference Documentation
For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)

### Guides
The following guides illustrate how to use some features concretely:

* [Service Registration and Discovery](https://spring.io/guides/gs/service-registration-and-discovery/)

* [Spring Cloud Netflix](https://cloud.spring.io/spring-cloud-netflix/reference/html/)

* [Spring Cloud Eureka Server](https://cloud.spring.io/spring-cloud-netflix/multi/multi_spring-cloud-eureka-server.html)