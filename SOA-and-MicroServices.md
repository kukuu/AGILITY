# SOA and Micro-services

## SOA
A Service Oriented Architecture is a software architecture pattern, which application components provide services to other components via a communications protocol over a network. The communication can involve either simple data passing or it could involve two or more services coordinating connecting services to each other. Services (such as RESTful Web services) carry out some small functions, such as validating an order, activating account, or providing shopping cart services.

There are 2 main roles in SOA, a service provider and a service consumer. 

A software agent may play both roles. The Consumer Layer is the point where consumers (human users, other services or third parties) interact with the SOA and Provider Layer consists of all the services defined within the SOA. The following figure shows a quick view of an SOA architecture.

Enterprise Service Bus (ESB) is a style of the integration architecture that allows communication via a common communication bus that consists of a variety of point-to-point connections between providers and consumers . In addition to above, the data storage is shared within all services in SOA.


So, SOA is an architectural pattern in which application components provide services to other components. Autonomous units of business functionality: each service provides a business function that is independent of other services.

### Architecture

https://github.com/kukuu/AGILITY/blob/master/white-paper/SOA-1.png

## Microservices Architecture

Microservices is a software architecture pattern in which complex applications are composed of small, independent processes communicating with each other using language-agnostic APIs. 
Microservices must be a real need in the system architecture as it could be designed wrongly. It means a service should be independently deployable, or be able to shut-down a service when is not required in the system and that should not have any impact on other services. The following figure shows a quick view of a Microservices architecture.

Microservices must be independently deployable, whereas SOA services are often implemented in deployment monoliths. Classic SOA is more platform driven, so microservices offer more choices in all dimensions.


### Architecture  
API Gateway  - https://github.com/kukuu/digitalTransformationStrategies/blob/master/APIgatewayResolution4microservices.png 

Model - https://github.com/kukuu/digitalTransformationStrategies/blob/master/MICRO-SERVICES-oriented%20Architecture.png


