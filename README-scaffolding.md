
#  Platform Blue Print (Scaffolding)

The patterns and best practices mentioned here should be discussed, mitigated and covered (be in place) in any software development cycle before coding begins. This is normally an agenda for SPRINT 0. 

 ## Digital Delivery

```
 Web App
 
 Mobile Web
 
 Mobile Apps
 
 Digital Platforms
 
 Architecting for High Availability / Fault tolerant (Design for failure, Multiple Availability zones, Scaling, Self Healing, Loose Coupling)
 
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

5.  CSS - BEM, SASS, 

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

A Module bundler, Webpack bundles a bunch of modules with require statements.

Bundlers such as Browserify and Webpack are steadily taking over from Gulp and Grunt, and there is very little room left for both stream-based tasks. The majority of the work which you were previously doing with Gulp is now handled by Webpack — bundling and optimization for JavaScript, CSS and images; code splitting; targeted bundles for different environments (see isomorphic apps).

As a build tool Webpack puts all of your assets, including Javascript, images, fonts, and CSS, in a dependency graph. Webpack lets you use require() in your source code to point to local files, like images, and decide how they're processed in your final Javascript bundle, like replacing the path 
with a URL pointing to a CDN.


 When to use  Webpack: 
 
 If you're building a complex Front End application with many non-code static assets such as CSS, images, fonts, etc, then yes, Webpack will give you great benefits.

If your application is fairly small, and you don't have many static assets and you only need to build one Javascript file to serve to the client, then Webpack might be more overhead than you need.


The Dependency Graph property, ad how it works: 

Webpack gives us a dependency graph. It lets you use require() on local "static assets," meaning non-code files.

When you run Webpack, it searches through all of your code for require() calls. It compares the path string for example "../../assets/logo.png" to the "loader" configuration you specify.

```

loaders: [  
    { test: /.png$/, loader: "file" }
]

```

Key concept: 

 The require source code never actually gets executed in the browser (nor in Node.js). Webpack builds a new Javascript file, replacing require() calls with valid Javascript code, such as URLs. The bundled file is what's executed by Node or the browser.



Webpack puts your static assets (and source code) in a true dependency graph. Grunt and Gulp are only tools for working with files, and have no concept of a depdency graph.

Browserify is mainly a tool to transform require() calls that work in Node.js into calls that work in the browser. It's a dependency graph for your source code only. 



## Back end

```
Error Handling

API / Services / End point

```

## SEO / Performance

```
1. SSR and Static Site Generators - GatsbyJS (REACT, GraphQL, Helmet, Plugins)

2. Google Analytics

3.  Universal JavaScript (Server Side Rendering)

4.  Lighthouse
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

## Architecture & API

```
1. Micro-services

2. SOA

3. APIs

4. TOGAF

5. SWAGGER

6. GraphQL

7. Fastify

```
