# Readings : Audio, Video, Images

## Images

> Controlling the size and alignment of 
your images using CSS keeps rules that 
affect the presentation of your page in 
the CSS and out of the HTML markup.

You can also achieve several interesting effects using 
background images. In this chapter you will learn how to:

+ Specify the size and alignment of an image using
+ Add background images to boxes
+ Create image rollovers in CSS

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT7hcqgYHVZTGLiGC0JBiGyocBM0DT2TkWvPg&usqp=CAU)


## CONTROLLING SIZES OF IMAGES IN CSS

+ You can control the size of an 
image using the width and 
height properties in CSS, just 
like you can for any other box. 
Specifying image sizes helps 
pages to load more smoothly 
because the HTML and CSS 
code will often load before the 
images, and telling the browser 
how much space to leave for an 
image allows it to render the rest 
of the page without waiting for 
the image to download.
+ You might think that your site 
is likely to have images of all 
different sizes, but a lot of sites 
use the same sized image across 
many of their pages. 
+ For example, an e-commerce site 
tends to show product photos 
at the same size. Or, if your site 
is designed on a grid, then you 
might have a selection of image 
sizes that are commonly used on 
+ all pages, such as:
Small portrait: 220 x 360
Small landscape: 330 x 210
Feature photo: 620 x 400
Whenever you use consistently 
sized images across a site, 
you can use CSS to control 
the dimensions of the 
images, instead of putting the 
dimensions in the HTML.

![](https://css-tricks.com/wp-content/csstricks-uploads/fullpagebackground.jpg)

## ALIGNING IMAGES USING CSS

+ In the last chapter, you saw how 
the float property can be used 
to move an element to the left or 
the right of its containing block, 
allowing text to flow around it.

+ Rather than using the 
element's align attribute, web 
page authors are increasingly 
using the float property to align 
images. There are two ways that 
this is commonly achieved:
1. The float property is added 
to the class that was created to 
represent the size of the image 
(such as the small class in our 
example).
2. New classes are created with 
names such as align-left or 
align-right to align the images 
to the left or right of the page. 
These class names are used in 
addition to classes that indicate 
the size of the image.

![](https://static.javatpoint.com/csspages/images/how-to-align-images-in-css.png)

## Centering images Using CSS

By default, images are inline 
elements. This means that they 
flow within the surrounding text. 
In order to center an image, it 
should be turned into a blocklevel element using the display
property with a value of block. 
Once it has been made into a 
block-level element, there are 
two common ways in which you 
can horizontally center an image:
1. On the containing element, 
you can use the text-align
property with a value of center.
2. On the image itself, you can 
use the use the margin property 
and set the values of the left and 
right margins to auto.
You can specify class names 
that allow any element to be 
centered, in the same way that 
you can for the dimensions or 
alignment of images.
The techniques for specifying 
image size and alignment of 
images can also be used with 
the HTML5  element, 
which you met on page 119.

![](https://www.freecodecamp.org/news/content/images/2020/08/centering-css-tweet.jpeg)

## Background Images , Repeating Images

+ The background-image
property allows you to place 
an image behind any HTML 
element. This could be the entire 
page or just part of the page. By 
default, a background image will 
repeat to fill the entire box.

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTdoBCbELJB4WX6gP1AWmPku_PclctyAx_sig&usqp=CAU)

![](https://miro.medium.com/max/1400/1*LjSWkPlCBhsOaB_QCJtaCw.png)


+ The background image is 
repeated both horizontally and 
vertically (the default way it 
is shown if the backgroundrepeat property isn't used)

![](https://i.ytimg.com/vi/6S3Lq4Vhu8o/maxresdefault.jpg)

## Background Position

+ When an image is not being 
repeated, you can use the 
background-position
property to specify where in the 
browser window the background 
image should be placed. 
+ This property usually has a pair 
of values. The first represents 
the horizontal position and the 
second represents the vertical.

![](https://i.stack.imgur.com/0yf9z.png)
![](https://academy.hsoub.com/uploads/monthly_2015_05/percentage-values-illustration.png.0dd5ea52994d5eba1ad2f29f1f545f3c.png)



## Summary

+ You can specify the dimensions of images using CSS. 
This is very helpful when you use the same sized 
images on several pages of your site.
+ Images can be aligned both horizontally and vertically 
using CSS.
+ You can use a background image behind the box 
created by any element on a page. 
+ Background images can appear just once or be 
repeated across the background of the box.
+ You can create image rollover effects by moving the 
background position of an image.
+ To reduce the number of images your browser has to 
load, you can create image sprites

***

## Practical Information

There are entire books written about each of the topics 
covered in this chapter but I will introduce you to the key 
themes that each subject deals with and give you pointers for 
what you need to be considering. You will see:
+ The basics of search engine optimization
+ Using analytics to understand how people are using your 
site after it has launched
+ Putting your site on the web

## Search Engine Optimization (SEO)

> SEO is a huge topic and several books have been written on the subject. 
The following pages will help you understand the key concepts so you can 
improve your website's visibility on search engines.

***

+ Search engine optimization helps visitors find your 
sites when using search engines.
+ Analytics tools such as Google Analytics allow you to 
see how many people visit your site, how they find it, 
and what they do when they get there.
+ To put your site on the web, you will need to obtain a 
domain name and web hosting.
+ FTP programs allow you to transfer files from your 
local computer to your web server.
+ Many companies provide platforms for blogging, email 
newsletters, e-commerce and other popular website 
tools (to save you writing them from scratch).

***

## Flash, Video & Audio

> Flash is a very popular technology used 
to add animations, video, and audio to 
websites. This chapter begins by looking 
at how to use it in your web pages

### How Flash Works

> Since the late 1990s, Flash has been a very 
popular tool for creating animations, and later 
for playing audio and video in websites

+ Whether you are creating an 
animation or a media player in 
Flash, the files you put on your 
website are referred to as Flash 
movies. 
+ If you want to create your 
own Flash movie, you need to 
purchase the Flash authoring 
environment from Adobe.
+ There are, however, several 
companies that offer Flash 
animations and slideshows, 
as well as video and audio 
players that you can use without 
purchasing this tool.
+ When you create a Flash file in 
the Flash authoring environment, 
it is saved with the .fla file 
extension. In order to use this file 
on a web page it has to be saved 
in a different format known 
as SWF. (It has the .swf file 
extension.)
+ When you export the movie 
into SWF format, Flash creates 
code that you can use to embed 
the Flash movie in your page. 
Traditionally, this code used the 
HTML 
tags. However, now it is more 
common to use JavaScript.
+ To view Flash, browsers need 
to use a plugin (an extra piece 
of software that runs in the 
browser) called the Flash Player. 
Statistics commonly indicate 
that 98% of browsers on 
desktop computers have the 
Flash plugin installed. (The 
percentage of mobiles and 
tablets with it is much less.) 
+ There is not space in this book 
to teach you how to create Flash 
movies (there are many books 
devoted to that one topic), but 
this chapter will show you how 
to add Flash movies to your site.

## Use of Flash

> Since 2005, a number of factors have meant 
that fewer websites are written in Flash or even 
use elements of Flash in their pages

![](https://aleen42.gitbooks.io/wiki/content/Programming/HTML/flash_video_audio/timeline.png)