# How a modern API works - Separation of Concerns (SoC)

Many modern applications separate the backend services from the frontend user interface. In this type of architecture, the backend will expose a web based API that the frontend client consumes. Typically, the backend will handle incoming requests and return a JSON or XML encoded response. The frontend will then be in charge of formatting, styling, and displaying this response to the user. We’ve all heard the term “separation of concerns” and applying it at this scale has many benefits.

The backend services can grow and evolve independent of the frontend client. New APIs, if properly versioned, can provide new features and functionality without breaking existing integrations. A single backend can interface with multiple clients and the frontend clients will not be limited to any specific framework or programming language. This means that your single backend can work with your app for both a web based implementation, your mobile app, and even with IoT devices.

The API needs to be protected with a digital security. In addition to protecting our API endpoints, you will also have to add specific roles to each of our clients and show how we can give granular access to our API.

For example, If you are challenged with building 4 different clients (3 user facing and an admin) which are linked, rather than building two separate backends for the user facing side and the admin application, you can  build and expose a single API with four endpoints. The user facing app will have access to the 3 endpoints, while the admin app will additionally have access to the 4th endpoint which can potentially be used for moderation, and not  publically accessible. 

## Building with nodeJS

You will require

1. Experess - dependency to pull down the express framework

2. express-jwt - To generate token

3. auth0-api-jwt-rsa-validation - Helper function to generate Secrete Key

4. Create a middleware functions to validate the access token when our API is called, and also authorise the diferent clients created from the SCOPE. See server.js- https://github.com/kukuu/-SECURE-API


## Protecting end points

In addition to protecting our API routes, we are also going to fine-tune access to specific endpoints. Use SCOPES.

Scopes allow us to grant specific permissions to clients that are authorized to use our API. For our demo, we are going to create two scopes, general and admin. In an actual application, you could further narrow down the scopes by giving read or write permissions and even go as far to protect each individual route with a separate scope. We’ll keep it fairly general here though. Go ahead and create the two scopes now.

Once the  scopes in place, the last thing we’ll need to do is authorize our two clients to work with the API we created (GENERAL and ADMIN).

We add the ability to check if the client has permissions to view the endpoint requested. To do this, we’ll create another middleware that will look at the decoded JWT and see if it the token has the correct scope. If it doesn’t we’ll send an appropriate forbidden message, otherwise we’ll send the data. Take a look at our implementation of this functionality below.

This guard middleware will be called on each request and will ensure that the token has the correct scope. If it does, we’ll send the data, otherwise we’ll return a 403 Forbidden status and appropriate message.
