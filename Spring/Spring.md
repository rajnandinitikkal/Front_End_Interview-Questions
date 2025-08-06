## What is a Library ?
- A collection of predefined methods, classes or interfaces used for solving common problem.
- Library is the collection of multiple packages
- come either bundled with a language or can be downloaded from the internet and used.

- Examples of libraries -
- Standard libraries: java.lang, java.util. java.io
- 3rd party Libraries : apache commons, twilio, iText

Benefits :
1) Reusability
2) Reduces Programmer's effort
3) Allow a programmer to focus on main problem

eg, ReactJs but it also consider as framework

## What is Framework ?

- Collection of multiple libraries.
- Provides foundation on which we can build our code.
- It provides pre-written common logics so that we can focus on business logic only.
- Provides reusable components.

eg. Spring

Benefits:
- Seeds up development precess
- Secure
- Forces us to follow standard programming practices and thus make our code clean.

### Types of framework
- Front Enf framework :Angular
- WEB Framework was: STRUCTS But is is oudated and spring is now in demand
- Application dev framework: Spring Framework
- ORM Framework: HILBERNATE

## Library vs Framework

- Libraries are focused to a specific task only while a framework has a wide range of functionality and used to build complete application.

- our code calls the library, while in case of framework it calls our code.

## Web Application Architecture

 USER INTERFACE (Front End Application) --> WEB LAYER = BUSINESS LAYER = DAO (Code for DB Access) --> DATABASE

## What Is Spring Framework ?

- Spring is the most popular java framework for building any type of java application.
- Spring is free & open framework handled by VMware
- Spring is developed in modular fashion
  - Modules in spring (there are 21 modules of spring)
  - spring cloud
  - spring social
  - spring JDBC
  - spring core (most recommend to learn it first)
- Commonly used as backend.

# Spring

## Advantages of Spring
- Frameworks of framework
- Loose Coupling (Use/connect more than one class), Dependency Injection, Inversion of control
- Simplified development
- Easy Integration (it integrate with other libaries and framework like react, hibernate, Angular, Thymly)
- Secure (spring secure module)
- Stable and lots of resources

Official website 
` spring.io `

## History of Spring

- Spring is versatile framework which can be used to develop any type of application
- First production is march 2004 1.0 version 

## Spring imp Modules

1) Spring core
2) Spring context
3) Spring JDBC
4) Spring ORM
5) Spring Data JPA
6) Spring Web MVC
7) Spring Rest
8) Spring Batch
9) Spring Boot
10) Spring AOP
11) Spring Security
12) Spring Cloud

## Spring Core

- Spring core is the base module in the Spring Framework.
- Its provide fundamental concepts of spring framework
- Two imp concepts given by spring core
1) IOC : Inversion of control
2) DI : Depenjency Injection

## Spring context

- Spring context helps us to set up configurations.
- Configuration means informing the spring Framework that which classes we went the spring/IOC container to mange for us.

## Spring JDBC

- Spring JDBC is used to simplyfy our database communication logic.

- In pure JDBC we need to write boiler plate code (repeated code) like below in several classes.
  1) Load Driver
  2) Get Connection
  3) Create statement
  4) Execute Query
  5) Process Result
  6) Close Connection

  - However using spring JDBC we only have to perform step 4 & 5 and the remaining steps are taken care of automatically.

## Spring ORM

- Object Relational Mapping
- Spring ORM is used to integrate ORM Framework like Hilbernate within the spring Environment.
- The benefit of ORM is taht allows us to represent table as java classes and the table data as java objects rather than rows.

## Spring Data JPA
- JPA: Java Persistent API

- Spring Data JPA is an extension to ORM
- It makes our DB Integration super easy
- This is because it provides us readymade to perform CRUD operation.

## Spring WEB MVC
- (Learn servlet before learning mvc)
- Spring Web MVC is used to develop both web Application as well as Distributed application.

- Web Applications: Those apps which are accessed by users using their browsers like gmail, facebook, Instagram etc.

- Distributed Application: Those apps that run on multiple computers simultaneouly and are designed by users from different devices and locations eg, Banking Applications.

## Spring REST
- Reprentational State TRansfer
- Spring Rest, focuses on building RESTful web services.
-  REST stands for Representational State Transfer, and it is an architectural style for designing distributed applications.

## Spring Batch
- The term Batch means Bulk Operations
    - for eg, Reading and storing multiple records in the database
    - Monthly account statements sent by bank to its customers
    - Sending SMS to students about new course launch
- To handle all such operation the spring framework provides us a module called spring Batch.

## Spring Boot
 
- Spring boot is an extension/module of spring Framework
- It provides the ability to create spring applications taht can run immediately without writing lots of additional code.
- The biggest advantage of using Spring boot versus Spring Framework is the ease of use and Faster development.

## Spring AOP

- AOP: Aspect Oriented Programming
- Just like POP and OOP it is also a methodology or approach
- It allows us to seprate the cross cutting logics in an application.

- The word cross cutting logics means secondary logics in an application like security , Trnsaction management, logging, exception handling etc.


## Spring Security

- Spring is the most crucial part of any application.

- And the spring security module helps us to acheive security in out spring application

- Using Spring security we can implement both Authentication and Authorization(Data validation/ permission) in out programs.

- Iy also provides us single sign on feature as well as protection against attacks like csrf, session fixation etc.

## Spring cloud

- Spring cloud provides us configuration for microservices

- Microservices is an architecture that allows us to break down a single large application into smaller and independently deployable services.








