
# What is BDD?

Behavioral Driven Development (BDD) is a software development approach that has evolved from TDD (Test Driven Development) but differs by being written in a shared language, which improves communication between tech and non-tech teams and stakeholders. In both development approaches, tests are written ahead of the code, but in BDD, tests are more user-focused and based on the system’s behavior.


## Choosing BDD

TDD works well, as long as the business owner is familiar with the unit test framework being used and their technical skills are strong enough, which is not always the case. In these circumstances, BDD has the advantage because the test cases will be written in a common language used by the stakeholders such as, for example, English. This access to better communication is probably the biggest advantage to using BDD, making it possible for collaboration between the technical and non-technical teams to run with improved efficiency.


## Characteristics of BDD

As described above, the advantage to BDD test cases being written in a common language is that details of how the application behaves can be understood by all. For example, test cases can be written so as to explain the behavior of the system, using real-time examples of the actual requirements.


## Essentials to have in place before implementing BDD

Requirements should be converted into user stories that can define concrete examples.
Each example should be a valid user scenario, rather than a mere test case.
An understanding of the ‘role-feature-reason’ matrix and the ‘give-when-then’ formula.
An awareness of the need to write ‘the specification of the behavior of a class’ rather than ‘the unit test of a class’.


## The ‘Given-When-Then’ formula BDD example

This is the proposed template for writing BDD test cases for a user story. It can be defined as:-

Given a certain scenario

When an action takes place


...............................


Then this should be the outcome.

A practical example would be:-


....................................


Given the User has not entered any data on the form


When they click the submit button


Then proper validation messages should be show.


## Role-Feature-Reason matrix

This template is also used in BDD, in order to aid user story creation. This template is defined as:-

As a

I want

So that

An example of such a user story would be: – 

As a retail customer, I want to return an electronic merchandise within 14 days, so that refund will be processed


## BDD Tools

### Cucumber

Cucumber is a test framework that supports BDD. In Cucumber, the BDD specifications are written in plain, simple English which is defined by Gherkin language. In other words, Gherkin is a language that Cucumber understands. Gherkin presents the behavior of the application used, from which Cucumber can generate the acceptance test cases. Cucumber is a framework developed by Ruby that can work across different technologies.


### Specflow

Specflow evolved from the Cucumber framework using Ruby on Rails, and is used mainly for .Net projects. SpecFlow also uses the Gherkin language.


## Some benefits to using BDD

If you plan to implement BDD, here are a few points that will benefit the software team.
You are no longer defining ‘test’, but are defining ‘behavior’.
There’s better communication between developers, testers, product owners.
Because BDD is explained using simple language, the learning curve will be much shorter.
Being non-technical in nature, it can reach a wider audience.
The behavioral approach defines acceptance criteria prior to development.


## Downfall of BDD

Even the best development approaches can have pitfalls and BDD is no exception. Some of them are:

To work in BDD, prior experience of TDD is required.

BDD is incompatible with the waterfall approach.

If the requirements are not properly specified, BDD may not be effective.

Testers using BDD need to have enough technical skills.


## Working with BDD

https://github.com/kukuu/CI-CD-pipeline-with-Jenkins/tree/master/BDD
