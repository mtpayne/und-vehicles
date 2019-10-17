## Vehicles API Instructions

In this project you will have the opportunity to create a REST-based Vehicles API that communicates with a location and pricing service using Spring Boot, along with converting the existing Pricing Service API to a microservice registered on a Eureka server. Follow the [README and code instructions](README.md) and make sure to check the [rubric](rubric.pdf) to ensure you have completed all items.

#### Convert the Pricing Service

Convert the Pricing Service to a microservice, registered on a Eureka server. Also, add an additional test for the microservice.

#### Implement the Vehicles API

Implement all TODOs for the CarService and CarController.

#### Test and Document the Vehicles API

- Add tests for the CarController class
- Use Swagger to implement API documentation for the Vehicles API

#### Run the applications

Note that the Boogle Maps, Pricing Service and Vehicles API applications must all be running for all operations to perform correctly, although they should be able to launch on their own.

You can either use these in separate windows in your favorite IDE, or use the below commands:

1. ``` $ mvn clean package``` (run this in each directory containing the separate applications)
2. Boogle Maps: ``` $ java -jar target/boogle-maps-0.0.1-SNAPSHOT.jar ```
   - The service is available by default on port 9191. You can check it on the command line by using ``` $ curl http://localhost:9191/maps\?lat\=20.0\&lon\=30.0 ```
3. Pricing Service: ``` $ java -jar target/pricing-service-0.0.1-SNAPSHOT.jar ```
4. Vehicles API: ``` $ java -jar target/vehicles-api-0.0.1-SNAPSHOT.jar ```
   - When the Swagger API documentation is implemented, it should be available at: http://localhost:8080/swagger-ui.html
