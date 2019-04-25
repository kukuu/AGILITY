
# Scaffolding Blue Print

The patterns and best practices mentioned here should be discussed, mitigated and covered (be in place) in any software development cycle before coding begins. This is normally an agenda for SPRINT 0. 

## UX

```
1.  Design Framework : Responsive Design, Mobile First

2.  Grids & Layout (Bootstrap, Material UI etc)

3.  Fonts

4.  Collaboration 

```

## Front end

```
1.  Programming Framework 

2.  Development environment 

3.  CI / CD, Automated testing Pipeline 

4.  Development platform

5.  CSS - BEM, SASS, 

6.  Linting

7.  Error Handling - Status Codes

8.  Minifying assets

9.  Managing Performance & SEO (PWA / Service Worker / Notification)

10. Enabling G-Zip on AWS

11. Managing Cookies

12. Cross Browser Compatibility

13. Fonts

14. Digital Security - Code, Infrastructure (DevSecOps)

15. Cache Strategy

16. Handling asynchronous requests and managing latency (Spinner)

18. Localising polyfills

17. Code portability

18. State Management - REDUX

19. Local Storage

20. Micro-services

21. API

22. Handling Client Queries - Graph Queries

23. Module Bundler - Webpack
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

## SEO

```
1.  Google Analytics

2.  Universal JavaScript (Server Side Rendering)

3.  Lighthouse
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

```
