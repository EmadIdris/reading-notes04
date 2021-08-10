# Forms and JS Events
# Forms

> The best known form on the web is probably 
the search box that sits right in the middle of 
Google's homepage

There are several types of form controls that 
you can use to collect information from visitors 
to your site

+ ADDING TEXT
+ Making Choices
+ Submitting Forms
+ Uploading Files

![](https://uicookies.com/wp-content/uploads/2018/03/contact-form-5-free-html-contact-forms.jpg)

## How Forms Work 

>A user fills in a form and then presses a button 
to submit the information to the server.

![](https://cdn.educba.com/academy/wp-content/uploads/2020/03/Registration-Form-in-HTML-1.6.png)

# Form Structure

+ Form controls live inside a 
element. This element 
should always carry the action
attribute and will usually have a 
method and id attribute too.
action
+ Every  element requires 
an action attribute. Its value
is the URL for the page on the 
server that will receive the 
information in the form when it 
is submitted.
method
+ Forms can be sent using one of 
two methods: get or post.
With the get method, the values 
from the form are added to 
the end of the URL specified in 
the action attribute. The get
method is ideal for:
+ short forms (such as search 
boxes)
+ when you are just retrieving 
data from the web server 
(not sending information that 
should be added to or deleted 
from a database)

# Summary

+ Whenever you want to collect information from 
visitors you will need a form, which lives inside a 
element.
+ Information from a form is sent in name/value pairs.
+ Each form control is given a name, and the text the 
user types in or the values of the options they select 
are sent to the server.
+ HTML5 introduces new form elements which make it 
easier for visitors to fill in forms


![](https://miro.medium.com/max/1200/1*wv2QKvaAWtNOkxK41xoQig.png)
![](https://qawithexperts.com/Images/Upload/23-09-2018/html-code-to-create-a-form-min.png)


# Lists, Tables & Forms 

> The list-style-type property 
allows you to control the shape 
or style of a bullet point (also 
known as a marker)

> You can specify an image to act 
as a bullet point using the
list-style-image property.
The value starts with the letters 
url and is followed by a pair 
of parentheses. Inside the 
parentheses, the path to the 
image is given inside double 
quotes.
This property can be used on 
rules that apply to the  and 
 elements.
The example on this page also 
shows the use of the margin
property to increase the vertical 
gap between each item in the 
list

# Table Properties

+ You have already met several 
properties that are commonly 
used with tables. Here we will 
put them together in a single 
example using the following:
+ width to set the width of the 
table
+ padding to set the space 
between the border of each table 
cell and its content
+ text-transform to convert the 
content of the table headers to 
uppercase
+ letter-spacing, font-size
to add additional styling to the 
content of the table headers
+ border-top, border-bottom
to set borders above and below 
the table headers
+ text-align to align the writing 
to the left of some table cells and 
to the right of the others
+ background-color to change 
the background color of the 
+ alternating table rows
:hover to highlight a table row 
when a user's mouse goes over i

# Summary

+ In addition to the CSS properties covered in other 
chapters which work with the contents of all elements, 
there are several others that are specifically used to 
control the appearance of lists, tables, and forms.
+ List markers can be given different appearances 
using the list-style-type and list-style image 
properties.
+ Table cells can have different borders and spacing in 
different browsers, but there are properties you can 
use to control them and make them more consistent. 
+ Forms are easier to use if the form controls are 
vertically aligned using CSS.
+ Forms benefit from styles that make them feel more 
interactive


***

# JS Events

When you browse the web, your browser registers different 
types of events. It's the browser's way of saying, "Hey, this 
just happened." Your script can then respond to these events. 
Scripts often respond to these events by updating the content of the web page (via the 
Document Object Model) which makes the page feel more interactive. In this chapter, you 
will learn how: 

+ INTERACTIONS EVENTS TRIGGER CODE RESPONDS 
+ CREATE EVENTS CODE TO USERS

> Events occur when users When an event occurs, In the last chapter, you 
click or tap on a link, hover or fires, it can be used saw how the DOM can 
or swipe over an element, to trigger a particular be used to update a page. 
t ype on the keyboard, function. Different code The events can trigger the 
resize the window, or can be triggered when -kinds of changes the DOM 
when the page they users interact with is capable of. This is how a 
requested has loaded. different parts of the page. web page reacts to users

![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/JavaScript-Event-Types.jpg)

## HOW EVENTS TRIGGER JAVASCRIPT CODE
When the user interacts with the HTML on a web page, there are three 
steps involved in getting it to trigger some JavaScript code. 
Together these steps are known as event handling.

+ Select t he element 
node(s) you want the 
script to respond to. 
For example, if you want to 
trigger a function when a user 
clicks on a specific link, you need 
to get the DOM node for that 
link element. You do this using a 
DOM query

+ Indicate which event on 
the selected node(s) will 
trigger the response. 
Programmers call this binding an 
event to a DOM node. 
The previous two pages showed 
a selection of the popular events 
that you can monitor for. 

+ State the code you want 
to run when the event 
occurs. 
W hen the event occurs, on a 
specified element, it will trigger 
a function. This may be a named 
or an anonymous function.

![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/JavaScript-event.jpg)

## THREE WAYS TO BIND AN EVENT TO AN ELEMENT

> Event handlers let you indicate which event you 
are waiting for on any particular element. 
There are three types of event handlers. 

![](https://img.youtube.com/vi/DXm6DGOv6_Q/hqdefault.jpg)

![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/05/Django-form-HTML-code.png)

## Summary

+ Events are the browser's way of indicating when 
something has happened (such as when a page has 
finished loading or a button has been clicked). 
+ Binding is the process of stating which event you are 
waiting to happen, and which element you are waiting 
for that event to happen upon. 
+ When an event occurs on an element, it can trigger a 
JavaScript function. When this function then changes 
the web page in some way, it feels interactive because 
it has responded to the user. 
+ You can use event delegation to monitor for events 
that happen on all of the children of an element. 
+ The most commonly used events are W3C DOM 
events, although there are others in the HTMLS 
specification as well as browser-specific events

