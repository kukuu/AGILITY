# Micro-services

Microservices architecture is an approach to application development in which a large application is built as a suite of modular services. Each module supports a specific business goal and uses a simple, well-defined interface to communicate with other sets of services.

When you choose to build your application as a set of microservices, you need to decide how your application’s clients will interact with the microservices. With a monolithic application there is just one set of (typically replicated, load‑balanced) endpoints. In a microservices architecture, however, each microservice exposes a set of what are typically fine‑grained endpoints.

Services must handle requests from the application’s clients. Furthermore, services must sometimes collaborate to handle those requests. They must use an inter-process communication protocol. Use asynchronous messaging for inter-service communication. Services communicating by exchanging messages over messaging channels. Examples of asynchronous messaging technologies are Apache Kafka and RabbitMQ.


## Benefits of Micro-services:

1. Loose coupling since it decouples client from services

2. Improved availability since the message broker buffers messages until the consumer is able to process them

3. Supports a variety of communication patterns including request/reply, notifications, request/async response, publish/subscribe, publish/async response etc

## Micro-services drawbacks:

i. Additional complexity of message broker, which must be highly available

ii. Request/reply-style communication is more complex

iii. Client needs to discover location of message broker

## Seting up a  microservice team

1.	Set up feature teams  that can possibly set up a new service in under four hours. What this means
	is Developing services should not   require knowledge of the infrastructure and changing 
	infrastructure should not require detailed knowledge of the services running on it. 
	If we need to change the hostname or port a service runs on it should require no changes
	to the service itself.

2.	All project configuration—from build process to health monitoring—must be contained within the 
	project repository. Anything else introduces hidden dependencies for deployment that threaten
	to break the pipeline and require specialist knowledge to debug.

3.	The above configuration should be declarative and not require adding dependencies to the project.

4.   Use Containerisation

## Implementing a Gateway

It makes sense,  to build the API Gateway on a platform that supports asynchronous, nonblocking I/O. There are a variety of different technologies that can be used to implement a scalable API Gateway.

On the JVM you can use one of the NIO‑based frameworks such Netty, Vertx, Spring Reactor, or JBoss Undertow. 

One popular non‑JVM option is Node.js, which is a platform built on Chrome’s JavaScript engine. 

Another option is to use NGINX Plus. NGINX Plus offers a mature, scalable, high‑performance web server and reverse proxy that is easily deployed, configured, and programmed. NGINX Plus can manage authentication, access control, load balancing requests, caching responses, and provides application‑aware health checks and monitoring.


Writing API composition code using the traditional asynchronous callback approach quickly leads you to callback hell. The code will be tangled, difficult to understand, and error‑prone. A much better approach is to write API Gateway code in a declarative style using a reactive approach. Examples of reactive abstractions include Future in Scala, CompletableFuture in Java 8, and Promise in JavaScript. There is also Reactive Extensions (also called Rx or ReactiveX), which was originally developed by Microsoft for the .NET platform. Netflix created RxJava for the JVM specifically to use in their API Gateway. There is also RxJS for JavaScript, which runs in both the browser and Node.js. Using a reactive approach will enable you to write simple yet efficient API Gateway code.


## Handling Partial Failures in API Gateways


Another issue you have to address when implementing an API Gateway is the problem of partial failure. This issue arises in all distributed systems whenever one service calls another service that is either responding slowly or is unavailable.

The API Gateway should never block indefinitely waiting for a downstream service. However, how it handles the failure depends on the specific scenario and which service is failing. For example, if the recommendation service of the application is unresponsive in the product details scenario, the API Gateway should return the rest of the product details to the client since they are still useful to the user. The recommendations could either be empty or replaced by, for example, a hardwired top ten list.

If, however, the product information service is unresponsive then API Gateway should return an error to the client.

The API Gateway could also return cached data if that was available. The data can be cached by the API Gateway itself or be stored in an external cache such as Redis or Memcached. By returning either default data or cached data, the API Gateway ensures that system failures do not impact the user experience.

A very good robust and scalable API Gateway must time out calls that exceed the specified threshold. It implements a circuit breaker pattern, which stops the client from waiting needlessly for an unresponsive service, can be added to the model's implementation. If the error rate for a service exceeds a specified threshold, it could trip a circuit breaker and all requests will fail immediately for a specified period of time. The module should define a fallback action when a request fails, such as reading from a cache or returning a default value.

For most microservices‑based applications, it makes sense to implement an API Gateway, which acts as a single entry point into a system. The API Gateway is responsible for request routing, composition, and protocol translation. It provides each of the application’s clients with a custom API. The API Gateway can also mask failures in the backend services by returning cached or default data.

### Summary

```

The microservices architecture is a design approach to build a single application as a set of
small modular services. Each service runs in its own process and communicates with other 
services through a well-defined interface using a lightweight mechanism, typically an 
HTTP-based application programming interface (API). Microservices are built around 
business capabilities; each service is scoped to a single purpose, and supports a busimess goal.
You can use different frameworks or programming languages to write microservices and deploy them
independently, as a single service, or as a group of services.


```

## Architecture

The tier systems - https://github.com/kukuu/AGILITY/blob/master/white-paper/tier-layer-README.md

Monolith - https://github.com/kukuu/AGILITY/blob/master/white-paper/monolith.jpg

microservice model : https://github.com/kukuu/digitalTransformationStrategies/blob/master/MICRO-SERVICES-oriented%20Architecture.png

SOA with Enterprise Service Bus (ESB) - https://github.com/kukuu/AGILITY/blob/master/white-paper/SOA.png

 Monolith vs Microservice - https://github.com/kukuu/AGILITY/blob/master/white-paper/monolithic_vs_microservices.jpg

SOA vs Microservices

i. https://github.com/kukuu/AGILITY/blob/master/SOA-and-MicroServices.md

ii. https://github.com/kukuu/AGILITY/blob/master/difference-between-monolithic-and-microservices-architecture-1.png

Micro-services API Gateway - https://github.com/kukuu/digitalTransformationStrategies/blob/master/APIgatewayResolution4microservices.png

## Applications

i. API - NodeJS, Express Framework, MongoDB & Swagger - https://github.com/kukuu/Microservice-NodeJS/tree/master/microservices

ii. NodeJS/NGINX/Docker  - https://github.com/kukuu/microservices-nodejs-docker-nginx 

iii. Node, MongoDB, Docker Swarm - https://github.com/kukuu/cinema-microservice

iv. from monolithic  to micro services - https://www.youtube.com/watch?v=xydpSPdglQw 

v. Communication Between Microservices - https://stackify.com/communication-microservices-avoid-common-problems/ 

## Resources 

1. Containers - https://github.com/kukuu/AGILITY/blob/master/containerisation.md

2. Docker - https://github.com/kukuu/AGILITY/tree/master/docker
