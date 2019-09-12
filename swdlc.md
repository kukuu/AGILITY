# Software Development Life Cycle (SDLC)


There are various software development approaches defined and designed which are used/employed during development process of software, these approaches are also referred as “Software Development Process Models” (e.g. Waterfall model, incremental model, V-model, iterative model, RAD model, Agile model, Spiral model, Prototype model etc.). Each process model follows a particular life cycle in order to ensure success in process of software development.

Software life cycle models describe phases of the software cycle and the order in which those phases are executed. Each phase produces deliverables required by the next phase in the life cycle. Requirements are translated into design, through architecture. Code is produced according to the design which is called development phase. Coding and  testing (in parallel) verifies the deliverable of the implementation phase against requirements. The testing team follows Software Testing Life Cycle (STLC) which is similar to the development cycle followed by the development team.

The SWDLC is preceeded by evaluating the contexts of Business goals, determining Quality attributes (Performance, Scalability, Security, Quality, Extensibility and Governance), and the Architecture.

There are following  phases in every Software development life cycle model:

```

1. Requirement gathering and analysis

2. Architecture

3. Design

4. Implementation or coding

5. Testing

6. Deployment

7. Maintenance / After care support

8. Continuous Improvement

```

## Requirement gathering and analysis

Requirement gathering and analysis:  Business requirements are gathered in this phase. This phase is the main focus of the project managers and stake holders. Meetings with managers, stake holders and users are held in order to determine the requirements like; 

```
1. Who is going to use the system? 

2. How will they use the system?  

3. What data should be input into the system?  

4. What data should be output by the system?  

```

These are general questions that get answered during a requirements gathering phase. After requirement gathering these requirements are:

```

1. Analyzed for their validity

2. The possibility of incorporating the requirements in the system to be development is also studied.

3. Finally, a Requirement Specification document is created which serves the purpose of guideline for 
the next phase of the model. 

4. The testing team follows the Software Testing Life Cycle and starts the Test Planning phase after 
the requirements analysis is completed.

```

## Design  

In this phase the system and software design is prepared from the requirement specifications which were studied in the first phase. System Design which is a derivative from the Architecture, helps in specifying hardware and system requirements and also helps in defining overall system architecture. The system design specifications serve as input for the next phase of the model.

In this phase the testers comes up with the Test strategy, where they mention what to test, how to test.

## Implementation or coding

Implementation / Coding:  On receiving system design documents, the work is divided in modules/units and actual coding is started. Since, in this phase the code is produced so it is the main focus for the developer. This is the longest phase of the software development life cycle.

For code integrity, security (SNYK) and upholding quality, reliability, portability and extensibility of the software Agile practices like TDD, BDD, CI/CD, Containerization (Docker), and Orchestrations(Kubernets) can be adopted.

This process will involve: Planning, Breaking feature stories into units, estimation, coding, SCRUM, code reviews, SPRINT reviews, retrospectives, and grooming. Other methodologies that can possibly adopted depending on business goals are include Waterfall, XP

## Testing 

Testing:  Quality Analysis and Testing is embeded into the code as is being developed. This is Agile Testing, using CI/CD. The code  is tested against the requirements to make sure that the product is actually solving the needs addressed and gathered during the requirements phase, together with the Architecture producing the code structure (with inherent identified disciplines, technical decisions and patterns). During this phase all types of functional testing like unit testing, integration testing, system testing, smoke testing, acceptance testing are done as well as non-functional testing are also done - black box(UI Testing) and white box testing.

Test Pyramid with coverage - https://github.com/kukuu/AGILITY/blob/master/test-pyramid-coverage.jpg 

Code Coverage - https://github.com/kukuu/AGILITY/blob/master/unit-test/code-coverage-fig-1.png 

Agile Software Testing Cycle - https://github.com/kukuu/AGILITY/blob/master/software-testing-life-cycle.md

### Tools

#### Selenium

Selenium is a portable framework for testing web applications. Selenium provides a playback (formerly also recording) tool for authoring functional tests without the need to learn a test scripting language (Selenium IDE).

Using Selenium type of testing can be done are:

Functional Testing.

Regression Testing.

Sanity Testing.

Smoke Testing.

Responsive Testing.

Cross Browser Testing.

UI testing (black box)

Integration Testing.


#### jMeter


Apache JMeter is open source software, a 100% pure Java desktop application, designed to load test functional behavior and measure performance of web sites. It was originally designed for load testing web applications but has since expanded to other test functions.


#### JUnit

Junit is widely used testing framework along with Java Programming Language. You can use this automation framework for both unit testing and UI testing.it helps us define the flow of execution of our code with different Annotations.7 D


## Deployment 

After successful testing the product is delivered / deployed to the customer for their use.

As soon as the product is given to the customers they will first do the beta testing. If any changes are required or if any bugs are caught, then they will report it to the engineering team. Once those changes are made or the bugs are fixed then the final deployment will happen.

## Maintenance / After care support:

 Once when the customers starts using the developed system then the actual problems comes up and needs to be solved from time to time. This process where the care is taken for the developed product is known as maintenance.
 
 ## Unveiling CADMA practicing methodology
 (Blue print & Copy right).
 
