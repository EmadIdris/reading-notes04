# Problem Domain, Objects, and the DOM

# Understanding The Problem Domain Is The Hardest Part Of Programming

There are many common answers to this question:
+ Learning a new technology
+ Naming things
+ Testing your code
+ Debugging
+ Fixing bugs
+ Making software maintainable

## Programming is easy if you understand the problem domain

## What can you do about it?

If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

1. Make the problem domain easier
2. Get better at understanding the problem domain

****
# JavaScript
# Object 

## WHAT IS AN OBJECT?
Objects group together a set of variables and functions to create a model 
of a something you would recognize from the real world. In an object, 
variables and functions take on new names

> IN AN OBJECT: VARIABLES BECOME 
KNOWN AS PROPERTIES 
If a variable is part of an object, it is called a 
**property**. Properties tell us about the object, such as 
the name of a hotel or the number of rooms it has. 
Each individual hotel might have a different name 
and a different number of rooms.

![](https://fireship.io/courses/javascript/img/js-object-props.png)


> IN AN OBJECT: FUNCTIONS BECOME 
KNOWN AS METHODS 
If a function is part of an object, it is called a **method**. 
Methods represent tasks that are associated with 
the object. For example, you can check how many 
rooms are available by subtracting the number of 
booked rooms from the total number of rooms.

![](https://dmitripavlutin.com/static/d0597f7819971bf2b124b653b673eb29/05127/cover-2.png)

+ Like variables and named functions, 
properties and methods have a 
name and a value. In an object, 
that name is called a key. 
+ An object cannot have two keys 
with the same name. This is 
because keys are used to access 
their corresponding values. 
+ The value of a property can be a 
string, number, Boolean, array, or 
even another object. The value of a 
method is always a function. 

![](https://miro.medium.com/max/795/1*rSHmnlUotrjc5lXV1xDtGA.png)
![](https://appdividend.com/wp-content/uploads/2019/03/Javascript-Objects-Tutorial-Example-Working-With-Objects-in-JS.png)
![](https://cdn.programiz.com/sites/tutorial2program/files/javascript-object-properties.png)

## Programmers use a lot of name/value pairs: 
+ HTML uses attribute names and values. 
+ CSS uses property names and values. 
In JavaScript: 
+ Variables have a name and you can assign them a 
value of a string, number, or Boolean. 
+ Arrays have a name and a group of values. (Each 
item in an array is a name/value pair because it 
has an index number and a value.) 
+ Named functions have a name and value that is a 
set of statements to run if the function is called. 
+ Objects consist of a set of name/value pairs 
(but the names are referred to as keys). 

## Literal notation is the easiest and most poplular way to create object

## you access the properties or method of an object using dot notation or square brackets

![](https://dmitripavlutin.com/static/50a87420915de18f26da616865fe9825/05127/access-object-properties-2.png)

***

# Document Object Model

![](https://simplesnippets.tech/wp-content/uploads/2018/10/what-is-document-object-model-in-JS-featured-image.jpg)

+ The browser represents the page using a DOM tree. 
+ DOM trees have four types of nodes: document nodes, 
element nodes, attribute nodes, and text nodes. 
+ You can select element nodes by their id or cl ass 
attributes, by tag name, or using CSS selector syntax. 
+ Whenever a DOM query can return more than one 
node, it will always return a Nadel i st. 
+ From an element node, you can access and update its 
content using properties such as textContent and 
i nnerHTML or using DOM manipulation techniques. 
+ An element node can contain multiple text nodes and 
child elements that are siblings of each other. 
+ In older browsers, implementation of the DOM is 
inconsistent (and is a popular reason for using jQuery). 
+ Browsers offer tools for viewing the DOM tree .

![](data:image/png;base64,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)