
# Integration Testing in CI

Traditionally, integration testing happened between unit testing and validation testing. That model fits well in a waterfall environment, where the development phases are clear and distinct.

Continuous integration (CI)  relies on the following best practices being in place:

1. Maintain a code repository.

2. Automate the build.

3. Make the build self-testing.

4. Everyone commits to the baseline every day.

5. Every commit (to baseline) should be built.

6. Keep the build fast.

7. Test in a clone of the production environment.


## Strategy you could consider for your testing regime:

1. Run integration tests until something fails

2. Determine what needs to be added or modified

3. Drill down into unit testing

4. Go back to integration testing once your unit tests pass

5. Repeat the process until your tests pass end-to-end


## How to apply strategy

[Comming soon]



## Best practices for continuous integration

The following best practices should help you in your quest for a smoother continuous integration process.

1. Do integration testing before unit testing

For most of us, this idea is counterintuitive. We've been taught that the later you discover a defect in the development cycle, the more expensive it is to fix. We try to get all the details perfected before moving on to the "big things," like integration testing.

The problem is that that claim was rooted in the waterfall development model, in which you didn't move to the next development until the current phase was complete. Once you move to agile development, however, the idea is no longer relevant. Agile empowers you with the flexibility to make any changes in the business logic that are necessary as you move along.

2. Don't test business logic with integration testing

That's what unit tests are for. Confusing unit tests with integration tests can have dire consequences on the time it takes to run your test suite. Unit tests are typically very fast, so they are run for every build triggered in the CI environment.

Since they target basic correctness of code, running them frequently is critical to detect bugs early on in business logic, so that the developer who introduced the bug can fix it immediately. Integration tests, on the other hand, take much longer to run, so they should not be included in every build cycle, but in something closer to a daily build.

3. Know why integration testing is different from unit testing

There are many telltale signs that help you easily differentiate a unit test from an integration test:

i. Encapsulation: While unit tests are well encapsulated and don't use external resources, integration tests use additional components or infrastructures like the network, database, or file system.

ii. Complexity: Unit tests target small and distinct parts of code, so they are usually simple to write. Integration tests are more complex, often requiring tooling and setting up different infrastructures.

iii. Test failure: When a unit test fails, there is clearly a bug in the business logic of the code. When an integration test fails, you shouldn't need to look at the code that implements business logic; the unit tests should flush out bugs at that level. It's more likely that something has changed in the environment and needs to be addressed.

4. Keep your testing suites separate

Integration tests should not be run together with unit tests. Developers working on specific business logic in the code must be able to run unit tests and get near-immediate feedback to ensure that they haven't broken anything before committing code. If their test suite takes too long and they can't afford to wait for it to finish before committing code, they are likely to just stop running tests altogether (both unit tests and integration tests). This also means that the unit tests are not properly maintained, which can eventually get you into a situation where the effort required to bring your test suite up to date with the code causes real delays in delivery.

By keeping your test suites separate, your developers can feel free to run the quick unit tests during development and before committing any code. The long and tedious integration tests should be reserved for the build server in a separate test suite, and can be run less frequently.

5. Log extensively

A unit test has a specific scope and tests a very small piece of your application, so when it fails, it's usually quite easy to understand why and fix the problem. Integration tests are quite different. Their scope may span several software modules, not to mention different devices and hardware components, in any functional flow. As a result, if an integration test fails, it may be much more complex to identify the cause.

Exhaustive logging is the only way to analyze a failure, allowing you to discover where the problem lies. Still, be mindful that exhaustive logging can have a significant effect on performance, so it should be done only when needed. Make sure you use a competent logging framework that can be controlled via flags that allow for minimal logging during normal production usage and progressively more detail to be logged in the event of a problem.


6. Don't stop at integration testing

Testing does not end with how your software modules work with one another, or even how they work with other, third-party modules. It goes beyond. Your software is going to be deployed in a complete production ecosystem that may include virtualization tools, databases, mail servers, load balancers, DNS servers, proxy servers, and more. Your customers' user experience depends not only on your application, but also on how it is deployed in your production environment and how it works with all those other peripheral components. These are the components (yes, all of them) that you should be targeting, so once you have validated (or while you are validating) your high-level architecture with integration testing, make sure you also run system tests that accurately simulate your production environment.

Integration testing is expensive but worthwhile

A key point in all of this is that it may be expensive to do integration testing properly and at the right time in the development cycle. However, it will be much more expensive to fix defects in your high-level architecture if it is discovered much later in the game.

Note, if you don't get your high-level architecture right, it's going to be much more expensive to rework it once the details of your application are already written—even if all of your unit tests pass. 


## Tools 

1. https://dzone.com/articles/10-essential-testing-tools-for-java-developers 

2. https://www.softwaretestinghelp.com/integration-testing-tools/ 

3. https://www.petrikainulainen.net/programming/testing/12-tools-that-i-use-for-writing-unit-and-integration-tests/



## Further Reading

1. https://www.atlassian.com/continuous-delivery/software-testing/types-of-software-testing 

