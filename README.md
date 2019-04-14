# Discovey Service

## Add maven dependency

```xml
<dependency>
	<groupId>org.springframework.cloud</groupId>
	<artifactId>spring-cloud-starter-netflix-eureka-server</artifactId>
</dependency>
```

## Enable discovery service

```java
@SpringBootApplication
@EnableEurekaServer
public class DiscoveryServiceApplication {

	public static void main(String[] args) {
		SpringApplication.run(DiscoveryServiceApplication.class, args);
	}

}
```

## Set properties

```properties
server.port=8761

spring.application.name=discovery-service

eureka.client.register-with-eureka=true
eureka.client.fetch-registry=true
```