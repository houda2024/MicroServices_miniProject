# MicroServices_miniProject
Microservices avec REST, GraphQL et gRPC


#Description

This project consists of two microservices: "Product" and "User". The microservices are built using REST and GraphQL for communication between the client and the API gateway, and gRPC for communication between the API gateway and the microservices. The project includes the following files:


product.proto: Protocol Buffers definition file for the "Product" microservice.


user.proto: Protocol Buffers definition file for the "User" microservice.


resolver.js: GraphQL resolver functions for handling requests related to the "Product" and "User" entities.


schema.js: GraphQL schema definition file that outlines the available queries and mutations for the API.

#Architecture Overview


The chosen architecture provides several benefits and conveniences:

Microservices: The microservices architecture allows for modular and independent development of the "Product" and "User" functionalities. Each microservice can be developed, tested, and scaled separately, resulting in better maintainability and scalability of the overall system.

REST and GraphQL: The RESTful API between the client and the API gateway provides a familiar and straightforward interface for traditional HTTP-based communication. GraphQL is used alongside REST to provide flexible and efficient data querying capabilities, allowing clients to request only the specific data they need, reducing unnecessary data transfer and improving performance.

gRPC: The use of gRPC between the API gateway and the microservices offers efficient and high-performance communication using Protocol Buffers. gRPC supports bi-directional streaming and uses binary serialization, which results in faster data transfer compared to traditional REST APIs. Additionally, gRPC provides strong typing and generates client and server stubs automatically based on the defined Protobuf messages, making it easier to work with the microservices.


![Untitled](https://github.com/houda2024/MicroServices_miniProject/assets/107250916/a3cb3b47-ca34-4ac6-8810-a4d325964968)







#Installation and Setup
To run the project locally, follow these steps:

Clone the repository: git clone https://github.com/your/repository.git


Install the required dependencies: npm install


Configure the necessary environment variables: cp .env.example .env and update the values accordingly.


Start the microservices: npm run start:product and npm run start:user.


Start the API gateway: npm run start:gateway.


Access the GraphQL playground at http://localhost:3000/graphql to interact with the API.

Usage


The API provides the following functionality:

Product Microservice:

Retrieve a list of products

Get product details by ID

Create a new product

Update product information

Delete a product

User Microservice:

Retrieve a list of users

Get user details by ID

Create a new user

Update user information

Delete a user

You can use the GraphQL playground to execute queries and mutations against the API.





