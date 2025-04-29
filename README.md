# S4.01-Spring-Nivel3

Testing Spring Boot Projects with Postman
This document outlines how to test the Maven and Gradle Spring Boot projects using Postman environments.

## Prerequisites
- Maven Spring Boot project running on port 9000.
- Gradle Spring Boot project running on port 9001.
- Postman application installed.

## Postman Environments

-- Two Postman environments are provided (exported as JSON files):

- Proyect Maven.postman_environment.json: Contains variables for testing the Maven project.

Servidor: http://localhost
Port: 9000

- Proyect Gradle.postman_environment.json: Contains variables for testing the Gradle project.

Servidor: http://localhost
Port: 9001

-- To import these environments into Postman:

- Open Postman.
- Click on the "Environment" quick look (eye icon) in the top right corner.
- Click on "Import".
- Select the downloaded JSON environment files.

## Testing the API Endpoints

Ensure that both the Maven and Gradle Spring Boot applications are running in Eclipse. You can then use Postman with the respective environments to test the API endpoints.

- Testing the Maven Project:

Select the "Proyecto Maven" environment in Postman.
Send a GET request to the following URLs (examples):
{{Servidor}}:{{Port}}/HelloWorld?nombre=PostmanMaven
{{Servidor}}:{{Port}}/HelloWorld2/PostmanMaven
Verify that you receive the expected response: "Hola, PostmanMaven. Estás ejecutando un proyecto Maven" (or similar).

- Testing the Gradle Project:

Select the "Proyecto Gradle" environment in Postman.
Send a GET request to the following URLs (examples):
{{Servidor}}:{{Port}}/api/HelloWorld?nombre=PostmanGradle
{{Servidor}}:{{Port}}/api/HelloWorld2/PostmanGradle
Verify that you receive the expected response: "Hola, PostmanGradle. Estás ejecutando un proyecto Gradle" (or similar).
Screenshots:

## Two screenshots are provided:

- One showing the successful execution of an API request against the Maven project in Postman using the "Proyecto Maven" environment.
- One showing the successful execution of an API request against the Gradle project in Postman using the "Proyecto Gradle" environment.
- These screenshots demonstrate the use of the defined environments and variables for testing.
