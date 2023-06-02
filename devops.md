# DevOps Cultural Philosophy

Transitioning to DevOps requires a change in culture and mindset. At its simplest, DevOps is about removing the barriers between two traditionally siloed teams, development and operations. In some organizations, there may not even be separate development and operations teams; engineers may do both. With DevOps, the two teams work together to optimize both the productivity of developers and the reliability of operations.

They strive to communicate frequently, increase efficiencies, and improve the quality of services they provide to customers. They take full ownership for their services, often beyond where their stated roles or titles have traditionally been scoped by thinking about the end customer’s needs and how they can contribute to solving those needs.

Quality assurance and security teams may also become tightly integrated with these teams. Organizations using a DevOps model, regardless of their organizational structure, have teams that view the entire development and infrastructure lifecycle as part of their responsibilities.

## Integration Approach

In-house: dev and production

In-house data with Cloud systems

Legacy systems



## Tools

GIT / GitHub - Probably the most common source management tool available. Used for Source Control Management. In addition to its great forking and pull request features, GitHub also has plugins that can connect with Jenkins to facilitate integration and deployment.

Ansible - Configuration Management Tool similar to Puppet and Chef.

Docker - It eases configuration management, control issues, and scaling by allowing containers to be moved from one place to another.

Jenkins - As an extensible automation server, Jenkins can be used as a simple CI server or turned into the continuous delivery hub for any project. Jenkins can easily distribute work across multiple machines, helping drive builds, tests and deployments across multiple platforms faster.


## Building an automation CI/CD  

Key steps to building CI/CD pipeline: 

### Define the Pipeline:
Identify the stages and steps needed in your CI/CD pipeline based on your project requirements.
Common stages include code linting, building, testing, deploying to staging environments, and deploying to production.

### Version Control and Repository Setup:
Use a version control system (e.g., Git) to manage your source code.
Set up a repository for your project and establish branching strategies (e.g., feature branches, release branches).
Ensure all team members follow proper branching and commit practices.

### Configure Build Automation:
Choose a build tool (e.g., Jenkins, CircleCI, GitLab CI/CD) that integrates with your version control system.
Configure the build automation tool to fetch the code, trigger builds, and execute build scripts or commands.
Set up build agents or runners for parallel and distributed builds, if necessary.

### Automated Testing:
Incorporate automated tests into your pipeline to ensure code quality and functionality.
Write unit tests, integration tests, and end-to-end tests depending on your project's needs.
Integrate testing frameworks (e.g., Jest, Selenium, Cypress) into your pipeline and execute tests automatically.

### Artifact Creation and Packaging:
Create deployable artifacts, such as compiled binaries, Docker images, or package archives.
Package the necessary dependencies and configuration files into the artifact.

### Deployment and Environment Setup:
Configure your pipeline to deploy the artifact to staging or testing environments after successful builds and tests.
Utilize infrastructure as code tools (e.g., Terraform, Ansible) to provision and configure the required infrastructure and environments.
Use configuration management tools (e.g., Chef, Puppet) to automate the setup and configuration of servers and services.

### Continuous Deployment to Production:
Implement a mechanism to promote the tested and approved artifact to production environments.
Use release management practices (e.g., feature flags, blue/green deployments) to control the rollout and minimize the impact of any issues.

### Monitoring and Feedback:
Integrate monitoring tools (e.g., Prometheus, New Relic) to gather metrics, logs, and performance data from your application.
Set up alerts and notifications to proactively detect and respond to issues.
Continuously gather feedback from users and stakeholders to iterate and improve your CI/CD pipeline.

### Iterate and Improve:
Regularly review and refine the CI/CD pipeline based on feedback and changing project requirements.
Automate repetitive tasks, optimize performance, and introduce new tools or techniques to enhance the pipeline.
It's essential to continually refine the pipeline for optimal efficiency and reliability.

## DORA - DevOps Research and Assessment 

The primary goal of DORA is to help organizations understand and improve their DevOps capabilities through evidence-based research and data-driven insights

 DORA provides valuable benchmarks and best practices for seeking and optimising DevOps initiatives.

### Key Metrics," 

- Lead Time: The time it takes to convert a customer request or idea into a production-ready feature or service.

- Deployment Frequency: The frequency at which an organization deploys changes or releases to production.

- Change Failure Rate: The percentage of changes or releases that result in failure or negatively impact the system's stability.

- Time to Restore Service: The time it takes to recover from a service disruption or failure and restore normal operations.

## Resources

1. https://github.com/kukuu/AGILITY/blob/master/devops-1.png 
2. https://github.com/kukuu/AGILITY/blob/master/devops-2.png
3. Learn How to Set Up a CI/CD Pipeline From Scratch - https://dzone.com/articles/learn-how-to-setup-a-cicd-pipeline-from-scratch

