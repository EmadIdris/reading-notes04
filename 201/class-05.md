# Readings : Images, Color, Text
## Images

> A picture can say a thousand words, and great 
images help make the difference between an 
average-looking site and a really engaging one

![Images](https://data-flair.training/blogs/wp-content/uploads/sites/2/2020/07/html-images-df.jpg)
![Images](https://www.wikihow.com/images_en/thumb/b/be/Set-Image-Width-and-Height-Using-HTML-Step-3-Version-3.jpg/v4-460px-Set-Image-Width-and-Height-Using-HTML-Step-3-Version-3.jpg.webp)

## Transparency
Creating an image that is partially transparent 
(or "see-through") for the web involves 
selecting one of two formats
> If the transparent part of the 
image has straight edges and 
it is 100% transparent (that is, 
not semi-opaque), you can save 
the image as a GIF (with the 
transparency option selected)

## Examining Images on the Web
> Checking the Size of Images
If you are updating a website, you might need to check the size of an 
existing image before creating a new one to replace it. This can be 
achieved by right-clicking on the image and making a selection from 
the pop-up menu that appears. (Mac users will need to hold down the 
control key and click rather than right-click.

## Summary Images

+ The <img> element is used to add images to a 
web page.
+ You must always specify a src attribute to indicate the 
source of an image and an alt attribute to describe the 
content of an image.
+ You should save images at the size you will be using 
them on the web page and in the appropriate format.
+ Photographs are best saved as JPEGs; illustrations or 
logos that use flat colors are better saved as GIFs

## Color

![Color](https://i.pinimg.com/564x/85/42/11/85421136c73b09066f2b27010c061648.jpg)
![Color](https://cdn.hashnode.com/res/hashnode/image/upload/v1627409580379/19ZqK8fGv.png)

## Example Color

This example shows a pH scale to demonstrate 
the different ways that colors can be specified 
using CSS (using color names, hex codes, RGB, 
and HSL)

## Summary Color

+ Color not only brings your site to life, but also helps 
convey the mood and evokes reactions.
+ There are three ways to specify colors in CSS: 
RGB values, hex codes, and color names.
+ Color pickers can help you find the color you want.
+ It is important to ensure that there is enough contrast 
between any text and the background color (otherwise 
people will not be able to read your content).
+ CSS3 has introduced an extra value for RGB colors to 
indicate opacity. It is known as RGBA.
+ CSS3 also allows you to specify colors as HSL values, 
with an optional opacity value. It is known as HSLA.

## Summary TEXT
+ There are properties to control the choice of font, size, 
weight, style, and spacing.
+ There is a limited choice of fonts that you can assume 
most people will have installed.
+ If you want to use a wider range of typefaces there are 
several options, but you need to have the right license 
to use them.
+ You can control the space between lines of text, 
individual letters, and words. Text can also be aligned 
to the left, right, center, or justified. It can also be 
indented.
+ You can use pseudo-classes to change the style of an 
element when a user hovers over or clicks on text, or 
when they have visited a link

![](https://startingelectronics.org/tutorials/arduino/ethernet-shield-web-server-tutorial/CSS-introduction/CSS-HTML-markup-ex1.png)

****
# **JPEG vs PNG vs GIF**

There are hundreds of image formats available each with a specific use case. I bet most of us wouldn’t have come across 90% of the image formats listed on Wikipedia.
In this post, we would only be looking at the three most commonly used image formats in websites and mobile applications — JPEG, PNG and GIF. Several statistics reports, including the one from HTTP Archive, indicate that these 3 formats together comprise of more than 95% of all images loaded on websites. However, these 3 image formats have significant differences amongst themselves thus making each of them suitable for specific use cases. Understanding these major differences would help us deliver the best possible images to our website and mobile app users.
****
**JPEG** is a lossy compression specification that takes advantage of human perception. It can achieve compression ratios of 1:10 without any perceivable difference in quality. Beyond this, the compression artefacts become more prominent. Because JPEG compression works by averaging out colours of nearby pixels (read Discrete Cosine Transform), JPEG images are best suited for photographs and paintings of natural scenes where the variations in colour and intensity are smooth. However, if an image contains text or lines, where a sharp contrast between adjacent pixels is desired to highlight the proper shape, this lossy compression technique does not yield good results.
****
**GIF** is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing. Given that PNG is now supported across all major devices and that PNG compression is about 5–25% better than GIF compression, GIF images are now mainly used only if the image contains animations.
****
**PNG** is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are introduced in the image. For this reason, a PNG image would retain higher quality than an image than JPEG and would look a lot sharper, it would also occupy more space on the disk. This makes it unsuitable for storing or transferring high-resolution digital photographs but a great choice for images with text, logos and shapes with sharp edges.
****
