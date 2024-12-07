**API Gateway**
**Overview**
The API Gateway acts as a single entry point for all microservices in the architecture. Built using Spring Cloud Gateway, it handles client requests by routing them to the appropriate microservices while managing concerns like authentication, rate-limiting, and error handling.

**Key Features**
Centralized Routing: Routes requests to the appropriate microservices based on predefined configuration.
Dynamic Routing: Works with the Service Registry to dynamically discover service instances and route requests accordingly.
Load Balancing: Distributes traffic evenly across multiple service instances.
Security: Provides centralized authentication and authorization mechanisms.
Request Filtering: Implements pre- and post-request processing for cross-cutting concerns like logging and monitoring.
Fault Tolerance: Provides fallback mechanisms and handles service failures gracefully.

**Technologies Used**
Java 17
Spring Boot
Spring Cloud Gateway
Maven

**Usage**
Start the API Gateway and configure its routing to microservices through either:
Static configuration: Using application.yml.
Dynamic discovery: Using the Service Registry (Eureka).
Access microservices through the Gateway’s base URL, e.g., http://localhost:8765/{service-name}/{endpoint}.

**Future Use Cases**
This repository is generic and reusable for any microservice architecture. Simply configure routing rules and integrate it with the Service Registry to handle new microservices.
