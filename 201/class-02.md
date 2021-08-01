# Duckett HTML book
## Text
+ HTML elements are used to describe the structure of 
the page (e.g. headings, subheadings, paragraphs).
+ They also provide semantic information (e.g. where 
emphasis should be placed, the definition of any 
acronyms used, when given text is a quotation)

![Test](https://www.thoughtco.com/thmb/EODIoetCRBiRHEmXVuEmrIsr2Ns=/1756x1317/smart/filters:no_upscale()/463376515-5804f6585f9b5805c2cc5fad.jpg)

****
### Headings
>Browsers display the contents of 
headings at different sizes. The 
contents of an <h1> element is 
the largest, and the contents of 
an <h6> element is the smallest. 
The exact size at which each 
browser shows the headings 
can vary slightly. Users can also 
adjust the size of text in their 
browser. You will see how to 
control the size of text, its color, 
and the fonts used when we 
come to look at CSS.

![Heading](https://www.schudio.com/wp-content/uploads/2016/10/html-headings.png?x43850)

### Paragraphs
>To create a paragraph, surround 
the words that make up the 
paragraph with an opening <p>
tag and closing </p> tag.
By default, a browser will show 
each paragraph on a new line 
with some space between it and 
any subsequent paragraphs

![Paragraphs](https://codebridgeplus.com/wp-content/uploads/html_paragraph.jpg)

### Bold & Italic
>By enclosing words in the tags 
<b> and </b> we can make 
characters appear bold.
The <b> element also represents 
a section of text that would be 
presented in a visually different 
way (for example key words in a 
paragraph) although the use of 
the <b> element does not imply 
any additional meaning
### Superscript & Subscript
>The <sup> element is used 
to contain characters that 
should be superscript such 
as the suffixes of dates or 
mathematical concepts like 
raising a number to a power such 
as 22

![Bold & Italic](http://developersdesire.files.wordpress.com/2014/09/biu-page-0.jpg?w=593)

### White Space

>In order to make code easier to 
read, web page authors often 
add extra spaces or start some 
elements on new lines.
When the browser comes across 
two or more spaces next to each 
other, it only displays one space. 
Similarly if it comes across a line 
break, it treats that as a single 
space too. This is known as 
white space collapsing.
You will often see that web page 
authors take advantage of white 
space collapsing to indent their 
code in order to make it easier 
to follow.

![White Space](https://www.impressivewebs.com/images/ws-prewrap.jpg)

### Line Breaks & Horizontal Rules

>As you have already seen, the 
browser will automatically show 
each new paragraph or heading 
on a new line. But if you wanted 
to add a line break inside the 
middle of a paragraph you can 
use the line break tag <br />

![Line Breaks & Horizontal Rules](https://slidetodoc.com/presentation_image_h/21cc658d525409cf2ca673d2e23cc943/image-14.jpg)


### Semantic Markup
>There are some text elements that are not intended to affect the 
structure of your web pages, but they do add extra information to the 
pages — they are known as semantic markup.

![Semantic Markup](https://miro.medium.com/max/1000/1*zHJFnu7QF-PgUb8108aLcA.png)

### Strong & Emphasis

>The use of the <strong>
element indicates that its 
content has strong importance. 
For example, the words 
contained in this element might 
be said with strong emphasis.
By default, browsers will show 
the contents of a <strong>
element in bold.

![Strong & Emphasis](https://slideplayer.com/slide/13763989/85/images/15/Using+Markup+Languages%3A+HTML.jpg)

### Quotations

> The <blockquote> element is 
used for longer quotes that take 
up an entire paragraph. Note 
how the <p> element is still 
used inside the <blockquote>
element. 
Browsers tend to indent the 
contents of the <blockquote>
element, however you should not 
use this element just to indent a 
piece of text — rather you should 
achieve this effect using CSS.

![Quotations](https://s1.o7planning.com/en/12467/images/47184216.png)

### Abbreviations & Acronyms
> If you use an abbreviation or 
an acronym, then the <abbr>
element can be used. A title
attribute on the opening tag is 
used to specify the full term.
In HTML 4 there was a separate 
<acronym> element for 
acronyms. To spell out the full 
form of the acronym, the title
attribute was used (as with the 
<abbr> element above). HTML5 
just uses the <abbr> element 
for both abbreviations and 
acronyms

![Abbreviations & Acronyms](https://www.android-examples.com/wp-content/uploads/2016/03/abbr-tag.png)

### Citations & Definitions

>When you are referencing a 
piece of work such as a book, 
film or research paper, the 
<cite> element can be used 
to indicate where the citation is 
from.
In HTML5, <cite> should not 
really be used for a person's 
name — but it was allowed in 
HTML 4, so most people are 
likely to continue to use it.
Browsers will render the content 
of a <cite> element in italics.


### Author Details

>The <address> element has 
quite a specific use: to contain 
contact details for the author of 
the page.
It can contain a physical address, 
but it does not have to. For 
example, it may also contain a 
phone number or email address.
Browsers often display the 
content of the <address>
element in italics.
You may also be interested in 
something called the hCard 
microformat for adding physical 
address information to your 
markup

### Changes to Content

>The <ins> element can be used 
to show content that has been 
inserted into a document, while 
the <del> element can show text 
that has been deleted from it.
The content of a <ins> element 
is usually underlined, while the 
content of a <del> element 
usually has a line through it

****

# Introducing CSS

![CSS](https://www.freetutorialsplus.com/css-tutorial/images/css-illustration.png)

CSS allows you to create rules that specify how the content of 
an element should appear. For example, you can specify that 
the background of the page is cream, all paragraphs should 
appear in gray using the Arial typeface, or that all level one 
headings should be in a blue, italic, Times typeface.

+ CSS treats each HTML element as if it appears inside 
its own box and uses rules to indicate how that 
element should look.
+ Rules are made up of selectors (that specify the 
elements the rule applies to) and declarations (that 
indicate what these elements should look like).
+ Different types of selectors allow you to target your 
rules at different elements.
+ Declarations are made up of two parts: the properties 
of the element that you want to change, and the values 
of those properties. For example, the font-family 
property sets the choice of font, and the value arial 
specifies Arial as the preferred typeface.
+ CSS rules usually appear in a separate document, 
although they may appear within an HTML page


****

# JavaScript

![JS](https://2.bp.blogspot.com/-z6q9nVbRxTI/XD-eNSUWtrI/AAAAAAAAMC0/bYratloel2AytKlQXuaFqD51D3P54xE5gCLcBGAs/s1600/%25D9%2585%25D8%25B5%25D8%25A7%25D8%25AF%25D8%25B1%2B%25D8%25AA%25D8%25B9%25D9%2584%25D9%2585%2B%25D8%25AC%25D8%25A7%25D9%2581%25D8%25A7%2B%25D8%25B3%25D9%2583%25D8%25B1%25D9%258A%25D8%25A8%25D8%25AA.png)

## Basic JavaScript Instructions
+ A script is made up of a series of statements. Each 
statement is like a step in a recipe. 
+ Scripts contain very precise instructions. For example, 
you might specify that a value must be remembered 
before creating a calculation using that value. 
+ Variables are used to temporarily store pieces of 
information used in the script. 
+ Arrays are special types of variables that store more 
than one piece of related information. 
+ JavaScript distinguishes between numbers (0-9), 
strings (text), and Boolean values (true or false). 
+ Expressions evaluate into a single value. 
+ Expressions rely on operators to calculate a value.
## Decisions and Loops
+ Conditional statements allow your code to make 
decisions about what to do next. 
+ Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>) 
are used to compare two operands. 
+ Logical operators allow you to combine more than one 
set of comparison operators. 
+ if ... else statements allow you to run one set of code 
+ if a condition is true, and another if it is false. 
+ switch statements allow you to compare a value 
against possible outcomes (and also provides a default 
option if none match). 
+ Data types can be coerced from one type to another. 
+ All values evaluate to either truthy or falsy. 
+ There are three types of loop: for, while, and 
do ... while. Each repeats a set of statements. 




