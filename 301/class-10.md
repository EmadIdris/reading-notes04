# Readings: In memory storage

+ Invoking a routine which consists of a name and parameters.

+ Only one at a time

> Last in, first out (LIFO) is a method used to account for inventory that records the most recently produced items as sold first. Under LIFO, the cost of the most recent products purchased (or produced) are the first to be expensed as cost of goods sold (COGS), which means the lower cost of older products will be reported as inventory.

![](https://www.easycalculation.com/maths-dictionary/images/lifo.jpg)

![](https://lh3.googleusercontent.com/proxy/A7DJ70toO7PrLDX49aCIP9oIY4WLWYVcREi5RpfnOW_tDgY5WTqrLlkig-0itKzLDtTvUSzS_w7NsH4x2p4VC27V8prH1ADooK5AH2ccMrCmVOrqVJva8_muDfcn8hMetr5o-2qpCW7fpg)

***

+ In JavaScript, a reference error is thrown when a code attempts to reference a non-existing variable. In this article, we will dive into the most common types of reference error triggers and how to fix them.

```
let firstName = "John"
let age = 23
 
console.log(lastName)
// Uncaught ReferenceError: lastName is not defined
let firstName = "John"
let lastName = "Smith"
let age = 23
 
console.log(lastName)
// returns Smith
```

+ The **SyntaxError** object represents an error when trying to interpret syntactically invalid code. It is thrown when the JavaScript engine encounters tokens or token order that does not conform to the syntax of the language when parsing code.

+ The **RangeError** object indicates an error when a value is not in the set or range of allowed values.

+ The **TypeError** object represents an error when an operation could not be performed, typically (but not exclusively) when a value is not of the expected type.

***

## Code Debugging

+ Programming code might contain syntax errors, or logical errors.

+ Many of these errors are difficult to diagnose.

+ Often, when programming code contains errors, nothing will happen. There are no error messages, and you will get no indications where to search for errors.

+ Searching for (and fixing) errors in programming code is called code debugging.

## JavaScript Debuggers

+ Debugging is not easy. But fortunately, all modern browsers have a built-in JavaScript debugger.

+ Built-in debuggers can be turned on and off, forcing errors to be reported to the user.

+ With a debugger, you can also set breakpoints (places where code execution can be stopped), and examine variables while the code is executing.

+ Normally, otherwise follow the steps at the bottom of this page, you activate debugging in your browser with the F12 key, and select "Console" in the debugger menu.

***

+ This error happens when you try to use a variable that isn't declared.