# API Testing Project - TestNG and RestAssured

## **Project Overview**
This project demonstrates **automated API testing** using **TestNG** and **RestAssured**. It performs **CRUD operations** (GET, POST, PUT, DELETE) on a mock REST API (https://jsonplaceholder.typicode.com). The tests verify that the API responses are correct by checking the **status codes**, **response bodies**, and **content types**.

## **Technologies Used**
- **Java** (JDK 8 or higher)
- **Maven** (Project Management Tool)
- **TestNG** (Testing Framework)
- **RestAssured** (API Testing Library)

## **Project Structure**
bash
.
├── pom.xml                      # Maven configuration file
├── src/
│   └── test/
│       └── java/
│           └── com/
│               └── vaish/
│                   └── a4/
│                       └── Assignment4/
│                           └── ApiTest.java    # API Test Class
└── resources/
    └── testng.xml               # TestNG Configuration File

## **Project Setup**

### **1. Prerequisites**
Ensure you have the following installed:
- **Java Development Kit (JDK)** installed (Version 8 or higher).
- **Maven** installed and configured.
- An IDE (e.g., IntelliJ IDEA, Eclipse, or VS Code).

### **2. Clone the Repository**
To clone the repository, run the following command in your terminal:

```bash
git clone https://github.com/your-username/API-Testing-Project.git
cd API-Testing-Project

## **Import the Project**
**Open your IDE (Eclipse).
Import the project as a Maven project.**
## **Build the Project**
**Navigate to the project directory and run the following command to build the project:
mvn clean install
Running the Tests
Option 1: Run Tests via IDE
Open the file ApiTest.java.
Right-click on the file or test method and select Run to execute the tests individually or as a suite.
Option 2: Run Tests via Maven
Run all tests using the Maven test goal:
mvn test
Option 3: Run Tests via TestNG
Navigate to the testng.xml file in the src/test/resources directory.
Right-click on testng.xml and select Run to execute the entire test suite.**

## **Key Test Cases**
-**GET Single Post
Verifies the response for a single post.
Validates the status code, response body, and content type.**
-**GET All Posts
Checks that a list of posts is returned and validates the response.**
-**POST New Post
Creates a new post and verifies the response.
Attempts to fetch the created post to validate its existence.**
-**Invalid Endpoint
Tests an invalid endpoint to ensure proper error handling.**
-**GET with Query Parameters
Filters posts based on query parameters and validate the response.**
## **Project Configuration**
**Maven Dependencies (pom.xml)
xml
Copy code
<dependencies>
    <dependency>
        <groupId>org.testng</groupId>
        <artifactId>testng</artifactId>
        <version>7.4.0</version>
        <scope>test</scope>
    </dependency>
    <dependency>
        <groupId>io.rest-assured</groupId>
        <artifactId>rest-assured</artifactId>
        <version>4.4.0</version>
    </dependency>
</dependencies>**

 
