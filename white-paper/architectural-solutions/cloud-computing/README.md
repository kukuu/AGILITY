
# Cloud Computing, Distributed Systems and CI

## DevOps Cultural Philosophy

Transitioning to DevOps requires a change in culture and mindset. At its simplest, DevOps is about removing the barriers between two traditionally siloed teams, development and operations. In some organizations, there may not even be separate development and operations teams; engineers may do both. With DevOps, the two teams work together to optimize both the productivity of developers and the reliability of operations.

They strive to communicate frequently, increase efficiencies, and improve the quality of services they provide to customers. They take full ownership for their services, often beyond where their stated roles or titles have traditionally been scoped by thinking about the end customer’s needs and how they can contribute to solving those needs.

Quality assurance and security teams may also become tightly integrated with these teams. Organizations using a DevOps model, regardless of their organizational structure, have teams that view the entire development and infrastructure lifecycle as part of their responsibilities.

## Integration Approach

In-house: dev and production

In-house data with Cloud systems

Legacy systems



## Tools

GIT / GitHub - Probably the most common source management tool available. Used for Source Control Management. In addition to its great forking and pull request features, GitHub also has plugins that can connect with Jenkins to facilitate integration and deployment.

Ansible - Configuration Management Tool similar to Puppet and Chef.

Docker - It eases configuration management, control issues, and scaling by allowing containers to be moved from one place to another.

Jenkins - As an extensible automation server, Jenkins can be used as a simple CI server or turned into the continuous delivery hub for any project. Jenkins can easily distribute work across multiple machines, helping drive builds, tests and deployments across multiple platforms faster.



## Cloud Computing Platforms & Service Models

Cloud Computing is a broad term that describes a broad range of services. Since the Cloud is a broad collection of services, organizations can choose where, when, and how they use Cloud Computing. Such services are, Software as a Service (SaaS), Platform as a Service (PaaS) and Infrastructure as a Service (IaaS).

Cloud computing is a model for enabling convenient, on-demand network access to a shared pool of configurable computing resources (e.g., networks, servers, storage, applications, and services) that can be rapidly provisioned and released with minimal management effort or service provider interaction. By using these services there is the potential to reduce IT support costs by outsourcing hardware and software maintenance and support to the providers.

Characteristics associated with Cloud Computing services include:

On-demand self-service. The ability for an end user to sign up and receive services without the long delays that have characterized traditional IT normally using thin client like the Browser.

Broad network access. Ability to access the service via standard platforms (desktop, laptop, mobile etc)

Resource pooling. Resources are pooled across multiple customers.

Rapid elasticity. Capability can scale to cope with demand peaks.

Measured Service. Billing is metered and delivered as a utility service

### Models

#### SaaS (Software as a Service) applications are designed for end-users, delivered over the web.

SaaS is a software distribution model in which applications are hosted by a vendor 
or service provider and made available to customers over a network, typically the Internet.

With Saas model you are provided with access to application softwares often 
referred to as on-demand softwares. 
You don't have to worry about the installation, setup and running of the application. 
Service provider will do that for you. You just have to pay and use it through some client.

Example: Google Apps, Microsoft Office 365.

#### PaaS
PaaS (Platform as a Service) is the set of tools and services designed to make coding and deploying those applications quick and efficient over the Internet.

The model is a category of cloud computing services that provides a platform allowing 
customers to develop, run, and manage web applications without the complexity of building and
maintaining the infrastructure typically associated with developing and launching 
an app - via the browser.

Examples: AWS Elastic Beanstalk, Windows Azure, Heroku, Force.com, Google App Engine, 
and Apache Stratos.
IaaS (Infrastructure as a Service), is the hardware and software that powers it all – servers, storage, networks, operating system.


#### IaaS

IaaS provides you the computing infrastructure, physical or (quite often) virtual machines and 
other resources like virtual-machine disk image library, block and file-based storage, firewalls,
load balancers, IP addresses, virtual local area networks etc. 

Examples: Amazon EC2, Windows Azure, Rackspace, Google Compute Engine.
Additional points to note:

AWS(Amazon web services) is a complete suite which involves a whole bunch of useful web services. 
Most popular are EC2 and S3 and they belong to IaaS service model.

Although Hadoop is based on previous works by Google(GFS and MapReduce), it is not from Google. 
It is an Apache project.It is just a distributed computing platform and does not fall into 
any of these service models

Windows Azure is both a PaaS and IaaS.

## Scalability

Performance
Hadoop MapReduce (Hadoop Map/Reduce) is a software framework for distributed processing of 
large data sets on compute clusters of commodity hardware. It is a sub-project of the 
Apache Hadoop project. The framework takes care of scheduling tasks, 
monitoring them and re-executing any failed tasks. 

Choose a particular platform based on your requirements and needs. For example, if you want to 
have a Hadoop cluster on which you would run MapReduce jobs, you will find EC2 a perfect fit, 
which is IaaS. On the other hand if you have some application, written in some language, 
and you want to deploy it over the cloud,  you would choose something like Heroku, 
which is an example of PaaS.


## Continuous Integration

Continuous integration is a software development practice where developers regularly merge their code changes into a central repository, after which automated builds and tests are run. The key goals of continuous integration are to find and address bugs quicker, improve software quality, and reduce the time it takes to validate and release new software updates.

## Continuous Delivery (RRASc)

Continuous delivery is a software development practice where code changes are automatically built, tested, and prepared for a release to production. It expands upon continuous integration by deploying all code changes to a testing environment and/or a production environment after the build stage. When continuous delivery is implemented properly, developers will always have a deployment-ready build artifact that has passed through a standardized test process.

Extensibly, it is  the ability to get changes of all types including new features, configuration changes, bug fixes and experiments into production, or into the hands of users, safely and quickly in a sustainable way.

The model behind this approach is to achieve a platform which is:

```

Reliable :: Repeatable :: Automation :: Source control

```


A logical extension of Continuous Integration, It is based on the use of smart automation. This is all about creating a repeatable and reliable process for delivering software. You have to automate pretty much everything in order to be able to achieve continuous delivery. Manual steps will get in the way or become a bottleneck. This goes for everything from requirements authoring to deploying to production.

The ultimate goal of continuous delivery is to minimise the iteration time of the code-test-deliver-measure experimentation cycle. Increasing deliverable throughput in this way is the key to not only more feature work being delivered but higher quality code as well. This might seem counter-intuitive at first but code is fixed and polished through that same cycle and less time spent on deployment is more time spent on designing quality code.

The high-level requirements FOR CD are:

1. Software must be easily testable, which means it must be loosely coupled.

2. Delivery must—under normal circumstances—require minimal human interaction.

3. Delivery—from commit to production—must be fast. Preferably under 10 minutes.

4. Rolling back a deployed feature if it is found to be broken or unwanted must be trivial.

5. Build binaries only once. Binaries should be compiled once and once only. 
   The binary should then be stored someplace which is accessible only to your deployment mechanism, 
   and your deployment mechanism should deploy this same binary to each successive environment

6. Use precisely the same mechanism to deploy to every environment. Both QA and production
   deployment must be both automated.

7. Smoke test your deployment. Write a smoke test and include that in the deployment process.

8. Stop the lines if anything fails.


Achieving CD

1. The process for releasing/deploying software MUST be repeatable and reliable. 

2. Automate everything!

3. If somethings difficult or painful, do it more often.

4. Keep everything in source control

5. Done means “released”.

6. Build quality in! 

7. Everybody has responsibility for the release process

8. Improve continuously
The most optimum path to achieve these goals is to use microservices architecture


## Microservices

The microservices architecture is a design approach to build a single application as a set of small modular services. Each service runs in its own process and communicates with other services through a well-defined interface using a lightweight mechanism, typically an HTTP-based application programming interface (API). Microservices are built around business capabilities; each service is scoped to a single purpose, and supports a busimess goal. You can use different frameworks or programming languages to write microservices and deploy them independently, as a single service, or as a group of services.

When you choose to build your application as a set of microservices, you need to decide how your application’s clients will interact with the microservices. With a monolithic application there is just one set of (typically replicated, load‑balanced) endpoints. In a microservices architecture, however, each microservice exposes a set of what are typically fine‑grained endpoints.

Services must handle requests from the application’s clients. Furthermore, services must sometimes collaborate to handle those requests. They must use an inter-process communication protocol. Use asynchronous messaging for inter-service communication. Services communicating by exchanging messages over messaging channels. Examples of asynchronous messaging technologies are Apache Kafka and RabbitMQ.


This pattern has the following benefits:

```
i. Loose coupling since it decouples client from services

ii. Quick results

iii. Improved availability since the message broker buffers messages until the consumer is able to process them

iii. Lower capital expenses

iv. Grow market share

Supports a variety of communication patterns including request/reply, notifications, request/async response, publish/subscribe, publish/async response etc.

```

This pattern has the following drawbacks:

```
Additional complexity of message broker, which must be highly available

This pattern has the following issues:

i. Request/reply-style communication is more complex

i. Client needs to discover location of message broker

```

Loose coupling::individual deployment:: repeatable deployment can only be achieved by repeatble context ==> containerisation
Microservices enforce loose coupling, plus it’s easier to develop fast and reliable deployment pipelines if they only have to handle small packages.

However, note microservices introduced a new problem: if adding a feature was often going to require adding a new, independently deployed and hosted service then that process had to be fast and not require any specialist knowledge.

Demanding that every single developer in the company learn the intricacies of maintaining Puppet configuration for all their services would have been impractical and more than a little cruel.

Resolution:

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


### Challenges and bottlenecks to Micro-services

Direct Client‑to‑Microservice Communication
In theory, a client could make requests to each of the microservices directly. Each microservice would have a public endpoint (https://serviceName.api.company.name). This URL would map to the microservice’s load balancer, which distributes requests across the available instances. To retrieve the product details, the mobile client would make requests to each of the services listed above.

Unfortunately, there are challenges and limitations with this option.

One problem is the mismatch between the needs of the client and the fine‑grained APIs exposed by each of the microservices. The client in this example has to make posibly a number of separate requests. In more complex applications it might have to make many more. While a client could make that many requests over a LAN, it would probably be too inefficient over the public Internet and would definitely be impractical over a mobile network. This approach also makes the client code much more complex.

Another problem with the client directly calling the microservices is that some might use protocols that are not web‑friendly. One service might use Thrift binary RPC while another service might use the AMQP messaging protocol. Neither protocol is particularly browser‑ or firewall‑friendly and is best used internally. An application should use protocols such as HTTP and WebSocket outside of the firewall.

Another drawback with this approach is that it makes it difficult to refactor the microservices. Over time we might want to change how the system is partitioned into services. For example, we might merge two services or split a service into two or more services. If, however, clients communicate directly with the services, then performing this kind of refactoring can be extremely difficult. Because of these kinds of problems it rarely makes sense for clients to talk directly to microservices.

### Resolving micro service complexity with an API Gateway

Usually a much better approach is to use what is known as an API Gateway. An API Gateway is a server (Serving as an interface) that is the single entry point into the system. It is similar to the Facade pattern from object‑oriented design. The API Gateway encapsulates the internal system architecture and provides an API that is tailored to each client. It might have other responsibilities such as authentication, monitoring, load balancing, caching, request shaping and management, and static response handling.

The Facade design pattern is often used when a system is very complex or difficult to understand because the system has a large number of interdependent classes or its source code is unavailable. This pattern hides the complexities of the larger system and provides a simpler interface to the client. It typically involves a single wrapper class that contains a set of members required by client. These members access the system on behalf of the facade client and hide the implementation details.

The API Gateway is responsible for request routing, composition, and protocol translation. All requests from clients first go through the API Gateway. It then routes requests to the appropriate microservice.

The API Gateway will often handle a request by invoking multiple microservices and aggregating the results. It can translate between web protocols such as HTTP and WebSocket and web‑unfriendly protocols that are used internally.

The API Gateway can also provide each client with a custom API. It typically exposes a coarse‑grained API for mobile clients. Consider, for example, the product details scenario. The API Gateway can provide an endpoint (/productdetails?productid=xxx) that enables a mobile client to retrieve all of the product details with a single request. The API Gateway handles the request by invoking the various services – product info, recommendations, reviews, etc. – and combining the results.

Benefits and Drawbacks of an API Gateway
Using an API Gateway has both benefits and drawbacks.

Benefit: A major benefit of using an API Gateway is that it encapsulates the internal structure of the application. Rather than having to invoke specific services, clients simply talk to the gateway. The API Gateway provides each kind of client with a specific API. This reduces the number of round trips between the client and application. It also simplifies the client code.

Drawback: The API Gateway also has some drawbacks. It is yet another highly available component that must be developed, deployed, and managed. There is also a risk that the API Gateway becomes a development bottleneck. Developers must update the API Gateway in order to expose each microservice’s endpoints. It is important that the process for updating the API Gateway be as lightweight as possible. Otherwise, developers will be forced to wait in line in order to update the gateway.

#### Implementing an API Gateway

Various design issues you need to consider.

##### Performance and Scalability

Only a handful of companies operate at the scale of Netflix and need to handle billions of requests per day. However, for most applications the performance and scalability of the API Gateway is usually very important. It makes sense, therefore, to build the API Gateway on a platform that supports asynchronous, nonblocking I/O. There are a variety of different technologies that can be used to implement a scalable API Gateway.

On the JVM you can use one of the NIO‑based frameworks such Netty, Vertx, Spring Reactor, or JBoss Undertow. One popular non‑JVM option is Node.js, which is a platform built on Chrome’s JavaScript engine. Another option is to use NGINX Plus. NGINX Plus offers a mature, scalable, high‑performance web server and reverse proxy that is easily deployed, configured, and programmed. NGINX Plus can manage authentication, access control, load balancing requests, caching responses, and provides application‑aware health checks and monitoring.

##### Using a Reactive Programming Model

The API Gateway handles some requests by simply routing them to the appropriate backend service. It handles other requests by invoking multiple backend services and aggregating the results. With some requests, such as a product details request, the requests to backend services are independent of one another.

In order to minimize response time, the API Gateway should perform independent requests concurrently. Sometimes, however, there are dependencies between requests. The API Gateway might first need to validate the request by calling an authentication service, before routing the request to a backend service. Similarly, to fetch information about the products in a customer’s wish list, the API Gateway must first retrieve the customer’s profile containing that information, and then retrieve the information for each product.

Writing API composition code using the traditional asynchronous callback approach quickly leads you to callback hell. The code will be tangled, difficult to understand, and error‑prone. A much better approach is to write API Gateway code in a declarative style using a reactive approach. Examples of reactive abstractions include Future in Scala, CompletableFuture in Java 8, and Promise in JavaScript. There is also Reactive Extensions (also called Rx or ReactiveX), which was originally developed by Microsoft for the .NET platform. Netflix created RxJava for the JVM specifically to use in their API Gateway. There is also RxJS for JavaScript, which runs in both the browser and Node.js. Using a reactive approach will enable you to write simple yet efficient API Gateway code.

##### Service Invocation

A microservices‑based application is a distributed system and must use an inter‑process communication mechanism. There are two styles of inter‑process communication. One option is to use an asynchronous, messaging‑based mechanism. Some implementations use a message broker such as JMS or AMQP.

Others, such as Zeromq, are brokerless and the services communicate directly. The other style of inter‑process communication is a synchronous mechanism such as HTTP or Thrift. A system will typically use both asynchronous and synchronous styles. It might even use multiple implementations of each style. Consequently, the API Gateway will need to support a variety of communication mechanisms (Websocket etc).

##### Service Discovery

The API Gateway needs to know the location (IP address and port) of each microservice with which it communicates. In a traditional application, you could probably hardwire the locations, but in a modern, cloud‑based microservices application this is a nontrivial problem. Infrastructure services, such as a message broker, will usually have a static location, which can be specified via OS environment variables.

However, determining the location of an application service is not so easy. Application services have dynamically assigned locations. Also, the set of instances of a service changes dynamically because of autoscaling and upgrades. Consequently, the API Gateway, like any other service client in the system, needs to use the system’s service discovery mechanism: either Server‑Side Discovery or Client‑Side Discovery.

##### Handling Partial Failures

Another issue you have to address when implementing an API Gateway is the problem of partial failure. This issue arises in all distributed systems whenever one service calls another service that is either responding slowly or is unavailable.

The API Gateway should never block indefinitely waiting for a downstream service. However, how it handles the failure depends on the specific scenario and which service is failing. For example, if the recommendation service of the application is unresponsive in the product details scenario, the API Gateway should return the rest of the product details to the client since they are still useful to the user. The recommendations could either be empty or replaced by, for example, a hardwired top ten list.

If, however, the product information service is unresponsive then API Gateway should return an error to the client.

The API Gateway could also return cached data if that was available. The data can be cached by the API Gateway itself or be stored in an external cache such as Redis or Memcached. By returning either default data or cached data, the API Gateway ensures that system failures do not impact the user experience.

A very good robust and scalable API Gateway must time out calls that exceed the specified threshold. It implements a circuit breaker pattern, which stops the client from waiting needlessly for an unresponsive service, can be added to the model's implementation. If the error rate for a service exceeds a specified threshold, it could trip a circuit breaker and all requests will fail immediately for a specified period of time. The module should define a fallback action when a request fails, such as reading from a cache or returning a default value.

For most microservices‑based applications, it makes sense to implement an API Gateway, which acts as a single entry point into a system. The API Gateway is responsible for request routing, composition, and protocol translation. It provides each of the application’s clients with a custom API. The API Gateway can also mask failures in the backend services by returning cached or default data.

## Containerisation 
1. https://github.com/kukuu/AGILITY/tree/master/docker


## Architectures

1. End to end integration - https://github.com/kukuu/AGILITY/blob/master/test-pyramid-coverage.jpg

2. AWS

	i. Architecting for High Availability & Multi-Availability Zones - https://github.com/kukuu/AGILITY/tree/master/AWS-AS 

	ii. Back end - https://github.com/kukuu/AGILITY/blob/master/aws-backend-app-pipeline.png

	iii. Front end - https://github.com/kukuu/AGILITY/blob/master/aws-web-app-pipeline.png 


3. Docker - https://github.com/kukuu/AGILITY/tree/master/docker 

4. Kubernetes - https://github.com/kukuu/AGILITY/tree/master/kubernetes 

5. CI Pipeline - https://github.com/kukuu/AGILITY/blob/master/CI-CDL-CDPL-pipeline.jpg 

6. Microservices - https://github.com/kukuu/AGILITY/blob/master/MICRO-SERVICES-oriented%20Architecture.png 

7. SOA - https://github.com/kukuu/AGILITY/blob/master/SOA-1.png 

8. Test Pyramid (Coverage) - https://github.com/kukuu/AGILITY/blob/master/test-pyramid-coverage.jpg


## Resources

1. AWS Auto scaling - https://aws.amazon.com/autoscaling/

2. Elastic Load Ballancers (ALP, Classic and Network - https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html 

2. Cloud Foundry 

i.  Overview - https://docs.cloudfoundry.org/concepts/overview.html 

ii. Pair Programming - https://www.armakuni.com/ak-thinking/ 

3. Cloud Native 

i. Container Solutions - https://container-solutions.com/what-is-cloud-native/ 

ii. Security Strategies - https://www.twistlock.com/2017/10/02/security-cloud-native-environments/?ads_cmpid=1071572634&ads_adid=54488335919&ads_matchtype=b&ads_network=g&ads_creative=269316971720&utm_term=&ads_targetid=dsa-446131505180&utm_campaign=&utm_source=adwords&utm_medium=ppc&ttv=2&gclid=EAIaIQobChMIld3mtZqF3QIVqrXtCh16MwdBEAAYAyAAEgLSO_D_BwE



