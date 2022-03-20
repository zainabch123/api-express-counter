# Express Counter

In this exercise we will build a simple counter API using express.

## Learning Objectives

- Explain how to set up and run an Express application
- Build a simple Express API and send a HTTP request to an available endpoint using a HTTP client
- Explain that JSON is a widely-used language-agnostic format for encoding data as attribute value pairs
- Diagram the request and response cycle for an Express API.
- Use console.log() and read the result in the server logs

## Instructions
Create a new express application and implement the following endpoints:

- POST `/counter/increment`-  Increments a counter on the server and returns the current value.
- POST `/counter/decrement`-  Decrements a counter on the server and returns the current value.
- POST `/counter/double`-  Double the value of the counter on the server and returns the current value. 
- DELETE `/counter` - Resets the counter to 0 and returns the current value.
- GET `/counter` - Returns the current value of the counter.

All endpoints should return the current value of the counter in following format: `{ counter: 0 }`

Test each route using:
- `fetch` 
- `curl`
- An API testing tool such as postman or insomnia

## Extension 1
Add a route PUT `/counter` that can be used to set the counter to a specific value. The value should be specified by a query string parameter. For example, making a PUT request to `/counter?value=20` should set the value of the counter to 20. Use the  `req.query` property in your callback to get the value provided. See the [express documentation](https://expressjs.com/en/api.html#req.query) If no value is provided, the counter should not be changed. 

## Extension 2
Using [route parameters](https://expressjs.com/en/guide/routing.html),  update your API to keep track of multiple counters. Allow the client to specify the counter name as part of the URL. For example, to update and access a counter called "cars", the client could make the following requests:

- POST `/counter/cars/increment`
- POST `/counter/cars/decrement`
- POST `/counter/cars/double`
- DELETE `/counter/cars`
- GET `/counter/cars`

It should be possible for the client to specify any counter name in the place of "cars".