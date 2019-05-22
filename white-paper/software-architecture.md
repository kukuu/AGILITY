
# Software Architecture

 Remember that you can use multiple patterns in a single system to optimize each section of code with the best architecture.
 
 https://github.com/kukuu/AGILITY/blob/master/white-paper/software-architecture.png
 

## Layered (n-tier) architecture

This approach is probably the most common because it is usually built around the database, and many applications in business naturally lend themselves to storing information in tables.
 
### MVC
 
 The code is arranged so the data enters the top layer and works its way down each layer until it 
 reaches the bottom, which is usually a database. Along the way, each layer has a specific task, 
 like checking the data for consistency or reformatting the values to keep them consistent. 
 It’s common for different programmers to work independently on different layers
 
 Just above the database is the model layer, which often contains business logic and information 
 about the types of data in the database. At the top is the view layer, which is often CSS, JavaScript, 
 and HTML with dynamic embedded code. In the middle, you have the controller, which has various rules
 and methods for transforming the data moving between the view and the model.
 
 The Model-View-Controller (MVC) structure, which is the standard software development approach offered by most of the popular web frameworks, is clearly a layered architecture. Just above the database is the model layer, which often contains business logic and information about the types of data in the database. At the top is the view layer, which is often CSS, JavaScript, and HTML with dynamic embedded code. In the middle, you have the controller, which has various rules and methods for transforming the data moving between the view and the model.

 This architecture can also contain additional open layers, like a service layer, that can be used to access shared services only in the business layer but also get bypassed for speed.


#### Benefits

The advantage of a layered architecture is the separation of concerns, which means that each layer can focus solely on its role. This makes it:

i.  Maintainable

ii.  Testable

iii. Easy to assign separate "roles"

iv.  Easy to update and enhance layers separately



#### Caveats

i.  Source code can turn into a “big ball of mud” if it is unorganized and the modules don’t have clear roles or relationships.

ii. Code can end up slow thanks to what some developers call the “sinkhole anti-pattern.” Much of the code can be devoted to   passing data through layers without using any logic.

iii. Layer isolation, which is an important goal for the architecture, can also make it hard to understand the architecture without understanding every module.

iv. Coders can skip past layers to create tight coupling and produce a logical mess full of complex interdependencies.
Monolithic deployment is often unavoidable, which means small changes can require a complete redeployment of the application.

#### Best for

i.   New applications that need to be built quickly

ii   Enterprise or business applications that need to mirror traditional IT departments and processes

iii. Teams with inexperienced developers who don’t understand other architectures yet

iv.  Applications requiring strict maintainability and testability standards
 
 
## Microservices architecture

 https://github.com/kukuu/Microservice-NodeJS 

### Benefits:

i. Loose coupling, scales, maintainable, easily testable, risk manageable

ii. High Availability. A result of buffering and queue set up. Result of asynchronous  data handling during request, response

iii. Supports multiple communication patterns: request/response, notification, publish/Subscribe, Async etc


### Caveats

i.  The services must be largely independent or else interaction can cause the cloud to become imbalanced.

ii. Not all applications have tasks that can’t be easily split into independent units.

iii. Performance can suffer when tasks are spread out between different microservices. The communication costs can be significant.

iv. Too many microservices can confuse users as parts of the web page appear much later than others. Anti-AJAX


### Best for

i.   Websites with small components

ii.  Corporate data centers with well-defined boundaries

iii. Rapidly developing new businesses and web applications

iv.   Development teams that are spread out, often across the globe


## Space-based architecture (Cloud)

The space-based architecture is designed to avoid functional collapse under high load by splitting up both the processing and the storage between multiple servers. 

The data is spread out across the nodes just like the responsibility for servicing calls. The name “space-based” refers to the “tuple space” of the users, which is cut up to partition the work between the nodes. 

The space-based architecture supports things that have unpredictable spikes by eliminating the database.

###  Caveats

i.  Finding an average or doing a statistical analysis—must be split up into subjobs, spread out across all of the nodes, and then aggregated when it’s done.

ii.  Transactional support is more difficult with RAM databases.

iii. Generating enough load to test the system can be challenging, but the individual nodes can be tested independently.

iv. Developing the expertise to cache the data for speed without corrupting multiple copies is difficult.

### Best for

i.  High-volume data like click streams and user logs

ii. Low-value data that can be lost occasionally without big consequences—in other words, not bank transactions
Social networks.

## Microkernel architecture 

The microkernel architecture pattern (aka plug-in architecture pattern) is a natural pattern for implementing product-based applications. A product-based application is one that is packaged and made available for download in versions as a typical third-party product.

The architecture has a core set of operations that are used again and again in different patterns that depend upon the data and the task at hand.

https://github.com/kukuu/AGILITY/blob/master/white-paper/mikrokernel-architecture.png

