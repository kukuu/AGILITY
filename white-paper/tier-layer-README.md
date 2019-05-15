
# TIER , Layer Architectures with  Monoliths & Microservice


Layers reside on the same machine where the tiers can reside on different machines.

 1. A monolithic application is simply deployed on a set of identical servers behind a load balancer.

 2. In contrast, a microservice application typically consists of a large number of services.

 3. In a monolith, the user interface and data acccess are combined in  a single program from a single platform



## n-Tier

 Multitier architecture (often referred to as n-tier architecture) or multilayered architecture is a client–server architecture in which presentation, application processing, and data management functions are physically separated.

 N-tier architecture usually has each layer separated by the network.  N-tier just refers to the physical structure of an implementation. These two are sometimes confused because an MVC design is often implemented using an N-tier architecture.


### One Tier Architecture

 A one tier architecture has all the layers such as Presentation, Business, Data Access layers in a single software package. Applications which handles all the three tiers such as MP3 player, MS Office are come under one tier application. The data is stored in the local system or a shared drive.


### Three Tier Architecture

 But 3 tier applications are not straight as 3 layers, because each tier will be deployed in different machines. So here, we need a mechanism to send the objects between different machines over the network hence we use technologies called Web Services, Remoting or WCF, etc. in order to implement 3 tier applications


### Three Layer Architecture

 In 3 Layer we have distinct namespaces and classes for the various layes i.e. we’re only talking about logical organization of code and passing objects between layers is easy as all assemblies will run under same application in single machine.


## Transitions

 Tier becomes a Layer if it could be physically separated from the Layers it consumes. N-Tier Architecture is a physical structuring, while a N-Layer Architecture is a logical structuring.


## Deployment

 In 3 layer architecture, the Database Access Layer (DAL), Business Logic Layer (BLL) and User Interface Layer (UIL) resides as 3 different project and the output of these 3 projects (.dll file) must be together in the same server or on same machine in order for the system to run.


 However in 3 tier architecture, the Database Access Layer (DAL), Business Logic Layer (BLL) and User Interface Layer (UIL) reside as 3 different projects. But each of the projects can be deployed at the different server or at the different machines and distributed functionality is explored.
 
