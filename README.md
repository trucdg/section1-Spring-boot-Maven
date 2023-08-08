# Section 1: JVM-JRE-JDK, Spring, Spring Boot and Maven
# 🌺 What is JVM? JRE? and JDK?
Resource: [Differences between JVM vs JRE vs JDK](https://byjus.com/gate/difference-between-jdk-jre-and-jvm/#:~:text=The%20JDK%20is%20an%20abbreviation,that%20develops%20applications%20in%20Java.)
1. [JVM - Java Virtual Machine](https://github.com/trucdg/java-virtual-machine):
   - Provides Runtime Environment in which Java bytecode can be executed.
   - Tasks of JVM:
     - Loads code
     - Verifies code
     - Executes code
     - Provides Runtime Environment
   - JVM doesn't exist physically, or to be more exact, tangibly. JVM is constructed in RAM, not in memory like JRE and JDK.
>Note: 
> - **Java is platform independent** while **JVM, JRE, and JDK are platform dependent.**
> - java is platform independent because java doesn't run directly on the operating system. It runs on the JVM which you have to install separately. The use of the same byte code for all JVMs on all platforms make the java language platform independent.

2. JRE = JVM + Set of Libraries:
- It is the implementation of JVM
- To run any Java code, JRE is the mimum required.
- JRE contains set of libraries that JVM uses at runtime
- JRE 'physically' exists.
- JRE is platform dependent

3. JDK = JRE + Development Tools:  
- The **Java Development Kit (JDK)** is a cross-platformed software development environment that offers a collection of tools and libraries necessary for developing Java-based software applications and applets.
- It is a core package used in Java, along with the **JVM (Java Virtual Machine)** and the **JRE (Java Runtime Environment)**.
- Beginners  often get confused with JRE and JDK, if you are only interested in running Java programs on your machine then you can easily do it using Java Runtime Environment. However, if you would like to develop a Java-based software application then along with JRE you need some additional tools, which is called JDK.
- Development Tools examples: Java debugger + Java compipler + JavaDoc

![image](https://github.com/trucdg/section1-SpringBoot3-intro/assets/91285203/4f606138-4538-40e1-84c4-c4916dc26480)

## ☃️ Spring and Spring Boot:
1. What is Spring?
   - Simply put, the Spring framework provides comprehensive infrastructure support for Java applications.
   - Spring is packed with some nice features like Dependency Injection, and out of the box modules like:
        - Spring JDBC (Spring Java Database Connectivity)
        - Spring MVC (Spring Model View Controller)
        - Spring AOP (Aspect-Oriented Programming)
        - Spring ORM (Object-Relational Mapping)
     ... etc.
2. What is Spring Boot?
   - Spring Boot is built on top of the conventional Spring framework. So, it provides all the features of spring and is yet easier to use than spring.
   - Some features in Spring Boot:
     - Opinionated 'starter' dependencies to simplify the build and application configuration
     - Embedded server to avoid complexity in application deployment
     - Automatic config. for Spring functionality - whenever possible

### Difference between Spring MVC and Spring Boot
1. **Spring MVC**:
   - Spring is widely used for creating scalable applications.
   - For web applications, Spring provides Spring MVC framework which is a module of spring, used to create scalable web applications.
   - Spring MVC framework enables the separation of modules, namely Model, View, and Controller.
   - The model object can be passed between View and Controller using maps.
   - The Spring MVC framework consists of the following components:
      - **Model** - a model can be an **object** or **collection of objects**, which basically contains the data of the application
      - **View** - a view is used for displaying the information to the user in a specific format.
      - **Controller** - contains the logical part of the application
        `@Controller` annotation is used to mark that class as a controller.
      - **Front Controller** - is responsible for managing the flow of the web application. **Dispatcher Servlet acts as a front controller in Spring MVC/
    
2. **Spring Boot**:
   - In Spring Boot, everything is auto-configured. We just need to use proper configuration for utilizing a particular functionality.
   - Spring Boot is very useful if we want to develop REST API.
   - There are 4 main layers in Spring Boot:
      - **Presentation Layer** - it consists of the view (front-end part)
      - **Data Access Layer** - CRUD operations on the database comes under this category.
      - **Service Layer** - consists of service classes and uses services provided by data access layer
      - **Integration Layer** - consists of different web services

## What is Maven?
- Maven is a project management tool.
- Most popular use of Maven is for build management and dependencies.
- Maven downloads the JAR files (Spring JAR files, Hibernate JAR files, etc) needed for our projects and make those JAR files available during compile/ run.

### Maven Project Structure:



















