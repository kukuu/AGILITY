# Technopedia

## Difference between a data warehouse and a data lake

The main difference between a data warehouse vs. data lake vs. relational database system is that a relational database is used to store and organize structured data from a single source, such as a transactional system, while data warehouses are built to hold structured data from multiple sources.

### Data lake

The biggest advantage of data lakes is flexibility. By allowing the data to remain in its native format, a far greater—and timelier—stream of data is available for analysis. Some of the benefits of a data lake include: Ability to derive value from unlimited types of data.

### Hadoop data lake

A Hadoop data lake is a data management platform comprising one or more Hadoop clusters. It is used principally to process and store nonrelational data, such as log files, internet clickstream records, sensor data, JSON objects, images and social media posts.

### Big data and Data Lake

 Perhaps the greatest difference between data lakes and data warehouses is the varying structure of raw vs. processed data.

 Raw data is data that has not yet been processed for a purpose. Much associated with Data Lake. Because of this, data lakes typically require much larger storage capacity than data warehouses.

## Benefits of REACT

1. Used for Single Page Applications

2. Better Performance - Businesses that use ReactJS are assured of better performance compared to those that use other frameworks - Avoids 2 way binding - Virtual DOM (DIFFING ALGORITHM). 

Because ReactJS helps to prevent updating of DOM, it means that the apps will be faster and deliver better UX. ReactJS was designed to help improve the total rendered pages from the website server.

  Virtual DOM - Any new view changes are first performed on the virtual DOM, which lives in memory and not on your screen. An efficient algorithm (DIFFING ALGORITHM) then determines the changes made to the virtual DOM to identify the changes that need to be made to the real DOM. It then determines the most effective way to make these changes and then applies only those changes to the real DOM. This guarantees a minimum update time to the real DOM, providing higher performance and a cleaner user experience all around.

3. It's used for handling view layer for web and mobile apps. 

4. React also allows us to create reusable UI components.

5. Another React js benefits is its ability to deal with a common search engine failure to read JavaScript-heavy apps. As a solution, React can run on the server, rendering and returning the virtual DOM to the browser as a regular webpage.

6. Speed. Fast and is optimised during compilation.

7. Handle errors at run time during compilation.

8. It’s the V in the MVC – the view part

9. Great Developer Tools

 React Developer Tools, available for Chrome and Firefox, is a browser extension for React. It allows you to inspect the React component hierarchies in the virtual DOM. 

10. JSX produces React “elements” and has a number of side benefits, including helping prevent injection attacks.


## What is JSX

 Basically, JSX is a JavaScript render function that helps you insert your HTML right into your JavaScript code.


 What ia BABEL?

 Babel is a JavaScript compiler. Babel is a toolchain that is mainly used to convert ECMAScript 2015+ code into a backwards compatible version of JavaScript in current and older browsers or environments.


## What are the 5 Scrum ceremonies?

Scrum suggests three roles: The team, ScrumMaster, and product owner; 

four ceremonies: the sprint planning meeting, Daily Scrum, sprint review meeting, and sprint retrospective meeting; 

 three artifacts: the product increment, product backlog, and sprint backlog.


## Principles of Lean Software Development

1. Eliminate Waste.

2. Build Quality In

3. Create Knowledge

4. Defer Commitment

5. Deliver Fast

6. Respect People

7. Optimize the Whole 



## CODE REVIEW


1. Does the code follow SOLID principles

2. Formatting: Where are the spaces and line breaks? Are they using tabs or spaces? How are the curly braces laid out?

3. Style: Are the variables/parameters declared as final? Are method variables defined close to the code where they’re used or at the start of the method?

4. Naming: Do the field/constant/variable/param/class names conform to standards? Are the names overly short?

5. Test coverage: Is there a test for this code?

6. Race conditions

7. What design patterns are used in the new code? Any anti-patterns (in loops etc)


## Attributes of a good leader


1. Honesty and Integrity

2. Creativity and Innovation.

3. Accountability. 

4. Provide Source of INSPIRATION - Inspire Others.

5. Show Commitment and Passion

6. Good Communicator.

7. Have decision-Making Capabilities.

8. Lead by example

9. Delegation and Empowerment. 

10. Clearly defines goals

11. Helps to refine the knowledge base


## ECS and ECR

Amazon Elastic Container Registry (ECR) is a fully-managed Docker container registry that makes it easy for developers to store, manage, and deploy Docker container images. Amazon ECR is integrated with Amazon Elastic Container Service (ECS), simplifying your development to production workflow.


## Tracking the metrics / KPI (of the team)

Keeping track of certain metrics is an important step in making sure your company’s software engineering team is performing as efficiently and productively as possible. Here are some of the most essential metrics for developers to track:

1. Lead time

Lead time is a general measurement of the amount of time that passes from product concept to final delivery. 

2. Impact

Impact measures how much changes to the code affect the overall project. It is also a measurement of how those changes impact the engineers who make them. 

3. Churn

Churn is the percentage of time developers spend editing, adding to, or deleting their own code. A high code churn indicates rework and may mean something is wrong in the development process.

4. Productivity

This measures the amount of each engineer’s efficient code, or code that provides business value. An engineer creating a whole new solution or implementing sweeping code changes will likely deal with lots of trial and error with a low efficiency rate. An engineer who is making a lot of small changes with a low churn rate, however, is likely to have a higher efficiency rate.

4. Cycle time

Cycle time, part of lead time, is how long it takes to make a desired change to the software and put it into production. When a team is using DevOps and employing continuous integration, continuous delivery (CI/CD) practices, they can often measure cycle time in minutes rather than months.

5. Open and close rates

The open and close rate is the number of issues or problems developers report and fix or close over a period of time.

6. Down time analysis

Downtime analysis is a measure of the mean time between failures (MTBF) and mean time to recover/repair (MTTR). This evaluates how well software performs in a production environment.



## HIGH Performing engineering team

The Leader:

1. Drives goal execution and are a catalyst for team performance

2. Sets the bar for performance

3. Sets the tone

4. Communicate goals


The team:

1. People have solid and deep trust in each other and in the team's purpose - they feel free to express feelings and ideas

2. Everybody is working toward the same goals.

2. A quick turn around 

3. Minimum or no down time

3. A good ROI

4. Meeting deadlines, and hiting targets from planning

5. Achieving definition of done,(DoD) over SPRINT period. From requirement gathering to production.

6. Managing low fault levels. Less or minimum  return rates/complaints/bugs from users

7. Accountable for end to end delivery of the products and services. Holding each one responsible.


## SPRINT BURN DOWN CHARTS

The Sprint Burndown Chart makes the work of the Team visible. It is a graphic representation that shows the rate at which work is completed and how much work remains to be done over the SPRINT period. The chart slopes downward over Sprint duration and across Story Points completed.

The outstanding work (or backlog) is often on the vertical axis, with time along the horizontal. That is, it is a run chart of outstanding work. It is useful for predicting/forecasting when all of the work will be completed

## SPRINT BURN UP CHARTS

Burn up chart shows how much work has been completed, and the total amount of work.

## ES5/ES6 

Features: 

Template strings

Destructuring 

Arrow functions

Setting Defaults

Block scopped - let/const 

Promises 

Spread operators

Generator functions 

Classes 

module imports

## REACT Life Cycle states

Lifecycle methods (with the exception of constructor) are hard to reason about. They add complexity to your app. Don’t use them unless you must.

1. Mounting

constructor:

The first thing that gets called is your component constructor, if your component is a class component. This does not apply to functional components.

Most Common Use Case For Constructor: Setting up state, creating refs and method binding.

2. getDerivedStateFromProps 

When mounting, getDerivedStateFromProps is the last method called before rendering.


3. render

Rendering does all the work. It returns the JSX of your actual component. When working with React, you’ll spend most of your time here.

Most Common Use Case For Render: Returning component JSX.

4. componentDidMount

After we’ve rendered our component for the first time, this method is called.

If you need to load data, here’s where you do it. Don’t try to load data in the constructor.

Most Common Use Case for componentDidMount: Starting AJAX calls to load in data for your component.

5. getDerivedStateFromProps

If you need to update your state based on a prop changing, you can do it here by returning a new state object.

Here’s some examples:

i. resetting a video or audio element when the source changes
ii. refreshing a UI element with updates from the server
iii. closing an accordion element when the contents change


Note: Even with the above cases, there’s usually a better way to do it. But getDerivedStateFromProps will have your back when worst comes to worst.

6. shouldComponentUpdate

Typical React dogma says that when a component receives new props, or new state, it should update.

But our component is a little bit anxious and is going to ask permission first.

Here’s what we get — a shouldComponentUpdate method, called with nextProps as the first argument, and nextState is the second.

shouldComponentUpdate should always return a boolean. If you’re worried about wasted renders, (i.e Age authentication) shouldComponentUpdate is an awesome place to improve performance.


7. getSnapshotBeforeUpdate


Note it’s called between render and the updated component actually being propagated to the DOM. It exists as a last-chance-look at your component with its previous props and state.

You should either return null or a value from getSnapshotBeforeUpdate.

Most Common Use Case: Taking a look at some attribute of the current DOM, and passing that value on to componentDidUpdate.

8. componentDidUpdate

Now, our changes have been committed to the DOM.

In componentDidUpdate, we have access to three things: the previous props, the previous state, and whatever value we returned from getSnapshotBeforeUpdate.

Most Common Use Case for componentDidUpdate: Reacting  to committed changes to the DOM.

9. componentWillUnmount

Your component is going to go away. Maybe forever. It’s very sad.

Before it goes, it asks if you have any last-minute requests.

Here you can cancel any outgoing network requests, or remove all event listeners associated with the component.


10. getDerivedStateFromError

i.e Something broke. Not in your component itself, but one of its descendants.

11. ComponentDidCatch

It is triggered when an error occurs in a child component.

The difference is rather than updating state in response to an error, we can now perform any side effects, like logging the error.


12. Note that componentDidCatch only works for errors in the render/lifecycle methods. If your app throws an error in a click handler, it will not be caught.

Most Common Use Case for componentDidCatch: Catching and logging errors.


## OutSystems platform

OutSystems is a low-code platform for the development of enterprise web and mobile applications, which run in the cloud, on-premises or in hybrid environments. The current version is 11, for both the paid and unpaid versions - developers are permitted personal cloud environments to use the platform without charge.

## JavaScript Design Patterns - https://scotch.io/bar-talk/4-javascript-design-patterns-you-should-know    

Developermust  strive to write maintainable, readable, and reusable code. Code structuring becomes more important as applications become larger. Design patterns prove crucial to solving this challenge - providing an organization structure for common issues in a particular circumstance.


i. Module Design Pattern

ii. Prototype Design Pattern

iii. Observer Design Pattern

iv. Singleton

### Module Design Pattern

JavaScript modules are the most prevalently used design patterns for keeping particular pieces of code independent of other components. This provides loose coupling to support well-structured code.


For those that are familiar with object-oriented languages, modules are JavaScript "classes". One of the many advantages of classes is encapsulation - protecting states and behaviors from being accessed from other classes. The module pattern allows for public and private (plus the lesser-know protected and privileged) access levels.

Modules should be Immediately-Invoked-Function-Expressions (IIFE) to allow for private scopes - that is, a closure that protect variables and methods (however, it will return an object instead of a function). This is what it looks like:

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

## DroneDeploy 

Is the leading cloud software platform worldwide for drone mapping and 3D modeling. The DroneDeploy mobile app allows you to fly your drone to make interactive maps and models. ... It works with many DJI drones such as Phantom 3, Phantom 4, Inspire 1 and 2, Mavic Pro, Matrice 100, 200 and 600 models.3 Mar 2019
