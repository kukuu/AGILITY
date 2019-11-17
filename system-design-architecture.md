
# System Design & Architecture

Software architecture refers to the high level structures of a software system and the discipline of creating such structures and systems. Each structure comprises software elements, relations among them, and properties of both elements and relations.

The architecture is a blend of technical decisions and architectural patterns, and considered the root of a software project, to ensure its scalability, security, quality, cost effectiveness and longevity.

The architecture is made so the code structure can satisfy every software prerequisite that is being developed while exemplifying transversal attributes such as performance, quality, scalability, maintainability, manageability, and usability.

You can use multiple patterns in a single system to optimize each section of code with the best architecture.

## Basic Programming Principles Every Programmer Must Follow

1. KISS. The “keep it simple, stupid” principle applies to pretty much all of life, but it's especially necessary in medium-to-large programming projects. 

2. DRY.

3. Develop iteratively

4. Composition > Inheritance. 

5. Single Responsibility. 

6. Separation of Concerns. 

7. Avoid Premature Optimization.


## Architectures

https://github.com/kukuu/AGILITY/blob/master/white-paper/software-architecture.md

i. Layers (n-tier):



ii. Microservices : 

Microservices are self contained processes that provides unique business capabilities. Each individual service boosts of its own data federation unlike momoliths for deployment.

ii. COTS/MicroKernel:

The microkernel architecture pattern (aka plug-in architecture pattern) is a natural pattern for implementing product-based applications. A product-based application is one that is packaged and made available for download in versions as a typical third-party product.

i.e - Microsoft 365

iv. Cloud/Space based: 

The space-based architecture is designed to avoid functional collapse under high load by splitting up both the processing and the storage between multiple servers.

The data is spread out across the nodes just like the responsibility for servicing calls.

v. Event Driven/Composition

Handling assynchronous calls (Gateways, Load Ballancers)

 Many programs spend most of their time waiting for something to happen. Sometimes there’s data that needs processing, and other times there isn’t. Common within network operations, and human driven.

The event-driven architecture helps manage this by building a central unit that accepts all data and then delegates it to the separate modules that handle the particular type. This handoff is said to generate an “event,” and it is delegated to the code assigned to that type. Functional programming.

Programming a web page with JavaScript involves writing the small modules that react to events like mouse clicks or keystrokes. The browser itself orchestrates all of the input and makes sure that only the right code sees the right events. Many different types of events are common in the browser, but the modules interact only with the events that concern them. This is very different from the layered architecture where all data will typically pass through all layers.

Benefits:

i. Are easily adaptable to complex, often chaotic environments

ii. Scale easily

iii. Are easily extendable when new event types appear

Caveats
i. Testing can be complex if the modules can affect each other. While individual modules can be tested independently, the interactions between them can only be tested in a fully functioning system.

ii. Error handling can be difficult to structure, especially when several modules must handle the same events. When modules fail, the central unit must have a backup plan.

iii. Messaging overhead can slow down processing speed, especially when the central unit must buffer messages that arrive in bursts.

iv. Developing a systemwide data structure for events can be complex when the events have very different needs.

v. Maintaining a transaction-based mechanism for consistency is difficult because the modules are so decoupled and independent.

Best for:
i. Asynchronous systems with asynchronous data flow

ii. Applications where the individual data blocks interact with only a few of the many modules

iii. User interfaces


## Principles of Software Design architecture

1. Principles of Software Architecture - https://github.com/kukuu/AGILITY/blob/master/white-paper/principles-of-sw-architecture.png

i. Business goals ii. Quality Attributes iii. Architecture

2. Design decisions - https://github.com/kukuu/AGILITY/blob/master/white-paper/software-architecture-main.jpg


## 10 ways to avoid cross-browser compatibility issues

1. Validate your code.

2. Fail gracefully. 

3. Use progressive enhancement

4. Know your audience. 

5. Consider using a framework. 

6. Keep your design simple. 

7. Reuse and reduce components.

8. Test with the difficult browsers first. 

9. Use automation - Create test scripts.



## JS Design Ptterns

1. Constructor Pattern

2. Module Pattern

3. Revealing Module Pattern

4. Singleton Pattern

5. Observer Pattern

6. Mediator Pattern

7. Prototype Pattern

8. Command Pattern

9. Facade Pattern

10. Factory Pattern

11. Mixin Pattern

12. Decorator Pattern

13. Flyweight Pattern



## JavaScript MV* Patterns

MVC Pattern

MVP Pattern

MVVM Pattern

## Modern Modular JavaScript Design Patterns

1. AMD

2. CommonJS

3. SystemJS

4. ES Harmony

## Best practices in software engineering

1. Develop iteratively.

2. Manage requirements and edge cases.

3. Use component architecture.

4. Model software visually.

5. Verify quality.

6. Control change.

7. Use SOLID Principles


## What is diff between functional and object oriented programming?

Both concepts have different methods for storing the data and how to manipulate the data. 

In object oriented programming, you store the data in attributes of objects and have functions that work for that object and do the manipulation. 

In functional programming, we view everything as data transformation.


OOP says that bringing together data and its associated behavior in a single location (called an “object”) makes it easier to understand how a program works. 

FP says that data and behavior are distinctively different things and should be kept separate for clarity.

Functional programming is stateless. ... The lack of state allows a functional language to be reasoned just by looking at a function's input and output.

FP treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

## JavaScript Design Patterns     

Developermust  strive to write maintainable, readable, and reusable code. Code structuring becomes more important as applications become larger. Design patterns prove crucial to solving this challenge - providing an organization structure for common issues in a particular circumstance.


i. Constructor Pattern

ii. Module Design Pattern

iii. Prototype Design Pattern

iv. Observer Design Pattern

v. Singleton


Also - https://scotch.io/bar-talk/4-javascript-design-patterns-you-should-know 

## System environmental Architectures

1. Multi tier - https://github.com/kukuu/AGILITY/blob/master/white-paper/restfulArchitecturalDesign-2.png

2. JWT - https://github.com/kukuu/AGILITY/blob/master/white-paper/restfulArchitecturalDesign-2.png

3. Micro service  - https://github.com/kukuu/Microservice-NodeJS/blob/master/microservice-snapshots/3.png

4. CI/CD - https://github.com/kukuu/AGILITY/blob/master/white-paper/CI-CDL-CDPL-pipeline.jpgS

5. Orchestrating with Kubernetes - https://github.com/kukuu/AGILITY/blob/master/white-paper/kubernetes/1.png

### Software Module Design Pattern

JavaScript modules are the most prevalently used design patterns for keeping particular pieces of code independent of other components, and consistent. This provides loose coupling to support well-structured code.


For those that are familiar with object-oriented languages, modules are JavaScript "classes". One of the many advantages of classes is encapsulation - protecting states and behaviors from being accessed from other classes. The module pattern allows for public and private (plus the lesser-know protected and privileged) access levels.

Modules should be Immediately-Invoked-Function-Expressions (IIFE) to allow for private scopes - that is, a closure that protect variables and methods.

#### Revealing Module Pattern

A variation of the module pattern is called the Revealing Module Pattern. The purpose is to maintain encapsulation and reveal certain variables and methods returned in an object literal. The direct implementation looks like this.


### Prototype Design Pattern

 The Prototype design pattern relies on the JavaScript prototypical inheritance. The prototype model is used mainly for creating objects in performance-intensive situations.


 The objects created are clones (shallow clones) of the original object that are passed around. One use case of the prototype pattern is performing an extensive database operation to create an object used for other parts of the application. If another process needs to use this object, instead of having to perform this substantial database operation, it would be advantageous to clone the previously created object.


 To clone an object, a constructor must exist to instantiate the first object. Next, by using the keyword prototype variables and methods bind to the object's structure. Let's look at a basic example.

#### Revealing Prototype Pattern

Similar to Module pattern, the Prototype pattern also has a revealing variation. The Revealing Prototype Pattern provides encapsulation with public and private members since it returns an object literal.

### Observer Design Pattern

There are many times when one part of the application changes, other parts needs to be updated. In AngularJS, if the $scope object updates, an event can be triggered to notify another component. The observer pattern incorporates just that - if an object is modified it broadcasts to dependent objects that a change has occurred.

Another prime example is the model-view-controller (MVC) architecture; The view updates when the model changes. One benefit is decoupling the view from the model to reduce dependencies.


### Publish/Subscribe

The Publish/Subscribe pattern, however, uses a topic/event channel that sits between the objects wishing to receive notifications (subscribers) and the object firing the event (the publisher). This event system allows code to define application-specific events that can pass custom arguments containing values needed by the subscriber. The idea here is to avoid dependencies between the subscriber and publisher.


Subscribers in the publish/subscribe pattern are notified through some messaging medium, but observers are notified by implementing a handler similar to the subject.

In AngularJS, a subscriber 'subscribes' to an event using $on('event', callback), and a publisher 'publishes' an event using $emit('event', args) or $broadcast('event', args).


### Singleton

A Singleton only allows for a single instantiation, but many instances of the same object. The Singleton restricts clients from creating multiple objects, after the first object created, it will return instances of itself.

Finding use cases for Singletons is difficult for most who have not yet used it prior. One example is using an office printer. If there are ten people in an office, and they all use one printer, ten computers share one printer (instance). By sharing one printer, they share the same resources.


In AngularJS, Singletons are prevalent, the most notable being services, factories, and providers. Since they maintain state and provides resource accessing, creating two instances defeats the point of a shared service/factory/provider.

Race conditions occur in multi-threaded applications when more than one thread tries to access the same resource. Singletons are susceptible to race conditions, such that if no instance were initialized first, two threads could then create two objects instead of returning and instance. This defeats the purpose of a singleton. Therefore, developers must be privy to synchronization when implementing singletons in multithreaded applications.

## Unit Tests 

Unit tests don't work in current mainstream languages anyway because the status quo pervasively includes use of globally accessible mutable state, platform dependence, and violation of encapsulation.

1. It's the usual cost/benefit analysis that may restrain Developers from writing Unit Tests.

2. Cost: You need to spend time developing and maintaining the tests, and put resources into actually running them.

3. Benefits are well known (mostly cheaper maintenance/refactoring with less bugs).


If it's a throw away quick hack you know will never be re-used, unit tests might not make sense. 

### In practice:


Use TDD if you are implementing an isolated library-like module. If you’re not implementing an isolated library-like module, it’s best to implement first and then conduct the tests. The important thing is to make sure you don’t implement too much without writing any tests. Ideally you should implement incrementally, and at the end of each step, do the unit tests.

Write unit tests daily. Do not code for days, or worse weeks, and leave unit tests to the end. By that time, you will have lost most of the context. Writing unit tests is inherently dull; it’s a daunting task to write them for a week’s worth of code.


## SonarQube 

SonarQube (formerly Sonar) is an open-source platform developed by SonarSource for continuous inspection of code quality to perform automatic reviews with static analysis of code to detect bugs, code smells, and security vulnerabilities on 20+ programming languages.

Code smell: They refer to any symptom in the source code of a program that possibly indicates a deeper problem.

## CloudBees Core

 Is a continuous delivery solution that provides manageability, security, best practices and supports multiple platforms, teams, and geographical locations. CloudBees Core on modern cloud platforms provides flexible, governed continuous delivery with the high availability and scalability of Kubernetes.


## IIFE

An IIFE, or Immediately Invoked Function Expression, is a common JavaScript design pattern used by most popular libraries (jQuery, Backbone.js, Modernizr, etc) to place all library code inside of a local scope. ... An IIFE protects a module's scope from the environment in which it is placed.

It is a JavaScript function that runs as soon as it is defined. Also known as a Self-Executing Anonymous Function and contains two major parts.

 IIFEs are very useful because they don't pollute the global object, and they are a simple way to isolate variables declarations.

## Closure

A closure gives you access to an outer function's scope from an inner function. In JavaScript, closures are created every time a function is created, at function creation time. To use a closure, define a function inside another function and expose it.

## Use strict directive

It is not a statement, but a literal expression, ignored by earlier versions of JavaScript. The purpose of "use strict" is to indicate that the code should be executed in "strict mode". With strict mode, you can not, for example, use undeclared variables.

## TOGAF

The Open Group Architecture Framework (TOGAF) is an enterprise architecture methodology that offers a high-level framework for enterprise software development. 


TOGAF helps organize the development process through a systematic approach aimed at reducing errors, maintaining timelines, staying on budget and aligning IT with business units to produce quality results.

Like other IT management frameworks, TOGAF helps businesses align IT goals with overall business goals, while helping to organize cross-departmental IT efforts. TOGAF helps businesses define and organize requirements before a project starts, keeping the process moving quickly with few errors.


The Open Group states that TOGAF is intended to:

1. Ensure everyone speaks the same language

2. Avoid lock-in to proprietary solutions by standardizing on open methods for enterprise architecture

3. Save time and money, and utilize resources more effectively

4. Achieve demonstrable ROI.

Different elements of TOGAF are:

BADT:

There are four architectural domains in TOGAF 9.1 that offer specializations for businesses.

i. Business architecture: includes information on business strategy, governance, organization and how to adapt any existing processes within the organization.

ii. Applications architecture: a blueprint for structuring and deploying application systems and in accordance with business goals, other organizational frameworks and all core business processes.


iii. Data architecture: defining the organization’s data storage, management and maintenance, including logical and physical data models.

iv. Technical architecture: also called technology architecture; it describes all necessary hardware, software and IT infrastructure involved in developing and deploying business applications.


## OWASP (Open Web Application Security Project )


OWASP (Open Web Application Security Project) is an organization that provides unbiased and practical, cost-effective information about computer and Internet applications.


The OWASP Top 10 list consists of the 10 most seen application vulnerabilities:

1. Injection.

2. Broken Authentication.

3. Broken Access control.

4. Sensitive data exposure.

5. XML External Entities (XXE)

6. Security misconfigurations.

7. Cross Site Scripting (XSS)

8. Insecure Deserialization.


## HTTP2 

1. Concurrent downloads streamlined within a single TCP connection

2. Enable browsers to fetch crucial assets of a web page first

3. Optimize and improve HTTP header compression

4. And integrating a feature known as 'Server Push' that allows the server to deliver crucial data before the browser asks for it.

## Coverage

https://github.com/kukuu/AGILITY/blob/master/white-paper/architectural-solutions/test-pyramid-coverage%20(1).jpg