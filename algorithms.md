# Algorithms

Applied to code, an algorithm is just a function that transforms a certain input data structure into a certain output data structure. The logic inside decides the transformation.

First and foremost, the inputs and outputs should clearly be defined, ideally, as unit tests. This requires fully understanding the problem at hand, which is not to be underestimated, because a thorough analysis of the problem can surface the solution naturally, without needing to write any code.

Once the problem domain is thoroughly grasped, brainstorming of the solution space can begin. What variables will be needed? How many loops and what kinds? Are there any clever built-in methods that can help? Edge cases to consider? Complex or repeated logic can be difficult to read and understand. 

Can helper functions be extracted or abstracted? An algorithm usually needs to be scalable. As input sizes grow, how will the function perform? Should there be some kind of caching mechanisms? Generally, memory optimizations (space) will need to be sacrificed for performance gains (time).

Finally, think about re-factoring and modularising at a stage.

Types of Algorithms - https://github.com/kukuu/algorithms/tree/master/algorithms

### Shallow and Deep clones

https://github.com/kukuu/algorithms/tree/master/algorithms/copy-clone

### Working with DEFAULT parameters - moving away from OLD to NEW school

https://github.com/kukuu/algorithms/blob/master/algorithms/es6/default-params/default-params.md

### Fibonacci

https://github.com/kukuu/algorithms/blob/master/algorithms/fibonacci.md 

https://github.com/kukuu/algorithms/blob/master/algorithms/fibonnaci.js


### map, filter , reduce

https://github.com/kukuu/javascript/tree/master/map-filter-reduce

https://github.com/kukuu/Apps-WebServices/blob/master/axios/examples/REACT/standard.jsx 

https://github.com/kukuu/Apps-WebServices/blob/master/axios/examples/all/index.html 

### Counter

https://github.com/kukuu/javascript/blob/master/counter/counter.jsx 

https://github.com/kukuu/javascript/blob/master/counter/index.html

### Anagrams

https://github.com/kukuu/algorithms/blob/master/algorithms/anagram.md 

https://github.com/kukuu/algorithms/blob/master/algorithms/anagrams.test.js

### Data Structures 

https://www.freecodecamp.org/news/the-top-data-structures-you-should-know-for-your-next-coding-interview-36af0831f5e3/

###  Game: Rock, Paper & Scissors - Beat the Computer!

This is  a web application GAME - Rock, Paper & Scissors, using vanilla JavaScript with some of its best practices. Including es6 and some new  JavaScript API objects.

This game has been engineered to be played against the Computer. 

You can read more on the game from here - https://en.wikipedia.org/wiki/Rock–paper–scissors. 

Note, the semantics  in descriptive names of the caching variables for the DOM elements.

The application's JavaScript document is versioned, and documented to reflect the iterations which went on in building the application (app.js[main], ap-v1.js, ap-v2.js, ap-v3.js,  ap-v4.js,  ap-v5.js). This is done for tutorial, coaching and learning purposes, and has substantial comments. The final output (app.js)is optimised. This MUST be understood.


### EJS Templating in Node.js Application

https://github.com/kukuu/javascript/tree/master/ejs/routes 

https://github.com/kukuu/javascript/blob/master/ejs/server.js


### Unit Test
1. Mocha Framework
2. Chai Assertion Library
4. Test suites:
- "draw".
- "user" wins.
- "comp" (Computer) wins.
5. package.json

```
{
  "name": "rock-paper-scissors",
  "version": "1.0.0",
  "description": "Mocha Chai NodeJS ",
  "main": "appsRPS.js",
  "dependencies": {
    "gulp": "^4.0.2"
  },
  "devDependencies": {
    "chai": "^4.2.0",
    "mocha": "^6.1.4"
  },
  "scripts": {
    "test": "mocha || true"
  },
  "author": "Alexander Adu-Sarkodie",
  "license": "ISC"
}

```
6. To execute test script: npm run test


##### Extended test

1. https://github.com/kukuu/unittests/tree/master/mocha-chai/test 

2. Requires Gulp, Mocha and Chai(npm install --save-dev).


### FizzBuzz

https://github.com/kukuu/siliconlabs/blob/master/fizzBuzz/fizzbuzz.md 

### JavaScript Algorithms 

https://medium.com/siliconwat/algorithms-in-javascript-b0bed68f4038 


### lowest common multiple

https://www.gcflcm.com/lcm-of-24-and-36 


### Filter list in  Python
https://github.com/kukuu/python/blob/master/filter-list 

### Making API calls with  AXIOS and  async / await

i. https://github.com/kukuu/microservices-nodejs-docker-nginx/blob/master/search/src/app.js 


ii. https://github.com/kukuu/secure-restful-react-redux-web-app/blob/master/bookworm/bookworm-react/src/api.js


### Hashing password with bcrypt

https://github.com/kukuu/siliconlabs/blob/master/bcrypt

### Snippets

https://github.com/kukuu/AGILITY/blob/master/white-paper/architectural-solutions/snippets.md


### Code Review tips

#### Functional

1. SOLID: Does the code follow SOLID principles?

i. Single responsibility principle
A class should only have a single responsibility, that is, only changes to one part of the software's specification should be able to affect the specification of the class.


ii. Open–closed principle
"Software entities ... should be open for extension, but closed for modification."

iii. Liskov substitution principle
"Objects in a program should be replaceable with instances of their subtypes without altering the correctness of that program." 

iv. Interface segregation principle
"Many client-specific interfaces are better than one general-purpose interface.

v. Dependency inversion principle
One should "depend upon abstractions, concretions."


2. Check for null pointers where exceptions are needed.

3. Buffer Overflows

4. Integer overflows

5. Uninitialised objects

6. DRY: Are re-usble properties, routines being cached?

7. Formatting: Where are the spaces and line breaks? Are they using tabs or spaces? How are the curly braces laid out?

8. Style: Are the variables/parameters declared as final? Are method variables defined close to the code where they’re used or at the start of the method?

9. Naming: Do the field/constant/variable/param/class names conform to standards? Are the names overly short?

10. Test coverage: Is there a test for this code?

11. Race conditions: Any global polution? Leakages? Managing callbacks and side effects.

12. Design patterns: What design patterns are used in the new code? Any anti-patterns (in loops etc)

13. Lines of code: Are functions too long?

14. Using modern syntaxes (ES6): Arrow functions, default parameters, block scoping, template strings, spread operators, generator functions, destructuring etc

15. Optimisation in multi-threaded code

#### Security

Attacks and vulnerabilities

1. DoS - denial of service attacks

2. XSS - Cross Site Scripting

3. MIM - Man in the Middle

4. CSRF - Cross Site Request Forgery (use CSRF token implementation )

5. CORS

##### Tools

1. Morgan - for logging vulnerabilities

2. SNYK - Checking vulnerabilities in NPM and other packages in CI/CD pipeline

3. Helmet - Helmet helps you secure your Express apps by setting various HTTP headers. It's not a silver bullet, but it can help! It includes a  11 packages that all work to block malicious parties from breaking or using an application to hurt its users.
