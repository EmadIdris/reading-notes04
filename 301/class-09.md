# Readings: FUNCTIONAL PROGRAMMING

+ ## **Functional programming** is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

***

+ It returns the same result if given the same arguments (it is also referred as deterministic)

+ It does not cause any observable side effects

***

+ Immediatly testable.
+ Easier maintaining, refactoring, and testing.
+ No need for mocking anything.

***

> In object-oriented and functional programming, an immutable object (unchangeable object) is an object whose state cannot be modified after it is created. This is in contrast to a mutable object (changeable object), which can be modified after it is created. In some cases, an object is considered immutable even if some internally used attributes change, but the object's state appears unchanging from an external point of view. For example, an object that uses memoization to cache the results of expensive computations could still be considered an immutable object.

***

> Referential transparency and referential opacity are properties of parts of computer programs. An expression is called referentially transparent if it can be replaced with its corresponding value (and vice-versa) without changing the program's behavior. This requires that the expression be pure, that is to say the expression value must be the same for the same inputs and its evaluation must have no side effects. An expression that is not referentially transparent is called referentially opaque.

***

+ Module in Node.js is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node.js application.

+ Each module in Node.js has its own context, so it cannot interfere with other modules or pollute global scope. Also, each module can be placed in a separate .js file under a separate folder.

+ Node.js implements CommonJS modules standard. CommonJS is a group of volunteers who define JavaScript standards for web server, desktop, and console application.

***

> Modules are created in Node.js by creating a JavaScript file. Every time you create a new file with .js extension, it becomes a module.Let’s write our first module. We will start by creating two functions to do simple calculations.Type the following code and save it as lib.js inside your nodejs directory.

***

+ It imports the data from a module, given it's path. 

***
+  access the module functions
