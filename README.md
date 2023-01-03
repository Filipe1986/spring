# Spring


<img src="https://github.com/Filipe1986/spring/blob/main/images/spring-framework.png" width="500">

Eco system

<img src="https://github.com/Filipe1986/spring/blob/main/images/Spring%20Ecosystem.png" width="500">


### Inversion Of Control (IOC) and Dependency Injection (DI)
IOC container is responsible to inject the dependency. 

Dependency Injection:

Dependency Injection is a *design pattern* that allows the spring container to ‘inject’ objects into other objects.

The control of creating objects and managing the spring components is taken care of by the Spring containers.


* makes the code loosely coupled so easy to maintain
* makes the code easy to test

## Spring boot
- Spring boot favours convention over configuration to get an application up and running as quickly as possible.
- Opinionated means - established standards and popularity.
- A developer can overwrite any of the choices anytime.


### Annotations:
* @SpringBootApplication includes 
    {@Configuration, @ComponentScan, @EnableAutoConfiguration}

``` Java
import org.springframework.boot.SpringApplication;

@SpringBootApplication
public class Application {

    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }

}
```
* @EnableAutoConfiguration 
    {tomcat, dispatcher server, MVC}

* @ConfigurationProperties maps properties to a @Component


application.properties file:

```
mail.hostname=host@mail.com
mail.port=9000
mail.from=mailer@mail.com
```

``` Java
@ConfigurationProperties(prefix = "mail") 
public class ConfigProperties { 

    private String hostName; 
    private int port; 
    private String from; 

}
```