
# Continuous Integration, Continuous Delivery , and Continuous Deployment

Continuous integration, continuous deployment, and continuous delivery are like vectors that have the same direction, but different magnitude. Their goal is the same: make our software development and release process faster and more robust.

The key difference between the three is in the scope of automation applied. What gets people who are new to the field confused is that they are not mutually exclusive, but include each other, like Russian dolls.


## The nucleus: continuous integration

Most developers start with Continuous Integration (CI), which is about everyone merging code changes to a central repository multiple times a day. Each merge triggers an automated build and testing sequence for the given project.

Depending on the programming language, the program may first need to be compiled. Today there is also an increasing need to package the code in a Docker container. Automated tests then verify specific units of code, UI behavior, application performance, API reliability, and more. Together, all these steps are commonly referred to as the "Build" stage.

CI acts as a safety net that lets developers prevent many issues before they reach users. As a result, developers ship code with more confidence, but not necessarily faster — the deployment process may still be manual, long, and error-prone.

The best initial investment developers can make is to ensure that their automated test suite is comprehensive and stable enough that they feel safe to deploy every passed CI build to a staging, and later production environment, without a long manual QA (quality assurance) process.

The second thing to pay attention to is CI speed: It is strongly recommmended that developers must get CI results within 10 minutes, otherwise their productivity shrinks due to lack of focus and frequent context switching. An easy way to optimize CI time is to run tests in parallel on a powerful platform.


## The leap to continuous delivery and deployment

Continuous Delivery (CD) is a practice of automating the entire software release process. The idea is to do CI, plus automatically prepare and track a release to production. The desired outcome is that anyone with sufficient privileges to deploy a new release can do so at any time in one or a few clicks. By eliminating nearly all manual tasks, developers become more productive.

The continuous delivery process typically includes at least one manual step of approving and initiating a deploy to production. In complex systems with multiple dependencies, the continuous delivery pipeline may include additional steps, which are either manual or automatic.

Continuous Deployment is a step up from Continuous Delivery in which every change in the source code is deployed to production automatically, without explicit approval from a developer. A developer's job typically ends at reviewing a pull request from a teammate and merging it to the master branch. A CI/CD service takes over from there by running all tests and deploying the code to production, while keeping the team informed about outcome of every important event.

Continuous deployment requires a highly developed culture of monitoring, being on call, and having the capacity to recover quickly.



## To sum up:

Continuous Integration (CI): short-lived feature branches, team is merging to master branch multiple times per day, fully automated build and test process which gives feedback within 10 minutes; deployment is manual.
Continuous Delivery (CD): CI + the entire software release process is automated, it may be composed of multiple stages, and deployment to production is manual.
Continuous Deployment: CI + CD + fully automated deployment to production.
