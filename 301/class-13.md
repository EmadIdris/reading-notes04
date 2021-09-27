# Readings: CRUD

## CRUD (Create, Read, Update, Delete)

+ These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. Like using a different protocol or telling the client that its request will fail before they start sending the body.

+ These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.

+ These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. This can have multiple reasons, be temporary or permanent, but the client has to issue a request to the new location.

+ These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication, etc. A client is sending incorrect input and should confirm the input parameters are correct before retrying the request.

+ These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. These errors can be temporary or permanent. Usually it’s best for the client to retry the same request.

### CREATE

+ 202 Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.

### READ

+ 308 Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

## UPDATE

+ 202 Accepted - If the update is done asynchronous, this code can be used. It should include an URL to access the updated resource or an URL to check if the update has been succeeded. It can also include an estimation of how long the update will take.

## DELETE

+ 202 Accepted - If the deletion is asynchronous and takes some time, which is the case in distributed systems, it can be appropriate to return this code with some information or URL to tell the client when it will be deleted.

***

+ 200 OK
+ 202 Accepted
+ 204 No Content
+ 400 Bad Request
+ 404 Not Found

> 403 Forbidden The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

***

+ Because when using the application we will use a different string that the local host.

+ Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next.

+ it allows the database to accept JSON in the body.

```
app.get('/summary/:id', function(req, res) {
    req.logout();
    Session.findOne({_id: req.params.id}, function(err, result) {
        if (err) {
            console.log(err);
            res.end(ERROR);
            return;
        }
        res.render('summary.ejs', {
            data: result._id,
            name : result.name
        });
    });
});
```
+  it means that this is a parameter.

+ In computing, the PATCH method is a request method supported by the Hypertext Transfer Protocol (HTTP) protocol for making partial changes to an existing resource.[1] The PATCH method provides an entity containing a list of changes to be applied to the resource requested using the HTTP Uniform Resource Identifier (URI).[1] The list of changes are supplied in the form of a PATCH document.[1] If the requested resource does not exist then the server may create the resource depending on the PATCH document media type and permissions. The changes described in the PATCH document must be semantically well defined but can have a different media type than the resource being patched. Frameworks such as XML, JSON can be used in describing the changes in the PATCH document.

+ Your schemas can define default values for certain paths. If you create a new document without that path set, the default will kick in.

+ by giving it a default parameter.

```
const schema = new Schema({
  name: String,
  role: { type: String, default: 'guitarist' }
});

const Person = db.model('Person', schema);

const axl = new Person({ name: 'Axl Rose', role: 'singer' });
assert.equal(axl.role, 'singer');

const slash = new Person({ name: 'Slash' });
assert.equal(slash.role, 'guitarist');

const izzy = new Person({ name: 'Izzy', role: undefined });
assert.equal(izzy.role, 'guitarist');

// Defaults do **not** run on `null`, `''`, or value other than `undefined`.
const foo = new Person({ name: 'Bar', role: null });
assert.strictEqual(foo.role, null);

Person.create(axl, slash, function(error) {
  assert.ifError(error);
  Person.find({ role: 'guitarist' }, function(error, docs) {
    assert.ifError(error);
    assert.equal(docs.length, 1);
    assert.equal(docs[0].name, 'Slash');
  });
});
```
+ generic error response.

+ 200 - OK
> The 200 status code is by far the most common returned. It means, simply, that the request was received and understood and is being processed.

+ 201 - Created
> A 201 status code indicates that a request was successful and as a result, a resource has been created (for example a new page).

