# Spring Boot Web Content Demo

A simple Spring Boot web application that demonstrates serving web content using Thymeleaf templates.

## Features

- Spring Boot web application
- Thymeleaf templating
- RESTful endpoint with request parameter handling
- Hot reload support with Spring DevTools

## Prerequisites

- Java 21
- Maven 3.9+

## Project Structure

```
src/
├── main/
│   ├── java/
│   │   └── com/
│   │       └── example/
│   │           └── demo/
│   │               ├── ServerWebContentApplication.java
│   │               └── GreetingController.java
│   └── resources/
│       ├── templates/
│       │   └── greeting.html
│       └── application.properties
```

## Quick Start

1. Clone the repository
2. Navigate to the project directory
3. Run the application:

```bash
./mvnw spring-boot:run
```

4. Open a browser and visit: http://localhost:8080/greeting

## API Endpoints

### Greeting Endpoint

```
GET /greeting
```

Query Parameters:
- `name` (optional) - Name to be displayed in greeting
  - Default value: "World"

Example:
```
http://localhost:8080/greeting?name=John
```

## Technologies

- [Spring Boot](https://spring.io/projects/spring-boot) 3.5.4
- [Thymeleaf](https://www.thymeleaf.org/)
- [Spring Web MVC](https://docs.spring.io/spring-framework/reference/web/webmvc.html)
- [Spring DevTools](https://docs.spring.io/spring-boot/docs/current/reference/html/using.html#using.devtools)

## Development

The project uses Spring Boot DevTools which enables:
- Automatic restart when code changes
- Live reload
- Property defaults optimization

## Building

To build the project:

```bash
./mvnw clean install
```

The built JAR will be in `target/demo-0.0.1-SNAPSHOT.jar`