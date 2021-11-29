# Articles API
Part of a tutorial on [My Day To-Do Blog], this is a REST API that exposes endpoints to create and retrieve articles. 

## Background 
This is a simple repository that aims to highlight "how-to" achieve building a REST API with Spring Boot, with implementations of both an in-memory datastore (cache) as well as a persistent data store.

### Caching Solution
This is a simple solution where by all the incoming data is saved into an [ArrayList] of Article Objects. The cache (ArrayList) is an in-memory data store that exists for the app's run time. The cache is highly volatie and all data is lost on application restart.

### Persistent database solution
A more versatile solution where the data is stored and retrieved from a relational database that persists data to disk. This offers the advantage of the app retaining data between application restarts. The database used is an in-memory database called [H2 Database] which has the option to persist the data on disk via setting it to file based storage. To know more about how to work with H2 Database in Spring, have a read of [Spring Boot With H2 Database].

## Technologies used
- Java 11
- Spring Framework (Spring Boot, JUnit)
- H2 database
- Maven 

## Project setup
To run and modify the project start by installing the prequisite software, followed by cloning the repository and performing the seps listed.
### Prequisite software
Install the following software on your machine to later use from command line.
1. [Java 11]
2. [Maven]
3. [VS Code], [Eclipse] or IDE of your choice?

### Repository setup
1. Clone the repository 
2. Launch the terminal
3. Navigate to the project directory
4. Install the dependant libraries dependant and run the project,
```sh
mvn install
//build by 
mvn package
//run by 
mvn spring-boot:run
//run tests by 
mvn test
```
5. Once the project is running
6. Launch the browser and enter
```sh
http://localhost:8080/all
```
The above url will show all the articles that are added on application startup to the local cache.
If you want to improve the code by making changes to it, then either import it as an existing maven project in Eclipse or simply open the folder in Visual Studio Code. 

## Code structure

> To be added...

# More great tutorials and code samples
Checkout [this blog] for more "how-to" code samples, tutorials and just info on how to solve problems.

If you like what I am doing, you can [buy me a coffee]

Click on the next link for more info on the 13+ year [software engineering career journey] of the author.


[software engineering career journey]: https://mydaytodo.com/the-3-stages-of-a-software-engineering-career/
[this blog]: https://mydaytodo.com/blog/
[Java 11]: https://www.oracle.com/au/java/technologies/javase-jdk11-downloads.html
[Maven]: https://maven.apache.org/
[VS Code]: https://code.visualstudio.com/
[ArrayList]: https://docs.oracle.com/javase/8/docs/api/java/util/ArrayList.html
[Eclipse]: https://www.eclipse.org/
[H2 Database]: https://www.h2database.com/html/main.html
[Spring Boot With H2 Database]: https://www.baeldung.com/spring-boot-h2-database
[My Day To-Do Blog]: https://mydaytodo.com/blog
[buy me a coffee]: https://www.buymeacoffee.com/bhumansoni
