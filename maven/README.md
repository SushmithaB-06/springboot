Maven Basics
---------
What is Maven

Apache Maven is a build automation and dependency management tool for Java projects.

It mainly helps to:

Manage project dependencies (libraries)

Build the project

Maintain a standard project structure

Think of Maven as a project manager for Java applications.




Problem Maven Solves

Modern backend projects often use multiple technologies such as:

MySQL

Spring Boot

JSON libraries

Logging libraries

Without Maven:

Download many .jar files manually

Add them to the project

Manage versions

Resolve dependency conflicts

This quickly becomes complex and error-prone.





How Maven Solves It

Maven uses a configuration file called:

pom.xml

Dependencies are declared inside it.

Example:

<dependency>
    <groupId>com.mysql</groupId>
    <artifactId>mysql-connector-j</artifactId>
    <version>9.0.0</version>
</dependency>

Maven automatically:

Downloads required libraries

Adds them to the project

Handles version compatibility

So developers do not download jars manually.





POM File

pom.xml stands for:

Project Object Model

It contains:

Project metadata

Dependencies

Build configuration

Plugins

Maven reads this file and configures the project automatically.





Example Use Case

Connecting Java to MySQL

Without Maven:

Download MySQL connector

Add .jar manually

With Maven:

Add dependency in pom.xml:

<dependency>
  <groupId>com.mysql</groupId>
  <artifactId>mysql-connector-j</artifactId>
  <version>9.0.0</version>
</dependency>

Maven downloads and configures it automatically.




Why Companies Use Maven

Maven is widely used because it:

Manages dependencies efficiently

Automates project builds

Maintains a consistent project structure

Simplifies collaboration in teams

Frameworks like Spring Boot rely heavily on Maven.




Standard Maven Project Structure
project
 ├── src
 │   ├── main
 │   │   ├── java
 │   │   └── resources
 │   └── test
 └── pom.xml

This structure is followed in most professional Java projects.




Simple Analogy

Without Maven
→ Download libraries from multiple places manually.

With Maven
→ Declare dependencies once and Maven downloads everything automatically.
