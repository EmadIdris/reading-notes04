# Readings: REST

+ Senior Principal Scientist at Adobe, is known for his pioneering work on the World Wide Web, open source, and software architecture.

***

+ Because they weren't designed to be used like that. When Fielding and his colleagues started building the web, being able to talk to any machine anywhere in the world was a primary concern. But most of the techniques developers later used to get computers to talk to each other didn't have those requirements. You just needed to talk to a small group of machines.

***

+ Web pages usually have images, right? Those are separate resources. The web page just specifies the URLs to the images and the browser goes and does more GETs using the HTTP protocol on them until all the resources are obtained and the web page is displayed. But the important thing here is that very different kinds of nouns can be treated the same. Whether the noun is an image, text, video, an mp3, a slideshow, whatever. I can GET all of those things the same way given a URL.


***

+ is used to **get** *resources* from their URLs

+ In computing, POST is a request method supported by HTTP used by the World Wide Web. By design, the POST request method requests that a web server accepts the data enclosed in the body of the request message, most likely for storing it. It is often used when uploading a file or when submitting a completed web form.

> POST is a method that is supported by HTTP and depicts that a web server accepts the data included in the body of the message, which is requested. POST is often used by World Wide Web to send user generated data to the web server or when you upload file.

***

+ **PUT** method is called when you have to modify a single resource while POST method is called when you have to add a child resource.
+ **PUT** method response can be cached but you cannot cache POST method responses.

***

+ A patch is a set of changes to a computer program or its supporting data designed to update, fix, or improve it.This includes fixing security vulnerabilities[ and other bugs, with such patches usually being called bugfixes or bug fixes.Patches are often written to improve the functionality, usability, or performance of a program.

+ Patches may be installed either under programmed control or by a human programmer using an editing tool or a debugger. They may be applied to program files on a storage device, or in computer memory. Patches may be permanent (until patched again) or temporary.

+ In **PUT** method, the client decides which URI resource should have, and in POST method, the server decides which URI resource should have.

+ **PUT** works as specific while POST work as abstract.

+ If you send the same **PUT** request multiple times, the result will remain the same but if you send the same POST request multiple times, you will receive different results.
PUT method is idempotent whereas POST method is not idempotent.

+ **PATCH** is somewhat analogous to the "update" concept found in CRUD (in general, HTTP is different than CRUD, and the two should not be confused).

+ A **PATCH** request is considered a set of instructions on how to modify a resource. Contrast this with PUT; which is a complete representation of a resource.

+ A **PATCH** is not necessarily idempotent, although it can be. Contrast this with PUT; which is always idempotent. The word "idempotent" means that any number of repeated, identical requests will leave the resource in the same state. For example if an auto-incrementing counter field is an integral part of the resource, then a PUT will naturally overwrite it (since it overwrites everything), but not necessarily so for PATCH.

+ **PATCH** (like POST) may have side-effects on other resources.