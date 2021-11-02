# Readings: Express REST API

< Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next.
1. As name suggests it comes in middle of something and that is request and response cycle
2. Middleware has access to request and response object
3. Middleware has access to next function of request-response life cycle

![](https://miro.medium.com/max/1400/1*wIkLR_9twvmG-LitHYoftw.png)

Middleware functions can perform the following tasks:

+ Execute any code.
+ Make changes to the request and the response objects.
+ End the request-response cycle.
+ Call the next middleware in the stack.

1. Enterprise Application Integration.
2. Data Integration.
3. Message Oriented Middleware.

If the current middleware function does not end the request-response cycle, it must call next() to pass control to the next middleware function. Otherwise, the request will be left hanging.


***
**True**
***
> **Middleware** functions are functions that have access to the request object (req), the response object (res), and the next function in the application’s request-response cycle. The next function is a function in the Express router which, when invoked, executes the middleware succeeding the current middleware.

**Middleware** functions can perform the following tasks:

Execute any code.
Make changes to the request and the response objects.
End the request-response cycle.
Call the next middleware in the stack.
If the current middleware function does not end the request-response cycle, it must call next() to pass control to the next middleware function. Otherwise, the request will be left hanging.

***

![](https://expressjs.com/images/express-mw.png)
***
> If one of the middleware has instructed the request object to redirect, the view that is ready to execute, will not execute.
For example, if the user is planned on going to the dashboard view, but middleware has told the request to redirect to the login page instead then the dashboard view, and therefore the controller, will not execute at all. It will be skipped over. Masonite checks if the request is redirecting before executing a view.
Also, the request object can be injected into middleware by passing the Request parameter into the constructor 
This will inject the Request class into the constructor when that middleware is executed.

***
> The error "Error: Can't set headers after they are sent." means that you're already in the Body or Finished state, but some function tried to set a header or statusCode. When you see this error, try to look for anything that tries to send a header after some of the body has already been written. For example, look for callbacks that are accidentally called twice, or any error that happens after the body is sent.

***
+ Middleware
> is a type of computer software that provides services to software applications beyond those available from the operating system. It can be described as "software glue"

+ Request Object
> The req object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.

+ Response Object
> The Response interface of the Fetch API represents the response to a request object.

+ Routing Middleware
> Express is a routing and middleware web framework that has minimal functionality of its own: An Express application is essentially a series of middleware function calls.

+ Test-Driven Development
> Test-driven development is a software development process relying on software requirements being converted to test cases before the software is fully developed, and tracking all software development by repeatedly testing the software against all test cases.

+ Behavioral Testing
> Behavioral Testing is a testing of the external behavior of the program, also known as black-box testing. It is usually functional testing.
