# School Web Application

This is a Maven-based web application for a school. The project is structured to build a .war package for deployment on a servlet container.

## Project Structure

```
school-webapp
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── school
│   │   │           └── App.java
│   │   ├── resources
│   │   │   └── application.properties
│   │   └── webapp
│   │       ├── WEB-INF
│   │       │   └── web.xml
│   │       └── index.jsp
│   └── test
│       └── java
│           └── com
│               └── school
│                   └── AppTest.java
├── pom.xml
└── README.md
```

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- Apache Maven 3.6 or higher

## Building the Project

To build the project and create the .war package, navigate to the project root directory and run the following command:

```
mvn clean package
```

This will compile the source code, run tests, and package the application into a .war file located in the `target` directory.

## Running the Application

Once the .war file is built, you can deploy it to a servlet container such as Apache Tomcat. Place the .war file in the `webapps` directory of your Tomcat installation and start the server.

Access the application by navigating to `http://localhost:8080/school-webapp` in your web browser.

## Configuration

Configuration properties can be set in the `src/main/resources/application.properties` file. This file can include settings such as database connection details and server port.

## Testing

Unit tests for the application can be found in the `src/test/java/com/school/AppTest.java` file. You can run the tests using the following command:

```
mvn test
```

## License

This project is licensed under the MIT License. See the LICENSE file for more details.