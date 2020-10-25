# Spring Security Demo

A spring security demo application with form based authentication, user roles, accounts, csrf protection, and more.

## Technology
Java 8+  
Spring Boot 2.3.4  
Maven  
Thymeleaf  
Guava
  
## Installation

Start a new project from version control using IntelliJ or another java IDE and checkout from this repository.

## Dependencies

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-security</artifactId>
</dependency>

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-thymeleaf</artifactId>
</dependency>

<dependency>
    <groupId>com.google.guava</groupId>
    <artifactId>guava</artifactId>
    <version>28.1-jre</version>
</dependency>

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-test</artifactId>
    <scope>test</scope>
    <exclusions>
        <exclusion>
            <groupId>org.junit.vintage</groupId>
            <artifactId>junit-vintage-engine</artifactId>
        </exclusion>
    </exclusions>
</dependency>
```

## Usage

Run the application. Travel to [localhost:8080](https:/localhost:8080) to view the index.hml available to all users.

Traveling to other destinations found in the TemplateController will require a login.

The Management API is accessible by users with the following roles: ROLE_ADMINTRAINEE, ROLE_ADMIN

The Student API is accessible by users with the following roles: ROLE_STUDENT

Demo login information can be found under ApplicationSecurityConfig.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)