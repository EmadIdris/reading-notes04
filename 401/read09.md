
## What header(s) are used in authentication and authorization
Basic Auth

> It is a simple authentication scheme built into the HTTP protocol. The client sends HTTP requests with the Authorization header that contains the word Basic, followed by a space and a base64-encoded(non-encrypted) string username: password. For example, to authorize as username / Pa$$w0rd the client would send.

*Bearer Token:*

> Commonly known as token authentication. It is an HTTP authentication scheme that involves security tokens called bearer tokens. As the name depicts “Bearer Authentication” gives access to the bearer of this token.
***
> What is safe to put into a JWT

A JWT needs to be stored in a safe place inside the user’s browser.

> To keep them secure, you should always store JWTs inside an httpOnly cookie. This is a special kind of cookie that’s only sent in HTTP requests to the server. It’s never accessible (both for reading or writing) from JavaScript running in the browser.

*How are JWTs validated*

> When you receive a JWT from the client, you can verify that JWT with this that secret key stored on the server.

> Any modification to the JWT will result in verification (JWT validation) failure.

> A JWT is simply a string but it contains three distinct parts separated with dots (.).

> The Application server, instead of just taking the username from the header, will first validate the JWT: if the signature is correct, then the user is correctly authenticated and the request goes through. if not, the application server can simply reject the request.

Document the following Vocabulary Terms

**RBAC**

> Role-based access control (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges. The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments.

**User Roles**

> User Roles are permission sets that control access to areas and features within the Professional Archive Platform. Each User account requires a Role assignment.

**JWT Token**

> JSON Web Token is a proposed Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims. The tokens are signed either using a private secret or a public/private key.