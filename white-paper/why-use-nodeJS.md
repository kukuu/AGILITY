# Why use nodeJS

If you're looking to create real time web apps (chats apps) Node will be the best technology for these type of applications. Ruby and Python can both accommodate these kind of features as well, but Node.js will do it exceptionally well in terms of performance.

If you're looking to build APIs or streaming applications, It's perfect for handling lots of requests that are I/O driven (e.g. operations on database) and scales very nicely - event loops. produces stacking/buffering with Asynchronous calls.

## Speed 

 Node.js is fast. Node.js uses JavaScript in the backend, and that’s enough to understand how fast the codes execute. Moreover, it runs on the Google’s V8 engine, which compiles the JavaScript directly into machine code making it faster than most.

## The ever-growing NPM

Being an open-source technology, node.js has a shared repository of good-to-go tools and modules. The number of modules in the Node Package Manager (NPM) has increased at a considerable pace, just on the verge of overtaking the RoR (Ruby on Rails) gems.

## The event-driven architecture of node.js 

Real-time web apps: Node.js is appropriate for real-time applications, especially chat applications and games. As both the client-side and the server-side are written in JavaScript, the synchronization process is better and quicker. Web socket protocol comes into picture here.


## Productivity

The productivity of a web app increases several folds with node.js because a lot of time is saved in between the lines. Merging the front-end and back-end into a single entity makes it efficient. That also implies a lesser number of employees and more profit on your side. PayPal reported 2 times increase in developer productivity after using node.js.

# Disadvantages of node.js


Two of the most argued about aspects of Node.js programming are its insufficiency with heavy computations and the so-called “callback hell”. 

## The single-threaded drawback

As we know, JavaScript (and, as a result, Node.js) is asynchronous by nature and has a non-blocking I/O (input/output) model. This means, it can process several simple tasks (for example, read/write database queries) queued in the background without blocking the main thread and do so quickly.

At the same time, Node.js is a single-threaded environment, which is often considered a serious drawback of the technology. Indeed, in some cases, a CPU-bound task (number crunching, various calculations) can block the event loop resulting in seconds of delay for all Node.js website users.

This represents a serious issue. That is why, to avoid it, it is recommended not to use Node.js with computation-heavy systems.

But then with query API languages like GraphQL in the market, which is supported by node.js this will soon be a thing of the past. Queries are passed through and managed at the client side level other than through end points to the server again and again.

## Immaturity of tooling

Although, the core Node.js modules are quite stable and can be considered mature, there are many tools in the npm registry which are either of poor quality or not properly documented/tested. Moreover, the registry itself isn’t structured well enough to offer the tools based on their rating or quality. Hence it might be difficult to find the best solution for your purposes without knowing what to look for.

The fact that the Node.js ecosystem is mostly open source, has its impact as well. While the quality of the core Node.js technology is supervised by Joyent and other major contributors, the rest of the tools might lack the quality and high coding standards set by global organizations.

## Mastering Serer side JavaScript!!

Despite a common belief, not all JavaScript developers are Node.js developers as well. Mastering server side JavaScript programming requires a significant amount of effort and a certain background in backend development. Due to such a steep learning curve, the number of Node.js engineers is significantly lower than the total number of JS professionals.

## More Reading 

Event loop - https://github.com/kukuu/AGILITY/blob/master/JavaScript-EventLoop.md

