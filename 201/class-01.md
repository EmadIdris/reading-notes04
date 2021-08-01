# **Introduction** 
#### two different types of people in mind
+ Those who want to learn how to design and build websites 
from scratch
+ Anyone who has a website (that may be built using a 
content management system, blogging software, or an 
e-commerce platform) and wants more control over the 
appearance of their pages

## Topic 

### Is it hard to Learn?
>At work, when people look 
at my screen and see it full of 
code, it's not unusual to get a 
comment about it looking very 
complicated or how clever I must 
be to understand it. The truth 
is, it's not that hard to learn how 
to write web pages and read 
the code used to create them; 
you certainly don't have to be a 
"programmer."
Understanding HTML and CSS 
can help anyone who works 
with the web; designers can 
create more attractive and 
usable sites, website editors can 
create better content, marketers 
can communicate with their 
audience more effectively, and 
managers can commission 
better sites and get the best out 
of their teams.

### The Structure ofThis Book
1. HTML
>We will spend the first chapter 
looking at how HTML is used to 
create web pages. You will see 
that you start by writing down 
the words you want to appear 
on your page. You then add tags 
or elements to the words so 
that the browser knows what is 
a heading, where a paragraph 
begins and ends, and so on

2. CSS
> We start this section with a 
chapter that explains how CSS 
uses rules to enable you to 
control the styling and layout 
of web pages. We then go on to 
look at the wide variety of CSS 
properties you can use in your 
CSS rules

3. Practical
>We end up with some helpful 
information that will assist you in 
building better websites.

### How People Access the Web
the different ways in which people access the web and clarify some terminology.
1. Browsers
> People access websites using 
software called a web browser. 
Popular examples include 
Firefox, Internet Explorer, Safari, 
Chrome, and Opera
2. Web Servers
> When you ask your browser for 
a web page, the request is sent 
across the Internet to a special 
computer known as a web 
server which hosts the website
3. Screen readers
> Screen readers are programs 
that read out the contents of a 
computer screen to a user. They 
are commonly used by people 
with visual impairments.
4. Devices
>  People are accessing websites 
on an increasing range of devices 
including desktop computers, 
laptops, tablets, and mobile 
phones. It is important to 
remember that various devices 
have different screen sizes and 
some have faster connections to 
the web than others.

### How Websites Are Created
1. What you see
> When you are looking at a 
website, it is most likely that 
your browser will be receiving 
HTML and CSS from the web 
server that hosts the site. The 
web browser interprets the 
HTML and CSS code to create 
the page that you see.

2. How it is Created
> Small websites are often written 
just using HTML and CSS.
Larger websites — in particular 
those that are updated regularly 
and use a content management 
system (CMS), blogging tools, or 
e-commerce software — often 
make use of more complex 
technologies on the web server, 
but these technologies are 
actually used to produce HTML 
and CSS that is then sent to the 
browser. So, if your site uses 
these technologies, you will be 
able to use your new HTML and 
CSS knowledge to take more 
control over how your site looks.

3. HTML5 & CSS3
> Since the web was first created 
there have been several versions 
of HTML and CSS — each 
intended to be an improvement 
on the previous version.

# **Structure**
## How Pages Use Structure
> Think about the stories you 
read in a newspaper: for each 
story, there will be a headline, 
some text, and possibly some 
images. If the article is a long 
piece, there may be subheadings 
that split the story into separate 
sections or quotes from those 
involved. Structure helps readers 
understand the stories in the 
newspaper.
The structure is very similar 
when a news story is viewed 
online (although it may also 
feature audio or video). This is 
illustrated on the right with a 
copy of a newspaper alongside 
the corresponding article on its 
website.
Now think about a very different 
type of document — an 
insurance form. Insurance forms 
often have headings for different 
sections, and each section 
contains a list of questions with 
areas for you to fill in details or 
checkboxes to tick. Again, the 
structure is very similar online.

## HTML Describes the Structure of Pages
> In the browser window you can see a web page that features exactly 
the same content as the Word document you met on the page 18. To 
describe the structure of a web page, we add code to the words we want 
to appear on the page.


# **Extra Markup**
## The Evolution of HTML
+ HTML 4
> With the exception of a few 
elements added in HTML5 
(which have been highlighted), 
the elements you have seen in 
this book were all available in 
HTML 4. 
+ XHTML 1.0
> In 1998, a language called XML 
was published. Its purpose 
was to allow people to write 
new markup languages. Since 
HTML was the most widely used 
markup language around, it was 
decided that HTML 4 should be 
reformulated to follow the rules 
of XML and it was renamed 
XHTML. This meant that 
authors had to follow some new, 
more strict rules about writing 
markup.

## DOCTYPES
>Because there have been 
several versions of HTML, each 
web page should begin with a 
DOCTYPE declaration to tell a 
browser which version of HTML 
the page is using (although 
browsers usually display the 
page even if it is not included). 
We will therefore be including 
one in each example for the rest 
of the book
 
## Comments in HTML
<!-- -->
> If you want to add a comment 
to your code that will not be 
visible in the user's browser, you 
can add the text between these 
characters:
<!-- comment goes here -->
It is a good idea to add 
comments to your code because, 
no matter how familiar you 
are with the page at the time 
of writing it, when you come 
back to it later (or if someone 
else needs to look at the code), 
comments will make it much 
easier to understand.

## ID Attribute
> Every HTML element can carry 
the id attribute. It is used to 
uniquely identify that element 
from other elements on the 
page. Its value should start with 
a letter or an underscore (not a 
number or any other character).
It is important that no two 
elements on the same page 
have the same value for their id
attributes (otherwise the value is 
no longer unique).

## Class Attribute
>Every HTML element can 
also carry a class attribute. 
Sometimes, rather than uniquely 
identifying one element within 
a document, you will want a 
way to identify several elements 
as being different from the 
other elements on the page. 
For example, you might have 
some paragraphs of text that 
contain information that is more 
important than others and want 
to distinguish these elements, or 
you might want to differentiate 
between links that point to other 
pages on your own site and links 
that point to external sites. 

## Block Elements
> Some elements will always 
appear to start on a new line in 
the browser window. These are 
known as block level elements

## Inline Elements
> Some elements will always 
appear to continue on the 
same line as their neighbouring 
elements. These are known as 
inline elements

## Grouping Text & Elements In a Block
> The <div> element allows you to 
group a set of elements together 
in one block-level box.
For example, you might create 
a <div> element to contain all 
of the elements for the header 
of your site (the logo and the 
navigation), or you might create 
a <div> element to contain 
comments from visitors

# **HTML5 Layout**
## Traditional HTML Layouts
> For a long time, web page authors used <div> elements to group 
together related elements on the page (such as the elements that form a 
header, an article, footer or sidebar). Authors used class or id attributes 
to indicate the role of the <div> element in the structure of the page

## New Html5 Layout Elements
> HTML5 introduces a new set of elements that allow you to divide up the 
parts of a page. The names of these elements indicate the kind of content 
you will find in them. They are still subject to change, but that has not 
stopped many web page authors using them already.

## Headers & Footers <header> <footer>
The  and 
elements can be used for:
+ The main header or footer 
that appears at the top or 
bottom of every page on the 
site.
+ A header or footer for an 
individual  within the page.

## Navigation <nav>
> The  element is used to 
contain the major navigational 
blocks on the site such as the 
primary site navigation.

## Articles <article>
>The  element acts as 
a container for any section of a 
page that could stand alone and 
potentially be syndicated.

## Article
>The element has two 
purposes, depending on whether 
it is inside an
element or not

# **Process & Design**
+ It's important to understand who your target audience 
is, why they would come to your site, what information 
they want to find and when they are likely to return.
+ Site maps allow you to plan the structure of a site.
+ Wireframes allow you to organize the information that 
will need to go on each page.
+ Design is about communication. Visual hierarchy helps 
visitors understand what you are trying to tell them.
+ You can differentiate between pieces of information 
using size, color, and style. 
+ You can use grouping and similarity to help simplify 
the information you present


*****

# JavaScript
> To get the most out of this book, you will need to know how to bui ld web pages using HTML 
and CSS. Beyond that. no prior experience with programming is necessary. Learning to 
program with JavaScript 

## The ABC of Programming
+ A script is a series of instructions that the computer 
can follow in order to achieve a goal. 
+ Each time the script runs, it might only use a subset of 
all the instructions. 
+ Computers approach tasks in a different way than 
humans, so your instructions must let the computer 
solve the task prggrammatically. 
+ To approach writing a script, break down your goal into 
a series of tasks and then work out each step needed 
to complete that task (a flowchart can help).