# Section 1: Spring Boot Overview
## What is JVM? JRE? and JDK?
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

