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

4. Provide Source of Inspiration - Inspire Others.

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


## SPRINT BURN DOWN CHARTS - KPI Measurement.

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

The first thing that gets called is your component constructor, if your component is a class component. This does not apply to functional components i.e REACT Hooks.

Most Common Use Case For Constructor: Setting up state, creating refs and method binding.

2. getDerivedStateFromProps 

When mounting, getDerivedStateFromProps is the last method called before rendering.
If you need to update your state based on a prop changing, you can do it here by returning a new state object.

Here’s some examples:

i. resetting a video or audio element when the source changes
ii. refreshing a UI element with updates from the server
iii. closing an accordion element when the contents change


Note: Even with the above cases, there’s usually a better way to do it. But getDerivedStateFromProps will have your back when worst comes to worst.


3. render

Rendering does all the work. It returns the JSX of your actual component. When working with React, you’ll spend most of your time here.

Most Common Use Case For Render: Returning component JSX.

4. componentDidMount

After we’ve rendered our component for the first time, this method is called.

If you need to load data, here’s where you do it. Don’t try to load data in the constructor.

Most Common Use Case for componentDidMount: Starting AJAX calls to load in data for your component.


5. shouldComponentUpdate

Typical React dogma says that when a component receives new props, or new state, it should update.

But our component is a little bit anxious and is going to ask permission first.

Here’s what we get — a shouldComponentUpdate method, called with nextProps as the first argument, and nextState is the second.

shouldComponentUpdate should always return a boolean. If you’re worried about wasted renders, (i.e Age authentication) shouldComponentUpdate is an awesome place to improve performance.


6. getSnapshotBeforeUpdate


Note it’s called between render and the updated component actually being propagated to the DOM. It exists as a last-chance-look at your component with its previous props and state.

You should either return null or a value from getSnapshotBeforeUpdate.

Most Common Use Case: Taking a look at some attribute of the current DOM, and passing that value on to componentDidUpdate.

7. componentDidUpdate

Now, our changes have been committed to the DOM.

In componentDidUpdate, we have access to three things: the previous props, the previous state, and whatever value we returned from getSnapshotBeforeUpdate.

Most Common Use Case for componentDidUpdate: Reacting  to committed changes to the DOM.

8. componentWillUnmount

Your component is going to go away. Maybe forever. It’s very sad.

Before it goes, it asks if you have any last-minute requests.

Here you can cancel any outgoing network requests, or remove all event listeners associated with the component.


9. getDerivedStateFromError

i.e Something broke. Not in your component itself, but one of its descendants.

10. ComponentDidCatch

It is triggered when an error occurs in a child component.

The difference is rather than updating state in response to an error, we can now perform any side effects, like logging the error.


 Note that componentDidCatch only works for errors in the render/lifecycle methods. If your app throws an error in a click handler, it will not be caught.

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

## DroneDeploy 

Is the leading cloud software platform worldwide for drone mapping and 3D modeling. The DroneDeploy mobile app allows you to fly your drone to make interactive maps and models. ... It works with many DJI drones such as Phantom 3, Phantom 4, Inspire 1 and 2, Mavic Pro, Matrice 100, 200 and 600 models.3 Mar 2019


## Traits of good Line Management & Essential Management  skills

Qualities of good line management:
1. Communicate well, be clear on vision to meet the needs of  both their employees  and bosses.
2. Emotional stability 
3. Enthusiasm 
4. Self assurance 
5. The understanding by a manager that members of a team strive to reach  their own personal  goals, as well as their teams.
6. Finding time for team members to discuss their strength and work on their weaknesses. 
7. Empathy allows one to identify gaps.
8. When you  work in a team it gives you sense of belonging.


Essential Management  skills:

1. Planning
2. Communication 
3. Decision making 
4. Delegation
5. Problem solving
6. Motivation - https://github.com/kukuu/AGILITY/blob/master/motivation.md
7. Demo strait g appropriate style of Management - https://github.com/kukuu/AGILITY/blob/master/ManagementStyles-InfluencingSkills.md


## Five Essential Project Management Skills

Communication. One of the most important skills for project managers is great communication. ...
Time Management. The ability to manage time and prioritize tasks is an essential characteristic of efficient project managers. ...
Organizational Awareness. ...
Problem Solving. ...
Leadership.

## Influencing

Effective leaders don’t just command; they inspire, persuade, and encourage. Leaders tap the knowledge and skills of a group, point individuals toward a common goal, and draw out a commitment to achieve results.

To influence one needs to be clear about own goals, values, assertive and have a dynamic model to meet the challenges of the technology changing market. This requires an aggregation of a network of skills, a dynamic model and flexible governance.

The goal is to influence others, not manipulate them. Effective, ethical leaders use different approaches in different situations. Leaders need to understand why they are doing something, and be clear about their own values and goals when applying their influence skills. Influencing then comes from a place of authenticity and has the greatest impact.

## Management Styles

Different types of leadership styles exist in work environments. The culture and goals of an organization determine which leadership style fits the firm best, while personality differences often dictate which is most often used. Some companies offer several leadership styles within the organization, dependent upon the necessary tasks to complete and departmental needs.

### The Laissez-Faire Leader

A laissez-faire leader lacks direct supervision of employees and fails to provide regular feedback to those under his supervision. 

### The Autocrat

The autocratic leadership style allows managers to make decisions alone without the input of others. This leadership style benefits employees who require close supervision. Creative employees who thrive in group functions detest this leadership style.

### The Participative Leader

Often called the democratic leadership style, participative leadership values the input of team members and peers, but the responsibility of making the final decision rests with the participative leader.

Participative leadership boosts employee morale because employees make contributions to the decision-making process. It causes them to feel as if their opinions matter. 

### The Transactional Leader

Managers using the transactional leadership style receive certain tasks to perform and provide rewards or punishments to team members based on performance results. Managers and team members set predetermined goals together, and employees agree to follow the direction and leadership of the manager to accomplish those goals. The manager possesses power to review results and train or correct employees when team members fail to meet goals. Employees receive rewards, such as bonuses, when they accomplish goals.

### The Transformational Leader

The transformational leadership style depends on high levels of communication from management to meet goals. Leaders motivate employees and enhance productivity and efficiency through communication and high visibility and empowerment. This style of leadership requires the involvement of management to meet goals. Leaders focus on the big picture within an organization and delegate smaller tasks to the team to accomplish goals.

## Continuous Delivery (RRASc)

Reliable :: Repeatable :: Automation :: Source control
CD is the ability to get changes of all types including new features, configuration changes, bug fixes and experiments into production, or into the hands of users, safely and quickly in a sustainable way.

A logical extension of Continuous Integration, It is based on the use of smart automation. This is all about creating a repeatable and reliable process for delivering software. You have to automate pretty much everything in order to be able to achieve continuous delivery. Manual steps will get in the way or become a bottleneck. This goes for everything from requirements authoring to deploying to production.

The ultimate goal of continuous delivery is to minimise the iteration time of the code-test-deliver-measure experimentation cycle. Increasing deliverable throughput in this way is the key to not only more feature work being delivered but higher quality code as well. This might seem counter-intuitive at first but code is fixed and polished through that same cycle and less time spent on deployment is more time spent on designing quality code. - https://github.com/kukuu/AGILITY 


## How to motivate your team

Teams are the way that most companies get important work done. When you combine the energy, knowledge, and skills of a motivated group of people, then you and your team can accomplish anything you set your minds to.

Hi-lighted below are some mistakes leaders make that drive away their top talent. Rule of thumb, "Reflect on your behavior, fix these mistakes, and get ready to boost your team performance and motivation."
1. Pay your people what they are worth

When you set your employees' salaries, be sure that their pay is consistent with what other companies in your industry and geographic area are paying. Remember: 26 percent of engaged employees say that they would leave their current job for just a 5 percent increase in pay. Don't lose great people because you're underpaying them.

2. Provide them with a pleasant place to work

Everyone wants to work in an office environment that is clean and stimulating, and that makes them feel good instead of bad. You don't have to spend a lot of money to make an office a more pleasant place to be.

3. Offer opportunities for self-development

The members of your team will be more valuable to your organization, and to themselves, when they have opportunities to learn new skills. Provide your team with the training they need to advance in their careers and to become knowledgeable about the latest technologies and industry news.

4. Foster collaboration within the team

Encourage the members of your team to fully participate by inviting their input and suggestions on how to do things better. Ask questions, listen to their answers, and, whenever possible, implement their solutions. Ensure retrospectives are continuously engaged.

5. Encourage happiness

Happy employees are enthusiastic and positive members of the team, and their attitude is infectious. Keep an eye on whether or not your people are happy with their work, their employer, and you. If they're not, you can count on this unhappiness to spread.

4. Don't punish failure

We all make mistakes. It's part of being human. The key is to learn valuable lessons from those mistakes so we don't make them again. When members of your team make honest mistakes, don't punish them--instead, encourage them to try again. Note the principle of fail fast in Agile.

5. Set clear goals

Sizeable amount of Employees have reported that they wasted time at work because they weren't aware of what work was a priority, and what wasn't. As a leader, it's your job to work with the members of your team to set clear goals. And once you do that, make sure everyone knows exactly what those goals are, what their relative priority is, and what the team's role is in reaching them.

6. Don't micromanage

No one likes a boss who is constantly looking over her shoulder and second-guessing her every decision. Sizeable percent of employees have reported that they would rather take on unpleasant activities than sit next to a micromanaging boss. Provide your people with clear goals, and then let them figure out the best way to achieve them.

7. Avoid useless meetings

Meetings can be an incredible waste of time--the average professional wastes 3.8 hours in unproductive meetings each and every week. Create an agenda for your meetings and distribute it in advance. Invite only the people who really need to attend, start the meeting on time, and then end it as quickly as you possibly can.


## Steps to Helping Your Team Advance

1. Discuss Goals. The first step is to sit down with each team member and discuss her desired career goals. 

2. Identify Your Team's Development Gaps.

3. Establish Specific Training Objectives. 

4. Celebrate and Make it Fun.

## Essential Steps to Develop Your Team

1. Ensure that each person truly understands their role.

2. Provide training and development tools. 

3. Step away and let them do their job. 

4. Meet with team members regularly to discuss goals. ...

5. Game plan for their growth.


## Straightforward strategies to help improve teamwork in your startup today:

1. Lead by example.

2. Build up trust and respect.

3. Encourage socializing.

4. Cultivate open communication.

5. Clearly outline roles and responsibilities.

6. Organize team processes.

7. Set defined goals.

8. Recognize good work.


## Factors of Successful Teams: The Keys to Ensure High Team Performance

1. Domain Knowledge


2. Cohesiveness -  The first factor to consider is how cohesive members are with one another.

Once a team is highly cohesive, a member’s commitment and willingness to strive for excellence thrives. Team cohesion affects the extent to which members like one another, get along with each other, and trust and respect one another’s abilities and opinions. 

Although these characteristics are difficult to observe, managers can look for signs that team members are well-acquainted past superficial meet-and-greet topics. Managers can also determine whether team members equally participate in group discussions and activities rather than forming cliques or subgroups of cohesive units.

3. Communication -  Efficient communication mechanisms are crucial to develop effective teams.

4. Groupthink -  This is when a group in a team tend to suppress the thinking and development of others.

Other signs of groupthink include individual conformity, apathy toward team goals and outcomes, peer-pressure exerted by leaders within the team, and discussions that tend to be one-sided.

5. Homogeneity -  Having the right ballanced composed members in the team. 

It is the extent to which members are similar or different to one another. The difficulty for most project managers is finding the right balance between overly homogenous and overly heterogeneous teams. When evaluating team homogeneity, a manager can consider similarities and differences in personal characteristics, education, skills, abilities, generational backgrounds, cultural background, and income levels.

6. Role Identity -  Role identity is the extent to which members are capable of assuming different roles throughout the team structure, thus diversifying efforts and developing subject matter experts. Delegating by having experts in different disciplines . Empowerment. 

7. Stability -  Teams that have higher turnover rates experience higher levels of group cohesion, better communication methods, and more effective role identity.

8. Team Size - By evaluating a team’s size, managers are able to maximize productivity to ensure high levels of team performance. The greater number of members within a team the more resources available to achieve a goal. However, as team size increases, so does the number of conflicts resulting in decreased levels of cohesion and inefficient productivity. To evaluate whether a team is too large or small, managers must consider how effectively and harmoniously members work together and whether the required tasks are being efficiently accomplished by all members of the team.

## Team building objectives

1. Learn to work as a team

2. Re-assess your team's goals and direction

4. Communicate better as a team

5. Give your team a boost of energy

6. Create trust amongst team members

7. Recognise individual strengths, styles and skills

8. Keep lines of communication flexible

9. Ensure tolerance

10. Encourage sharing of ideas

11. Allow for differences


## Achieving CD

Automation::Reliable::Elastic::Traceable
Repeatable, Automation, Source Control

1. The process for releasing/deploying software MUST be repeatable and reliable. 

2. Automate everything!

3. If somethings difficult or painful, do it more often.

4. Keep everything in source control

5. Done means “released”.

6. Build quality in! 

7. Everybody has responsibility for the release process

8. Improve continuously

## Micro-services

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

iv. Need to mitigate performance

v. Log monitoring

## Seeting up a  microservice team

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

## Containerisation

Source code of any program cannot fully describe the function of that program without the context it will be compiled and run in. Most unexpected behaviour during deployment comes from build environments being different than expected. To make deployment repeatable, we need to make a program’s context repeatable. That’s where Docker and Kubernetes comes in.

Docker essentially allows you to specify a “source code” for a program’s context that can then be “compiled” to an image and run as a container. This means that once we have tested an image we can have high confidence that it will perform equally well in every environment it is deployed to.

Additionally, Docker allows you to specify deploy configurations made up of multiple containers all linked in a private network and DNS that allows services that depend strongly on each other to be deployed and scaled together.

To be fully context-agnostic, deployment should be able to happen to any host on the network on whatever port the host happens to have free. This presents a challenge: how do services link up when their network locations are fluid? You need a reverse proxy (like nginx) and a way to keep its configuration up to date in a changing service landscape. You will need a Consul to store and manage service states.

## Deployment steps for Docker Container:

1.	Build Docker image.

2.	Test that image in isolation.

3.	Push that image to the in-house image registry.

4.	Pull all images you need to deploy linked.

5.	Deploy them to a test environment.

6.	Run automated tests against the container system.

7.	Upload service configuration to Consul API (if changed).

8.	Deploy the containers to all hosts, tagged with the offline colour.

9.	Wait until they are all responding and passing automated checks.

10.	Flip environment alias to point at the offline colour.

11.	The new build is now online.

## Docker File:  Configuration infrastructure code

```
FROM node: latest

COPY . /src

WORKDIR  /src

RUN npm install --production

EXPOSE 3000

CMD  npm start

```


## Micro-service Docker Compose file - For a NodeJS Micro-service

```
version: '3'

services: 
    web: 
      build: './web'
      ports:
        - "3000: 3000"

    serach: 
      build: './serach'
      ports:
        - "3001: 3000"
      depends_on: 
        - db
      environment: 
        - MONGO_DB_URI = mongo://db/microservices

    books: 
      build: './books'
      ports: 
        - "3002: 3000"
      depends_on: 
        - db
      environment: 
        - MONGO_DB_URI=mongodb://db/microservices

    videos:
      build: './videos'
      ports: 
        - "3003: 3000"
      depends_on: 
        - db
      environment: 
        - MONGO_DB_URI = mongo://db/microservices

    db: 
      image: mongo:latest
      ports: 
        - "27018:27018"

    nginx: 
      image: nginx:latest
      ports: 
        - "8080"
      volumes: 
        - ./web/public:/svr/www/static
        -  ./default/.conf:/etc/nginx/conf.d/default.conf
      depends_on:
          - web
          - serach
          - books
          - videos

```

## Web Services

A web service is a collection of open protocols and standards used for exchanging data between applications or systems over the internet and uses a standardized XML messaging system. XML is used to encode all communications to a web service. For example, a client invokes a web service by sending an XML message, then waits for a corresponding XML response.

As all communication is in XML, web services are not tied to any one operating system or programming language - Java can talk with Perl; Windows applications can talk with Unix applications.

Web services are self-contained, modular, distributed, dynamic applications. These applications can be local, distributed, or web-based. Web services are built on top of open standards such as TCP/IP, HTTP, Java, HTML, and XML.

## Differences between SOA and Micro-services

The core difference between SOA and microservices lies in the size and scope. Microservices must be independently deployable, whereas SOA services are often implemented in deployment monoliths. Classic SOA is more platform driven, so microservices offer more choices in all dimensions.

Features of SOA:

1. Boundaries are explicit

2. Services are autonomous

3. Services share schema and contract, not class

4. Service compatibility is based on policy


## Cloud Computing - Architecting for High Availability

1. Design for Failure - Horizontal scaling : Elastic IPs, EBS, EC2, Cloud Watch

2. Multiplle Availability Zones - Offset natural disaster (Low prone disaster zones)

3. Scaling

4. Loose Coupling

5. Self Healing (Policy - Responsive to Peaks[Calculated and abrupt])


## Functional and NFR (Non functional requirements)

1. Functional

Functional requirement (FR) focus on the behavioral aspects.

2. NFR

NFRs are the requirements defined to cover the operational aspects of a product or an app.

Efficiency 

Portability 

security 

Reliability 

Usability

Caching

## Cloud Architectures

1. SaaS (Software as a Service) applications are designed for end-users, delivered over the web.

SaaS is a software distribution model in which applications are hosted by a vendor or service provider and made available to customers over a network, typically the Internet.

With Saas model you are provided with access to application softwares often referred to as on-demand softwares. You don't have to worry about the installation, setup and running of the application. Service provider will do that for you. You just have to pay and use it through some client.

Example: Google Apps, Microsoft Office 365.


2. PaaS

PaaS (Platform as a Service) is the set of tools and services designed to make coding and deploying those applications quick and efficient over the Internet.

The model is a category of cloud computing services that provides a platform allowing customers to develop, run, and manage web applications without the complexity of building and maintaining the infrastructure typically associated with developing and launching an app - via the browser.

Examples: AWS Elastic Beanstalk, Windows Azure, Heroku, Force.com, Google App Engine, and Apache Stratos. IaaS (Infrastructure as a Service), is the hardware and software that powers it all – servers, storage, networks, operating system.


3. IaaS

IaaS provides you the computing infrastructure, physical or (quite often) virtual machines and other resources like virtual-machine disk image library, block and file-based storage, firewalls, load balancers, IP addresses, virtual local area networks etc.

Examples: Amazon EC2, Windows Azure, Rackspace, Google Compute Engine. Additional points to note:

AWS(Amazon web services) is a complete suite which involves a whole bunch of useful web services. Most popular are EC2 and S3 and they belong to IaaS s

Windows Azure is both a PaaS and IaaS.


## DevOps

DevOps is a software development approach which involves continuous development, continuous testing, continuous integration, continuous deployment, and continuous monitoring of the software throughout its development lifecycle.

Meanwhile, in every step, if there is an error, you can shoot an email back to the development team so that they can fix it. Then they will push it into the version control system and it goes back into the pipeline.

Using Jenkins 

From Git, Jenkins pulls the code and then Jenkins moves it into the commit phase, where the code is committed from every branch. The build phase is where we compile the code. If it is Java code, we use tools like maven in Jenkins and then compile that code, which can be deployed to run a series of tests. These test cases are overseen by Jenkins again.

Then, it moves on to the staging server to deploy it using Docker. After a series of unit tests or sanity tests, it moves on to production.

Docker is just like a virtual environment in which we can create a server. It takes a few seconds to create an entire server and deploy the artifacts we want to test. But here the question arises:

Why do we use Docker?

As we said earlier, you can run the entire cluster in a few seconds. We have a storage registry for images where you build your image and store it forever. You can use it anytime in any environment which can replicate itself.

## Continuous Integration and Continuous Delivery

1. Maintain a code repository.

2. Automate your build.

3. Make your build self-testing.

4. Daily commits to the baseline by everyone on the team.

5. Every commit (to the baseline) should be built.

6. Keep your builds fast.

7. Clone the production environment and test there.

## Quicksort 

This is one of the most efficient methods for sorting an array in computer science.

Quicksort works by picking an element from the array and denoting it as the “pivot.” All other elements in the array are split into two categories — they are either less than or greater than this pivot element.

Each of the two resulting arrays (array of values less-than-the-pivot and array of values greater-than-the-pivot) is then put through that very same algorithm. A pivot is chosen and all other values are separated into two arrays of less-than and greater-than values.

Eventually, a sub-array will contain a single value or no value at all, as there will be no more values with which to compare it. The rest of the values were all denoted to be “pivots” at some previous point and did not trickle down to this lowest sub-array. At that point, the values will be sorted, as all values have now been declared as less than or greater than all other values in the array.

## Using es6 Spread operator

```
export default function sum(...figures) {
  return figures.reduce((total, current) => {
    return total + current;
  });
}

```

## JAM Stack

JAMSTACK  is a set of best practices and not a technology.
Focuses on Build Time Rendering (changes responsibility of the backend). Other than Server Side. No need for backend to (publish) server side  rendering. The backend will contune to focus on the API Layer

Technologies: Gatsby, GraphQL (gives a consistent API Layer). Keeps the Backend decoupled from the backend. No worries abot passing JSON up and down. You can configure the plugins for GrphQL to do this.

Great for Blogs, eCommerce, Static Contents


Downsides of JAM Stack
i. Not good for Big DATA and Analytics
ii. Not good for Real Time Systems
iii. Non Developer interactions


## REFS in REACT

refs are used to get reference to a DOM(Document Object Model) node or an instance of a component in a React Application i.e. refs would return the node we are referencing .

## Monolith to Microservice - Strategy


Note any changes should not change the user experience. Just the underlying architecture. Changing architecture can allow the product serve multiple channels, IMPROVE USER EXPERIENCE AND ENHANCE EFFICIENCY.


1. Define Business context

2. Security

3. Technology

4. Architecture

5. Configuration Management

6. Monitoring

7. Aggregating logs

8. Deployment

9. Documentation

.................

Implementation

In the conversion we use a dispatcher proxy to the monolithic (legacy system) to capture requests and direct it to the micro-service
ii. Use Apache config file to do re-write rule for the new urls (end points) - Apache's re-write engine switched on. Each URL with a string in it will be re-written.


## Typescript

Modules in typescript are loaded on demand. This enhances efficiency. Module loaders are hence required i.e SystemJS,RequireJS, Webpck, CommonJS.

Some Typecsript features

- Classes
- Properties
- Methods
- Implementing Inheritance and Interfaces
- Import and Export
- Loading modules using module loader (System loading - On Demand Loading)

Data Types

- number 
- string 
- boolean 
- enum 
- void 
- null 
- undefined 
- any 
- never 
- Array 
- tuple 

## Data-driven 

Data-driven approach is when a team makes strategic decisions based on data analysis and interpretation, rather than by intuition or by personal experience. The process of democratising data means making data accessible to as many people as possible within a company.

-  Data-driven learning: A learning approach driven by research-like access to data. 

- Data-driven science, an interdisciplinary field of scientific methods to extract knowledge from data.


## Parcel

An out of the box support for JS, CSS, HTML, file assets, and more (perfect for React)

## Apollo GraphQL

Apollo Client is a fully-featured caching GraphQL client with integrations for React, Angular, and more. It allows you to easily build UI components that fetch data via GraphQL. ... Apollo Client can be used in any JavaScript frontend where you want to use data from a GraphQL server.

The client is designed to help you quickly build a UI that fetches data with GraphQL, and can be used with any JavaScript front-end.