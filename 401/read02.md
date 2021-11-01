# Readings: Express

# PUT vs PATCH
> When learning web development and HTTP specification, it is not unlikely to find yourself getting confused about the type of verb to use, and when to use it. With most applications on the internet being CRUD (create, read/retrieve, updates, delete), developers must learn how to match HTTP verbs to these actions. Typically, the verbs and actions are matched as follows:

+ POST – Create
+ GET – Read/Retrieve
+ PUT/PATCH – Update
+ DELETE – Delete

> From this mapping, it is not surprising that most people think that PUT and PATCH are allies that do the same thing. However, the reality is far more complex, especially when it comes to overlapping functionality and other complications. Actually, PUT and PATCH might be doing the same thing of updating a resource at a location, but they do it differently. Therefore, to understand more about these verbs, let’s dive deep into HTTP specification and identify the subtle differences between the two.

### What is PUT?

> PUT is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely. PUT is similar to POST in that it can create resources, but it does so when there is a defined URI. PUT overwrites the entire entity if it already exists, and creates a new resource if it doesn’t exist.

> For example, when you want to change the first name of a person in a database, you need to send the entire resource when making a PUT request.

```{“first": "John", "last": "Stone”}```
To make a PUT request, you need to send the two parameters; the first and the last name.

### What is PATCH?
Unlike PUT, PATCH applies a partial update to the resource.

> This means that you are only required to send the data that you want to update, and it won’t affect or change anything else. So if you want to update the first name on a database, you will only be required to send the first parameter; the first name.

## Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

+ [jayson](https://www.npmjs.com/package/jayson) 
+ [json-graphql-server](https://www.npmjs.com/package/json-graphql-server) 
+ [fakerest](https://www.npmjs.com/package/fakerest)

##

> Swagger is similar to Postman. you can create request in the swagger site, you will see the console.logs in your terminal when that request is ran APIdoc.js is a node module that "creates a documentation from API descriptions in your source"

+ **Swagger**
```
  '200':
    description: OK
  '400':
    description: Bad request. User ID must be an integer and larger than 0.
  '401':
    description: Authorization information is missing or invalid.
  '404':
    description: A user with the specified ID was not found.
  '5XX':
    description: Unexpected error
```


+ ***APIDoc.js 1***

```
  '200':
  	Successful request and response.
  '400':
  	Malformed parameters or other bad request.
```

##

1. SOAP is a XML-based message protocol, while REST is an architectural style
2. SOAP uses WSDL for communication between consumer and provider, whereas REST just uses XML or JSON to send and receive data
3. SOAP invokes services by calling RPC method, REST just simply calls services via URL path
4. SOAP doesn't return human readable result, whilst REST result is readable with is just plain XML or JSON
5. SOAP is not just over HTTP, it also uses other protocols such as SMTP, FTP, etc, REST is over only HTTP

***

+ Web Server

> A web server is computer software and underlying hardware that accepts requests and send responses via HTTP or its secure variant HTTPS, the network protocols created to distribute web contents to client user agents.

+ Express
> Express.js, or simply Express, is a back end web application framework for Node.js, released as free and open-source software under the MIT License. It is designed for building web applications and APIs. It has been called the de facto standard server framework for Node.js.

+ Routing
> Routing is the process of selecting a path for traffic in a network or between or across multiple networks. Broadly, routing is performed in many types of networks, including circuit-switched networks, such as the public switched telephone network, and computer networks, such as the Internet.

+ WRRC
> web Request/Response Cycle The request line is made up of a HTTP method, the URI( path of the resource), and the HTTP version. The headers are made up of metadata and components of information about the request being sent such as cookies and authentication tokens. The body contains information that is being sent to the server ("payload"). Examples of information sent to the server may include form data.