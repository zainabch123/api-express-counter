# Express Counter

In this exercise we will build a simple counter API using express.

## Learning Objectives

- Explain how to set up and run an Express application
- Build a simple Express API and send a HTTP request to an available endpoint using a HTTP client
- Explain that JSON is a widely-used language-agnostic format for encoding data as attribute value pairs
- Diagram the request and response cycle for an Express API.
- Use console.log() and read the result in the server logs

## Instructions
Create a new express application using the steps provided in the [express intro](https://github.com/boolean-uk/api-address-book). 

Your application should maintain a simple numeric counter and provide the endpoints detailed in the [API Spec](https://boolean-uk.github.io/api-express-counter/).

Each route should be detailed in a sequence diagram in the same way you did during the API address book exercise.

Test each route using:
- `fetch`
- `curl`
- An API testing tool such as postman or insomnia

## Extension 1
Add a route as detailed in the [API Spec Extension 1](https://boolean-uk.github.io/api-express-counter/#tag/extension-1). For example, making a PUT request to `/counter?value=20` should set the value of the counter to 20. Use the `req.query` property in your callback to get the value provided. See the [express documentation](https://expressjs.com/en/api.html#req.query). If no value is provided, the counter should not be changed.

## Extension 2
Using [route parameters](https://expressjs.com/en/guide/routing.html), update your API to keep track of multiple counters. Allow the client to specify the counter name as part of the URL. With this in mind, build the endpoints as detailed in the [API Spec Extension 2](https://boolean-uk.github.io/api-express-counter/#tag/extension-2).
