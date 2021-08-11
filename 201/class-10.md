# Debugging

![](https://image.slidesharecdn.com/debugging-javascript-web-141030080414-conversion-gate02/95/debugging-javascript-1-638.jpg?cb=1415345877)


## Error Handling & Debugging

> JavaScript can be hard to learn and everyone makes 
mistakes when writing it. This chapter will help you learn 
how to find the errors in your code. It will also teach you how 
to write scripts that deal with potential errors gracefully. 
When you are writing JavaScript, do not expect to write it perfectly the first time. 
Programming is like problem solving: you are given a puzzle and not only do you have to solve 
it, but you also need to create the instructions that allow the computer to solve it. too. 
When writing a long script, nobody gets everything right in their first attempt. The error 
messages that a browser gives look cryptic at first, but they can help you determine what 
went wrong in your JavaScript and how to fix it. In this chapter you will learn about

![](https://javascript.info/article/debugging-chrome/chrome-sources-debugger-trace-1.svg)

![](https://docs.microsoft.com/en-us/visualstudio/javascript/media/tutorial-nodejs-react-set-breakpoint.png?view=vs-2019)


## ORDER OF EXECUTION

To find the source of an error, it helps to know how scripts are processed. 
The order in which statements are executed can be complex; some tasks 
cannot complete until another statement or function has been run

![](https://i.stack.imgur.com/lHuHk.png)

## EXECUTION CONTEXTS

> The JavaScript interpreter uses the concept of execution contexts. 
There is one global execution context; plus, each function creates a new 
new execution context. They correspond to variable scope.

![](https://miro.medium.com/max/1400/1*e-A-jDYmBTIfN2ADj13iaw.png)

![](https://cpentalk.com/?qa=blob&qa_blobid=6137021251521763964)

## EXECUTION CONTEXT & HOISTING

Each time a script enters a new execution context, there are two phases 
of activity: 
1. PREPARE 
+ The new scope is created 
+ Variables, functions, and arguments are created 
+ The value of the this keyword is determined 

> Understanding that these two phases happen helps 
with understanding a concept called hoisting. You 
may have seen that you can:

+ Call functions before they have been declared 
(if they were created using function declarations 
+ not function expressions, see p96) 
+ Assign a value to a variable that has not yet been 
declared 
This is because any variables and functions within 
each execution context are created before they are 
executed. 
+ The preparation phase is often described as taking 
all of the variables and functions and hoisting them 
to the top of the execution context. Or you can think 
of them as having been prepared. 
Each execution context also creates its own 
vari ab 1 es object. This object contains details of all 
of the variables, functions, and parameters for that 
execution context.


## UNDERSTANDING SCOPE

> In the interpreter, each execution context has its own va ri ables object. 
It holds the variables, functions, and parameters available within it. 
Each execution context can also access its parent's variables object. 

## UNDERSTANDING ERRORS

> If a JavaScript statement generates an error, then it throws an exception. 
At that point, the interpreter stops and looks for exception-handl ing code.

## ERROR OBJECTS

> Error objects can help you find where your mistakes are 
and browsers have tools to help you read them. 

## A DEBUGGING WORKFLOW

> Debugging is about deduction: eliminating potential causes of an error. 
Here is a workflow for techniques you will meet over the next 20 pages. 
Try to narrow down where the problem might be, then look for clues. 

### WHERE IS THE PROBLEM? 
First, should try to can narrow down the area where 
the problem seems to be. In a long script, this is 
especially important. 
1. Look at the error message, it tells you: 
+ The relevant script that caused the problem. 
+ The line number where it became a problem for 
the interpreter. (As you will see, the cause of 
the error may be earlier in a script; but this is the 
point at which the script could not continue.) 
+ The type of error (although the underlying cause 
of the error may be different). 
2. Check how far the script is running. 
Use tools to write messages to the console to tell 
how far your script has executed. 
3. Use breakpoints where things are going wrong. 
They let you pause execution and inspect the values 
that are stored in variables. 

![](https://geshan.com.np/images/debugging-node-js/03ndb-continue.png)

## A DEBUGGING WORKFLOW

> Debugging is about deduction: eliminating potential causes of an error. 
Here is a workflow for techniques you will meet over the next 20 pages. 
Try to narrow down where the problem might be, then look for clues.

## BROWSER DEVTOOLS & JAVASCRIPT CONSOLE 

> The JavaScript console will tell you when there is a problem with a script, 
where to look for the problem, and what kind of issue it seems to be.

![](https://docs.microsoft.com/en-us/microsoft-edge/devtools-guide-chromium/media/console-javascript-console-history.msft.png)

## Summary

+ If you understand execution contexts (which have two 
stages) and stacks, you are more likely to find the error 
in your code. 
+ Debugging is the process of finding errors. It involves a 
process of deduction. 
+ The console helps narrow down the area in which the 
error is located, so you can try to find the exact error. 
+ JavaScript has 7 different types of errors. Each creates 
its own error object, which can tell you its line number 
and gives a description of the error. 
+ If you know that you may get an error, you can handle 
it gracefully using the try, catch, finally statements. 
Use them to give your users helpful feedback.