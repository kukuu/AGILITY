# Severless Computing vs Containers

Both serverless computing and containers enable developers to build applications with far less overhead and more flexibility than applications hosted on traditional servers or virtual machines. Which style of architecture a developer should use depends on the needs of the application, but serverless applications are more scalable and usually more cost-effective.

## What are containers?

A container 'contains' both an application and all the elements the application needs to run properly, including system libraries, system settings, and other dependencies. Like a 'just add water' pancake mix, containers only need one thing – to be hosted and run – in order to perform their function.

Any kind of application can be run in a container. A containerized application will run the same way no matter where it is hosted. Containers can easily be moved around and deployed wherever needed, much like physical shipping containers, which are a standard size and can therefore be shipped anywhere via a variety of means of transport (ships, trucks, trains, etc.) regardless of their contents.

In technical terms, containers are a way of partitioning a machine, or server, into separate user space environments such that each environment runs only one application and doesn’t interact with any other partitioned sections on the machine. Each container shares the machine's kernel with other containers (the kernel is the foundation of the operating system, and it interacts with the computer's hardware), but it runs as if it were the only system on the machine.

## Containers vs. virtual machines

A virtual machine is a piece of software that imitates a complete computer system. It is isolated from the rest of the machine that hosts it and behaves as if it were the only operating system on it, including having its own kernel. Virtual machines are another common way of hosting multiple environments on one server, but they use a lot more processing power than containers.

## What is serverless computing?

Serverless applications are broken up into functions, and hosted by a third-party vendor who charges the application developer only based on the amount of time each function runs. For more on serverless computing, see What is serverless computing?

## What are the key differences between serverless computing and containers?

```
1. Physical machines

'Serverless' computing actually runs on servers, but it is up to the serverless vendor to provision
server space as it is needed by the application; no specific machines are assigned for a given 
function or application. On the other hand, each container lives on one machine at a time and uses 
the operating system of that machine, though they can be moved easily to a different machine if desired.

2. Scalability

In a container-based architecture, the number of containers deployed is determined by the developer in advance. In contrast, in a serverless architecture, the backend inherently and automatically scales to meet demand.

To continue the shipping container metaphor, a shipping company could try to forecast an increase in demand
for a certain product and ship more containers to the destination to meet that demand, but it could not snap
its fingers and produce more containers full of goods if demand were to exceed expectations.

Serverless architecture is a way to do exactly that. When it comes to computing power, serverless computing is
like a water supply in a modern home: by turning on the tap, consumers can acquire and use as much water as 
they need at any time, and they only pay for what they use. This is far more scalable than attempting to buy 
water one bucket, or one shipping container, at a time.

3. Cost

Containers are constantly running, and therefore cloud providers have to charge for the server space even if 
no one is using the application at the time.

There are no continued expenses in a serverless architecture because application code does not run unless it
is called. Instead, developers are only charged for the server capacity that their application does in fact use.

4. Maintenance

Containers are hosted in the cloud, but cloud providers do not update or maintain them. Developers have to 
manage and update each container they deploy.

From a developer's perspective, a serverless architecture has no backend to manage. The vendor takes care of 
all management and software updates for the servers that run the code.

5. Time of deployment

Containers take longer to set up initially than serverless functions because it is necessary to configure
system settings, libraries, and so on. Once configured, containers take only a few seconds to deploy. 
But because serverless functions are smaller than container microservices and do not come bundled with 
system dependencies, they only take milliseconds to deploy. Serverless applications can be live as soon 
as the code is uploaded.

6. Testing

It is difficult to test serverless web applications because the backend environment is hard to replicate 
on a local environment. In contrast, containers run the same no matter where they are deployed, making it 
relatively simple to test a container-based application before deploying it to production.

```

## How are serverless computing and containers similar?

Both are cloud-based, and both greatly reduce infrastructure overhead – serverless computing more so than containers. In both kinds of architecture, applications are broken down and deployed as smaller components. In a container-based architecture, each container will run one microservice.

## What are microservices?

Microservices are segments of an application. Each segment is a microservice, performs one service, and multiple integrated microservices combine to make up the application. Although the name seems to imply that microservices are tiny, they do not have to be.

One of the advantages of building an application as a collection of microservices is that developers can update one microservice at a time instead of updating the entire application when they need to make changes. Building an application as a collection of functions, as in a serverless architecture, offers the same benefit but at a more granular level.

## How should developers choose between serverless architecture and containers?

Developers who choose a serverless architecture will be able to release and iterate new applications quickly, without having to worry about whether or not the application can scale. In addition, if an application does not see consistent traffic or usage, serverless computing will be more cost-efficient than containers, because the code does not need to be constantly running.

Containers give developers more control over the environment the application runs in (although this also comes with more maintenance) and the languages and libraries used. Because of this, containers are extremely useful for migrating legacy applications to the cloud, since it is possible to more closely replicate the application's original running environment.

And finally, it is possible to use a hybrid architecture, with some serverless functions and some functions deployed in containers. For instance, if an application function requires more memory than allotted by the serverless vendor, if a function is too large, or if certain functions but not others need to be long-running, a hybrid architecture enables developers to reap the benefits of serverless while still using containers for the functions serverless cannot support.
