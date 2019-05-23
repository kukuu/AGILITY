
#  Platform Blue Print (Scaffolding) - SPRINT 0 / Discovery

The patterns and best practices mentioned here should be discussed, mitigated and covered (be in place) in any software development cycle before coding begins. This is normally an agenda for SPRINT 0, and during the period of writing up the SDD (Software Design Document). 


 ## Softwared Architecture & Standards
 
 Software architecture refers to the high level structures of a software system and the discipline of creating such structures and systems. Each structure comprises software elements, relations among them, and properties of both elements and relations.

The architecture  is a blend of technical decisions and architectural patterns, and considered the root of a software project, to ensure its scalability, security, quality, cost effectiveness and longevity.

The architecture is made so the code structure can satisfy every software prerequisite that is being developed while exemplifying transversal attributes such as performance, quality, scalability, maintainability, manageability, and usability.

Failure of attributes may result in productivity loss for users, damaged customer relations, revenue loss, cost overruns due to redesign, and missed market windows. Therefore, a software architect must focus on the initial issues in the development process during the architectural design phase, to avoid poor performance.

In order to start testing the design against requirements and assumptions, don't try to get it all right in the first attempt. Iteratively add details to the design over different tries, to ensure that you get the big decision right first, and then focus on the details later. A common setback is to dive into the details too quickly to evaluate your architecture effectively.
 
You can use multiple patterns in a single system to optimize each section of code with the best architecture.
 
 1. Principles of Software Architecture -  https://github.com/kukuu/AGILITY/blob/master/white-paper/principles-of-sw-architecture.png
 
 2. Architecture Design Decisions -  https://github.com/kukuu/AGILITY/blob/master/white-paper/software-architecture-main.jpg
 
 3. Major architectures - https://github.com/kukuu/AGILITY/blob/master/white-paper/software-architecture.md
 
 4. What makes a good software - https://github.com/kukuu/AGILITY/blob/master/white-paper/what-makes-a-good-software.png
 
 4. The tier systems - https://github.com/kukuu/AGILITY/blob/master/white-paper/tier-layer-README.md 
 
 5. NodeJS micro-service - https://github.com/kukuu/Microservice-NodeJS
 
 ### Adaptable Design
 
Adaptable designs are on trend to enhance viability. Developers prefer using flexible designs because they make use of free linking, whose impact on viability is imperative. By using pluggable designs, developers are able to offer extensibility even in the post-deployment period. You can use service-oriented architecture (SOA) and different strategies in service orientation to provide interoperability with other programming frameworks.


 ### Points to consider during Software Architecture Development
 
A software architect must:

1. Define the solution clearly.

2. What he expects to create based on the concerns of the different groups of people/stakeholders who will interface with his software. He should consider the following: 

```

i.  The concerns of the end users, including right and instinctive behavior, reliability,
performance, security, availability, and usability.

ii.  The concerns of the system administrator, including intuitive behavior, observing, 
and administrative tools.

iii. The concerns of the marketer, including cost, positioning relative to other software, 
time for marketing and competitive features.

iv.  The concerns of the customer, which incorporate: cost, schedule, and stability.

v.   The concerns of the developer, including project requirements and a steady yet basic
design approach.

vi. The concerns of the project manager include budget, schedule, and consistency, as it 
identifies with following the task, and the most effective use of the available resources.

vii. The concerns of the maintainer, which include the simplicity of making modifications,
and a consistent and complete design approach that is well documented.

```

 ## Digital Delivery

```
 Web App
 
 Mobile Web
 
 Mobile Apps
 
 Digital Platforms
 
 Architecting for High Availability / Fault tolerant (Design for failure, Multiple Availability zones, 
 Scaling, Self Healing, Loose Coupling)
 
 Cloud Computing (AWS / AZURE)
 
 Identity Management
 
 Security Architectures
 
 Disaster Recovery
 
 Capacity planning
 
 Performance Management
 
 SOA 
 
 Hosting
 
 Microservices
 
 Integration
 
 Implementation & evolving systems (in which all knowledge workers operate)
 
 Non Functional Requirements
 
 Reporting
 
 Finances
 
 Implementation of Agile delivery practices.
 
 Risk Management
 
 Stakeholder Management
 
 Infrastructure as Code
 
 ```

## UX

```
1.  Design Framework : Extensible, Responsive Design, Mobile First, Bottom to top

2.  Grids & Layout (Bootstrap, Material UI etc)

3.  Fonts

4.  Collaboration 

5.  KISS

6. Customer engagement / AB/MV Testing

7. User experience

```

## Front end

```
1.  Programming Framework 

2.  Source Control / Development environment 

3.  CI / CD  Pipeline (Reliable, Repeatable, Automation, Elastic, Source Control) 

4.  Development platform

5.  CSS - BEM, SASS, CSSModules, Style Components, PostCSS

6.  Linting

7.  Error Handling - Status Codes

8.  Minifying assets

9.  Managing Performance & SEO (PWA / Service Worker / Notification)

10. Enabling G-Zip on AWS

11. Managing Cookies & Sessions

12. Cross Browser Compatibility

13. Fonts

14. Digital Security - JWT, 2FA,OAuth, Infrastructure (DevSecOps)

15. Cache Strategy

16. Handling asynchronous requests and managing latency (Spinner)

18. Localising polyfill and third party libraries

17. Code re-usability

18. State Management 

19. Local Storage

20. Micro-services and Componentization

21. REST / RESTful API & Security

22. Handling Client Queries - Graph Queries

23. Module Bundler - Webpack

24. Security in Coding (DevSecOps - SNYK)
 
```

## Back end

```
Programming languages

Error Handling

API / Services / End point

Middlewares

```

## Continuous Integration

```

Jenkins

TeamCity

Travis CI

Go CD

Bamboo

GitLab CI

CircleCI

Codeship

```

## SEO, Performance, Caching  & Tools 

```
1. SSR / Universal JavaScript (Server Side Rendering)

2. Static Site Generators - GatsbyJS (REACT, GraphQL, Helmet, Plugins)

3. Google Analytics

4. Lighthouse

5. PWA (Service Worker)

6. Memcache

7. Service Worker

```


## DevSecOps

```
1.  Designing for Failure

2.  Multiple Availability Zones

3.  Cloud Watch

4.  Auto Scaling

5.  Loose Coupling

6.  Error Logging

7.  Micro-services

8.  Deployment: AWS / AZURE 

9.  Reporting back - Service Desk

10. Infrastructure as code

11. Containerisation (Docker Kubernetes)

12. Prometheus

13. SNYK

14. Server Security (SSL, TLS) & Monitoring (KIBANA, Prometheus)

15. Deploymnet Servers  (Jenkins, Tomcat)

```

## APIs &Tools

```

1. SWAGGER

2. Axios

3. Fetch

4. Postman

5. GraphQL

7. Fastify

```

## Static Site Generators

```
1. Gatsby

```

## Further reading

1. AGILITY - https://github.com/kukuu/AGILITY

2. Software Development Life Cycle - https://github.com/kukuu/AGILITY/blob/master/swdlc.md

3. Architecture - https://github.com/kukuu/AGILITY/blob/master/white-paper/tier-layer-README.md

4. Choosing a Technology stack - https://github.com/kukuu/AGILITY/tree/master/white-paper/tech-stack

5. CI 

- Team  City :  https://github.com/kukuu/AGILITY/blob/master/continuous-integration-with-team-city.png

-  CI, Continuous Delivery and Continuous Deployment Pipelines - https://github.com/kukuu/AGILITY/blob/master/CI-CDL-CDPL-pipeline.jpg

6. Software Design Specifications (SDD) - https://github.com/kukuu/AGILITY/blob/master/white-paper/SDD.md 

7. Statement of Work (SoW) - https://github.com/kukuu/AGILITY/blob/master/white-paper/SoW.md

8. Functional and Non-functional (NFR) requirements - https://github.com/kukuu/AGILITY/blob/master/white-paper/F-NFR.md 

9. Indexes for measuring code quality - https://github.com/kukuu/AGILITY/blob/master/white-paper/code-quality.md 

10. AWS 

- Web Pipeline :  https://github.com/kukuu/AGILITY/blob/master/aws-web-app-pipeline.png 

- Back end pipeline : https://github.com/kukuu/AGILITY/blob/master/white-paper/aws-backend-app-pipeline.png

11. Containerisation 

- Docker API : https://github.com/kukuu/digitalTransformationStrategies/blob/master/Docker-API.png

- Orchestration with Kubernetes Cluster - https://github.com/kukuu/AGILITY/blob/master/white-paper/kubernetes/1.png 

12. PWA - https://github.com/kukuu/AGILITY/blob/master/ProgressiveWebApp.md 

13. SOA vs Microservices  -  https://github.com/kukuu/AGILITY/blob/master/SOA-and-MicroServices.md 

- Architectural differences : https://github.com/kukuu/AGILITY/blob/master/difference-between-monolithic-and-microservices-architecture-1.png
- A microservice model : https://github.com/kukuu/digitalTransformationStrategies/blob/master/MICRO-SERVICES-oriented%20Architecture.png

- Micro-services API Gateway - https://github.com/kukuu/digitalTransformationStrategies/blob/master/APIgatewayResolution4microservices.png 

- SOA with Enterprise Service Bus (ESB) -  https://github.com/kukuu/AGILITY/blob/master/white-paper/SOA.png 

14. The Test Pyramid and Coverage - https://github.com/kukuu/AGILITY/blob/master/test-pyramid-coverage.jpg 

15. Certificates & Digital Security 
-  SSL & TLS : https://github.com/kukuu/AGILITY/blob/master/certificates.md 

- JWT - https://github.com/kukuu/AGILITY/blob/master/white-paper/JWT-architecture.png

16. The ISO 7 Layer model - https://github.com/kukuu/digitalTransformationStrategies/blob/master/7-osi-Layers-ii.jpg

17. The DevOps feedback loop - https://github.com/kukuu/digitalTransformationStrategies/blob/master/DevOps_feedback-diagram.png

18. Web Services - https://github.com/kukuu/Apps-WebServices/blob/master/README.md

19. Severless vs Containers - https://github.com/kukuu/AGILITY/blob/master/white-paper/severlessComputing-vs-containers/README-severless-computing-vs-containers.md

20. Software Development Cost estimation - https://github.com/kukuu/AGILITY/blob/master/white-paper/project-estimation/estimating-cost.md

