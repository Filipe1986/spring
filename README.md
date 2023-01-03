# Spring

![framwwork](spring-framework.png)

Eco system

![framwwork](spring-framework.png)

### Inversion Of Control (IOC) and Dependency Injection (DI)
IOC container is responsible to inject the dependency. 

Dependency Injection:

* makes the code loosely coupled so easy to maintain
* makes the code easy to test

## Spring boot
- Spring boot favours convention over configuration to get an application up and running as quickly as possible.
- Opinionated means - established standards and popularity.
- A developer can overwrite any of the choices anytime.


### Annotations:
* @SpringBootApplication includes 
    {@Configuration, @ComponentScan, @EnableAutoConfiguration}
* @EnableAutoConfiguration 
    {tomcat, dispatcher server, MVC}
* @ConfigurationProperties maps properties to a @Component