
# Continuous Integration, Continuous Delivery , and Continuous Deployment

The key difference between the three is in the scope of automation applied. What gets people who are new to the field confused is that they are not mutually exclusive, but include each other, like Russian dolls.

## Continuous Integration

Continuous integration is a software development practice where developers regularly merge their code changes into a central repository, after which automated builds and tests are run. The key goals of continuous integration are to find and address bugs quicker, improve software quality, and reduce the time it takes to validate and release new software updates.
Continuous integration, continuous deployment, and continuous delivery are like vectors that have the same direction, but different magnitude. Their goal is the same: make our software development and release process faster and more robust.

## The nucleus: continuous integration

Most developers start with Continuous Integration (CI), which is about everyone merging code changes to a central repository multiple times a day. Each merge triggers an automated build and testing sequence for the given project.

Depending on the programming language, the program may first need to be compiled. Today there is also an increasing need to package the code in a Docker container. Automated tests then verify specific units of code, UI behavior, application performance, API reliability, and more. Together, all these steps are commonly referred to as the "Build" stage.

CI acts as a safety net that lets developers prevent many issues before they reach users. As a result, developers ship code with more confidence, but not necessarily faster — the deployment process may still be manual, long, and error-prone.

The best initial investment developers can make is to ensure that their automated test suite is comprehensive and stable enough that they feel safe to deploy every passed CI build to a staging, and later production environment, without a long manual QA (quality assurance) process.

The second thing to pay attention to is CI speed: It is strongly recommmended that developers must get CI results within 10 minutes, otherwise their productivity shrinks due to lack of focus and frequent context switching. An easy way to optimize CI time is to run tests in parallel on a powerful platform.


## The leap to continuous delivery and deployment - RRASc

### Continuous delivery
Continuous Delivery (CD) is a practice of automating the entire software release process. The idea is to do CI, plus automatically prepare and track a release to production. The desired outcome is that anyone with sufficient privileges to deploy a new release can do so at any time in one or a few clicks. By eliminating nearly all manual tasks, developers become more productive.

The continuous delivery process typically includes at least one manual step of approving and initiating a deploy to production. In complex systems with multiple dependencies, the continuous delivery pipeline may include additional steps, which are either manual or automatic.

Continuous delivery is a software development practice where code changes are automatically built, tested, and prepared for a release to production. It expands upon continuous integration by deploying all code changes to a testing environment and/or a production environment after the build stage. When continuous delivery is implemented properly, developers will always have a deployment-ready build artifact that has passed through a standardized test process.

Extensibly, it is  the ability to get changes of all types including new features, configuration changes, bug fixes and experiments into production, or into the hands of users, safely and quickly in a sustainable way.

The model behind this approach is to achieve a platform which is:

```

Reliable :: Repeatable :: Automation :: Source control

```

A logical extension of Continuous Integration, It is based on the use of smart automation. This is all about creating a repeatable and reliable process for delivering software. You have to automate pretty much everything in order to be able to achieve continuous delivery. Manual steps will get in the way or become a bottleneck. This goes for everything from requirements authoring to deploying to production.

The ultimate goal of continuous delivery is to minimise the iteration time of the code-test-deliver-measure experimentation cycle. Increasing deliverable throughput in this way is the key to not only more feature work being delivered but higher quality code as well. This might seem counter-intuitive at first but code is fixed and polished through that same cycle and less time spent on deployment is more time spent on designing quality code.

The high-level requirements FOR CD are:

1. Software must be easily testable, which means it must be loosely coupled.

2. Delivery must—under normal circumstances—require minimal human interaction.

3. Delivery—from commit to production—must be fast. Preferably under 10 minutes.

4. Rolling back a deployed feature if it is found to be broken or unwanted must be trivial.

5. Build binaries only once. Binaries should be compiled once and once only. 
   The binary should then be stored someplace which is accessible only to your deployment mechanism, 
   and your deployment mechanism should deploy this same binary to each successive environment

6. Use precisely the same mechanism to deploy to every environment. Both QA and production
   deployment must be both automated.

7. Smoke test your deployment. Write a smoke test and include that in the deployment process.

8. Stop the lines if anything fails.

### Continuous deployment
Continuous Deployment is a step up from Continuous Delivery in which every change in the source code is deployed to production automatically, without explicit approval from a developer. A developer's job typically ends at reviewing a pull request from a teammate and merging it to the master branch. A CI/CD service takes over from there by running all tests and deploying the code to production, while keeping the team informed about outcome of every important event.

Continuous deployment requires a highly developed culture of monitoring, being on call, and having the capacity to recover quickly.


## Achieving CD

1. The process for releasing/deploying software MUST be repeatable and reliable. 

2. Automate everything!

3. If somethings difficult or painful, do it more often.

4. Keep everything in source control

5. Done means “released”.

6. Build quality in! 

7. Everybody has responsibility for the release process

8. Improve continuously
The most optimum path to achieve these goals is to use microservices architecture


## To sum up:

Continuous Integration (CI): short-lived feature branches, team is merging to master branch multiple times per day, fully automated build and test process which gives feedback within 10 minutes; deployment is manual.
Continuous Delivery (CD): CI + the entire software release process is automated, it may be composed of multiple stages, and deployment to production is manual.
Continuous Deployment: CI + CD + fully automated deployment to production.


## Resources

Containerisation - https://github.com/kukuu/AGILITY/blob/master/containerisation.md

DevOps - https://github.com/kukuu/AGILITY/blob/master/devops.md


