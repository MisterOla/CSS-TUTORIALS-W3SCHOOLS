# CSS-TUTORIALS-W3SCHOOLS
This repository contains the most important take-aways from w3schools' CSS tutorial. 
## The notes are currently being updated and edited. 
> Source: https://www.w3schools.com/css/default.asp

Table of contents<a name="#homepage">

[CSS Tutorial](#css-tutorial)
[CSS HOME](#css-tutorial)
[CSS Introduction](#css-introduction)
[CSS Syntax](#css-syntax)
[CSS Selectors](#css-selectors)
[CSS How To](#css-how-to)
[CSS Comments](#css-comments)
[CSS Colors](#css-colors)
[CSS Backgrounds](#css-backgrounds)
[CSS Borders](#css-borders)
[CSS Margins](#css-margins)
[CSS Padding](#css-padding)
[CSS Height or Width](#css-height-or-width)
[CSS Box Model](#css-box-model)
[CSS Outline](#css-outline)
[CSS Text](#css-text)
[CSS Fonts](#css-fonts)
[CSS Icons](#css-icons)
[CSS Links](#css-links)
[CSS Lists](#css-lists)
[CSS Tables](#css-tables)
[CSS Display](#css-display)
[CSS Max width](#css-max-width)
[CSS Position](#css-position)
[CSS Overflow](#css-overflow)
[CSS Float](#css-float)
[CSS Inline block](#css-inline-block)
[CSS Align](#css-align)
[CSS Combinators](#css-combinators)
[CSS Pseudo class](#css-pseudo-class)
[CSS Pseudo element](#css-pseudo-element)
[CSS Opacity](#css-opacity)
[CSS Navigation Bar](#css-navigation-bar)
[CSS Dropdowns](#css-dropdowns)
[CSS Image Gallery](#css-image-gallery)
[CSS Image Sprites](#css-image-sprites)
[CSS Attr Selectors](#css-attr-selectors)
[CSS Forms](#css-forms)
[CSS Counters](#css-counters)
[CSS Website Layout](#css-website-layout)
[CSS Units](#css-units)
[CSS Specificity](#css-specificity)
[CSS important](#css-important)


[CSS Advanced](#css-advanced)
[CSS Rounded Corners](#css-rounded-corners)
[CSS Border Images](#css-border-images)
[CSS Backgrounds](#css-backgrounds)
[CSS Colors](#css-colors)
[CSS Color Keywords](#css-color-keywords)
[CSS Gradients](#css-gradients)
[CSS Shadows](#css-shadows)
[CSS Text Effects](#css-text-effects)
[CSS Web Fonts](#css-web-fonts)
[CSS 2D Transforms](#css-2d-transforms)
[CSS 3D Transforms](#css-3d-transforms)
[CSS Transitions](#css-transitions)
[CSS Animations](#css-animations)
[CSS Tooltips](#css-tooltips)
[CSS Style Images](#css-style-images)
[CSS Image Reflection](#css-image-reflection)
[CSS object fit](#css-object-fit)
[CSS object position](#css-object-position)
[CSS Buttons](#css-buttons)
[CSS Pagination](#css-pagination)
[CSS Multiple Columns](#css-multiple-columns)
[CSS User Interface](#css-user-interface)
[CSS Variables](#css-variables)
[CSS Box Sizing](#css-box-sizing)
[CSS Media Queries](#css-media-queries)
[CSS MQ Examples](#css-mq-examples)
[CSS Flexbox](#css-flexbox)

[CSS Responsive](#css-responsive)
[RWD Intro](#rwd-intro)
[RWD Viewport](#rwd-viewport)
[RWD Grid View](#rwd-grid-view)
[RWD Media Queries](#rwd-media-queries)
[RWD Images](#rwd-images)
[RWD Videos](#rwd-videos)
[RWD Frameworks](#rwd-frameworks)
[RWD Templates](#rwd-templates)

[CSS Grid](#css-grid)
[Grid Intro](#grid-intro)
[Grid Container](#grid-container)
[Grid Item](#grid-item)

[CSS References](#css-references)

- - - - - - - - - - - - - - - - - -  - - - - - - - - - - - - - - - - - - --  - - -- - - - - - -- - - - - - - - - - - -- - - - - - -- -- - --  -- - - -- - - - - -- - - 

css Tutorial

CSS HOME:::


CSS dictates how HTML Should be displayed

CSS( Cascading Style Sheets) describe how HTML elements are to be displayed on screen, paper, or in other 

media. It saves a lot of work and can control layout of multiple pages at once. It also stores external 

stylesheets in css files.

CSS is used to define styles for your web pages, including the design, layout and variations in display for 

different devices and screen sizes.

An example of a simple CSS is shown below

body {
  background-color: lightblue;
}

h1 {
  color: white;
  text-align: center;
}

p {
  font-family: verdana;
  font-size: 20px;
}


CSS INTRODUCTION:::


CSS Solved a Big problem:
HTML was NEVER intended to contain tags for formatting a web page!

HTML was created to describe the content of a web page, like:

<h1>This is a heading</h1>

<p>This is a paragraph.</p>

Adding fonts color to HTML elements which was introduced in html 3 was a deviation from what HTML was meant 

to do in the first place.

CSS Saves a Lot of Work!

The style definitions are normally saved in external .css files.

With an external stylesheet file, you can change the look of an entire website by changing just one file!


CSS SYNTAX:::

h1 {color:blue;font-size:12px;}

selector {property:value;property:value;} 

property+value=declaration block.

```
p {
  color: red;
  text-align: center;
} 

```

the p is set to red and centered automatically.




CSS Selectors:::

They help in dictating the styles of specific html elements

Categories of css selectors::

Simple selectors: use name, id, and class to select elements
Combinator selectors: use relationship between elements to select them
Pseudo-class selectors: To select elements based on a certain state
Pseudo-elements selectors:select and style part of an element
Attribute selectors: Use an attribute or attribute value to select an element

Explaining the most basic css selectors

1. CSS element Selector: Uses element name to select html elements

```
p {
  text-align: center;
  color: red;
}

```


2. CSS id Selector: Uses the id attribute of an element to select it. Element id is unique within a webpage 

and it can select one unique element. 
To use id to select element, use hash(#) followed by the id of the element.The name of an id cannot start 

with a number.

```
<!DOCTYPE html>
<html>
<head>
<style>
#para1 {
  text-align: center;
  color: red;
}
</style>
</head>
<body>

<p id="para1">Hello World!</p>
<p>This paragraph is not affected by the style.</p>

</body>
</html>

```



The CSS class Selector: Selects html elements with specific class attribute. Use (.) character followed by 

class name. The code below makes class="center" red and center-aligned

```

<!DOCTYPE html>
<html>
<head>
<style>
.center {
  text-align: center;
  color: red;
}
</style>
</head>
<body>

<h1 class="center">Red and center-aligned heading</h1>
<p class="center">Red and center-aligned paragraph.</p> 

</body>
</html>

```


You can also specify only html elements that should be affected by a class styling. In the code below, only 

```p``` elements with ```class="center"``` will be red and center aligned.

```

<!DOCTYPE html>
<html>
<head>
<style>
p.center {
  text-align: center;
  color: red;
}
</style>
</head>
<body>

<h1 class="center">This heading will not be affected</h1>
<p class="center">This paragraph will be red and center-aligned.</p> 

</body>
</html>

```

HTMl elements can refer to more than one class. In that case, p elemen is styled according to all the 

classes


```
<!DOCTYPE html>
<html>
<head>
<style>
p.center {
  text-align: center;
  color: red;
}

p.large {
  font-size: 300%;
}
</style>
</head>
<body>

<h1 class="center">This heading will not be affected</h1>
<p class="center">This paragraph will be red and center-aligned.</p>
<p class="center large">This paragraph will be red, center-aligned, and in a large font-size.</p> 

</body>
</html>
```


The CSS Universal Selector::

The * selects all the HTML elements on a page

```
<!DOCTYPE html>
<html>
<head>
<style>
* {
  text-align: center;
  color: blue;
}
</style>
</head>
<body>

<h1>Hello world!</h1>

<p>Every element on the page will be affected by the style.</p>
<p id="para1">Me too!</p>
<p>And me!</p>

</body>
</html>

```


The CSS Grouping Selector::

Selects all the html elements with same sty le definitions. 


rather than having the code below:

```
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```

we can simply have:
```

h1, h2, p {
  text-align: center;
  color: red;
}

```
and still get the same result


Summary of all CSS selectors:

All CSS Simple Selectors
Selector 	Example 	Example description

#id 	#firstname 	Selects the element with id="firstname"
.class 	.intro 	Selects all elements with class="intro"
element.class 	p.intro 	Selects only <p> elements with class="intro"
* 	* 	Selects all elements
element 	p 	Selects all <p> elements
element,element,.. 	div, p 	Selects all <div> elements and all <p> elements




HOW TO ADD CSS

Browser formats html using the information in the style sheet or <style>


External CSS::

It is a file that you can use to change the style of an entire website. Each page of the website then 

include <link> , in the <head> section, which contains a link to the external styling sheet that controls 

the style of the whole document. You can create the external file with any text editor. This file should be 

saved with a .css extension and the file must not contain any HTML tags. 


when "mystyle.css" contains the code:

body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}



The mystyle can be inherited below:

<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>


NB: No space between property value and it's unit. I.e use: 20px not 20 px




Internal CSS::

Can be used if one single HTML page has a unique style. You should define inside the <style> element, inside 

the <head> section. Example of internal CSS is shown below:

!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
} 
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>



Inline CSS::

You can use an inline style to apply unique style to just a single element. To use inline styles, add the 

style attribute to the appropriate element. Style attribute can contain any of the CSS properties.


<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>


NB: And inline style denies you the benefits of a style sheet since you now have to edit the styling of 

elements individually. Only use CSS inline when necessary



Multiple Style Sheets::

If you have styles for same element in different style sheet, the last read style of sheet for the elements 

is applied to the element.


if mystyle.css contains:

h1 {
  color: navy;
}

and internal style sheet contains the following:


h1 {
  color: orange;   
}


Case A: Internal style defined after the link to external style sheet, <h1> elements will take an orange 

color since the internal style comes last


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
<style>
h1 {
  color: orange;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>The style of this document is a combination of an external stylesheet, and internal style</p>

</body>
</html>


Case B: If the internal style is defined before the link the external style sheet, then the <h1> elements 

will take the navy color defined in the style sheet. 

<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  color: orange;
}
</style>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>The style of this document is a combination of an external stylesheet, and internal style</p>

</body>
</html>



Cascading Order::

When an HTML element has more than one style specified for it, all styles will 'cascade' into a new virtual 

style sheet according to the rules below 1. has highest priority and 3. has the least.


1. Inline style (inside an HTML element)
2. External and internal style sheets (in the head section)
3. Browser default


Inline style is highest priority and can override external styles and browser defaults.






CSS COMMENTS


They do not show in the browser but improve code readability:


They may help you edit the source code later on. The comment is placed inside <style> element, starts with 

/* and ends with */   and you can have the comment anywhere in the code you like.


 /* This is a single-line comment */
p {
  color: red;
} 


/* This is
a multi-line
comment */


p {
  color: red;
} 



HTML and CSS Comments

The HTML comment is: <!--this is a comment--!>. You can combine HTML style with a CSS for an element:


<!DOCTYPE html>
<html>
<head>
<style>
p {
  color: red; /* Set text color to red */
}
</style>
</head>
<body>

<h2>My Heading</h2>

<!-- These paragraphs will be red -->
<p>Hello World!</p>
<p>This paragraph is styled with CSS.</p>
<p>HTML and CSS comments are not shown in the output.</p>

</body>
</html>





CSS COLORS


Colors:: 

You can specify color with predefined color names: RGB, HEX, HSL, RGBA, HSLA.


CSS Color names: There are 140 supported standard color names. See the link below for the full list.



CSS Background Color: Set the background color as shown below

<h1 style="background-color:DodgerBlue;">Hello World</h1>

<p style="background-color:Tomato;">


CSS Text Color: You can also set the color of the text as shown below:


<h1 style="color:Tomato;">Hello World</h1>
<p style="color:DodgerBlue;">Lorem ipsum...</p>
<p style="color:MediumSeaGreen;">Ut wisi enim...</p> 


CSS Border Color: Use can use this to change the color of the border (the box around a text). The


<body>

<h1 style="border: 2px solid Tomato;">Hello World</h1>

<h1 style="border: 2px solid DodgerBlue;">Hello World</h1>

<h1 style="border: 2px solid Violet;">Hello World</h1>

</body>


CSS Color values

You can specify color using RGB values, HEX values, HSL values, and RGBA values, and HSLA values.



The three below are still tomato colors


rgb(255, 99, 71)
#ff6347
hsl(9, 100%, 64%)




The below are tomato with 50% transparency:


rgba(255, 99, 71, 0.5)
hsla(9, 100%, 64%, 0.5)


See the application below:

<!DOCTYPE html>
<html>
<body>

<p>Same as color name "Tomato":</p>

<h1 style="background-color:rgb(255, 99, 71);">rgb(255, 99, 71)</h1>
<h1 style="background-color:#ff6347;">#ff6347</h1>
<h1 style="background-color:hsl(9, 100%, 64%);">hsl(9, 100%, 64%)</h1>

<p>Same as color name "Tomato", but 50% transparent:</p>
<h1 style="background-color:rgba(255, 99, 71, 0.5);">rgba(255, 99, 71, 0.5)</h1>
<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">hsla(9, 100%, 64%, 0.5)</h1>

<p>In addition to the predefined color names, colors can be specified using RGB, HEX, HSL, or even 

transparent colors using RGBA or HSLA color values.</p>

</body>
</html>




CSS RGB::

RGB Value: RGB rep red, green, and blue light sources


format: rgb(red_value,green_value,blue_value)


Each of the color values range from 0 to 255


red= rgb(255,0,0); since red color is max while blue and green are absent.


black=rgb(0,0,0); since there is absence of light

white=rgb(255,255,255); since there is an excess of all the lights...no color shows

grey=rgb(x,x,x); equal color values produce grey. So, you have black at rgb(0,0,0), and white at rgb

(255,255,255).Every other equal mix between 0 and 255 is grey but to different extent. The closer the equal 

values are to zero the darker the grey color is. 



RGBA Value: It includes alpha channel ( a measure of opacity) for each of the colors. 

format: rgba(red_value,green_value,blue_value,alpha)

Fully transparent: alpha=0.0
Not transparent at all: alpha=1.0



CSS HEX COLORS::

hexadecimal color format: #RRGGBB   (RR=RED, GG=GREEN, BB=BLUE)

The hexadecimal integers specify the component of the color. 


HEX Value ranges from  00 to ff, just like decimal ranges from 0 to 255


#ff0000=red because red is set to max while green and blue are set to zero. 

#000000: black because no color light present

#ffffff: white because max color light present in all the cases.

Any equal values between 000000 and ffffff gives grey

#787878=grey


3 Digit HEX Value: It is a short form ofsome 6 digit hex codes 
The format of the 3 digit hex code is: #rgb

You can only use the 3digit hex code when both red, green, and blue component values are the same for 

example:

body {
  background-color: #fc9; /* same as #ffcc99 */
}

h1 {
  color: #f0f; /* same as #ff00ff */
}

p {
  color: #b58; /* same as #bb5588 */
}




CSS HSL Colors::

HSL = Hue, Saturation, Lightness


format: hsl(hue, saturation, lightness)


Hue=Degree on color wheel from  0 to 360 ( Hue=0 (Red), Hue=120(Green), Hue=240(Blue))

Saturation: Percentage value from shade of gray (0%) to full color(100%)

LIghtness: Percentage value from Black(0%) to white(100%), to neither white or black (50%)



Saturation::: Intensity of a color. Pure color+no shades of gray=100%, Gray+invisible color=50%, Completely 

gray=0% and you can no longer see the color


Lightness: CAn be described by how much light you want give the color. No light( black)=0%, Neither light 

nor dark=50%, full lightness (white) = 100%


Shades of gray involves setting hue and saturation to zero and then adjusting lightness from 0% to 100% to 

get darker/lighter shades. 

hsl(0%,0%,0%)=black

hsl(0%,0%,100%)=white
hsl(0%,0%,47%)=grey


HsLA Value::: They are an extension of the HSL color values by including an alpha channel

hsla(hue, saturation, lightness, alpha)





CSS BACKGROUNDS

They are used to add background effects for elements


CSS Background Color:: 

specification: "background-color"

Specifies the background color of an element. You can specify color by name, hex value or rgb 

value...typically.

To give the whole page a blue background:

<style>
body {
  background-color: lightblue;
}
</style>


You can also add background color for each element including the div element as shown below.

!DOCTYPE html>
<html>
<head>
<style>
h1 {
  background-color: green;
}

div {
  background-color: lightblue;
}

p {
  background-color: yellow;
}
</style>
</head>
<body>

<h1>CSS background-color example!</h1>
<div>
This is a text inside a div element.
<p>This paragraph has its own background color.</p>
We are still in the div element.
</div>

</body>
</html>



Opacity/ Transparency::: Specifies how transparent an element is. Ranges from (0) for fully transparent to 

(1) to non transparent/ opaque

Below is how to use the opacity element. Note that "div.first" means that the style is only applied to div 

elements with "first" class


<style>
div {
  background-color: green;
}

div.first {
  opacity: 0.1;
}

div.second {
  opacity: 0.3;
}

div.third {
  opacity: 0.6;
}
</style>
</head>
<body>

<h1>Transparent Box</h1>
<p>When using the opacity property to add transparency to the background of an element, all of its child 

elements become transparent as well. This can make the text inside a fully transparent element hard to 

read:</p>

<div class="first">
  <h1>opacity 0.1</h1>
</div>

<div class="second">
  <h1>opacity 0.3</h1>
</div>

<div class="third">
  <h1>opacity 0.6</h1>
</div>

<div>
  <h1>opacity 1 (default)</h1>
</div>

</body>
</html>


Transparency using RGBA::: You can also use the RGBA if you did not use the opacity to specify the 

transparency of the elements. The alpha value has the same function as the opacity. 0.0(fully transparent) 

and 1.0 (opaque)

The code below confirms that fact that rgba and the use of opacity and rgb gives the same result. 
<!DOCTYPE html>
<html>
<head>
<style>
div {
  background: rgb(0, 128, 0);
}

div.first {
  background: rgba(0, 128, 0, 0.1);
}

div.second {
  background: rgba(0, 128, 0, 0.3);
}

div.third {
  background: rgba(0, 128, 0, 0.6);
}
</style>
</head>
<body>

<h1>Transparent Box</h1>
<p>With opacity:</p>

<div style="opacity:0.1;">
  <h1>10% opacity</h1>
</div>

<div style="opacity:0.3;">
  <h1>30% opacity</h1>
</div>

<div style="opacity:0.6;">
  <h1>60% opacity</h1>
</div>

<div>
  <h1>opacity 1</h1>
</div>

<p>With RGBA color values:</p>
<div class="first">
  <h1>10% opacity</h1>
</div>

<div class="second">
  <h1>30% opacity</h1>
</div>

<div class="third">
  <h1>60% opacity</h1>
</div>

<div>
  <h1>default</h1>
</div>

<p>Notice how the text gets transparent as well as the background color when using the opacity property.</p>

</body>
</html>



CSS Background Image::

Specification: background-image


The css background-image property defines what image to be used as a background. Image is usually repeated 

by default to cover an entire element.

Below is an example of how to insert an image in the background. Always use an image that will not disturb 

the text or make it impossible for the text to be easily read.

<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-image: url("paper.gif");
}
</style>
</head>
<body>

<h1>Hello World!</h1>

<p>This page has an image as the background!</p>

</body>
</html>


You can also give a specific element a background image as shown below (giving a paragraph a background 

image):

<!DOCTYPE html>
<html>
<head>
<style>
p {
  background-image: url("paper.gif");
}
</style>
</head>
<body>

<h1>Hello World!</h1>

<p>This paragraph has an image as the background!</p>

</body>
</html>



CSS Background Repeat::

Specification: background-repeat


Since the background-image property repeats image both horizontally and vertically, you do not have to 

control over whether horizontal or vertical repeat is the best for each image. 

The background-repeat enables you to repeat only horizontally or only vertically, and this allows you to 

avoid wierdly looking images.


To repeat an image horizontally, set background-repeat: repeat-x
To repeat an image vertically, set background-repeat: repeat-y


<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-image: url("gradient_bg.png");
  background-repeat: repeat-x;
}
</style>
</head>
<body>

<h1>Hello World!</h1>
<p>Here, a background image is repeated only horizontally!</p>

</body>
</html>

To repeat an image only once, set background-repeat:no-repeat

See example below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
}
</style>
</head>
<body>

<h1>Hello World!</h1>
<p>W3Schools background image example.</p>
<p>The background image is only showing once, but it is disturbing the reader!</p>

</body>
</html>


To position the background image such that it does not disturb the text much, set
 background-position: right top; (You can also set it to "left bottom"

Below is an example of how to set the background image:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  margin-right: 200px;
}
</style>
</head>
<body>

<h1>Hello World!</h1>
<p>W3Schools background no-repeat, set position example.</p>
<p>Now the background image is only shown once, and positioned away from the text.</p>
<p>In this example we have also added a margin on the right side, so the background image will never disturb 

the text.</p>

</body>
</html>



CSS Background Attachment::

Specification: background-attachment


The background attachment property lets you set your preferences regarding whether you want the background 

image should scroll or be fixed ( should not scroll with the rest of the page)

To get a fixed background image:
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  margin-right: 200px;
  background-attachment: fixed;
}
</style>
</head>
<body>

<h1>The background-attachment Property</h1>

<p>The background-attachment property specifies whether the background image should scroll or be fixed (will 

not scroll with the rest of the page).</p>

<p><strong>Tip:</strong> If you do not see any scrollbars, try to resize the browser window.</p>

<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>
<p>The background-image is fixed. Try to scroll down the page.</p>

</body>
</html>



To set background image to scroll with the rest of the page:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  margin-right: 200px;
  background-attachment: scroll;
}
</style>
</head>
<body>

<h1>The background-attachment Property</h1>

<p>The background-attachment property specifies whether the background image should scroll or be fixed (will 

not scroll with the rest of the page).</p>

<p><strong>Tip:</strong> If you do not see any scrollbars, try to resize the browser window.</p>

<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>
<p>The background-image scrolls. Try to scroll down the page.</p>

</body>
</html>




CSS Background Shorthand property::

You can shorten your css style code by specifying al the background properties in one property. This is 

known as the shorthand property. Cases A and B below are the same. Case B uses the shorthand property.

CASE A: Full format

body {
  background-color: #ffffff;
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}


CASE B: Shorthand format 
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background: #ffffff url("img_tree.png") no-repeat right top;
  margin-right: 200px;
}
</style>
</head>
<body>

<h1>The background Property</h1>

<p>The background property is a shorthand property for specifying all the background properties in one 

declaration.</p>

<p>Here, the background image is only shown once, and it is also positioned in the top-right corner.</p>

<p>We have also added a right margin, so that the text will not write over the background image.</p>

</body>
</html>


The sequence of the property values when you are using the shorthand property for background is:


background-color
background-image
background-repeat
background-attachment
background-position



All CSS background properties:::

All CSS Background Properties
Property 	Description
background 	Sets all the background properties in one declaration
background-attachment 	Sets whether a background image is fixed or scrolls with the rest of the page
background-clip 	Specifies the painting area of the background
background-color 	Sets the background color of an element
background-image 	Sets the background image for an element
background-origin 	Specifies where the background image(s) is/are positioned
background-position 	Sets the starting position of a background image
background-repeat 	Sets how a background image will be repeated
background-size 	Specifies the size of the background image(s)



CSS Borders

CSS Border Style

The border-style property specifies what kind of border to display.

The following values are allowed:

dotted - Defines a dotted border
dashed - Defines a dashed border
solid - Defines a solid border
double - Defines a double border
groove - Defines a 3D grooved border. The effect depends on the border-color value
ridge - Defines a 3D ridged border. The effect depends on the border-color value
inset - Defines a 3D inset border. The effect depends on the border-color value
outset - Defines a 3D outset border. The effect depends on the border-color value
none - Defines no border
hidden - Defines a hidden border

The border-style property can have from one to four values (for the top border, right border, bottom border, 

and the left border).


<!DOCTYPE html>
<html>
<head>
<style>
p.dotted {border-style: dotted;}
p.dashed {border-style: dashed;}
p.solid {border-style: solid;}
p.double {border-style: double;}
p.groove {border-style: groove;}
p.ridge {border-style: ridge;}
p.inset {border-style: inset;}
p.outset {border-style: outset;}
p.none {border-style: none;}
p.hidden {border-style: hidden;}
p.mix {border-style: dotted dashed solid double;}
</style>
</head>
<body>

<h2>The border-style Property</h2>
<p>This property specifies what kind of border to display:</p>

<p class="dotted">A dotted border.</p>
<p class="dashed">A dashed border.</p>
<p class="solid">A solid border.</p>
<p class="double">A double border.</p>
<p class="groove">A groove border.</p>
<p class="ridge">A ridge border.</p>
<p class="inset">An inset border.</p>
<p class="outset">An outset border.</p>
<p class="none">No border.</p>
<p class="hidden">A hidden border.</p>
<p class="mix">A mixed border.</p>

</body>
</html>



Note: None of the OTHER CSS border properties (such as borders width, border colors, border sides, border 

shorthand, rounded borders) will have ANY effect unless the border-style property is set!


Border Width::

<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-width: 5px;
}

p.two {
  border-style: solid;
  border-width: medium;
}

p.three {
  border-style: dotted;
  border-width: 2px;
}

p.four {
  border-style: dotted;
  border-width: thick;
}

p.five {
  border-style: double;
  border-width: 15px;
}

p.six {
  border-style: double;
  border-width: thick;
}
</style>
</head>
<body>

<h2>The border-width Property</h2>
<p>This property specifies the width of the four borders:</p>

<p class="one">Some text.</p>
<p class="two">Some text.</p>
<p class="three">Some text.</p>
<p class="four">Some text.</p>
<p class="five">Some text.</p>
<p class="six">Some text.</p>

<p><b>Note:</b> The "border-width" property does not work if it is used alone. 
Always specify the "border-style" property to set the borders first.</p>

</body>
</html>






CSS Border Width

The border-width property specifies the width of the four borders (top border, right border, bottom border, 

and left border) using px, pt, cm, em, etc. or using thin,medium, or thick. For specific side widths, two 

borders are specified. The first represents top and bottom border with, while the second represents the 

width for the sides borders. 



<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-width: 5px 20px; /* 5px top and bottom, 20px on the sides */
}

p.two {
  border-style: solid;
  border-width: 20px 5px; /* 20px top and bottom, 5px on the sides */
}

p.three {
  border-style: solid;
  border-width: 25px 10px 4px 35px; /* 25px top, 10px right, 4px bottom and 35px left */
}
</style>
</head>
<body>

<h2>The border-width Property</h2>
<p>The border-width property can have from one to four values (for the top border, right border, bottom 

border, and the left border):</p>

<p class="one">Some text.</p>
<p class="two">Some text.</p>
<p class="three">Some text.</p>

</body>
</html>

CSS Border Color::

The border-color property is used to set the color of the four borders using name ( e.g. red), HEX value 

(e.g. #ff0000), RGB value (e.g. rgb(255,0,0), and HSL value (e.g. hsl (0, 100%, 50%), and transparency

(specified using alpha value). 


Note: The elements's color is the default border-color whenever you did not set the border color.

<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-color: red;
}

p.two {
  border-style: solid;
  border-color: green;
} 

p.three {
  border-style: dotted;
  border-color: blue;
} 
</style>
</head>
<body>

<h2>The border-color Property</h2>
<p>This property specifies the color of the four borders:</p>

<p class="one">A solid red border</p>
<p class="two">A solid green border</p>
<p class="three">A dotted blue border</p>

<p><b>Note:</b> The "border-color" property does not work if it is used alone. Use the "border-style" 

property to set the borders first.</p>

</body>
</html>



Specific Side Colors


The border-color property can have from one to four values (for the top border, right border, bottom border, 

and the left border). 


<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-color: red green blue yellow; /* red top, green right, blue bottom and yellow left */
}
</style>
</head>
<body>

<h2>The border-color Property</h2>
<p>The border-color property can have from one to four values (for the top border, right border, bottom 

border, and the left border):</p>

<p class="one">A solid multicolor border</p>

</body>
</html>


Hexadecimal (HEX) Values

The color of the border can also be specified using HEX values. 


<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-color: #ff0000; /* red */
}

p.two {
  border-style: solid;
  border-color: #0000ff; /* blue */
}

p.three {
  border-style: solid;
  border-color: #bbbbbb; /* grey */
}
</style>
</head>
<body>

<h2>The border-color Property</h2>
<p>The color of the border can also be specified using a hexadecimal value (HEX):</p>

<p class="one">A solid red border</p>
<p class="two">A solid blue border</p>
<p class="three">A solid grey border</p>

</body>
</html>



RGB Values

RGB values can also be used to specify color. 

<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-color: rgb(255, 0, 0); /* red */
}

p.two {
  border-style: solid;
  border-color: rgb(0, 0, 255); /* blue */
}

p.three {
  border-style: solid;
  border-color: rgb(187, 187, 187); /* grey */
}
</style>
</head>
<body>

<h2>The border-color Property</h2>
<p>The color of the border can also be specified using RGB values:</p>

<p class="one">A solid red border</p>
<p class="two">A solid blue border</p>
<p class="three">A solid grey border</p>

</body>
</html>


HSL Values

HSL values can be used to specify.

<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  border-color: hsl(0, 100%, 50%); /* red */
}

p.two {
  border-style: solid;
  border-color: hsl(240, 100%, 50%); /* blue */
}

p.three {
  border-style: solid;
  border-color: hsl(0, 0%, 73%); /* grey */
}
</style>
</head>
<body>

<h2>The border-color Property</h2>
<p>The color of the border can also be specified using HSL values:</p>

<p class="one">A solid red border</p>
<p class="two">A solid blue border</p>
<p class="three">A solid grey border</p>

</body>
</html>



CSS Border Sides::

CSS Border - Individual Sides

You can use some CSS properties to specify the type of border each side (top, right, bottom, and left) has


<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-top-style: dotted;
  border-right-style: solid;
  border-bottom-style: dotted;
  border-left-style: solid;
}
</style>
</head>
<body>

<h2>Individual Border Sides</h2>
<p>2 different border styles.</p>

</body>
</html>


The code above can also be written as (dotted and solid represent top+bottom, and left+right respectively: 

<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-style: dotted solid;
}
</style>
</head>
<body>

<h2>Individual Border Sides</h2>
<p>2 different border styles.</p>

</body>
</html>


Border style explanation : 
If the border-style property has four values:

    border-style: dotted solid double dashed;
        top border is dotted
        right border is solid
        bottom border is double
        left border is dashed

If the border-style property has three values:

    border-style: dotted solid double;
        top border is dotted
        right and left borders are solid
        bottom border is double

If the border-style property has two values:

    border-style: dotted solid;
        top and bottom borders are dotted
        right and left borders are solid

If the border-style property has one value:

    border-style: dotted;
        all four borders are dotted


The above also works with border-width and border-color

See code below for example of practical use of the border styling parameters

<!DOCTYPE html>
<html>
<head>
<style>
body {
  text-align: center;
}
/* Four values */
p.four {
  border-style: dotted solid double dashed;
}

/* Three values */
p.three {
  border-style: dotted solid double;
}

/* Two values */
p.two {
  border-style: dotted solid;
}

/* One value */
p.one {
  border-style: dotted;
}
</style>
</head>
<body>

<h2>Individual Border Sides</h2>
<p class="four">4 different border styles.</p>
<p class="three">3 different border styles.</p>
<p class="two">2 different border styles.</p>
<p class="one">1 border style.</p>

</body>
</html>

CSS Border-Shorthand property::
Enable shortening of the border styling codes. The 'border' property is a shorthand for individual border 

properties, as shown below (for example)


    border-width
    border-style (required)
    border-color
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border: 5px solid red;
}
</style>
</head>
<body>

<h2>The border Property</h2>

<p>This property is a shorthand property for border-width, border-style, and border-color.</p>

</body>
</html>



Border properties can also be specified for each side:
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-left: 6px solid red;
  background-color: lightgrey;
}
</style>
</head>
<body>

<h2>The border-left Property</h2>
<p>This property is a shorthand property for border-left-width, border-left-style, and border-left-

color.</p>

</body>
</html>


To repeat the same for bottom border:

<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-bottom: 6px solid red;
  background-color: lightgrey;
}
</style>
</head>
<body>

<h2>The border-bottom Property</h2>
<p>This property is a shorthand property for border-bottom-width, border-bottom-style, and border-bottom-

color.</p>

</body>
</html>


CSS Rounded Borders::
Use border radius to add rounded borders to an element


<!DOCTYPE html>
<html>
<head>
<style>
p.normal {
  border: 2px solid red;
}

p.round1 {
  border: 2px solid red;
  border-radius: 5px;
}

p.round2 {
  border: 2px solid red;
  border-radius: 8px;
}

p.round3 {
  border: 2px solid red;
  border-radius: 12px;
}
</style>
</head>
<body>

<h2>The border-radius Property</h2>
<p>This property is used to add rounded borders to an element:</p>

<p class="normal">Normal border</p>
<p class="round1">Round border</p>
<p class="round2">Rounder border</p>
<p class="round3">Roundest border</p>

</body>
</html>


NB: Some shortcuts on border styling

To set all properties of top border in one go:
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-style: solid;
  border-top: thick double #ff0000;
}
</style>
</head>
<body>

<p>This is some text in a paragraph.</p>

</body>
</html>


To set the style of the bottom border

<!DOCTYPE html>
<html>
<head>
<style>
p {border-style: solid;}
p.none {border-bottom-style: none;}
p.dotted {border-bottom-style: dotted;}
p.dashed {border-bottom-style: dashed;}
p.solid {border-bottom-style: solid;}
p.double {border-bottom-style: double;}
p.groove {border-bottom-style: groove;}
p.ridge {border-bottom-style: ridge;}
p.inset {border-bottom-style: inset;}
p.outset {border-bottom-style: outset;}
</style>
</head>
<body>

<p class="none">No bottom border.</p>
<p class="dotted">A dotted bottom border.</p>
<p class="dashed">A dashed bottom border.</p>
<p class="solid">A solid bottom border.</p>
<p class="double">A double bottom border.</p>
<p class="groove">A groove bottom border.</p>
<p class="ridge">A ridge bottom border.</p>
<p class="inset">An inset bottom border.</p>
<p class="outset">An outset bottom border.</p>

</body>
</html>



To set the width of the left border

<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-style: solid;
  border-left-width: 15px;
}
</style>
</head>
<body>

<p><b>Note:</b> The "border-left-width" property does not work if it is used alone. Use the "border-style" 

property to set the borders first.</p>

</body>
</html>


To set the color of the four borders:

<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: solid;
  
  border-color: #0000ff;
}

p.two {
  border-style: solid;
  border-color: #ff0000 #0000ff;
}

p.three {
  border-style: solid;
  border-color: #ff0000 #00ff00 #0000ff;
}

p.four {
  border-style: solid;
  border-color: #ff0000 #00ff00 #0000ff rgb(250,0,255);
}
</style>
</head>
<body>

<p class="one">One-colored border!</p>
<p class="two">Two-colored border!</p>
<p class="three">Three-colored border!</p>
<p class="four">Four-colored border!</p>
<p><b>Note:</b> The "border-color" property does not work if it is used alone. Use the "border-style" 

property to set the borders first.</p>

</body>
</html>


To set the color of the right border:
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-style: solid;
  border-right-color: #ff0000;
}
</style>
</head>
<body>

<p>This is some text in a paragraph.</p>

</body>
</html>


All CSS Border Properties
Property 	Description
border 	Sets all the border properties in one declaration
border-bottom 	Sets all the bottom border properties in one declaration
border-bottom-color 	Sets the color of the bottom border
border-bottom-style 	Sets the style of the bottom border
border-bottom-width 	Sets the width of the bottom border
border-color 	Sets the color of the four borders
border-left 	Sets all the left border properties in one declaration
border-left-color 	Sets the color of the left border
border-left-style 	Sets the style of the left border
border-left-width 	Sets the width of the left border
border-radius 	Sets all the four border-*-radius properties for rounded corners
border-right 	Sets all the right border properties in one declaration
border-right-color 	Sets the color of the right border
border-right-style 	Sets the style of the right border
border-right-width 	Sets the width of the right border
border-style 	Sets the style of the four borders
border-top 	Sets all the top border properties in one declaration
border-top-color 	Sets the color of the top border
border-top-style 	Sets the style of the top border
border-top-width 	Sets the width of the top border
border-width 	Sets the width of the four borders




CSS Margins

To create space around an element outside of specified borders. the 'margin' gives control over the margin 

around an element. You can also set margin on the four sides. There are properties for setting the margin 

for each side of an element (top, right, bottom, and left).

The code below add a 70px margin space around <p> element. 

<!DOCTYPE html>
<html>
<head>
<style>
div {
  margin: 70px;
  border: 1px solid #4CAF50;
}
</style>
</head>
<body>

<h2>CSS Margins</h2>
<div>This element has a margin of 70px.</div>

</body>
</html>



Margin - Individual Sides::

CSS has properties for specifying the margin for each side of an element:

    margin-top
    margin-right
    margin-bottom
    margin-left

All the margin properties can have the following values:

    auto - the browser calculates the margin
    length - specifies a margin in px, pt, cm, etc.
    % - specifies a margin in % of the width of the containing element
    inherit - specifies that the margin should be inherited from the parent element

Tip: Negative values are allowed.

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>Using individual margin properties</h2>

<div>This div element has a top margin of 100px, a right margin of 150px, a bottom margin of 100px, and a 

left margin of 80px.</div>

</body>
</html>



Margin Shorthand Property

To shorten the code, it is possible to specify all the margin properties in one property.

The margin property is a shorthand property for the following individual margin properties:

    margin-top
    margin-right
    margin-bottom
    margin-left

So, here is how it works:

If the margin property has four values:

    margin: 25px 50px 75px 100px;
        top margin is 25px
        right margin is 50px
        bottom margin is 75px
        left margin is 100px


Example:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  margin: 25px 50px 75px 100px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The margin shorthand property - 4 values</h2>

<div>This div element has a top margin of 25px, a right margin of 50px, a bottom margin of 75px, and a left 

margin of 100px.</div>

<hr>

</body>
</html>


If the margin property has three values:

    margin: 25px 50px 75px;
        top margin is 25px
        right and left margins are 50px
        bottom margin is 75px

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  margin: 25px 50px 75px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The margin shorthand property - 3 values</h2>

<div>This div element has a top margin of 25px, a right and left margin of 50px, and a bottom margin of 

75px.</div>

<hr>

</body>
</html>


If the margin property has two values:

    margin: 25px 50px;
        top and bottom margins are 25px
        right and left margins are 50px


<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  margin: 25px 50px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The margin shorthand property - 2 values</h2>

<div>This div element has a top and bottom margin of 25px, and a right and left margin of 50px.</div>

<hr>

</body>
</html>



If the margin property has one value:

    margin: 25px;
        all four margins are 25px




<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  margin: 25px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The margin shorthand property - 1 value</h2>

<div>This div element has a top, bottom, left, and right margin of 25px.</div>

<hr>

</body>
</html>




The margin: auto,  Value

You can set the margin property to auto to horizontally center the element within its container.

The element will then take up the specified width, and the remaining space will be split equally between the 

left and right margins.


<!DOCTYPE html>
<html>
<head>
<style>
div {
  width:300px;
  margin: auto;
  border: 1px solid red;
}
</style>
</head>
<body>

<h2>Use of margin:auto</h2>
<p>You can set the margin property to auto to horizontally center the element within its container. The 

element will then take up the specified width, and the remaining space will be split equally between the 

left and right margins:</p>

<div>
This div will be horizontally centered because it has margin: auto;
</div>

</body>
</html>


The inherit Value for margin
To let the left margin of the <p class="ex1"> element be inherited from the parent element.


<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid red;
  margin-left: 100px;
}

p.ex1 {
  margin-left: inherit;
}
</style>
</head>
<body>

<h2>Use of the inherit value</h2>
<p>Let the left margin be inherited from the parent element:</p>

<div>
<p class="ex1">This paragraph has an inherited left margin (from the div element).</p>
</div>

</body>
</html>


CSS Margin Collapse::
Enables you to collapse 2 margins into one.

Margin Collapse

Top and bottom margins of elements are sometimes collapsed into a single margin that is equal to the largest 

of the two margins.

This does not happen on left and right margins! Only top and bottom margins!


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  margin: 0 0 50px 0;
}

h2 {
  margin: 20px 0 0 0;
}
</style>
</head>
<body>

<p>In this example the h1 element has a bottom margin of 50px and the h2 element has a top margin of 20px. 

So, the vertical margin between h1 and h2 should have been 70px (50px + 20px). However, due to margin 

collapse, the actual margin ends up being 50px.</p>

<h1>Heading 1</h1>
<h2>Heading 2</h2>

</body>
</html>


In the example above, the <h1> element has a bottom margin of 50px and the <h2> element has a top margin set 

to 20px.

Common sense would seem to suggest that the vertical margin between the <h1> and the <h2> would be a total 

of 70px (50px + 20px). But due to margin collapse, the actual margin ends up being 50px.



All CSS Margin Properties
Property 	Description
margin 	A shorthand property for setting the margin properties in one declaration
margin-bottom 	Sets the bottom margin of an element
margin-left 	Sets the left margin of an element
margin-right 	Sets the right margin of an element
margin-top 	Sets the top margin of an element




CSS Padding

CSS 'padding' is used to create spaces outside an element inside any specified borders. To use css padding, 

see below for an example. You can also use CSS to set padding for all the four sides of a CSS element. 

<!DOCTYPE html>
<html>
<head>
<style>
div {
  padding: 100px;
  border: 1px solid #4CAF50;
}
</style>
</head>
<body>

<h2>CSS Padding</h2>
<div>This element has a padding of 70px.</div>

</body>
</html>



Padding - Individual Sides


CSS has properties for specifying the padding for each side of an element:

    padding-top
    padding-right
    padding-bottom
    padding-left

All the padding properties can have the following values:

    length - specifies a padding in px, pt, cm, etc.
    % - specifies a padding in % of the width of the containing element
    inherit - specifies that the padding should be inherited from the parent element

Note: Negative values are not allowed.


For the used of padding on all the four sides, see below for example of use case:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  background-color: lightblue;
  padding-top: 50px;
  padding-right: 30px;
  padding-bottom: 50px;
  padding-left: 80px;
}
</style>
</head>
<body>

<h2>Using individual padding properties</h2>

<div>This div element has a top padding of 50px, a right padding of 30px, a bottom padding of 50px, and a 

left padding of 80px.</div>

</body>
</html>




Padding - Shorthand Property

These properties enable shortening padding properties in one property. For example: 


The padding property is a shorthand property for the following individual padding properties:

    padding-top
    padding-right
    padding-bottom
    padding-left

So, here is how it works:

If the padding property has four values:

    padding: 25px 50px 75px 100px;
        top padding is 25px
        right padding is 50px
        bottom padding is 75px
        left padding is 100px


For example:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  padding: 25px 50px 75px 100px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The padding shorthand property - 4 values</h2>

<div>This div element has a top padding of 25px, a right padding of 50px, a bottom padding of 75px, and a 

left padding of 100px.</div>

</body>
</html>


For padding properties having three values:

If the padding property has three values:

    padding: 25px 50px 75px;
        top padding is 25px
        right and left paddings are 50px
        bottom padding is 75px


For example,


<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  padding: 25px 50px 75px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The padding shorthand property - 3 values</h2>

<div>This div element has a top padding of 25px, a right and left padding of 50px, and a bottom padding of 

75px.</div>

</body>
</html>




For padding properties with two values,

If the padding property has two values:

    padding: 25px 50px;
        top and bottom paddings are 25px
        right and left paddings are 50px


For example:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  padding: 25px 50px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The padding shorthand property - 2 values</h2>

<div>This div element has a top and bottom padding of 25px, and a right and left padding of 50px.</div>

</body>
</html>



When padding property has one value:

If the padding property has one value:

    padding: 25px;
        all four paddings are 25px


For example,
<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  padding: 25px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>The padding shorthand property - 1 value</h2>

<div>This div element has a top, bottom, left, and right padding of 25px.</div>

</body>
</html>




Padding and Element Width

The width element specify width of element's content area ( the area inside the padding, border, and margin 

of the element accordingt to the box model). For an element witrh specified width, the padding of such 

element is added to the value of the specified width ( an often undesirable result).


For example,

<!DOCTYPE html>
<html>
<head>
<style>
div.ex1 {
  width: 300px;
  background-color: yellow;
}

div.ex2 {
  width: 300px;
  padding: 25px;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>Padding and element width</h2>

<div class="ex1">This div is 300px wide.</div>
<br>

<div class="ex2">The width of this div is 350px, even though it is defined as 300px in the CSS.</div>

</body>
</html>


Whenever you need to maintain the widht, the box-sizing property is used to keep width constant irrespective 

of the amount of padding. This effect will collapse available space for the element inwards of the defined 

borders. 

 
For example.

<!DOCTYPE html>
<html>
<head>
<style>
div.ex1 {
  width: 300px;
  background-color: yellow;
}

div.ex2 {
  width: 300px;
  padding: 25px;
  box-sizing: border-box;
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>Padding and element width - with box-sizing</h2>

<div class="ex1">This div is 300px wide.</div>
<br>

<div class="ex2">The width of this div remains at 300px, in spite of the 50px of total left and right 

padding, because of the box-sizing: border-box property.
</div>

</body>
</html>



Other padding examples,


To set the left padding of an element,


<!DOCTYPE html>
<html>
<head>
<style>
p.padding {
  padding-left: 2cm;
}
p.padding2 {
  padding-left: 50%;
}
</style>
</head>
<body>

<h1>The padding-left Property</h1>

<p>This is a text with no left padding.</p>
<p class="padding">This text has a left padding of 2 cm.</p>
<p class="padding2">This text has a left padding of 50%.</p>

</body>
</html>



To set the right padding,

<!DOCTYPE html>
<html>
<head>
<style>
p.padding {
  padding-right: 2cm;
}

p.padding2 {
  padding-right: 50%;
}
</style>
</head>
<body>

<h1>The padding-right Property</h1>

<p>This is a text with no right padding. This is a text with no right padding. This is a text with no right 

padding.</p>
<p class="padding">This text has a right padding of 2 cm. This text has a right padding of 2 cm. This text 

has a right padding of 2 cm.</p>
<p class="padding2">This text has a right padding of 50%. This text has a right padding of 50%. This text 

has a right padding of 50%.</p>

</body>
</html>


To set the top padding,

<!DOCTYPE html>
<html>
<head>
<style>
p.padding {
  padding-top: 2cm;
}

p.padding2 {
  padding-top: 50%;
}
</style>
</head>
<body>

<h1>The padding-top Property</h1>

<p>This is a text with no top padding. This is a text with no top padding. This is a text with no top 

padding.</p>
<p class="padding">This text has a top padding of 2 cm. This text has a top padding of 2 cm. This text has a 

top padding of 2 cm.</p>
<p class="padding2">This text has a top padding of 50%. This text has a top padding of 50%. This text has a 

top padding of 50%.</p>

</body>
</html>


To set the bottom padding,


<!DOCTYPE html>
<html>
<head>
<style>
p.padding {
  padding-bottom:2cm;
}

p.padding2 {
  padding-bottom:50%;
}
</style>
</head>
<body>

<h1>The padding-bottom Property</h1>

<p>This is a text with no bottom padding. This is a text with no bottom padding. This is a text with no 

bottom padding.</p>
<p class="padding">This text has a bottom padding of 2 cm. This text has a bottom padding of 2 cm. This text 

has a bottom padding of 2 cm.</p>
<p class="padding2">This text has a bottom padding of 50%. This text has a bottom padding of 50%. This text 

has a bottom padding of 50%.</p>

</body>
</html>



All CSS Padding Properties summary
Property 	Description
padding 	A shorthand property for setting all the padding properties in one declaration
padding-bottom 	Sets the bottom padding of an element
padding-left 	Sets the left padding of an element
padding-right 	Sets the right padding of an element
padding-top 	Sets the top padding of an element





CSS Height and Width


The CSS 'height' and 'width' properties are used to set the height and width of an element.

The CSS 'max-width' property is used to set the maximum width of an element.


For example,

<!DOCTYPE html>
<html>
<head>
<style>
div {
  height: 50px;
  width: 100%;
  border: 1px solid #4CAF50;
}
</style>
</head>
<body>

<h2>CSS height and width properties</h2>

<div>This element has a height of 50 pixels and a width of 100%.</div>

</body>
</html>


NB: the width of 100% enables the block level elements in <div> to fill any of the available spaces inside 

of its <div> parent element.



CSS Setting height and width

The height and width properties are used to set the height and width of an element.

The height and width properties do not include padding, borders, or margins. It sets the height/width of the 

area inside the padding, border, and margin of the element.



CSS height and width Values

The height and width properties may have the following values:

    auto - This is default. The browser calculates the height and width
    length - Defines the height/width in px, cm etc.
    % - Defines the height/width in percent of the containing block
    initial - Sets the height/width to its default value
    inherit - The height/width will be inherited from its parent value


For example,

<!DOCTYPE html>
<html>
<head>
<style>
div {
  height: 200px;
  width: 50%;
  background-color: powderblue;
}
</style>
</head>
<body>

<h2>Set the height and width of an element</h2>

<div>This div element has a height of 200px and a width of 50%.</div>

</body>
</html>


To set the height and width of a div element.

<!DOCTYPE html>
<html>
<head>
<style>
div {
  height: 100px;
  width: 500px;
  background-color: powderblue;
}
</style>
</head>
<body>

<h2>Set the height and width of an element</h2>

<div>This div element has a height of 100px and a width of 500px.</div>

</body>
</html>


Note: Remember that the height and width properties do not include padding, borders, or margins! They set 

the height/width of the area inside the padding, border, and margin of the element!


Setting max-width


The max-width property is used to set the maximum width of an element.

The max-width can be specified in length values, like px, cm, etc., or in percent (%) of the containing 

block, or set to none (this is default. Means that there is no maximum width).

The problem with the <div> above occurs when the browser window is smaller than the width of the element 

(500px). The browser then adds a horizontal scrollbar to the page.

Using max-width instead, in this situation, will improve the browser's handling of small windows.

Tip: Drag the browser window to smaller than 500px wide, to see the difference between the two divs!


Note: If you for some reason use both the width property and the max-width property on the same element, and 

the value of the width property is larger than the max-width property; the max-width property will be used 

(and the width property will be ignored).



For example,

<!DOCTYPE html>
<html>
<head>
<style>
div {
  max-width: 500px;
  height: 100px;
  background-color: powderblue;
}
</style>
</head>
<body>

<h2>Set the max-width of an element</h2>

<div>This div element has a height of 100px and a max-width of 500px.</div>

<p>Resize the browser window to see the effect.</p>

</body>
</html>


Max width enables the browser to easily adjust the width in case of smaller screen, without the introduction 

of horizontal scroll bar.


Other examples

<!DOCTYPE html>
<html>
<head>
<style>
img.one {
  height: auto;
}

img.two {
  height: 200px;
  width: 200px;
}

div.three {
  height: 300px;
  width: 300px;
  background-color: powderblue;
}
</style>
</head>
<body>

<h2>Set the height and width of elements</h2>

<p>Original image:</p>
<img class="one" src="ocean.jpg" width="300" height="300"><br>

<p>Sized image (200x200 pixels):</p>
<img class="two" src="ocean.jpg" width="300" height="300"><br>

<p>The height and width of this div element is 300px:</p>
<div class="three"></div>

</body>
</html>



Set the height and width of an image using percent value,

<!DOCTYPE html>
<html>
<head>
<style>
html, body {
  height: 100%;
}

img.one {
  height: auto;
  width: auto;
}

img.two {
  height: 50%;
  width: 50%;
}
</style>
</head>
<body>

<h2>Set the height and width in %</h2>
<p>Resize the browser window to see the effect.</p>

<p>Original image:</p>
<img class="one" src="ocean.jpg" width="300" height="300"><br>

<p>Sized image (in %):</p>
<img class="two" src="ocean.jpg" width="300" height="300">

</body>
</html>


Set min-width and max-width of an element



<!DOCTYPE html>
<html>
<head>
<style>
div {
  max-width: 400px;
  min-width: 100px;
  background-color: powderblue;
}
</style>
</head>
<body>

<h2>Set the max-width and min-width of an element</h2>
<p>Resize the browser window to see the effect.</p>

<div>This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.</div>

</body>
</html>




Set min-height and max-height of an element using pixel value,

<!DOCTYPE html>
<html>
<head>
<style>
div {
  max-height: 600px;
  min-height: 400px;
  background-color: powderblue;
}
</style>
</head>
<body>

<h2>Set the max-height and min-height of an element</h2>
<p>Resize the browser window to see the effect.</p>

<div>This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.</div>

</body>
</html>




All CSS Dimension Properties
Property 	Description
height 	Sets the height of an element
max-height 	Sets the maximum height of an element
max-width 	Sets the maximum width of an element
min-height 	Sets the minimum height of an element
min-width 	Sets the minimum width of an element
width 	Sets the width of an element





CSS Box Model

All html elements can be considered to be boxes. The box model wraps around every HTML element and consists 

of margins, borders, padding, and the actual content ( when you go from outside the element to inside the 

element. 



Explanation of the different parts:

    Content - The content of the box, where text and images appear
    Padding - Clears an area around the content. The padding is transparent
    Border - A border that goes around the padding and content
    Margin - Clears an area outside the border. The margin is transparent

For example,

<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: lightgrey;
  width: 300px;
  border: 15px solid green;
  padding: 50px;
  margin: 20px;
}
</style>
</head>
<body>

<h2>Demonstrating the Box Model</h2>

<p>The CSS box model is essentially a box that wraps around every HTML element. It consists of: borders, 

padding, margins, and the actual content.</p>

<div>This text is the content of the box. We have added a 50px padding, 20px margin and a 15px green border. 

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 

Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. 

Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est 

laborum.</div>

</body>
</html>


Width and height of an element

The knowledge of the box model allows you to set the width and height of website elements correctly in al 

browsers.


Important: When you set the width and height properties of an element with CSS, you just set the width and 

height of the content area. To calculate the full size of an element, you must also add padding, borders and 

margins.


In the script below,

<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 320px;
  padding: 10px;
  border: 5px solid gray;
  margin: 0;
}
</style>
</head>
<body>

<h2>Calculate the total width:</h2>

<img src="klematis4_big.jpg" width="350" height="263" alt="Klematis">
<div>The picture above is 350px wide. The total width of this element is also 350px.</div>

</body>
</html>

The total width can be calculated as shown below,


320px (width)
+ 20px (left + right padding)
+ 10px (left + right border)
+ 0px (left + right margin)
= 350px 


The total width of an element should be calculated like this:

Total element width = width + left padding + right padding + left border + right border + left margin + 

right margin

Similarly, the total height of an element should be calculated as shown below:

Total element height = height + top padding + bottom padding + top border + bottom border + top margin + 

bottom margin





CSS Outline


Outline::

An outline is a line drawn around the elements (outside borders) to make the element "stand out"..

An outline can be created around an element using the script shown below:

<!DOCTYPE html>
<html>
<head>
<style>
p {
  border: 2px solid black;
  outline: #4CAF50 solid 2px;
  margin: auto;  
  padding: 20px;
  text-align: center;
}
</style>
</head>
<body>

<h2>CSS Outline</h2>
<p>This element has a 2px black border and a green outline with a width of 10px.</p>

</body>
</html>



The outline properties of CSS include,

    outline-style
    outline-color
    outline-width
    outline-offset
    outline


Note: Outline differs from borders! Unlike border, the outline is drawn outside the element's border, and 

may overlap other content. Also, the outline is NOT a part of the element's dimensions; the element's total 

width and height is not affected by the width of the outline.


CSS Outline Style

The outline-style property specifies the style of the outline, and can have one of the following values:

    dotted - Defines a dotted outline
    dashed - Defines a dashed outline
    solid - Defines a solid outline
    double - Defines a double outline
    groove - Defines a 3D grooved outline
    ridge - Defines a 3D ridged outline
    inset - Defines a 3D inset outline
    outset - Defines a 3D outset outline
    none - Defines no outline
    hidden - Defines a hidden outline


The implementation of the above outlines is shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p {outline-color:red;}

p.dotted {outline-style: dotted;}
p.dashed {outline-style: dashed;}
p.solid {outline-style: solid;}
p.double {outline-style: double;}
p.groove {outline-style: groove;}
p.ridge {outline-style: ridge;}
p.inset {outline-style: inset;}
p.outset {outline-style: outset;}
</style>
</head>
<body>

<h2>The outline-style Property</h2>

<p class="dotted">A dotted outline</p>
<p class="dashed">A dashed outline</p>
<p class="solid">A solid outline</p>
<p class="double">A double outline</p>
<p class="groove">A groove outline. The effect depends on the outline-color value.</p>
<p class="ridge">A ridge outline. The effect depends on the outline-color value.</p>
<p class="inset">An inset outline. The effect depends on the outline-color value.</p>
<p class="outset">An outset outline. The effect depends on the outline-color value.</p>

</body>
</html>


NB: Note: None of the other outline properties (which you will learn more about in the next chapters) will 

have ANY effect unless the outline-style property is set!




CSS Outline Width

The width of the outline is specified using outline-width property, and this outline-width can have multiple 

values:



    thin (typically 1px)
    medium (typically 3px)
    thick (typically 5px)
    A specific size (in px, pt, cm, em, etc)

An example of how to specify outline-width is shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: thin;
}

p.ex2 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: medium;
}

p.ex3 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: thick;
}

p.ex4 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: 4px;
}
</style>
</head>
<body>

<h2>The outline-width Property</h2>

<p class="ex1">A thin outline.</p>
<p class="ex2">A medium outline.</p>
<p class="ex3">A thick outline.</p>
<p class="ex4">A 4px thick outline.</p>

</body>
</html>




CSS Outline Color::


CSS Outline Color

The outline-color property is used to set the color of the outline.

The color can be set by:

    name - specify a color name, like "red"
    HEX - specify a hex value, like "#ff0000"
    RGB - specify a RGB value, like "rgb(255,0,0)"
    HSL - specify a HSL value, like "hsl(0, 100%, 50%)"
    invert - performs a color inversion (which ensures that the outline is visible, regardless of color 

background)


An example of the application of the outline-color property is shown below:

<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: red;
}

p.ex2 {
  border: 2px solid black;
  outline-style: dotted;
  outline-color: blue;
}

p.ex3 {
  border: 2px solid black;
  outline-style: outset;
  outline-color: grey;
}
</style>
</head>
<body>

<h2>The outline-color Property</h2>
<p>The outline-color property is used to set the color of the outline.</p>

<p class="ex1">A solid red outline.</p>
<p class="ex2">A dotted blue outline.</p>
<p class="ex3">An outset grey outline.</p>

</body>
</html>




HEX Values

The hexadecimal value can be used to specify the color of the outline as shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: #ff0000; /* red */
}

p.ex2 {
  border: 2px solid black;
  outline-style: dotted;
  outline-color: #0000ff; /* blue */
}

p.ex3 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: #bbbbbb; /* grey */
}
</style>
</head>
<body>

<h2>The outline-color Property</h2>
<p>The color of the outline can also be specified using a hexadecimal value (HEX):</p>

<p class="ex1">A solid red outline.</p>
<p class="ex2">A dotted blue outline.</p>
<p class="ex3">A solid grey outline.</p>

</body>
</html>


RGB Values

The RGB values can also be used to specify the color of the outline as shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: rgb(255, 0, 0); /* red */
}

p.ex2 {
  border: 2px solid black;
  outline-style: dotted;
  outline-color: rgb(0, 0, 255); /* blue */
}

p.ex3 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: rgb(187, 187, 187); /* grey */
}
</style>
</head>
<body>

<h2>The outline-color Property</h2>
<p>The color of the outline can also be specified using RGB values:</p>

<p class="ex1">A solid red outline.</p>
<p class="ex2">A dotted blue outline.</p>
<p class="ex3">A solid grey outline.</p>

</body>
</html>




HSL Values

The HSL values (hue, saturation, and lightness values) can also be used to specify the color of a CSS 

outline as shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: hsl(0, 100%, 50%); /* red */
}

p.ex2 {
  border: 2px solid black;
  outline-style: dotted;
  outline-color: hsl(240, 100%, 50%); /* blue */
}

p.ex3 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: hsl(0, 0%, 73%); /* grey */
}
</style>
</head>
<body>

<h2>The outline-color Property</h2>
<p>The color of the outline can also be specified using HSL values:</p>

<p class="ex1">A solid red outline.</p>
<p class="ex2">A dotted blue outline.</p>
<p class="ex3">A solid grey outline.</p>

</body>
</html>





Invert Color

The outline-color: invert performs color inversion which enables visibility of the outline irrespective of 

the background color.

<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  border: 1px solid yellow;
  outline-style: solid;
  outline-color: invert;
}
</style>
</head>
<body>

<h2>Using outline-color:invert</h2>

<p class="ex1">A solid invert outline.</p>

</body>
</html>


CSS Outline Shorthand::


CSS Outline - Shorthand property

The outline property is a shorthand property for setting the following individual outline properties:

    outline-width
    outline-style (required)
    outline-color

The outline property is specified as one, two, or three values from the list above. The order of the values 

does not matter.

The following example shows some outlines specified with the shorthand outline property:


<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {outline: dashed;}
p.ex2 {outline: dotted red;}
p.ex3 {outline: 5px solid yellow;}
p.ex4 {outline: thick ridge pink;}
</style>
</head>
<body>

<h2>The outline Property</h2>

<p class="ex1">A dashed outline.</p>
<p class="ex2">A dotted red outline.</p>
<p class="ex3">A 5px solid yellow outline.</p>
<p class="ex4">A thick ridge pink outline.</p>

</body>
</html>



CSS Outline Offset

The outline-offset property is used to include space between an outline and the edge/border of an element, 

leaving the space between an element and its outline transparent.


The script below shows how the outline offset is added to an element, such that the outline is 15px outside 

the border of the <p> element:


<!DOCTYPE html>
<html>
<head>
<style>
p {
  margin: 30px;
  border: 1px solid black;
  outline: 1px solid red;
  outline-offset: 15px;
}
</style>
</head>
<body>

<h2>The outline-offset Property</h2>

<p>This paragraph has an outline 15px outside the border edge.</p>

</body>
</html>



To visualize that the space between an element's border and its outline offset is transparent


<!DOCTYPE html>
<html>
<head>
<style>
p {
  margin: 30px;
  background:yellow;
  border: 1px solid black;
  outline: 1px solid red;
  outline-offset: 15px;
}
</style>
</head>
<body>

<h2>The outline-offset Property</h2>

<p>This paragraph has an outline of 15px outside the border edge.</p>

</body>
</html>



All CSS Outline Properties Summarized

All CSS Outline Properties
Property 	Description
outline 	A shorthand property for setting outline-width, outline-style, and outline-color in one 

declaration
outline-color 	Sets the color of an outline
outline-offset 	Specifies the space between an outline and the edge or border of an element
outline-style 	Sets the style of an outline
outline-width 	Sets the width of an outline





CSS Text

We explain properties used in formatting texts in CSS under this section and subsections that follow.


Text formatting example is shown below:



<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid gray;
  padding: 8px;
}

h1 {
  text-align: center;
  text-transform: uppercase;
  color: #4CAF50;
}

p {
  text-indent: 50px;
  text-align: justify;
  letter-spacing: 3px;
}

a {
  text-decoration: none;
  color: #008CBA;
}
</style>
</head>
<body>

<div>
  <h1>text formatting</h1>
  <p>This text is styled with some of the text formatting properties. The heading uses the text-align, 

text-transform, and color properties.
  The paragraph is indented, aligned, and the space between characters is specified. The underline is 

removed from this colored
  <a target="_blank" href="tryit.asp?filename=trycss_text">"Try it Yourself"</a> link.</p>
</div>

</body>
</html>




Text Color::

The color property is used to set the color of the text using:


    a color name - like "red"
    a HEX value - like "#ff0000"
    an RGB value - like "rgb(255,0,0)"
NB: The default text color or a page is defined in the 'body' selector, under the <style> tags. See below 

for example:



<!DOCTYPE html>
<html>
<head>
<style>
body {
  color: blue;
}

h1 {
  color: green;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<p>This is an ordinary paragraph. Notice that this text is blue. The default text color for a page is 

defined in the body selector.</p>
<p>Another paragraph.</p>

</body>
</html>


Note: For W3C compliant CSS: If you define the color property, you must also define the background-color.



Text Color and Background Color

In this example, we define both the background-color property and the color property (for an element):


<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: lightgrey;
  color: blue;
}

h1 {
  background-color: black;
  color: white;
}
</style>
</head>
<body>

<h1>This Heading is Black with White Text</h1>
<p>This page has a grey background color and a blue text.</p>
<p>Another paragraph.</p>

</body>
</html>




CSS Text Alignment::

the css text-align property is used to set the horizontal alignment of a text to left, right, or justified 

aligned. If text direction is left-to-right, the default alignment is left. On the other hand, if the text 

is from right-to-left, the default alignment is right. An example of the use of text-align property is shown 

below:

<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-align: center;
}

h2 {
  text-align: left;
}

h3 {
  text-align: right;
}
</style>
</head>
<body>

<h1>Heading 1 (center)</h1>
<h2>Heading 2 (left)</h2>
<h3>Heading 3 (right)</h3>

<p>The three headings above are aligned center, left and right.</p>

</body>
</html>


When the text-align property is set to "justify", each line is stretched so that every line has equal width, 

and the left and right margins are straight (like in magazines and newspapers):

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  padding: 10px;
  width: 200px;
  height: 200px;
  text-align: justify;
}
</style>
</head>
<body>

<h1>Example text-align: justify;</h1>

<p>The text-align: justify; value stretches the lines so that each line has equal width (like in newspapers 

and magazines).</p>

<div>
In my younger and more vulnerable years my father gave me some advice that I've been turning over in my mind 

ever since. 'Whenever you feel like criticizing anyone,' he told me, 'just remember that all the people in 

this world haven't had the advantages that you've had.'
</div>

</body>
</html>



Text Direction

The direction and unicode-bidi (invert each of the letters from left to right) properties can be used to 

change the text direction of an element:

<!DOCTYPE html>
<html>
<head>
<style>
p.ex1 {
  direction: rtl;
  unicode-bidi: bidi-override;
}
</style>
</head>
<body>

<p>This is the default text direction.</p>

<p class="ex1">This is right-to-left text direction.</p>

</body>
</html>


Vertical Alignment

The vertical-align property sets the vertical alignment of an element. The example below shows how to set 

the vertical alignment of an image in a text.



<!DOCTYPE html>
<html>
<head>
<style>
img.a {
  vertical-align: baseline;
}

img.b {
  vertical-align: text-top;
}

img.c {
  vertical-align: text-bottom;
}

img.d {
  vertical-align: sub;
}

img.e {
  vertical-align: super;
}
</style>
</head>
<body>

<h1>The vertical-align Property</h1>

<h2>vertical-align: baseline (default):</h2>
<p>An <img class="a" src="sqpurple.gif" width="9" height="9"> image with a default alignment.</p> 

<h2>vertical-align: text-top:</h2>
<p>An <img class="b" src="sqpurple.gif" width="9" height="9"> image with a text-top alignment.</p> 

<h2>vertical-align: text-bottom:</h2>
<p>An <img class="c" src="sqpurple.gif" width="9" height="9"> image with a text-bottom alignment.</p>

<h2>vertical-align: sub:</h2>
<p>An <img class="d" src="sqpurple.gif" width="9" height="9"> image with a sub alignment.</p> 

<h2>vertical-align: sup:</h2>
<p>An <img class="e" src="sqpurple.gif" width="9" height="9"> image with a super alignment.</p>

</body>
</html>



CSS Text Decoration


Text Decoration

The text-decoration property is used to set or remove decorations from text.

The value text-decoration: none; is often used to remove underlines from links:



<!DOCTYPE html>
<html>
<head>
<style>
a {
  text-decoration: none;
}
</style>
</head>
<body>

<p>A link with no underline: <a href="https://www.w3schools.com">W3Schools.com</a></p>

</body>
</html>




Other text decoration values are shown below:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-decoration: overline;
}

h2 {
  text-decoration: line-through;
}

h3 {
  text-decoration: underline;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>

</body>
</html>


Note: It is not recommended to underline text that is not a link, as this often confuses the reader.



Text Transformation::

The text-transform property is used to specify uppercase and lowercase letters in a text.

It can be used to turn everything into uppercase or lowercase letters, or capitalize the first letter of 

each word:



<!DOCTYPE html>
<html>
<head>
<style>
p.uppercase {
  text-transform: uppercase;
}

p.lowercase {
  text-transform: lowercase;
}

p.capitalize {
  text-transform: capitalize;
}
</style>
</head>
<body>

<p class="uppercase">This is some text.</p>
<p class="lowercase">This is some text.</p>
<p class="capitalize">This is some text.</p>

</body>
</html>






CSS Text Spacing::

The text-indent property is used to specify the indentation of the first line of a text.



<!DOCTYPE html>
<html>
<head>
<style>
p {
  text-indent: 50px;
}
</style>
</head>
<body>

<p>In my younger and more vulnerable years my father gave me some advice that I've been turning over in my 

mind ever since. 'Whenever you feel like criticizing anyone,' he told me, 'just remember that all the people 

in this world haven't had the advantages that you've had.'</p>

</body>
</html>



Letter Spacing

The letter-spacing property is used to specify the space between the characters in a text.

The following example demonstrates how to increase or decrease the space between characters:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  letter-spacing: 3px;
}

h2 {
  letter-spacing: -3px;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>

</body>
</html>




Line Height

The line-height property is used to specify the space between lines:


<!DOCTYPE html>
<html>
<head>
<style>
p.small {
  line-height: 0.7;
}

p.big {
  line-height: 1.8;
}
</style>
</head>
<body>

<p>
This is a paragraph with a standard line-height.<br>
The default line height in most browsers is about 110% to 120%.<br>
</p>

<p class="small">
This is a paragraph with a smaller line-height.<br>
This is a paragraph with a smaller line-height.<br>
</p>

<p class="big">
This is a paragraph with a bigger line-height.<br>
This is a paragraph with a bigger line-height.<br>
</p>

</body>
</html>















































Word Spacing

The word-spacing property is used to specify the space between the words in a text.

The following example demonstrates how to increase (positive value) or decrease (negative value) the space 

between words:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  word-spacing: 10px;
}

h2 {
  word-spacing: -5px;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>

</body>
</html>




White Space

The white-space property specifies how white-space inside an element is handled.

This example demonstrates how to disable text wrapping inside an element:



<!DOCTYPE html>
<html>
<head>
<style>
p {
  white-space: nowrap;
}
</style>
</head>
<body>

<h2>White Space</h2>

<p>
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
</p>

<p>Try to remove the white-space property to see the difference.</p>

</body>
</html>






CSS Text Shadow::


Text Shadow

The text-shadow property adds shadow to text.

In its simplest use, you only specify the horizontal shadow (2px) and the vertical shadow (2px):


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-shadow: 2px 2px;
}
</style>
</head>
<body>

<h1>Text-shadow effect!</h1>

</body>
</html>




To add a color (red) to the shadow:

<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-shadow: 2px 2px red;
}
</style>
</head>
<body>

<h1>Text-shadow effect!</h1>

</body>
</html>




To add a blur effect (5px) to the shadow:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-shadow: 2px 2px 5px red;
}
</style>
</head>
<body>

<h1>Text-shadow effect!</h1>

</body>
</html>




CSS Fonts


The right fond can improve UX of a website and can create a unique and strong brand identity. Readability of 

a font is very crucial, for font to add value to text. Color and text size of a font are important too while 

choosing a font.



Generic Font Families

In CSS there are five generic font families:

    Serif fonts have a small stroke at the edges of each letter. They create a sense of formality and 

elegance.
    Sans-serif fonts have clean lines (no small strokes attached). They create a modern and minimalistic 

look.
    Monospace fonts - here all the letters have the same fixed width. They create a mechanical look. 
    Cursive fonts imitate human handwriting.
    Fantasy fonts are decorative/playful fonts.

All the different font names belong to one of the generic font families. 



Note: On computer screens, sans-serif fonts are considered easier to read than serif fonts.


Some Font Examples

Generic Font Family    Examples of Font Names


Serif    		Times New Roman, Georgia, Garamond

Sans-serif		Arial Verdana, Helvetica

Monospace               Courier New, Lucida Console, Monaco,

Cursive			Brush Script MT, Lucida Handwriting

Fantasy			Copperplate, Papyrus



The CSS font-family Property

In CSS, we use the font-family property to specify the font of a text.

The font-family property should hold several font names as a "fallback" system, to ensure maximum 

compatibility between browsers/operating systems. Start with the font you want, and end with a generic 

family (to let the browser pick a similar font in the generic family, if no other fonts are available). The 

font names should be separated with comma.

Note: If the font name is more than one word, it must be in quotation marks, like: "Times New Roman". 

An example of the application of font-family in CSS is shown below:


<!DOCTYPE html>
<html>
<head>
<style>
.p1 {
  font-family: "Times New Roman", Times, serif;
}

.p2 {
  font-family: Arial, Helvetica, sans-serif;
}

.p3 {
  font-family: "Lucida Console", "Courier New", monospace;
}
</style>
</head>
<body>

<h1>CSS font-family</h1>
<p class="p1">This is a paragraph, shown in the Times New Roman font.</p>
<p class="p2">This is a paragraph, shown in the Arial font.</p>
<p class="p3">This is a paragraph, shown in the Lucida Console font.</p>

</body>
</html>




CSS Web Safe Fonts::

They are fonts that are universally installed on all browsers and devices. 


Fallback Fonts: since there are no 100% web safe fonts, always use fallback fonts in case a font is not 

found or is not properly installed on the browser or device.


You should always add a list of similar 'backup fonts' in the font-family property.If the first font does 

not work, the browser will try the next one, and the next one, and so on. Always end the list with a generic 

font family name.



An illustration of this concept is shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p {
font-family: Tahoma, Verdana, sans-serif;
}
</style>
</head>
<body>

<h1>CSS Fallback Fonts</h1>

<p>This is a paragraph.</p>
<p>This is another paragraph.</p>

</body>
</html>



Best Web Safe Fonts for HTML and CSS

The following list are the best web safe fonts for HTML and CSS:

    Arial (sans-serif)
    Verdana (sans-serif)
    Helvetica (sans-serif)
    Tahoma (sans-serif)
    Trebuchet MS (sans-serif)
    Times New Roman (serif)
    Georgia (serif)
    Garamond (serif)
    Courier New (monospace)
    Brush Script MT (cursive)

Note: Before you publish your website, always check how your fonts appear on different browsers and devices, 

and always use fallback fonts!


Arial (sans-serif)

Arial is the most widely used font for both online and printed media. Arial is also the default font in 

Google Docs.

Arial is one of the safest web fonts, and it is available on all major operating systems.

An example of specifying arial font with font-family 



<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Arial, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Verdana (sans-serif)

Verdana is a very popular font. Verdana is easily readable even for small font sizes.


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Verdana, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Helvetica (sans-serif)

The Helvetica font is loved by designers. It is suitable for many types of business. See example below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Helvetica, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>




Tahoma (sans-serif)

The Tahoma font has less space between the characters. See example below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Tahoma, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>


Trebuchet MS (sans-serif)

Trebuchet MS was designed by Microsoft in 1996. Use this font carefully. Not supported by all mobile 

operating systems. See example below:



<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: 'Trebuchet MS', sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Times New Roman (serif)

Times New Roman is one of the most recognizable fonts in the world. It looks professional and is used in 

many newspapers and "news" websites. It is also the primary font for Windows devices and applications. See 

example bnw


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: 'Times New Roman', serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Georgia (serif)

Georgia is an elegant serif font. It is very readable at different font sizes, so it is a good candidate for 

mobile-responsive design. See example below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Georgia, serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Garamond (serif)

Garamond is a classical font used for many printed books. It has a timeless look and good readability. See 

example below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Garamond, serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Courier New (monospace)

Courier New is the most widely used monospace serif font. Courier New is often used with coding displays, 

and many email providers use it as their default font. Courier New is also the standard font for movie 

screenplays.



<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: 'Courier New', monospace;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>


Brush Script MT (cursive)

The Brush Script MT font was designed to mimic handwriting. It is elegant and sophisticated, but can be hard 

to read. Use it carefully. See example below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: 'Brush Script MT', cursive;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



CSS Font Fallbacks::


Commonly Used Font Fallbacks

Below are some commonly used font fallbacks, organized by the 5 generic font families:

    Serif
    Sans-serif
    Monospace
    Cursive
    Fantasy

The different font families and the corresponding script to implement them are shown below:


Serif Fonts:::


font-family ("Times New Roman", Times, serif). see the code below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: "Times New Roman", Times, serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



font-family (Georgia, serif). See the code below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Georgia, serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



font-family (Garamond, serif). See the code to apply them below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Garamond, serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>




Sans-Serif Fonts:::

font-family (Arial, Helvetica, san-serif). See the implementation below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Arial, Helvetica, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



font-family (Tahoma, Verdana, sans-serif). See the implementation below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Tahoma, Verdana, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



font-family ("Trebuchet MS", Helvetica, sans-serif). See the implementation below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: "Trebuchet MS", Helvetica, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



font-family (Georgia, Verdana, sans-serif). See implementation below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Georgia, Verdana, sans-serif;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Monospace Fonts:::

font-family ("Courier New", Courier, monospace). See implementation below:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: "Courier New", Courier, monospace;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Cursive Fonts:::

font-family ("Brush Script MT", cursive). See how to implement this font family below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: "Brush Script MT", cursive;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Fantasy Fonts:::

font-family (Copperplate, Papyrus, fantasy). See how to implement this font family below:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Copperplate, Papyrus, fantasy;
}
</style>
</head>
<body>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>





CSS Font Style::


Font Style

The font-style property is mostly used to specify italic text.

This property has three values:

    normal - The text is shown normally
    italic - The text is shown in italics
    oblique - The text is "leaning" (oblique is very similar to italic, but less supported)


The implementation of font-style is shown below:


<!DOCTYPE html>
<html>
<head>
<style>
p.normal {
  font-style: normal;
}

p.italic {
  font-style: italic;
}

p.oblique {
  font-style: oblique;
}
</style>
</head>
<body>

<p class="normal">This is a paragraph in normal style.</p>
<p class="italic">This is a paragraph in italic style.</p>
<p class="oblique">This is a paragraph in oblique style.</p>

</body>
</html>




Font Weight

The font-weight property specifies the weight of a font:


<!DOCTYPE html>
<html>
<head>
<style>
p.normal {
  font-weight: normal;
}

p.light {
  font-weight: lighter;
}

p.thick {
  font-weight: bold;
}

p.thicker {
  font-weight: 900;
}
</style>
</head>
<body>

<p class="normal">This is a paragraph.</p>
<p class="light">This is a paragraph.</p>
<p class="thick">This is a paragraph.</p>
<p class="thicker">This is a paragraph.</p>

</body>
</html>


Font Variant

The font-variant property specifies whether or not a text should be displayed in a small-caps font.

In a small-caps font, all lowercase letters are converted to uppercase letters. However, the converted 

uppercase letters appears in a smaller font size than the original uppercase letters in the text.

<!DOCTYPE html>
<html>
<head>
<style>
p.normal {
  font-variant: normal;
}

p.small {
  font-variant: small-caps;
}
</style>
</head>
<body>

<p class="normal">My name is Hege Refsnes.</p>
<p class="small">My name is Hege Refsnes.</p>

</body>
</html>





CSS Font Size::



Font Size

The font-size property sets the size of the text.

Being able to manage the text size is important in web design. However, you should not use font size 

adjustments to make paragraphs look like headings, or headings look like paragraphs.

Always use the proper HTML tags, like <h1> - <h6> for headings and <p> for paragraphs.

The font-size value can be an absolute, or relative size.

Absolute size:

    Sets the text to a specified size
    Does not allow a user to change the text size in all browsers (bad for accessibility reasons)
    Absolute size is useful when the physical size of the output is known

Relative size:

    Sets the size relative to surrounding elements
    Allows a user to change the text size in browsers


Note: If you do not specify a font size, the default size for normal text, like paragraphs, is 16px 

(16px=1em).

Convertion factor: 1em=12pt=16px=100%



Set Font Size With Pixels

Setting the text size with pixels gives you full control over the text size:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  font-size: 40px;
}

h2 {
  font-size: 30px;
}

p {
  font-size: 14px;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>

</body>
</html>


Tip: If you use pixels, you can still use the zoom tool to resize the entire page.



Set Font Size With Em

To allow users to resize the text (in the browser menu), many developers use em instead of pixels.

1em is equal to the current font size. The default text size in browsers is 16px. So, the default size of 

1em is 16px.

The size can be calculated from pixels to em using this formula: pixels/16=em

See application below:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  font-size: 2.5em; /* 40px/16=2.5em */
}

h2 {
  font-size: 1.875em; /* 30px/16=1.875em */
 }

p {
  font-size: 0.875em; /* 14px/16=0.875em */
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<p>This is a paragraph.</p>
<p>Specifying the font-size in em allows all major browsers to resize the text.
Unfortunately, there is still a problem with older versions of IE. When resizing the text, it becomes 

larger/smaller than it should.</p>

</body>
</html>



In the example above, the text size in em is the same as the previous example in pixels. However, with the 

em size, it is possible to adjust the text size in all browsers.

Unfortunately, there is still a problem with older versions of Internet Explorer. The text becomes larger 

than it should when made larger, and smaller than it should when made smaller.




Use a Combination of Percent and Em

The solution that works in all browsers, is to set a default font-size in percent for the <body> element:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-size: 100%;
}

h1 {
  font-size: 2.5em;
}

h2 {
  font-size: 1.875em;
}

p {
  font-size: 0.875em;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<p>This is a paragraph.</p>
<p>Specifying the font-size in percent and em displays the same size in all major browsers, and allows all 

browsers to resize the text!</p>

</body>
</html>


NB: Our code now works great! It shows the same text size in all browsers, and allows all browsers to zoom 

or resize the text!



Responsive Font Size

The text size can be set with a vw unit, which means the "viewport width". Viewport is the browser window 

size. 1vw = 1% of viewport width. If the viewport is 50cm wide, 1vw is 0.5cm.

That way the text size will follow the size of the browser window:


<!DOCTYPE html>
<html>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<body>

<h1 style="font-size:10vw;">Responsive Text</h1>

<p style="font-size:5vw;">Resize the browser window to see how the text size scales.</p>

<p style="font-size:5vw;">Use the "vw" unit when sizing the text. 10vw will set the size to 10% of the 

viewport width.</p>

<p>Viewport is the browser window size. 1vw = 1% of viewport width. If the viewport is 50cm wide, 1vw is 

0.5cm.</p>

</body>
</html>





CSS Google Fonts::


Google fonts are 1000+ free-to-use additoinal fonts for people who prefer not to use the standard HTML 

fonts.

How To Use Google Fonts

Just add a special style sheet link in the <head> section and then refer to the font in the CSS.



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
<style>
body {
  font-family: "Sofia", sans-serif;
}
</style>
</head>
<body>

<h1>Sofia Font</h1>
<p>Lorem ipsum dolor sit amet.</p>
<p>123456790</p>

</body>
</html>



To use a font named "Trirong" from Google Fonts:

<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Trirong">
<style>
body {
  font-family: "Trirong", serif;
}
</style>
</head>
<body>

<h1>Trirong Font</h1>
<p>Lorem ipsum dolor sit amet.</p>
<p>123456790</p>

</body>
</html>


To use a font named "Audiowide" from Google Fonts:

<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide">
<style>
body {
  font-family: "Audiowide", sans-serif;
}
</style>
</head>
<body>

<h1>Audiowide Font</h1>
<p>Lorem ipsum dolor sit amet.</p>
<p>123456790</p>

</body>
</html>




Note: When specifying a font in CSS, always list at minimum one fallback font (to avoid unexpected 

behaviors). So, also here you should add a generic font family (like serif or sans-serif) to the end of the 

list.

See all available google fonts here: https://www.w3schools.com/howto/howto_google_fonts.asp


To use multiple Google fonts, just separate the font names with a pipe character (|), like this:



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide|Sofia|Trirong">
<style>
h1.a {
  font-family: "Audiowide", sans-serif;
}

h1.b {
  font-family: "Sofia", sans-serif;
}

h1.c {
  font-family: "Trirong", serif;
}
</style>
</head>
<body>

<h1 class="a">Audiowide Font</h1>

<h1 class="b">Sofia Font</h1>

<h1 class="c">Trirong Font</h1>

</body>
</html>



NB: Requesting multiple fonts may slow down your web pages! So be careful about that.



Styling Google Fonts

CSS can be used to style Google Fonts as shown below:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
<style>
body {
  font-family: "Sofia", sans-serif;
  font-size: 30px;
  text-shadow: 3px 3px 3px #ababab;
}
</style>
</head>
<body>

<h1>Sofia Font</h1>
<p>Lorem ipsum dolor sit amet.</p>
<p>123456790</p>

</body>
</html>




Enabling Font Effects

Google have also enabled different font effects that you can use.

First add effect=effectname to the Google API, then add a special class name to the element that is going to 

use the special effect. The class name always starts with font-effect- and ends with the effectname.


To add the fire effect to the "Sofia" font


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=fire">
<style>
body {
  font-family: "Sofia", sans-serif;
  font-size: 30px;
}
</style>
</head>
<body>

<h1 class="font-effect-fire">Sofia on Fire</h1>
<p class="font-effect-fire">Lorem ipsum dolor sit amet.</p>
<p class="font-effect-fire">123456790</p>

</body>
</html>


To request multiple font effects, just separate the effect names with a pipe character (|), like this:



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=neon|outline|emboss|

shadow-multiple">
<style>
body {
  font-family: "Sofia", sans-serif;
  font-size: 30px;
}
</style>
</head>
<body>

<h1 class="font-effect-neon">Neon Effect</h1>
<h1 class="font-effect-outline">Outline Effect</h1>
<h1 class="font-effect-emboss">Emboss Effect</h1>
<h1 class="font-effect-shadow-multiple">Multiple Shadow Effect</h1>

</body>
</html>





CSS Great Font Pairings::

It is important for a website to have great font pairings. This improves the design.


Font Pairing Rules

Here are some basic rules to create great font pairings:
1. Complement

It is always safe to find font pairings that complement one another.

A great font combination should harmonize, without being too similar or too different.
2. Use Font Superfamilies

A font superfamily is a set of fonts designed to work well together. So, using different fonts within the 

same superfamily is safe.

For example, the Lucida superfamily contains the following fonts: Lucida Sans, Lucida Serif, Lucida 

Typewriter Sans, Lucida Typewriter Serif and Lucida Math.
3. Contrast is King

Two fonts that are too similar will often conflict. However, contrasts, done the right way, brings out the 

best in each font.

Example: Combining serif with sans serif is a well known combination.

A strong superfamily includes both serif and sans serif variations of the same font (e.g. Lucida and Lucida 

Sans).
4. Choose Only One Boss

One font should be the boss. This establishes a hierarchy for the fonts on your page. This can be achieved 

by varying the size, weight and color.


In the example below, Georgia font family is the boss as it is larger and a compatible but different fonts:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: black;
  font-family: Verdana, sans-serif;
  font-size: 16px;
  color: gray;  
}

h1 {
  font-family: Georgia, serif;
  font-size: 60px;
  color: white;
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html>




Some of the available popular font pairings that will suit many brands and contexts are shown in the 

examples below:


Georgia and Verdana

Georgia and Verdana is a classic combination. It also sticks to the web safe font standards. Use "Georgia" 

font for headings, and "Verdana" font for text. See example below:



<!DOCTYPE html>
<html>
<head>
<style>
body  {
  font-family: Verdana, sans-serif;
  font-size: 16px;
}

h1 {
  font-family: Georgia, serif;
  font-size: 46px;  
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 



Helvetica and Garamond

Helvetica and Garamond is another classic combination that uses web safe fonts. Use "Helvetica" font for 

headings and "Garamond" font for text. See example below:



<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-family: Garamond, serif;
  font-size: 16px;  
}

h1 {
  font-family: Helvetica, sans-serif;
  font-size: 46px;  
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 





Popular Google Font Pairings

Google fonts provide 1000+ alternatives to traditional HTML fonts.They are free to use on your website. 


Below are the compatible google fonts




Merriweather and Open Sans 

Meriwether font for headings, and "Open Sans" for text::


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Merriweather|Open+Sans">
<style>
body {
  font-family: "Open Sans", sans-serif;
  font-size: 16px;
}

h1 {
  font-family: Merriweather, serif;
  font-size: 46px;
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 




Ubuntu and Lora

USe Ubuntu for headings and Lora for text. See example below:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Ubuntu|Lora">
<style>
body {
  font-family: Lora, serif;
  font-size: 16px;  
}

h1 {
  font-family: Ubuntu, sans-serif;
  font-size: 46px;  
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 



Abril Fatface and Poppins

Use "Abril Fatface" font for headings, and "Poppins" for text. For example:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Abril+Fatface|Poppins">
<style>
body {
  font-family: Poppins, sans-serif;
  font-size: 16px;  
}

h1 {
  font-family: 'Abril Fatface', serif;
  font-size: 46px;  
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 



Cinzel and Fauna One

Use "Cinzel" font for headings and "Fauna One" for text.



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Cinzel|Fauna+One">
<style>
body {
  font-family: 'Fauna One', serif;
  font-size: 16px;  
}

h1 {
  font-family: Cinzel, serif;
  font-size: 46px;  
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 



Fjalla One and Libre Baskerville


The "Fjalla One" font should be used for headings and "Libre Baskerville" for text.


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Fjalla+One|Libre+Baskerville">
<style>
body {
  font-family: 'Libre Baskerville', serif;
  font-size: 16px;  
}

h1 {
  font-family: 'Fjalla One', sans-serif;
  font-size: 46px;  
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 




Space Mono and Muli

Use "Space Mono" font for headings, and "Muli" for text. See example below:



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Space+Mono|Muli">
<style>
body {
  font-family: Muli, sans-serif;
  font-size: 16px;
}

h1 {
  font-family: "Space Mono", monospace;
  font-size: 46px;
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 



Spectral and Rubik

Use the Spectral font for headings and "Rubik" for text:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Spectral|Rubik">
<style>
body {
  font-family: Rubik, sans-serif;
  font-size: 16px;
}

h1 {
  font-family: Spectral, serif;
  font-size: 46px;
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 





Oswald and Noto Sans

Use the "Oswald" font for headings and "Noto Sans" for text. See an example below:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Oswald|Noto+Sans">
<style>
body {
  font-family: "Noto Sans", sans-serif;
  font-size: 16px;
}

h1 {
  font-family: Oswald, sans-serif;
  font-size: 46px;
}
</style>
</head>
<body>

<h1>Beautiful Norway</h1>

<p>Norway has a total area of 385,252 square kilometers and a population of 5,438,657 (December 2020). 

Norway is bordered by Sweden, Finland and Russia to the north-east, and the Skagerrak to the south, with 

Denmark on the other side.</p>

<p>Norway has beautiful mountains, glaciers and stunning fjords. Oslo, the capital, is a city of green 

spaces and museums. Bergen, with colorful wooden houses, is the starting point for cruises to the dramatic 

Sognefjord. Norway is also known for fishing, hiking and skiing.</p>

</body>
</html> 




CSS Font Property::


To shorten the code, it is also possible to specify all the individual font properties in one property.

The font property is a shorthand property for:

    font-style
    font-variant
    font-weight
    font-size/line-height
    font-family

See an example of this application below:

<!DOCTYPE html>
<html>
<head>
<style>
p.a {
  font: 20px Arial, sans-serif;
}

p.b {
  font: italic bold 12px/30px Georgia, serif;
}
</style>
</head>
<body>

<h1>The font Property</h1>

<p class="a">This is a paragraph. The font size is set to 20 pixels, and the font family is Arial.</p>

<p class="b">This is a paragraph. The font is set to italic and bold, the font size is set to 12 pixels, the 

line height is set to 30 pixels, and the font family is Georgia.</p>

</body>
</html>


Note: The font-size and font-family values are required. If one of the other values is missing, their 

default value are used.




CSS Icons

There is an icon library in CSS that facilitates the addition of icons to an HTML page. 


How to Add Icons

Icon can be simply added to an HTML page with an icon library like Font Awesome. You simply add the name of 

the specified icon class to any inline HTML element (like <i> or <span>). The resulting icons are scalable 

vectors that you can customize using the CSS styling tools to change the size, color, shadow, etc of such 

icons.

 

Font Awesome Icons

Go to fontawesome.com and sign in. The code needed to be added to the <head> section of the HTML page can be 

obtained on this website as shown below:

<script src="https://kit.fontawesome.com/yourcode.js" crossorigin="anonymous"></script>


To learn more about how to get started in font-awesome, check here: 

https://www.w3schools.com/icons/fontawesome5_intro.asp

YOu do not need any downloading or installation to use font awesome


A full list of references of all icons available in font awesome can be see here: 

https://www.w3schools.com/icons/icons_reference.asp


An example of implementation of font awesome is shown below:


<!DOCTYPE html>
<html>
<head>
<title>Font Awesome Icons</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
<!--Get your own code at fontawesome.com-->
</head>
<body>

<p>Some Font Awesome icons:</p>
<i class="fas fa-cloud"></i>
<i class="fas fa-heart"></i>
<i class="fas fa-car"></i>
<i class="fas fa-file"></i>
<i class="fas fa-bars"></i>

<p>Styled Font Awesome icons (size and color):</p>
<i class="fas fa-cloud" style="font-size:24px;"></i>
<i class="fas fa-cloud" style="font-size:36px;"></i>
<i class="fas fa-cloud" style="font-size:48px;color:red;"></i>
<i class="fas fa-cloud" style="font-size:60px;color:lightblue;"></i>

</body>
</html>




Bootstrap Icons

To use the Bootstrap glyphicons, add the following line inside the <head> section of your HTML page:

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">

Note: No downloading or installation is required!


See example of the implementation of Boostrap icon below:

<!DOCTYPE html>
<html>
<head>
<title>Bootstrap Icons</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
</head>
<body class="container">

<p>Some Bootstrap icons:</p>
<i class="glyphicon glyphicon-cloud"></i>
<i class="glyphicon glyphicon-remove"></i>
<i class="glyphicon glyphicon-user"></i>
<i class="glyphicon glyphicon-envelope"></i>
<i class="glyphicon glyphicon-thumbs-up"></i>
<br><br>

<p>Styled Bootstrap icons (size and color):</p>
<i class="glyphicon glyphicon-cloud" style="font-size:24px;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:36px;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:48px;color:red;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:60px;color:lightblue;"></i>

</body>
</html>



Google Icons

To use the Google icons, add the following line inside the <head> section of your HTML page:

<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">

Note: No downloading or installation is required!

See the example of the implementation of google icon below:



<!DOCTYPE html>
<html>
<head>
<title>Google Icons</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
</head>
<body>

<p>Some Google icons:</p>
<i class="material-icons">cloud</i>
<i class="material-icons">favorite</i>
<i class="material-icons">attachment</i>
<i class="material-icons">computer</i>
<i class="material-icons">traffic</i>
<br><br>

<p>Styled Google icons (size and color):</p>
<i class="material-icons" style="font-size:24px;">cloud</i>
<i class="material-icons" style="font-size:36px;">cloud</i>
<i class="material-icons" style="font-size:48px;color:red;">cloud</i>
<i class="material-icons" style="font-size:60px;color:lightblue;">cloud</i>

</body>
</html>




CSS Links


There are multiple ways of styling links using CSS and with the aid of CSS color, font-family, and 

background properties. See example below:


<!DOCTYPE html>
<html>
<head>
<style>
a {
  color: hotpink;
}
</style>
</head>
<body>

<h2>CSS Links</h2>
<p><b><a href="default.asp" target="_blank">This is a link</a></b></p>

</body>
</html>



In addition, links can be styled differently depending on what state they are in.

The four links states are:

    a:link - a normal, unvisited link
    a:visited - a link the user has visited
    a:hover - a link when the user mouses over it
    a:active - a link the moment it is clicked


When setting the style for several link states, there are some order rules:

    a:hover MUST come after a:link and a:visited
    a:active MUST come after a:hover



<!DOCTYPE html>
<html>
<head>
<style>
/* unvisited link */
a:link {
  color: red;
}

/* visited link */
a:visited {
  color: green;
}

/* mouse over link */
a:hover {
  color: hotpink;
}

/* selected link */
a:active {
  color: blue;
}
</style>
</head>
<body>

<h2>CSS Links</h2>
<p><b><a href="default.asp" target="_blank">This is a link</a></b></p>
<p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be 

effective.</p>
<p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>

</body>
</html>



Text Decoration:::
This is mostly used to remove underlines from links. See example below:

<!DOCTYPE html>
<html>
<head>
<style>
a:link {
  text-decoration: none;
}

a:visited {
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

a:active {
  text-decoration: underline;
}
</style>
</head>
<body>

<h2>CSS Links</h2>
<p><b><a href="default.asp" target="_blank">This is a link</a></b></p>
<p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be 

effective.</p>
<p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>

</body>
</html>




Background Color:::

The background-color property can be used to specify a background color for links:

<!DOCTYPE html>
<html>
<head>
<style>
a:link {
  background-color: yellow;
}

a:visited {
  background-color: cyan;
}

a:hover {
  background-color: lightgreen;
}

a:active {
  background-color: hotpink;
} 
</style>
</head>
<body>

<h2>CSS Links</h2>
<p><b><a href="default.asp" target="_blank">This is a link</a></b></p>
<p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be 

effective.</p>
<p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>

</body>
</html>



Link Buttons:::

The examples below are more advanced as they combine different CSS properties to display links as  boxes/ 

buttons. See  example below:


<!DOCTYPE html>
<html>
<head>
<style>
a:link, a:visited {
  background-color: #f44336;
  color: white;
  padding: 14px 25px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
}

a:hover, a:active {
  background-color: red;
}
</style>
</head>
<body>

<h2>Link Button</h2>
<p>A link styled as a button:</p>
<a href="default.asp" target="_blank">This is a link</a>

</body>
</html>


Other examples of styling CSS links

<!DOCTYPE html>
<html>
<head>
<style>
a.one:link {color:#ff0000;}
a.one:visited {color:#0000ff;}
a.one:hover {color:#ffcc00;}

a.two:link {color:#ff0000;}
a.two:visited {color:#0000ff;}
a.two:hover {font-size:150%;}

a.three:link {color:#ff0000;}
a.three:visited {color:#0000ff;}
a.three:hover {background:#66ff66;}

a.four:link {color:#ff0000;}
a.four:visited {color:#0000ff;}
a.four:hover {font-family:monospace;}

a.five:link {color:#ff0000;text-decoration:none;}
a.five:visited {color:#0000ff;text-decoration:none;}
a.five:hover {text-decoration:underline;}
</style>
</head>
<body>

<p>Mouse over the links and watch them change layout:</p>

<p><b><a class="one" href="default.asp" target="_blank">This link changes color</a></b></p>
<p><b><a class="two" href="default.asp" target="_blank">This link changes font-size</a></b></p>
<p><b><a class="three" href="default.asp" target="_blank">This link changes background-color</a></b></p>
<p><b><a class="four" href="default.asp" target="_blank">This link changes font-family</a></b></p>
<p><b><a class="five" href="default.asp" target="_blank">This link changes text-decoration</a></b></p>

</body>
</html>


Another example

<!DOCTYPE html>
<html>
<head>
<style>
a:link, a:visited {
  background-color: white;
  color: black;
  border: 2px solid green;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
}

a:hover, a:active {
  background-color: green;
  color: white;
}
</style>
</head>
<body>

<a href="default.asp" target="_blank">This is a link</a>

</body>
</html>





Different types of cursors that can be used for links

<!DOCTYPE html>
<html>
<body>

<p>Mouse over the words to change the cursor.</p>
<span style="cursor:auto">auto</span><br>
<span style="cursor:crosshair">crosshair</span><br>
<span style="cursor:default">default</span><br>
<span style="cursor:e-resize">e-resize</span><br>
<span style="cursor:help">help</span><br>
<span style="cursor:move">move</span><br>
<span style="cursor:n-resize">n-resize</span><br>
<span style="cursor:ne-resize">ne-resize</span><br>
<span style="cursor:nw-resize">nw-resize</span><br>
<span style="cursor:pointer">pointer</span><br>
<span style="cursor:progress">progress</span><br>
<span style="cursor:s-resize">s-resize</span><br>
<span style="cursor:se-resize">se-resize</span><br>
<span style="cursor:sw-resize">sw-resize</span><br>
<span style="cursor:text">text</span><br>
<span style="cursor:w-resize">w-resize</span><br>
<span style="cursor:wait">wait</span><br>

</body>
</html>






CSS Lists

HTML Lists and CSS List properties


The unordered lists (<ul>) and ordered (<ol>) lists are the two main types of lists in HTML. Unordered lists 

are marked with bullets while ordered lists are marked with numbers or letters.


The CSS list properties allow you to:

    Set different list item markers for ordered lists
    Set different list item markers for unordered lists
    Set an image as the list item marker
    Add background colors to lists and list items



Different List Item Markers

The list-style-type property is used to specify the type of list item marker used. For example,

<!DOCTYPE html>
<html>
<head>
<style>
ul.a {
  list-style-type: circle;
}

ul.b {
  list-style-type: square;
}

ol.c {
  list-style-type: upper-roman;
}

ol.d {
  list-style-type: lower-alpha;
}
</style>
</head>
<body>

<h2>Lists</h2>
<p>Example of unordered lists:</p>
<ul class="a">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

<ul class="b">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

<p>Example of ordered lists:</p>
<ol class="c">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="d">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

</body>
</html>


Note: Some of the values are for unordered lists, and some for ordered lists.



An Image as the List Item Marker

The list-style-image property is used to spedify image as an item list marker. For instance,


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-image: url('sqpurple.gif');
}
</style>
</head>
<body>

<h2>CSS Lists</h2>
<p>The list-style-image property specifies an image as the list item marker:</p>

<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

</body>
</html>



Position the List Item Markers

The position of the list-item markers (bullet points) is specified using list-style-position. 


"list-style-position: outside;" means that the bullet points will be outside the list item. The start of 

each line of a list item will be aligned vertically. This is default:


"list-style-position: inside;" means that the bullet points will be inside the list item. As it is part of 

the list item, it will be part of the text and push the text at the start:



<!DOCTYPE html>
<html>
<head>
<style>
ul.a {
  list-style-position: outside;
}

ul.b {
  list-style-position: inside;
}
</style>
</head>
<body>

<h1>The list-style-position Property</h1>

<h2>list-style-position: outside (default):</h2>
<ul class="a">
  <li>Coffee - A brewed drink prepared from roasted coffee beans, which are the seeds of berries from the 

Coffea plant</li>
  <li>Tea - An aromatic beverage commonly prepared by pouring hot or boiling water over cured leaves of the 

Camellia sinensis, an evergreen shrub (bush) native to Asia</li>
  <li>Coca Cola - A carbonated soft drink produced by The Coca-Cola Company. The drink's name refers to two 

of its original ingredients, which were kola nuts (a source of caffeine) and coca leaves</li>
</ul>

<h2>list-style-position: inside:</h2>
<ul class="b">
  <li>Coffee - A brewed drink prepared from roasted coffee beans, which are the seeds of berries from the 

Coffea plant</li>
  <li>Tea - An aromatic beverage commonly prepared by pouring hot or boiling water over cured leaves of the 

Camellia sinensis, an evergreen shrub (bush) native to Asia</li>
  <li>Coca Cola - A carbonated soft drink produced by The Coca-Cola Company. The drink's name refers to two 

of its original ingredients, which were kola nuts (a source of caffeine) and coca leaves</li>
</ul>

</body>
</html>




NB: Align outside is the default for list-style position and in this case, the first letter in the second 

line of each bullet content is directly under the first letter in the first line. However, when the list-

style-position is set to inside, the First letter of the second line in a list item is directly under the 

bullet symbol in the first line.   



Remove Default Settings

The list-style-type:none property can also be used to remove the markers/bullets. Note that the list also 

has default margin and padding. To remove this, add margin:0 and padding:0 to <ul> or <ol>:

<!DOCTYPE html>
<html>
<head>
<style>
ul.demo {
  list-style-type: none;
  margin: 0;
  padding: 0;
}
</style>
</head>
<body>

<p>Default list:</p>
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

<p>Remove bullets, margin and padding:</p>
<ul class="demo">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

</body>
</html>



List - Shorthand property

The list-style property is a shorthand property. It is used to set all the list properties in one 

declaration:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style: square inside url("sqpurple.gif");
}
</style>
</head>
<body>

<h2>CSS Lists</h2>
<p>The list-style property is a shorthand property, which is used to set all the list properties in one 

declaration.</p>

<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

</body>
</html>



When using the shorthand property, the order of the property values are:

1. list-style-type (if a list-style-image is specified, the value of this property will be displayed if the 

image for some reason cannot be displayed)
2. list-style-position (specifies whether the list-item markers should appear inside or outside the content 

flow)
3. list-style-image (specifies an image as the list item marker)

If one of the property values above are missing, the default value for the missing property will be 

inserted, if any.


Styling List With Colors

We can also style lists with colors, to make them look a little more interesting.

Anything added to the <ol> or <ul> tag, affects the entire list, while properties added to the <li> tag will 

affect the individual list items:



<!DOCTYPE html>
<html>
<head>
<style>
ol {
  background: #ff9999;
  padding: 20px;
}

ul {
  background: #3399ff;
  padding: 20px;
}

ol li {
  background: #ffe5e5;
  padding: 5px;
  margin-left: 35px;
}

ul li {
  background: #cce5ff;
  margin: 5px;
}
</style>
</head>
<body>

<h1>Styling Lists With Colors:</h1>

<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

</body>
</html>



More examples:

Customized list with a red left border:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  border-left: 5px solid red;
  background-color: #f1f1f1;
  list-style-type: none;
  padding: 10px 20px;
}
</style>
</head>
<body>

<p>List with a red left border:</p>
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

</body>
</html>


Full width bordered list:

<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  padding: 0;
  border: 1px solid #ddd;
}

ul li {
  padding: 8px 16px;
  border-bottom: 1px solid #ddd;
}

ul li:last-child {
  border-bottom: none
}
</style>
</head>
<body>

<p>Full-width bordered list:</p>
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

</body>
</html>



All the different list-item markers for lists:


<!DOCTYPE html>
<html>
<head>
<style>
ul.a {list-style-type: circle;}
ul.b {list-style-type: disc;}
ul.c {list-style-type: square;}

ol.d {list-style-type: armenian;}
ol.e {list-style-type: cjk-ideographic;}
ol.f {list-style-type: decimal;}
ol.g {list-style-type: decimal-leading-zero;}
ol.h {list-style-type: georgian;}
ol.i {list-style-type: hebrew;}
ol.j {list-style-type: hiragana;}
ol.k {list-style-type: hiragana-iroha;}
ol.l {list-style-type: katakana;}
ol.m {list-style-type: katakana-iroha;}
ol.n {list-style-type: lower-alpha;}
ol.o {list-style-type: lower-greek;}
ol.p {list-style-type: lower-latin;}
ol.q {list-style-type: lower-roman;}
ol.r {list-style-type: upper-alpha;}
ol.s {list-style-type: upper-latin;}
ol.t {list-style-type: upper-roman;}
ol.u {list-style-type: none;}
ol.v {list-style-type: inherit;}
</style>
</head>
<body>

<ul class="a">
  <li>Circle type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

<ul class="b">
  <li>Disc type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

<ul class="c">
  <li>Square type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ul>

<ol class="d">
  <li>Armenian type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="e">
  <li>Cjk-ideographic type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="f">
  <li>Decimal type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="g">
  <li>Decimal-leading-zero type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="h">
  <li>Georgian type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="i">
  <li>Hebrew type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="j">
  <li>Hiragana type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="k">
  <li>Hiragana-iroha type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="l">
  <li>Katakana type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="m">
  <li>Katakana-iroha type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="n">
  <li>Lower-alpha type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="o">
  <li>Lower-greek type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="p">
  <li>Lower-latin type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="q">
  <li>Lower-roman type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="r">
  <li>Upper-alpha type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="s">
  <li>Upper-latin type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="t">
  <li>Upper-roman type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="u">
  <li>None type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

<ol class="v">
  <li>inherit type</li>
  <li>Tea</li>
  <li>Coca Cola</li>
</ol>

</body>
</html>





CSS Tables

CSS helps to improve the appearance of HTML tables


An example of table is shown below:

<!DOCTYPE html>
<html>
<head>
<style>
#customers {
  font-family: Arial, Helvetica, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

#customers td, #customers th {
  border: 1px solid #ddd;
  padding: 8px;
}

#customers tr:nth-child(even){background-color: #f2f2f2;}

#customers tr:hover {background-color: #ddd;}

#customers th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: left;
  background-color: #04AA6D;
  color: white;
}
</style>
</head>
<body>

<table id="customers">
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Berglunds snabbköp</td>
    <td>Christina Berglund</td>
    <td>Sweden</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
  <tr>
    <td>Ernst Handel</td>
    <td>Roland Mendel</td>
    <td>Austria</td>
  </tr>
  <tr>
    <td>Island Trading</td>
    <td>Helen Bennett</td>
    <td>UK</td>
  </tr>
  <tr>
    <td>Königlich Essen</td>
    <td>Philip Cramer</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Laughing Bacchus Winecellars</td>
    <td>Yoshi Tannamuri</td>
    <td>Canada</td>
  </tr>
  <tr>
    <td>Magazzini Alimentari Riuniti</td>
    <td>Giovanni Rovelli</td>
    <td>Italy</td>
  </tr>
  <tr>
    <td>North/South</td>
    <td>Simon Crowther</td>
    <td>UK</td>
  </tr>
  <tr>
    <td>Paris spécialités</td>
    <td>Marie Bertrand</td>
    <td>France</td>
  </tr>
</table>

</body>
</html>




Table Borders


Table Borders

To specify table borders in CSS, use the border property.

The example below specifies a black border for <table>, <th>, and <td> elements:


<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
}
</style>
</head>
<body>

<h2>Add a border to a table:</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
  </tr>
</table>

</body>
</html>



Full-Width Table:


If you wish to create a table that will span the entire screen (full-width), add width:100% to the <table>
 elemnt as shown below:



<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
}

table {
  width: 100%;
}
</style>
</head>
<body>

<h2>Full-width Table</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
  </tr>
</table>

</body>
</html>




Double Borders

Notice that the table in the examples above have double borders. This is because both the table and the <th> 

and <td> elements have separate borders.

To remove double borders, take a look at the example below.




<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  width: 100%;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Let the borders collapse</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
  </tr>
</table>

</body>
</html>



To create a table with just border around the table, only specify border property for <table> 


<!DOCTYPE html>
<html>
<head>
<style>
table {
  width: 100%;
  border-collapse: collapse;
  border: 1px solid black;
}
</style>
</head>
<body>

<h2>Single Border Around The Table</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
  </tr>
</table>

</body>
</html>



Table Size

Table Width and Height

The width and height of a table are defined by the width and height properties.

The example below sets the width of the table to 100%, and the height of the <th> elements to 70px:



<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  border-collapse: collapse;
  width: 100%;
}

th {
  height: 70px;
}
</style>
</head>
<body>

<h2>The width and height Properties</h2>
<p>Set the width of the table, and the height of the table header row:</p>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>



To create a table that should only span half of the page, use the width:50% specification.  See illustration 

below:


<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  border-collapse: collapse;
  width: 50%;
}

th {
  height: 70px;
}
</style>
</head>
<body>

<h2>The width and height Properties</h2>
<p>Set the width of the table, and the height of the table header row:</p>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>


CSS Table Alignment::

Horizontal Alignment

The text-align property sets the horizontal alignment (like left, right, or center) of the content in <th> 

or <td>.

By default, the content of <th> elements are center-aligned and the content of <td> elements are left-

aligned.

To center-align the content of  <td> elements as well, use text-align: center:



<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  border-collapse: collapse;
  width: 100%;
}

td {
  text-align: center;
}
</style>
</head>
<body>

<h2>The text-align Property</h2>
<p>This property sets the horizontal alignment (like left, right, or center) of the content in th or td.</p>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>



To left-align the content, force the alignment of <th> elements to be left-aligned, with the text-align: 

left property:


<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  border-collapse: collapse;
  width: 100%;
}

th {
  text-align: left;
}
</style>
</head>
<body>

<h2>The text-align Property</h2>
<p>This property sets the horizontal alignment (like left, right, or center) of the content in th or td.</p>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>



Vertical Alignment


The vertical-align property sets the vertical alignment (like top, bottom, or middle) of the content in <th> 

or <td>. By default, the vertical alignment of the content in a table is middle (for both <th> and <td> 

elements).

The following example sets the vertical text alignment to bottom for <td> elements:

<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  border-collapse: collapse;
  width: 100%;
}

td {
  height: 50px;
  vertical-align: bottom;
}
</style>
</head>
<body>

<h2>The vertical-align Property</h2>
<p>This property sets the vertical alignment (like top, bottom, or middle) of the content in th or td.</p>
<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>


CSS Table Style

Table Padding

To control the space between the border and the content in a table, use the padding property on <td> and 

<th> elements:

<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {  
  border: 1px solid #ddd;
  text-align: left;
}

table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  padding: 15px;
}
</style>
</head>
<body>

<h2>The padding Property</h2>
<p>This property adds space between the border and the content in a table.</p>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>



Horizontal Dividers

Add the border-bottom property to <th> and <td> for horizontal dividers:


<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  padding: 8px;
  text-align: left;
  border-bottom: 1px solid #ddd;
}
</style>
</head>
<body>

<h2>Bordered Table Dividers</h2>
<p>Add the border-bottom property to th and td for horizontal dividers:</p>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>





Hoverable Table

Use the :hover selector on <tr> to highlight table rows on mouse over:



<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  padding: 8px;
  text-align: left;
  border-bottom: 1px solid #ddd;
}

tr:hover {background-color: yellow;}
</style>
</head>
<body>

<h2>Hoverable Table</h2>
<p>Move the mouse over the table rows to see the effect.</p>

<table>
  <tr>
    <th>First Name</th>
    <th>Last Name</th>
    <th>Points</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
  </tr>
</table>

</body>
</html>



Striped Tables

For zebra-striped tables, use the nth-child() selector and add a background-color to all even (or odd) table 

rows:

first row is the heading (odd beginning with <th>)



<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {background-color: #f2f2f2;}
</style>
</head>
<body>

<h2>Striped Table</h2>
<p>For zebra-striped tables, use the nth-child() selector and add a background-color to all even (or odd) 

table rows:</p>

<table>
  <tr>
  <th>First Name</th>
  <th>Last Name</th>
  <th>Points</th>
  </tr>
  <tr>
  <td>Peter</td>
  <td>Griffin</td>
  <td>$100</td>
  </tr>
  <tr>
  <td>Lois</td>
  <td>Griffin</td>
  <td>$150</td>
  </tr>
  <tr>
  <td>Joe</td>
  <td>Swanson</td>
  <td>$300</td>
  </tr>
  <tr>
  <td>Cleveland</td>
  <td>Brown</td>
  <td>$250</td>
  </tr>
</table>

</body>
</html>




Table Color

The example below specifies the background color and text color of <th> elements:

<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  text-align: left;
  padding: 8px;
}

tr:nth-child(even){background-color: #f2f2f2}

th {
  background-color: #04AA6D;
  color: white;
}
</style>
</head>
<body>

<h2>Colored Table Header</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Griffin</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>Lois</td>
    <td>Griffin</td>
    <td>$150</td>
  </tr>
  <tr>
    <td>Joe</td>
    <td>Swanson</td>
    <td>$300</td>
  </tr>
  <tr>
    <td>Cleveland</td>
    <td>Brown</td>
    <td>$250</td>
</tr>
</table>

</body>
</html>




CSS Responsive Table

Responsive Table

A responsive table will display a horizontal scroll bar if the screen is too small to display the full 

content:

Add a container element (like <div>) with overflow-x:auto around the <table> element to make it responsive:


Note: In OS X Lion (on Mac), scrollbars are hidden by default and only shown when being used (even though 

"overflow:scroll" is set).

<!DOCTYPE html>
<html>
<head>
<style>
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {background-color: #f2f2f2;}
</style>
</head>
<body>

<h2>Responsive Table</h2>
<p>A responsive table will display a horizontal scroll bar if the screen is too 
small to display the full content. Resize the browser window to see the effect:</p>
<p>To create a responsive table, add a container element (like div) with <strong>overflow-x:auto</strong> 

around the table element:</p>

<div style="overflow-x:auto;">
  <table>
    <tr>
      <th>First Name</th>
      <th>Last Name</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
      <th>Points</th>
    </tr>
    <tr>
      <td>Jill</td>
      <td>Smith</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
      <td>50</td>
    </tr>
    <tr>
      <td>Eve</td>
      <td>Jackson</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
      <td>94</td>
    </tr>
    <tr>
      <td>Adam</td>
      <td>Johnson</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
      <td>67</td>
    </tr>
  </table>
</div>

</body>
</html>



More table examples:


To make a fancy table


<!DOCTYPE html>
<html>
<head>
<style>
#customers {
  font-family: Arial, Helvetica, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

#customers td, #customers th {
  border: 1px solid #ddd;
  padding: 8px;
}

#customers tr:nth-child(even){background-color: #f2f2f2;}

#customers tr:hover {background-color: #ddd;}

#customers th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: left;
  background-color: #04AA6D;
  color: white;
}
</style>
</head>
<body>

<table id="customers">
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Berglunds snabbköp</td>
    <td>Christina Berglund</td>
    <td>Sweden</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
  <tr>
    <td>Ernst Handel</td>
    <td>Roland Mendel</td>
    <td>Austria</td>
  </tr>
  <tr>
    <td>Island Trading</td>
    <td>Helen Bennett</td>
    <td>UK</td>
  </tr>
  <tr>
    <td>Königlich Essen</td>
    <td>Philip Cramer</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Laughing Bacchus Winecellars</td>
    <td>Yoshi Tannamuri</td>
    <td>Canada</td>
  </tr>
  <tr>
    <td>Magazzini Alimentari Riuniti</td>
    <td>Giovanni Rovelli</td>
    <td>Italy</td>
  </tr>
  <tr>
    <td>North/South</td>
    <td>Simon Crowther</td>
    <td>UK</td>
  </tr>
  <tr>
    <td>Paris spécialités</td>
    <td>Marie Bertrand</td>
    <td>France</td>
  </tr>
</table>

</body>
</html>




To set the position of table caption

<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

caption {
  caption-side: bottom;
}
</style>
</head>
<body>

<table>
<caption>Table 1.1 Customers</caption>
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr class="alt">
    <td>Berglunds snabbköp</td>
    <td>Christina Berglund</td>
    <td>Sweden</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
  <tr class="alt">
    <td>Ernst Handel</td>
    <td>Roland Mendel</td>
    <td>Austria</td>
  </tr>
  <tr>
    <td>Island Trading</td>
    <td>Helen Bennett</td>
    <td>UK</td>
  </tr>
</table>

</body>
</html>




CSS Display

CSS Layout - The display Property

The most important CSS property for controlling layout is the  'display' property, and it states how an 

element is to be displayed. The default display value for most HTML elements is block or inline


Block-level Elements


A block-level element always starts on a new line and takes up the full width available (stretches out to 

the left and right as far as it can).
The <div> element is a block-level element.

Examples of block-level elements:

    <div>
    <h1> - <h6>
    <p>
    <form>
    <header>
    <footer>
    <section>


Inline Elements

Inline Elements

An inline element does not start on a new line and only takes up as much width as necessary.

This is an inline <span> element inside a paragraph.

Examples of inline elements:

    <span>
    <a>
    <img>


Display: none;

display: none; is commonly used with JavaScript to hide and show elements without deleting and recreating 

them. Take a look at our last example on this page if you want to know how this can be achieved.

The <script> element uses display: none; as default. 






Override The Default Display Value
To override the default display value of every element, simply change an inline element to a block element 

or vice versa. This also allows you to make the page the way you like while complying with the web 

standards. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
li {
  display: inline;
}
</style>
</head>
<body>

<p>Display a list of links as a horizontal menu:</p>

<ul>
  <li><a href="/html/default.asp" target="_blank">HTML</a></li>
  <li><a href="/css/default.asp" target="_blank">CSS</a></li>
  <li><a href="/js/default.asp" target="_blank">JavaScript</a></li>
</ul>

</body>
</html>


Note: Setting the display property of an element only changes how the element is displayed, NOT what kind of 

element it is. So, an inline element with display: block; is not allowed to have other block elements inside 

it.


To display <span> elements as block elements:


<!DOCTYPE html>
<html>
<head>
<style>
span {
  display: block;
}
</style>
</head>
<body>

<span>A display property with a value of "block" results in</span> <span>a line break between the two 

elements.</span>

</body>
</html>



The following example displays <a> elements as block elements:


<!DOCTYPE html>
<html>
<head>
<style>
a {
  display: block;
}
</style>
</head>
<body>

<p>Display links as block elements:</p>

<a href="/html/default.asp" target="_blank">HTML</a>
<a href="/css/default.asp" target="_blank">CSS</a>
<a href="/js/default.asp" target="_blank">JavaScript</a>

</body>
</html>



Hide an Element - display:none or visibility:hidden?

Setting the display property to none enables an element to be hidden and display the page as if the element 

is not there. See example below:


<!DOCTYPE html>
<html>
<head>
<style>
h1.hidden {
  display: none;
}
</style>
</head>
<body>

<h1>This is a visible heading</h1>
<h1 class="hidden">This is a hidden heading</h1>
<p>Notice that the h1 element with display: none; does not take up any space.</p>

</body>
</html>





Setting visibility:hidden; also hides an element. However, the element will still take up the same space as 

before. The element will be hidden, but still affect the layout: 


<!DOCTYPE html>
<html>
<head>
<style>
h1.hidden {
  visibility: hidden;
}
</style>
</head>
<body>

<h1>This is a visible heading</h1>
<h1 class="hidden">This is a hidden heading</h1>
<p>Notice that the hidden heading still takes up space.</p>

</body>
</html>


Additional Examples:

The differences between display:none; and visibility:hidden; is shown in the example below. 

visibility:hidden hides the element, but it still takes up space in the layout.

display:none removes the element from the document. It does not take up any space.


<!DOCTYPE html>
<html>
<head>
<style>
.imgbox {
  float: left;
  text-align: center;
  width: 120px;
  border: 1px solid gray;
  margin: 4px;
  padding: 6px;
}

button {
  width: 100%;
}
</style>
</head>
<body>

<h3>Difference between display:none and visiblity: hidden</h3>
<p><strong>visibility:hidden</strong> hides the element, but it still takes up space in the layout.</p>
<p><strong>display:none</strong> removes the element from the document. It does not take up any space.</p>

<div class="imgbox" id="imgbox1">Box 1<br>
  <img src="img_5terre.jpg" alt="Italy" style="width:100%">
  <button onclick="removeElement()">Remove</button>
</div>

<div class="imgbox" id="imgbox2">Box 2<br>
  <img src="img_lights.jpg" alt="Lights" style="width:100%">
  <button onclick="changeVisibility()">Hide</button>
</div>

<div class="imgbox">Box 3<br>
  <img src="img_forest.jpg" alt="Forest" style="width:100%">
  <button onclick="resetElement()">Reset All</button>
</div>

<script>
function removeElement() {
  document.getElementById("imgbox1").style.display = "none";
}

function changeVisibility() {
  document.getElementById("imgbox2").style.visibility = "hidden";
}

function resetElement() {
  document.getElementById("imgbox1").style.display = "block";
  document.getElementById("imgbox2").style.visibility = "visible";
}
</script>

</body>
</html>



CSS can also be used together with Javascript to show an element on click as shown below:

CSS Display/Visibility Properties
Property 	Description
display 	Specifies how an element should be displayed
visibility 	Specifies whether or not an element should be visible


CSS Layout - width and max-width

Using width, max-width and margin: auto;

Since block-level element takes up the whole available width, you can limit that stretching of the block-

level element by setting the 'width'. Then, you can set the margins to auto, to horizontally center the 

element within its container. The element will take up the specified width, and the remaining space will be 

split equally between the two margins:

Using max-width prevents the introduction of horizontal scroll bars in situations where smaller devices with 

screen smaller than the specified width is used to acces the website.

Tip: In the example below: resize the browser window to less than 500px wide, to see the difference between 

the two divs!


<!DOCTYPE html>
<html>
<head>
<style>
div.ex1 {
  width: 500px;
  margin: auto;
  border: 3px solid #73AD21;
}

div.ex2 {
  max-width: 500px;
  margin: auto;
  border: 3px solid #73AD21;
}
</style>
</head>
<body>

<h2>CSS Max-width</h2>

<div class="ex1">This div element has width: 500px;</div>
<br>

<div class="ex2">This div element has max-width: 500px;</div>

<p><strong>Tip:</strong> Drag the browser window to smaller than 500px wide, to see the difference between 
the two divs!</p>

</body>
</html>

 




CSS Position

CSS Layout - The position Property

The position property is used to specify whether the positioning of an element is static, relative, fixed, 

absolute, or sticky. The elements are then positioned using top, bottom, left, and right properties (these 

properties only work after position property is first set). These properties work differently depending on 

the CSS position set.



position: static;  ::

Static position is the default for all html elements. Static positioned element are not affected by top 

bottom, left, and right properties. They are not positioned in a special way but rather follow the normal 

flow of the page. See the illustration of the usage of position;static; below. 

<!DOCTYPE html>
<html>
<head>
<style>
div.static {
  position: static;
  border: 3px solid #73AD21;
}
</style>
</head>
<body>

<h2>position: static;</h2>

<p>An element with position: static; is not positioned in any special way; it is 
always positioned according to the normal flow of the page:</p>

<div class="static">
  This div element has position: static;
</div>

</body>
</html>




position:relative;  ::

The relative position property enables an element to be positioned relative to its normal position. Settng 

the top,right, bottom, and left properties of an element with position: relative; adjusts such element from 

its normal position. The rest of the contents do not occupy any gap left by the element. See an illustration 

below:


<!DOCTYPE html>
<html>
<head>
<style>
div.relative {
  position: relative;
  left: 30px;
  border: 3px solid #73AD21;
}
</style>
</head>
<body>

<h2>position: relative;</h2>

<p>An element with position: relative; is positioned relative to its normal position:</p>

<div class="relative">
This div element has position: relative;
</div>

</body>
</html>




NB: left: 30px;  position the element 30px away from its original position (moved to the right by 30px).




position: fixed; ::

This enables an element positioning relative to the viewport; element stays in the same place even if page 

is scrolled. A fixed element does not leave a gap in the page where it would normally have been located.

The top, right, bottom, and left properties are used to position the element.


See example below:


<!DOCTYPE html>
<html>
<head>
<style>
div.fixed {
  position: fixed;
  bottom: 0;
  right: 0;
  width: 300px;
  border: 3px solid #73AD21;
}
</style>
</head>
<body>

<h2>position: fixed;</h2>

<p>An element with position: fixed; is positioned relative to the viewport, which means it always stays in 

the same place even if the page is scrolled:</p>

<div class="fixed">
This div element has position: fixed;
</div>

</body>
</html>

NB: bottom:0; right:0; means that the element is positioned in the right bottom corner exactly without any 

gap between the element borders and the viewport.




position: absolute; ::

An element with position:absolute; is positioned relative to its closest ancestor, rather than position 

relative to the viewport. The absolute positioned element uses the document body as ancestor if it has no 

positioned ancestor, and they move along with page scrolling. See example below:


Note: Absolute positioned elements are removed from the normal flow, and can overlap elements.



<!DOCTYPE html>
<html>
<head>
<style>
div.relative {
  position: relative;
  width: 400px;
  height: 200px;
  border: 3px solid #73AD21;
} 

div.absolute {
  position: absolute;
  top: 80px;
  right: 0;
  width: 200px;
  height: 100px;
  border: 3px solid #73AD21;
}
</style>
</head>
<body>

<h2>position: absolute;</h2>

<p>An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of 

positioned relative to the viewport, like fixed):</p>

<div class="relative">This div element has position: relative;
  <div class="absolute">This div element has position: absolute;</div>
</div>

</body>
</html>



Position: sticky; :::

An element positioned as sticky is positioned relative the the user's position during scrolling. The stick 

element position is toggled between relative and fixed depending on the scroll position. It is positioned 

relative until a given offset position is met in the viewport - then it "sticks" in place (like 

position:fixed). You must also specify top, right, bottom, or left position for sticky position to work. 


To  make the sticky elemnt sticks to the top of the page (top: 0) when you reach its scroll position, see 

how to do it below:


<!DOCTYPE html>
<html>
<head>
<style>
div.sticky {
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  padding: 5px;
  background-color: #cae8ca;
  border: 2px solid #4CAF50;
}
</style>
</head>
<body>

<p>Try to <b>scroll</b> inside this frame to understand how sticky positioning works.</p>

<div class="sticky">I am sticky!</div>

<div style="padding-bottom:2000px">
  <p>In this example, the sticky element sticks to the top of the page (top: 0), when you reach its scroll 

position.</p>
  <p>Scroll back up to remove the stickyness.</p>
  <p>Some text to enable scrolling.. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
  <p>Some text to enable scrolling.. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
</div>

</body>
</html>



Overlapping elements::

The positioned elements can overlap other elements.  The z-index property specifies the order of stacking 

the element (which element should be placed in front of (z is positive) or behind (z is negative) the 

others). The z-index can be positive or negative.

<!DOCTYPE html>
<html>
<head>
<style>
img {
  position: absolute;
  left: 0px;
  top: 0px;
  z-index: -1;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<img src="w3css.gif" width="100" height="140">
<p>Because the image has a z-index of -1, it will be placed behind the text.</p>

</body>
</html>



An element with greater stack order is always in front of an element with a lower stack order.

Note: If two positioned elements overlap without a z-index specified, the element positioned last in the 

HTML code will be shown on top.



Positioning Text In an Image.


Top left:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.topleft {
  position: absolute;
  top: 8px;
  left: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>
<p>Add some text to an image in the top left corner:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="topleft">Top Left</div>
</div>

</body>
</html>


Top right:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.topright {
  position: absolute;
  top: 8px;
  right: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>
<p>Add some text to an image in the top right corner:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="topright">Top Right</div>
</div>

</body>
</html>




Bottom left:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.bottomleft {
  position: absolute;
  bottom: 8px;
  left: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>
<p>Add some text to an image in the bottom left corner:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="bottomleft">Bottom Left</div>
</div>

</body>
</html>



Bottom Right:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.bottomright {
  position: absolute;
  bottom: 8px;
  right: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>
<p>Add some text to an image in the bottom right corner:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="bottomright">Bottom Right</div>
</div>

</body>
</html>




Centered::

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.center {
  position: absolute;
  top: 50%;
  width: 100%;
  text-align: center;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>
<p>Center text in image:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="center">Centered</div>
</div>

</body>
</html>



To set the shape of an element::

<!DOCTYPE html>
<html>
<head>
<style>
img {
  position: absolute;
  clip: rect(0px,60px,200px,0px);
}
</style>
</head>
<body>

<img src="w3css.gif" width="100" height="140">

</body>
</html>




All CSS Positioning Properties
Property 	Description
bottom 	Sets the bottom margin edge for a positioned box
clip 	Clips an absolutely positioned element
left 	Sets the left margin edge for a positioned box
position 	Specifies the type of positioning for an element
right 	Sets the right margin edge for a positioned box
top 	Sets the top margin edge for a positioned box
z-index 	Sets the stack order of an element


NB: position, left:-20px; means that the element is moved 20px left away from its normal position. 



CSS Layout - Overflow

States what happens if text exceed the space provided for it to occcupy.

An illustration of this property is shown below:

<!DOCTYPE html>
<html>
<head>
<style>
#overflowTest {
  background: #4CAF50;
  color: white;
  padding: 15px;
  width: 50%;
  height: 100px;
  overflow: scroll;
  border: 1px solid #ccc;
}
</style>
</head>
<body>

<h2>CSS Overflow</h2>
<p>The overflow property controls what happens to content that is too big to fit into an area.</p>

<div id="overflowTest">This text is really long and the height of its container is only 100 pixels. 

Therefore, a scrollbar is added to help the reader to scroll the content. Lorem ipsum dolor sit amet, 

consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat 

volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut 

aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse 

molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio 

dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam liber 

tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim 

assum. Typi non habent claritatem insitam; est usus legentis in iis qui facit eorum claritatem.</div>

</body>
</html>




CSS Overflow

Specifies whether the introduction of scroll bars or clipping content will occur when content of  an element 

is too big to fit in the specified area.


Properties of overflow property:
visible:This is the default, and ensures that the overflow is not clipped. Content appears outside the 

element's box. 

hidden: clips the overflow, making the remaining content of the element visible
scroll: clips the overflow, adding scrollbars with which the rest of the content of the element would be 

seen. 
auto: Works similar to scroll, just that it adds scroll bars only when necessary. 

NB: Overflow property works for block elements which has specified height. Also,

In OS X Lion (on Mac), scrollbars are hidden by default and only shown when being used (even though 

"overflow:scroll" is set).



overflow: visible;  ::

this is the default value for overflow. It is not clipped and renders outside the element's box. See the 

illustration of overflow: visible below:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: #eee;
  width: 200px;
  height: 50px;
  border: 1px dotted black;
  overflow: visible;
}
</style>
</head>
<body>

<h2>CSS Overflow</h2>
<p>By default, the overflow is visible, meaning that it is not clipped and it renders outside the element's 

box:</p>

<div>You can use the overflow property when you want to have better control of the layout. The overflow 

property specifies what happens if content overflows an element's box.</div>

</body>
</html>


overflow: hidden; ::

The hidden overflow property value is clipped (fits inside the provided box), and the rest of the content is 

hidden. See illustration of overflow: hidden; below:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: #eee;
  width: 200px;
  height: 50px;
  border: 1px dotted black;
  overflow: hidden;
}
</style>
</head>
<body>

<h2>CSS Overflow</h2>
<p>With the hidden value, the overflow is clipped, and the rest of the content is hidden:</p>
<p>Try to remove the overflow property to understand how it works.</p>

<div>You can use the overflow property when you want to have better control of the layout. The overflow 

property specifies what happens if content overflows an element's box.</div>

</body>
</html>



overflow: scroll; ::

When the overflow is set to scroll, such overflow is clipped and a scrollbar is added inside the box. This 

option adds both horizontal and vertical scroll bars, even in circumstances where they are not needed. See 

an illustration of overflow: scroll; below:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: #eee;
  width: 200px;
  height: 100px;
  border: 1px dotted black;
  overflow: scroll;
}
</style>
</head>
<body>

<h2>CSS Overflow</h2>
<p>Setting the overflow value to scroll, the overflow is clipped and a scrollbar is added to scroll inside 

the box. Note that this will add a scrollbar both horizontally and vertically (even if you do not need 

it):</p>

<div>You can use the overflow property when you want to have better control of the layout. The overflow 

property specifies what happens if content overflows an element's box.</div>

</body>
</html>



overflow: auto; ::

The overflow:auto; is similar to scroll, but only add scrollbars only when it is necessary. In essence, it 

resolves issues of useless scrollbars that arise when overflow:scroll; is used. See illustration of 

overflow:auto; below:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: #eee;
  width: 200px;
  height: 50px;
  border: 1px dotted black;
  overflow: auto;
}
</style>
</head>
<body>

<h2>CSS Overflow</h2>
<p>The auto value is similar to scroll, only it add scrollbars when necessary:</p>

<div>You can use the overflow property when you want to have better control of the layout. The overflow 

property specifies what happens if content overflows an element's box.</div>

</body>
</html>



overflow-x and overflow-y; ::

overflow-x and overflow-y property enable setting overflow of content to only horizontal, just vertical, or 

both. This can give similar advantage given by overflow: auto: over overflow:scroll;
See illustration of overflow-x and overflow-y below:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: #eee;
  width: 200px;
  height: 50px;
  border: 1px dotted black;
  overflow-x: hidden;
  overflow-y: scroll;
}
</style>
</head>
<body>

<h2>CSS Overflow</h2>
<p>You can also change the overflow of content horizontally or vertically.</p>
<p>overflow-x specifies what to do with the left/right edges of the content.<br>
overflow-y specifies what to do with the top/bottom edges of the content.</p>

<div>You can use the overflow property when you want to have better control of the layout. The overflow 

property specifies what happens if content overflows an element's box.</div>

</body>
</html>



All CSS Overflow Properties
Property 	Description
overflow 	Specifies what happens if content overflows an element's box
overflow-x 	Specifies what to do with the left/right edges of the content if it overflows the element's 

content area
overflow-y 	Specifies what to do with the top/bottom edges of the content if it overflows the element's 

content area




CSS Layout - float and clear

CSS float property specifies how an element should float
css clear property specifies what elements can float beside the cleared element and on which side.


The float property

Float property is used to position and format content. for example, an image can be float left to the text 

in a container.

possible values of float property:


    left - The element floats to the left of its container
    right - The element floats to the right of its container
    none - The element does not float (will be displayed just where it occurs in the text). This is default
    inherit - The element inherits the float value of its parent


The simplest application of float property is in wrapping text around images. for instance, to implement 

float:right; see example below:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  float: right;
}
</style>
</head>
<body>

<h2>Float Right</h2>

<p>In this example, the image will float to the right in the paragraph, and the text in the paragraph will 

wrap around the image.</p>

<p><img src="pineapple.jpg" alt="Pineapple" style="width:170px;height:170px;margin-left:15px;">
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi 

lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue 

eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Mauris ante ligula, facilisis sed ornare 

eu, lobortis in odio. Praesent convallis urna a lacus interdum ut hendrerit risus congue. Nunc sagittis 

dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare 

turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed 

dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.</p>

</body>
</html>


To float an image to the left in a text (inside a container), see implementation below:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  float: left;
}
</style>
</head>
<body>

<h2>Float Left</h2>

<p>In this example, the image will float to the left in the paragraph, and the text in the paragraph will 

wrap around the image.</p>

<p><img src="pineapple.jpg" alt="Pineapple" style="width:170px;height:170px;margin-right:15px;">
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi 

lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue 

eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Mauris ante ligula, facilisis sed ornare 

eu, lobortis in odio. Praesent convallis urna a lacus interdum ut hendrerit risus congue. Nunc sagittis 

dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare 

turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed 

dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.</p>

</body>
</html>


No float- float:none; 

Displays an image exactly where it occurs in a text. See illustration below:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  float: none;
}
</style>
</head>
<body>

<h2>Float None</h2>

<p>In this example, the image will be displayed just where it occurs in the text (float: none;).</p>

<p><img src="pineapple.jpg" alt="Pineapple" style="width:170px;height:170px;">
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi 

lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue 

eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Mauris ante ligula, facilisis sed ornare 

eu, lobortis in odio. Praesent convallis urna a lacus interdum ut hendrerit risus congue. Nunc sagittis 

dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare 

turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed 

dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.</p>

</body>
</html>



Float next to eachother:

Since div elements are block elements, they are usually displayed on top of each other. We can, however, use 

float to place elements next to each other (such as in the news headlines on major websites. See 

illustration below:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  float: left;
  padding: 15px; 
}

.div1 {
  background: red;
}

.div2 {
  background: yellow;
}

.div3 {
  background: green;
}
</style>
</head>
<body>

<h2>Float Next To Each Other</h2>

<p>In this example, the three divs will float next to each other.</p>

<div class="div1">Div 1</div>
<div class="div2">Div 2</div>
<div class="div3">Div 3</div>

</body>
</html>


NB: The div above resemble nav bars. You can set a margin to create spaces between the div elements with 

classes div1, div2, and div3 successively. 



CSS Layout - clear and clearfix


The clear property
In cases where we use float property and we want next element(such as text) below (not on right or left), we 

use the clear property. Clear property specify what happens to element next to floating element. The 

possible values of clear properties include:



    none - The element is not pushed below left or right floated elements. This is default
    left - The element is pushed below left floated elements
    right - The element is pushed below right floated elements
    both - The element is pushed below both left and right floated elements
    inherit - The element inherits the clear value from its parent

You should match clear to the float: clear to the left for the element floated to the left. The enables 

floated element to continue floating, but cleared element appear below the floated (left) element on the web 

page. 

An example of clearing float to the left, wherein element is pushed below the left floated <div1> element:


<!DOCTYPE html>
<html>
<head>
<style>
.div1 {
  float: left;
  padding: 10px;
  border: 3px solid #73AD21;
}

.div2 {
  padding: 10px;
  border: 3px solid red;
}

.div3 {
  float: left;
  padding: 10px;  
  border: 3px solid #73AD21;
}

.div4 {
  padding: 10px;
  border: 3px solid red;
  clear: left;
}
</style>
</head>
<body>

<h2>Without clear</h2>
<div class="div1">div1</div>
<div class="div2">div2 - Notice that div2 is after div1 in the HTML code. However, since div1 floats to the 

left, the text in div2 flows around div1.</div>
<br><br>

<h2>With clear</h2>
<div class="div3">div3</div>
<div class="div4">div4 - Here, clear: left; moves div4 down below the floating div3. The value "left" clears 

elements floated to the left. You can also clear "right" and "both".</div>

</body>
</html>




The clearfix Hack

Floated elements taller than the containing element tend to "overflow outside of its container". The 

clearfix hack can be used to solve this problem by adding a clearfix class to the container containing the 

oversized image, and then make the overflow:auto; as settings in the CSS styling in <style> portion of 

header.


<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 3px solid #4CAF50;
  padding: 5px;
}

.img1 {
  float: right;
}

.img2 {
  float: right;
}

.clearfix {
  overflow: auto;
}
</style>
</head>
<body>

<h2>Without Clearfix</h2>

<p>This image is floated to the right. It is also taller than the element containing it, so it overflows 

outside of its container:</p>

<div>
  <img class="img1" src="pineapple.jpg" alt="Pineapple" width="170" height="170">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet...
</div>

<h2 style="clear:right">With Clearfix</h2>
<p>We can fix this by adding a clearfix class with overflow: auto; to the containing element:</p>

<div class="clearfix">
  <img class="img2" src="pineapple.jpg" alt="Pineapple" width="170" height="170">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet...
</div>

</body>
</html>



NB: The overflow: auto clearfix works well as long as you are able to keep control of your margins and 

padding (else you might see scrollbars). The new, modern clearfix hack however, is safer to use, and the 

following code (for the new modern clearfix) is used for most webpages:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 3px solid #4CAF50;
  padding: 5px;
}

.img1 {
  float: right;
}

.img2 {
  float: right;
}

.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
</style>
</head>
<body>

<h2>Without Clearfix</h2>

<p>This image is floated to the right. It is also taller than the element containing it, so it overflows 

outside of its container:</p>

<div>
  <img class="img1" src="pineapple.jpg" alt="Pineapple" width="170" height="170">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet...
</div>

<h2 style="clear:right">With New Modern Clearfix</h2>
<p>Add the clearfix hack to the containing element, to fix this problem:</p>

<div class="clearfix">
  <img class="img2" src="pineapple.jpg" alt="Pineapple" width="170" height="170">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet...
</div>

</body>
</html>



NB: the "::" represent pseud-element. More explanations later.


CSS Layout - Float Examples

Below are common float examples:



Grid of Boxes / Equal Width Boxes

The float property can be easily used to float boxed of content side by side. See illustration below:

<!DOCTYPE html>
<html>
<head>
<style>
* {
  box-sizing: border-box;
}

.box {
  float: left;
  width: 33.33%;
  padding: 50px;
}

.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
</style>
</head>
<body>

<h2>Grid of Boxes</h2>
<p>Float boxes side by side:</p>

<div class="clearfix">
  <div class="box" style="background-color:#bbb">
  <p>Some text inside the box.</p>
  </div>
  <div class="box" style="background-color:#ccc">
  <p>Some text inside the box.</p>
  </div>
  <div class="box" style="background-color:#ddd">
  <p>Some text inside the box.</p>
  </div>
</div>

<p><strong>Note:</strong> Here, we use the clearfix hack to take care of the layout flow. 
We also use the box-sizing property to make sure that the box doesn't break due to extra padding. Try to 

remove this code to see the effect.</p>

</body>
</html>



Images Side By Side (such as is popularly used in news websites)

The grid of boxes can also be employed in displaying images side-by-side.You can put all images in same 

class and set padding to create spaces between the images. Also clearfix hack is also used as described 

previously. See the illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
* {
  box-sizing: border-box;
}

.img-container {
  float: left;
  width: 33.33%;
  padding: 3px;
}

.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
</style>
</head>
<body>

<h2>Images Side by Side</h2>
<p>Float images side by side:</p>

<div class="clearfix">
  <div class="img-container">
  <img src="img_5terre.jpg" alt="Italy" style="width:100%">
  </div>
  <div class="img-container">
  <img src="img_forest.jpg" alt="Forest" style="width:100%">
  </div>
  <div class="img-container">
  <img src="img_mountains.jpg" alt="Mountains" style="width:100%">
  </div>
</div>

<p>Note that we also use the clearfix hack to take care of the layout flow, and that we add the box-sizing 

property to make sure that the image container doesn't break due to extra padding. Try to remove this code 

to see the effect.</p>

</body>
</html>



Equal Height Boxes

We have previously examined floating boxes side by side of equal width. To create floating boxes with equal 

height is more nuanced. You can quickly set fixed height to address the challenges as shown below:


<!DOCTYPE html>
<html>
<head>
<style>
* {
  box-sizing: border-box;
}

.box {
  float: left;
  width: 50%;
  padding: 50px;
  height: 300px;
}

.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
</style>
</head>
<body>

<h2>Equal Height Boxes</h2>
<p>Floating boxes with equal heights:</p>

<div class="clearfix">
  <div class="box" style="background-color:#bbb">
  <h2>Box 1</h2>
  <p>Some content, some content, some content</p>
  </div>
  <div class="box" style="background-color:#ccc">
  <h2>Box 2</h2>
  <p>Some content, some content, some content</p>
  <p>Some content, some content, some content</p>
  <p>Some content, some content, some content</p>
  </div>
</div>

<p>This example not very flexible. It is ok to use CSS height if you can guarantee that the boxes will 

always have the same amount of content in them, but that's not always the case. If you try the example above 

on a mobile phone (or resize the browser window), you will see that the second box's content will be 

displayed outside of the box.</p>
<p>Go back to the tutorial and find another solution, if this is not what you want.</p>

</body>
</html>

The method above is not very flexible if there is no certainty that the boxes will always contain same 

amount of content in them. Where content stays out of box(es), CSS3 Flexbox can be automatically used to 

stretch boxes as long as longest box:


See example below for the use of Flexbox  to create flexible boxes:

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  flex-wrap: nowrap;
  background-color: DodgerBlue;
}

.flex-container .box {
  background-color: #f1f1f1;
  width: 50%;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>
<h1>Flexible Boxes</h1>

<div class="flex-container">
  <div class="box">Box 1 - This is some text to make sure that the content gets really tall. This is some 

text to make sure that the content gets really tall.</div>
  <div class="box">Box 2 - My height will follow Box 1.</div>
</div>

<p>Try to resize the browser window to see the flexible layout.</p>
<p><strong>Note:</strong> Flexbox is not supported in Internet Explorer 10 or earlier versions.</p>

</body>
</html>


Navigation Menu

Float can be used with a list of hyperlinks to create a horizontal menu. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a {
  display: inline-block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #111;
}

.active {
  background-color: red;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home" class="active">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>



Web Layout

The entire web layout can be done with float property and this is a common practice. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
* {
  box-sizing: border-box;
}

.header, .footer {
  background-color: grey;
  color: white;
  padding: 15px;
}

.column {
  float: left;
  padding: 15px;
}

.clearfix::after {
  content: "";
  clear: both;
  display: table;
}

.menu {
  width: 25%;
}

.content {
  width: 75%;
}

.menu ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.menu li {
  padding: 8px;
  margin-bottom: 8px;
  background-color: #33b5e5;
  color: #ffffff;
}

.menu li:hover {
  background-color: #0099cc;
}
</style>
</head>
<body>

<div class="header">
  <h1>Chania</h1>
</div>

<div class="clearfix">
  <div class="column menu">
    <ul>
      <li>The Flight</li>
      <li>The City</li>
      <li>The Island</li>
      <li>The Food</li>
    </ul>
  </div>

  <div class="column content">
    <h1>The City</h1>
    <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two 

parts, the old town and the modern city.</p>
    <p>You will learn more about web layout and responsive web pages in a later chapter.</p>
  </div>
</div>

<div class="footer">
  <p>Footer Text</p>
</div>

</body>
</html>


More examples with CSS float

An image with border and margins that floats to the right in a paragraph (similar to that used in news 

websites):

<!DOCTYPE html>
<html>
<head>
<style>
img {
  float: right;
  border: 1px dotted black;
  margin: 0px 0px 15px 20px;
}
</style>
</head>
<body>

<p>In the paragraph below, the image will float to the right. A dotted black border is added to the image. 
We have also added margins to the image to push the text away from the image:
0 px margin on the top and right side, 15 px margin on the bottom, and 20 px margin on the left side of the 

image.
</p>

<p><img src="w3css.gif" width="100" height="140">
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
</p>

</body>
</html>




An image with caption that float to the right:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  float: right;
  width: 120px;
  margin: 0 0 15px 20px;
  padding: 15px;
  border: 1px solid black;
  text-align: center;
}
</style>
</head>
<body>

<div>
<img src="w3css.gif" width="100" height="140"><br>CSS is fun!
</div>

<p>
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
</p>

<p>
In the paragraph above, the div element is 120 pixels wide and it contains the image.
The div element will float to the right. Margins are added to the div to push the text away from the div.
Borders and padding are added to the div to frame in the picture and the caption.
</p>

</body>
</html>


Let the first letter of a paragraph float to the left (such as is found in online news paper articles):

<!DOCTYPE html>
<html>
<head>
<style>
span {
  float: left;
  width: 0.7em;
  font-size: 400%;
  font-family: algerian, courier;
  line-height: 80%;
}
</style>
</head>
<body>

<p>
<span>T</span>his is some text.
This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
This is some text. This is some text. This is some text.
</p>

<p>
In the paragraph above, the first letter of the text is embedded in a span element.
The span element has a width that is 0.7 times the size of the current font.
The font-size of the span element is 400% (quite large) and the line-height is 80%.
The font of the letter in the span will be in "Algerian".
</p>

</body>
</html>


in the above, the font size of the span is 400% and the letter is just 0.7 times the curentl font size of 

the current font. The line height is also 80%



Creating a website with float:


<!DOCTYPE html>
<html>
<head>
<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
}

.header {
  background-color: #2196F3;
  color: white;
  text-align: center;
  padding: 15px;
}

.footer {
  background-color: #444;
  color: white;
  padding: 15px;
}

.topmenu {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #777;
}

.topmenu li {
  float: left;
}

.topmenu li a {
  display: inline-block;
  color: white;
  text-align: center;
  padding: 16px;
  text-decoration: none;
}

.topmenu li a:hover {
  background-color: #222;
}

.topmenu li a.active {
  color: white;
  background-color: #4CAF50;
}

.column {
  float: left;
  padding: 15px;
}

.clearfix::after {
  content: "";
  clear: both;
  display: table;
}

.sidemenu {
  width: 25%;
}

.content {
  width: 75%;
}

.sidemenu ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.sidemenu li a {
  margin-bottom: 4px;
  display: block;
  padding: 8px;
  background-color: #eee;
  text-decoration: none;
  color: #666;
}

.sidemenu li a:hover {
  background-color: #555;
  color: white;
}

.sidemenu li a.active {
  background-color: #008CBA;
  color: white;
}
</style>
</head>
<body>

<ul class="topmenu">
  <li><a href="#home" class="active">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<div class="clearfix">
  <div class="column sidemenu">
    <ul>
      <li><a href="#flight">The Flight</a></li>
      <li><a href="#city" class="active">The City</a></li>
      <li><a href="#island">The Island</a></li>
      <li><a href="#food">The Food</a></li>
      <li><a href="#people">The People</a></li>
      <li><a href="#history">The History</a></li>
      <li><a href="#oceans">The Oceans</a></li>
    </ul>
  </div>

  <div class="column content">
    <div class="header">
      <h1>The City</h1>
    </div>
    <h1>Chania</h1>
    <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two 

parts, the old town and the modern city.</p>
    <p>You will learn more about responsive web pages in a later chapter.</p>
  </div>
</div>

<div class="footer">
  <p>Footer Text</p>
</div>

</body>
</html>


All CSS Float Properties
Property 	Description
box-sizing 	Defines how the width and height of an element are calculated: should they include padding 

and borders, or not
clear 	Specifies what should happen with the element that is next to a floating element
float 	Specifies whether an element should float to the left, right, or not at all
overflow 	Specifies what happens if content overflows an element's box
overflow-x 	Specifies what to do with the left/right edges of the content if it overflows the element's 

content area
overflow-y 	Specifies what to do with the top/bottom edges of the content if it overflows the element's 

content area




CSS Inline-block

CSS Layout - display: inline-block;

The display: inline-block Value:

Unlike display:inline; which does not respect the top and bottom margins/ paddings, display:inline-block 

respects the top and bottom margins/ paddings and also allows one to set a width and height on the element. 

Compared to display:block; the display:inline-block does not add a line-break after the element, so the 

element can sit next to other elements.Note that display:inline; is the default for span. See the 

illustration of the difference between display: inline; , display: inline-block; , and display:block;


<!DOCTYPE html>
<html>
<head>
<style>
span.a {
  display: inline; /* the default for span */
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;  
  background-color: yellow; 
}

span.b {
  display: inline-block;
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;    
  background-color: yellow; 
}

span.c {
  display: block;
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;    
  background-color: yellow; 
}
</style>
</head>
<body>

<h1>The display Property</h1>

<h2>display: inline</h2>
<div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum consequat scelerisque elit sit amet 

consequat. Aliquam erat volutpat. <span class="a">Aliquam</span> <span class="a">venenatis</span> gravida 

nisl sit amet facilisis. Nullam cursus fermentum velit sed laoreet. </div>

<h2>display: inline-block</h2>
<div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum consequat scelerisque elit sit amet 

consequat. Aliquam erat volutpat. <span class="b">Aliquam</span> <span class="b">venenatis</span> gravida 

nisl sit amet facilisis. Nullam cursus fermentum velit sed laoreet. </div>

<h2>display: block</h2>
<div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum consequat scelerisque elit sit amet 

consequat. Aliquam erat volutpat. <span class="c">Aliquam</span> <span class="c">venenatis</span> gravida 

nisl sit amet facilisis. Nullam cursus fermentum velit sed laoreet. </div>

</body>
</html>


Using inline-block to create navigation links;

A common application of display:inline-block is displaying list items horizontally instead of vertically. 

See below for an example of a horizontal navigation links:


<!DOCTYPE html>
<html>
<head>
<style>
.nav {
  background-color: yellow; 
  list-style-type: none;
  text-align: center;
  margin: 0;
  padding: 0;
}

.nav li {
  display: inline-block;
  font-size: 20px;
  padding: 20px;
}
</style>
</head>
<body>

<h1>Horizontal Navigation Links</h1>
<p>By default, list items are displayed vertically. In this example we use display: inline-block to display 

them horizontally (side by side).</p>
<p>Note: If you resize the browser window, the links will automatically break when it becomes too 

crowded.</p>

<ul class="nav">
  <li><a href="#home">Home</a></li>
  <li><a href="#about">About Us</a></li>
  <li><a href="#clients">Our Clients</a></li>  
  <li><a href="#contact">Contact Us</a></li>
</ul>

</body>
</html>




CSS Align

Center Align Elements;

To center a block element (like <div>) horizontally,use margin: auto;. Setting the element width (usually in 

%) prevents the <div> block from stretching out to the edges of its container. The div element then assumes 

the specified width x% while the remaining (100-x)% space is split equally between the two margins. Meaning 

The div block is in the midle and occupies x% of the page horizontally, while the margins on left and right 

hand side of the div block are equally [(100-x)/2]%. Note that center aligning the block using margin:auto; 

has no effect if the width property is not set (or set to 100%). See illustration of margin:auto = below:


<!DOCTYPE html>
<html>
<head>
<style>
.center {
  margin: auto;
  width: 60%;
  border: 3px solid #73AD21;
  padding: 10px;
}
</style>
</head>
<body>

<h2>Center Align Elements</h2>
<p>To horizontally center a block element (like div), use margin: auto;</p>

<div class="center">
  <p>Hello World!</p>
</div>

</body>
</html>




Center Align Text;

To center text inside an element, the text-align: center; allows that to be done. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
.center {
  text-align: center;
  border: 3px solid green;
}
</style>
</head>
<body>

<h2>Center Text</h2>

<div class="center">
  <p>This text is centered.</p>
</div>

</body>
</html>



Center an Image;

To center an image, set left and right margins to auto and make the image into a block element. This centers 

the image. See illustration of how to center an image below: 

<!DOCTYPE html>
<html>
<head>
<style>
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
</head>
<body>

<h2>Center an Image</h2>
<p>To center an image, set left and right margin to auto, and make it into a block element.</p>

<img src="paris.jpg" alt="Paris" style="width:40%">

</body>
</html>



Left and Right Align - Using position;

You can align an element using position:absolute;.Note that Absolute positioned elements are removed from 

the normal flow, and can overlap elements. See illustration of absolute positioned elements for right 

alignment below:



<!DOCTYPE html>
<html>
<head>
<style>
.right {
  position: absolute;
  right: 0px;
  width: 300px;
  border: 3px solid #73AD21;
  padding: 10px;
}
</style>
</head>
<body>

<h2>Right Align</h2>
<p>An example of how to right align elements with the position property:</p>

<div class="right">
  <p>In my younger and more vulnerable years my father gave me some advice that I've been turning over in my 

mind ever since.</p>
</div>

</body>
</html>


NB: Setting right margin to zero aligns the element to the right. On the other hand, setting the left margin 

to zero aligns the element to the left. 



Left and Right Align - Using float;

You can also align elements using float property as shown below:


<!DOCTYPE html>
<html>
<head>
<style>
.right {
  float: right;
  width: 300px;
  border: 3px solid #73AD21;
  padding: 10px;
}
</style>
</head>
<body>

<h2>Right Align</h2>
<p>An example of how to right align elements with the float property:</p>

<div class="right">
  <p>In my younger and more vulnerable years my father gave me some advice that I've been turning over in my 

mind ever since.</p>
</div>

</body>
</html>



The clearfix Hack;

Whenever an element is taller than the element containing it (parent element), its overflow outside of its 

container can be fixed the "clearfix hack". Once the clearfix hack is added to the parent element, the 

problem will be fixed. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 3px solid #4CAF50;
  padding: 5px;
}

.img1 {
  float: right;
}

.img2 {
  float: right;
}

.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
</style>
</head>
<body>

<h2>Without Clearfix</h2>

<p>This image is floated to the right. It is also taller than the element containing it, so it overflows 

outside of its container:</p>

<div>
  <img class="img1" src="pineapple.jpg" alt="Pineapple" width="170" height="170">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet...
</div>

<h2 style="clear:right">With New Modern Clearfix</h2>
<p>Add the clearfix hack to the containing element, to fix this problem:</p>

<div class="clearfix">
  <img class="img2" src="pineapple.jpg" alt="Pineapple" width="170" height="170">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet...
</div>

</body>
</html>




Center Vertically - Using padding;

A simple way to center an element vertically in CSS is to use top and bottom padding. See illustration of 

how to center vertically. Note that there are other methods which can be used to center element vertically, 

the one provided here just happens to be a simpler one. 

<!DOCTYPE html>
<html>
<head>
<style>
.center {
  padding: 70px 0;
  border: 3px solid green;
}
</style>
</head>
<body>

<h2>Center Vertically</h2>
<p>In this example, we use the padding property to center the div element vertically:</p>

<div class="center">
  <p>I am vertically centered.</p>
</div>

</body>
</html>


To center both vertically and horizontally, use padding and text-align: center; as shown below:

<!DOCTYPE html>
<html>
<head>
<style>
.center {
  padding: 70px 0;
  border: 3px solid green;
  text-align: center;
}
</style>
</head>
<body>

<h2>Centering</h2>
<p>In this example, we use padding and text-align to center the div element vertically and horizontally:</p>

<div class="center">
  <p>I am vertically and horizontally centered.</p>
</div>

</body>
</html>




Center Vertically - Using line-height;

You can also center text vertically by  using line-height property with a value that is equal to the height 

property. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
.center {
  line-height: 200px;
  height: 200px;
  border: 3px solid green;
  text-align: center;
}

.center p {
  line-height: 1.5;
  display: inline-block;
  vertical-align: middle;
}
</style>
</head>
<body>

<h2>Centering</h2>
<p>In this example, we use the line-height property with a value that is equal to the height property to 

center the div element:</p>

<div class="center">
  <p>I am vertically and horizontally centered.</p>
</div>

</body>
</html>
 



Center Vertically - Using position & transform;

You can also use positioning and transform to center vertically if you cannot use padding and line-height. 

You will learn more about transform property in the 2D Transforms Chapter. See the illustration of the use 

of position and transform to center vertically.


 
<!DOCTYPE html>
<html>
<head>
<style>
.center { 
  height: 200px;
  position: relative;
  border: 3px solid green; 
}

.center p {
  margin: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
}
</style>
</head>
<body>

<h2>Centering</h2>
<p>In this example, we use positioning and the transform property to vertically and horizontally center the 

div element:</p>

<div class="center">
  <p>I am vertically and horizontally centered.</p>
</div>

</body>
</html>



Center Vertically - Using Flexbox;

Flexbox can also help to center things. Meanwhile, it is not supported in IE10 and earlier versions. The CSS 

Flexbox will be covered later. 


<!DOCTYPE html>
<html>
<head>
<style>
.center {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 200px;
  border: 3px solid green; 
}
</style>
</head>
<body>

<h2>Flexbox Centering</h2>

<p>A container with both the justify-content and the align-items properties set to <em>center</em> will 

align the item(s) in the center (in both axis).</p>

<div class="center">
  <p>I am vertically and horizontally centered.</p>
</div>

</body>
</html>



CSS Combinators

The relationship between the selectors in an HTML page is explained by combinators.

More than one single selector can be contained in a CSS selector, and we can include a combinator between 

simple selectors. The four unique combinators, and their representation (in parenthesis) in CSS include:



    descendant selector (space)
    child selector (>)
    adjacent sibling selector (+)
    general sibling selector (~)



Descendant Selector  ( );

Descendant selector matches all the elements that are descendants of the same specified element. It is 

specified using empty space. For example, in the code below, the <p> elements that are inside the <div> 

elements are selected:


<!DOCTYPE html>
<html>
<head>
<style>
div p {
  background-color: yellow;
}
</style>
</head>
<body>

<h2>Descendant Selector</h2>
<p>The descendant selector matches all elements that are descendants of a specified element.</p>

<div>
  <p>Paragraph 1 in the div.</p>
  <p>Paragraph 2 in the div.</p>
  <section><p>Paragraph 3 in the div.</p></section>
</div>

<p>Paragraph 4. Not in a div.</p>
<p>Paragraph 5. Not in a div.</p>

</body>
</html>


Child Selector (>)

Child selector selects all elements that are the children of a specified element. It is denoted using the 

greater than symbol. In the code below for example, all the <p> elements that are children of a <div> 

element are selected:



<!DOCTYPE html>
<html>
<head>
<style>
div > p {
  background-color: yellow;
}
</style>
</head>
<body>

<h2>Child Selector</h2>
<p>The child selector (>) selects all elements that are the children of a specified element.</p>

<div>
  <p>Paragraph 1 in the div.</p>
  <p>Paragraph 2 in the div.</p>
  <section><p>Paragraph 3 in the div.</p></section> <!-- not Child but Descendant -->
  <p>Paragraph 4 in the div.</p>
</div>

<p>Paragraph 5. Not in a div.</p>
<p>Paragraph 6. Not in a div.</p>

</body>
</html>



Note that elements not directly under a parent but have a sub-parent is a descendant not a child of another.




Adjacent Sibling Selector (+);


The adjacent sibling selector is used to select an element that is located after another specific element. 

Here adjacent means "immediately following". Sibling elements must have same parent. The adjacent sibling 

selector is denoted with the plus (+) sign. In the example below, only the first <p> elements that are 

placed "immediately" after <div> elements are selected.

<!DOCTYPE html>
<html>
<head>
<style>
div + p {
  background-color: yellow;
}
</style>
</head>
<body>

<h2>Adjacent Sibling Selector</h2>

<p>The + selector is used to select an element that is directly after another specific element.</p>
<p>The following example selects the first p element that are placed immediately after div elements:</p>

<div>
  <p>Paragraph 1 in the div.</p>
  <p>Paragraph 2 in the div.</p>
</div>

<p>Paragraph 3. After a div.</p>
<p>Paragraph 4. After a div.</p>

<div>
  <p>Paragraph 5 in the div.</p>
  <p>Paragraph 6 in the div.</p>
</div>

<p>Paragraph 7. After a div.</p>
<p>Paragraph 8. After a div.</p>

</body>
</html>


General Sibling Selector (~);

The general sibling selector selects 'all' elements that are "next siblings" of a specified element. It is 

denoted by tilda sign (~). Remember that all elements in the body are siblings of <html>. In the example 

below, all the <p> elements that are next siblings of <div> elements are selected:



<!DOCTYPE html>
<html>
<head>
<style>
div ~ p {
  background-color: yellow;
}
</style>
</head>
<body>

<h2>General Sibling Selector</h2>
<p>The general sibling selector (~) selects all elements that are next siblings of a specified element.</p>

<p>Paragraph 1.</p>

<div>
  <p>Paragraph 2.</p>
</div>

<p>Paragraph 3.</p>
<code>Some code.</code>
<p>Paragraph 4.</p>

</body>
</html>


All CSS Combinator Selectors
Selector 	Example 	Example description
element element 	div p 	Selects all <p> elements inside <div> elements
element>element 	div > p 	Selects all <p> elements where the parent is a <div> element
element+element 	div + p 	Selects the first <p> element that are placed immediately after 

<div> elements
element1~element2 	p ~ ul 	Selects every <ul> element that are preceded by a <p> element



CSS Pseudo-classes

A pseudo-class is used to define a special state of an element. For instance, you can use psedo-class to 

style:

-an element when a user mouses over it
-visited and unvisited links differently
-an element when it gets focus


The general syntax for pseudo-classes is:

selector:pseudo-class {
  property: value;
}

alternatively, you can specify the class of the selector.

selector.class:pseudo-class {
  property: value;
}





Anchor Pseudo-classes;

They are used to display links in different ways.See illustration below for some ways links can be displayed 

based on the action of mouse on it (visited, hovered on, unvisited, during click):


<!DOCTYPE html>
<html>
<head>
<style>
/* unvisited link */
a:link {
  color: red;
}

/* visited link */
a:visited {
  color: green;
}

/* mouse over link */
a:hover {
  color: hotpink;
}

/* selected link */
a:active {
  color: blue;
}
</style>
</head>
<body>

<h2>CSS Links</h2>
<p><b><a href="default.asp" target="_blank">This is a link</a></b></p>
<p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be 

effective.</p>
<p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>

</body>
</html>


Note: a:hover MUST come after a:link and a:visited in the CSS definition in order to be effective! a:active 

MUST come after a:hover in the CSS definition in order to be effective! Pseudo-class names are not case-

sensitive.



Pseudo-classes and CSS Classes;

Pseudo-classes can be combined with CSS classes. This enables a specific application of pseudo classes to 

elements. In the example below, hovering over the link will make the link change color:


<!DOCTYPE html>
<html>
<head>
<style>
a.highlight:hover {
  color: #ff0000;
} 
</style>
</head>
<body>

<h2>Pseudo-classes and CSS Classes</h2>
<p>When you hover over the first link below, it will change color:</p>

<p><a class="highlight" href="css_syntax.asp">CSS Syntax</a></p>
<p><a href="default.asp">CSS Tutorial</a></p>

</body>
</html>




Hover on <div>;

The example below shows how to use :hover pseudo-class on a <div> element:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: green;
  color: white;
  padding: 25px;
  text-align: center;
}

div:hover {
  background-color: blue;
}
</style>
</head>
<body>

<p>Mouse over the div element below to change its background color:</p>

<div>Mouse Over Me</div>

</body>
</html>



Simple Tooltip Hover;

This enables you to show a <p> element(like a tooltip) by hovering over a <div> element. You can also use it 

for other selectors. See illustration below:

<!DOCTYPE html>
<html>
<head>
<style>
p {
  display: none;
  background-color: yellow;
  padding: 20px;
}

div:hover p {
  display: block;
}
</style>
</head>
<body>

<div>Hover over me to show the p element
  <p>Tada! Here I am!</p>
</div>

</body>
</html>



CSS - The :first-child Pseudo-class

The :first-child pseudo-class matches a specified element that is the first child of another element. 


Match the first <p> element::

In the example below, the selector matches any <p> element that is the first child of any element:



<!DOCTYPE html>
<html>
<head>
<style>
p:first-child {
  color: blue;
} 
</style>
</head>
<body>

<p>This is some text.</p>
<p>This is some text.</p>

</body>
</html>



Match the first <i> element in all <p> elements::

In the example below, the selector matches the first <i> element in all <p> elements:

<!DOCTYPE html>
<html>
<head>
<style>
p i:first-child {
  color: blue;
} 
</style>
</head>
<body>

<p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>
<p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>

</body>
</html>



Match all <i> elements in all first child <p> elements::

In the example below, the selector matches all <i> elements in <p> elements which are first child of another 

element:


<!DOCTYPE html>
<html>
<head>
<style>
p:first-child i {
  color: blue;
} 
</style>
</head>
<body>

<p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>
<p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>

</body>
</html>


CSS - The :lang Pseudo-class::

The :lang pseudo class allows you to define special rules for different languages. The :lang in the example 

below defines the quotations marks for <q> elements with lang= "no" (the quotation mark used in this case is 

~text here~:


<!DOCTYPE html>
<html>
<head>
<style>
q:lang(no) {
  quotes: "~" "~";
}
</style>
</head>
<body>

<p>Some text <q lang="no">A quote in a paragraph</q> Some text.</p>
<p>In this example, :lang defines the quotation marks for q elements with lang="no":</p>

</body>
</html>


Some Additional Examples of Pseudo Class::

Adding different styles to hyperlinks:::

<!DOCTYPE html>
<html>
<head>
<style>
a.one:link {color:#ff0000;}
a.one:visited {color:#0000ff;}
a.one:hover {color:#ffcc00;}

a.two:link {color:#ff0000;}
a.two:visited {color:#0000ff;}
a.two:hover {font-size:150%;}

a.three:link {color:#ff0000;}
a.three:visited {color:#0000ff;}
a.three:hover {background:#66ff66;}

a.four:link {color:#ff0000;}
a.four:visited {color:#0000ff;}
a.four:hover {font-family:monospace;}

a.five:link {color:#ff0000;text-decoration:none;}
a.five:visited {color:#0000ff;text-decoration:none;}
a.five:hover {text-decoration:underline;}
</style>
</head>
<body>

<h2>Styling Links</h2>

<p>Mouse over the links and watch them change layout:</p>

<p><b><a class="one" href="default.asp" target="_blank">This link changes color</a></b></p>
<p><b><a class="two" href="default.asp" target="_blank">This link changes font-size</a></b></p>
<p><b><a class="three" href="default.asp" target="_blank">This link changes background-color</a></b></p>
<p><b><a class="four" href="default.asp" target="_blank">This link changes font-family</a></b></p>
<p><b><a class="five" href="default.asp" target="_blank">This link changes text-decoration</a></b></p>

</body>
</html>



Use of focus:::

The :focus pseudo-class is used to style the part of a page while work is being done on it. For example, you 

may define a specific style, using pseudo-class, for a Form bar in focus (currently being filled):


<!DOCTYPE html>
<html>
<head>
<style>
input:focus {
  background-color: yellow;
}
</style>
</head>
<body>

<form action="/action_page.php" method="get">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <input type="submit" value="Submit">
</form>

</body>
</html>





Here are additional Pseudo-classes and tips to help in their usage:



All CSS Pseudo Classes

Selector 	Example 	Example description
:active 	a:active 	Selects the active link
:checked 	input:checked 	Selects every checked <input> element
:disabled 	input:disabled 	Selects every disabled <input> element
:empty 	p:empty 	Selects every <p> element that has no children
:enabled 	input:enabled 	Selects every enabled <input> element
:first-child 	p:first-child 	Selects every <p> elements that is the first child of its parent
:first-of-type 	p:first-of-type 	Selects every <p> element that is the first <p> element of its 

parent
:focus 	input:focus 	Selects the <input> element that has focus
:hover 	a:hover 	Selects links on mouse over
:in-range 	input:in-range 	Selects <input> elements with a value within a specified range
:invalid 	input:invalid 	Selects all <input> elements with an invalid value
:lang(language) 	p:lang(it) 	Selects every <p> element with a lang attribute value starting with 

"it"
:last-child 	p:last-child 	Selects every <p> elements that is the last child of its parent
:last-of-type 	p:last-of-type 	Selects every <p> element that is the last <p> element of its parent
:link 	a:link 	Selects all unvisited links
:not(selector) 	:not(p) 	Selects every element that is not a <p> element
:nth-child(n) 	p:nth-child(2) 	Selects every <p> element that is the second child of its parent
:nth-last-child(n) 	p:nth-last-child(2) 	Selects every <p> element that is the second child of its 

parent, counting from the last child
:nth-last-of-type(n) 	p:nth-last-of-type(2) 	Selects every <p> element that is the second <p> element of 

its parent, counting from the last child
:nth-of-type(n) 	p:nth-of-type(2) 	Selects every <p> element that is the second <p> element of 

its parent
:only-of-type 	p:only-of-type 	Selects every <p> element that is the only <p> element of its parent
:only-child 	p:only-child 	Selects every <p> element that is the only child of its parent
:optional 	input:optional 	Selects <input> elements with no "required" attribute
:out-of-range 	input:out-of-range 	Selects <input> elements with a value outside a specified range
:read-only 	input:read-only 	Selects <input> elements with a "readonly" attribute specified
:read-write 	input:read-write 	Selects <input> elements with no "readonly" attribute
:required 	input:required 	Selects <input> elements with a "required" attribute specified
:root 	root 	Selects the document's root element
:target 	#news:target 	Selects the current active #news element (clicked on a URL containing that 

anchor name)
:valid 	input:valid 	Selects all <input> elements with a valid value
:visited 	a:visited 	Selects all visited links



All CSS Pseudo Elements

Selector 	Example 	Example description
::after 	p::after 	Insert content after every <p> element
::before 	p::before 	Insert content before every <p> element
::first-letter 	p::first-letter 	Selects the first letter of every <p> element
::first-line 	p::first-line 	Selects the first line of every <p> element
::selection 	p::selection 	Selects the portion of an element that is selected by a user




CSS Pseudo-elements;

A CSS pseudo-element is used to style specific parts of an element such as: 
Styling the first letter, or line of an element; or 
Inserting content befor, or after, the content of another element. 



The syntax of pseudo-elements is:

selector::pseudo-element {
  property: value;
}




The ::first-line Pseudo-element ;;

The ::first-line pseudo-element is used to add a special style to the first line of a text. In the example 

below, the first line of text in all <p> elements is formatted:


<!DOCTYPE html>
<html>
<head>
<style>
p::first-line {
  color: #ff0000;
  font-variant: small-caps;
}
</style>
</head>
<body>

<p>You can use the ::first-line pseudo-element to add a special effect to the first line of a text. Some 

more text. And even more, and more, and more, and more, and more, and more, and more, and more, and more, 

and more, and more, and more.</p>

</body>
</html>


Please note that the ::first-line  pseudo-element can only be applied to block level elements. The following 

properties apply to the ::first-line pseudo-element:font properties, color properties, background 

properties, word-spacing, letter-spacing, text-decoration, vertical-align, text-transform, and line-height, 

clear.

The double colon notation of ::first-line is the standard used in CSS3 (unlike CSS 1 and 2 where single 

colon was used i.e. :first-line). This helps distinguish between pseudo-elements and pseudo-classes. For 

backward compatibility, the single-color syntax is acceptable in CSS2 and CSS1 pseudo-elements. 




The ::first-letter Pseudo-element ;;

The ::first-letter pseudo-element is used to add a special style to the first letter of a text. The example 

below shows how to use ::first-letter pseudo element to format the first letter of the text in all <p> 

elements:

<!DOCTYPE html>
<html>
<head>
<style>
p::first-letter {
  color: #ff0000;
  font-size: xx-large;
}
</style>
</head>
<body>

<p>You can use the ::first-letter pseudo-element to add a special effect to the first character of a text!

</p>

</body>
</html>



Note that: The ::first-letter pseudo element can only be applied to block-level elements. The following 

properties apply to the ::first-letter pseudo-element:font properties, color properties, background 

properties, margin properties, padding properties, border properties, text-decoration, vertical-align (only 

if "float" is "none"), text-transform, line-height, float, and clear.



Pseudo-elements and CSS Classes::

The Pseudo-elements can also be combined with CSS classes. This ensures that you can select a specific <p> 

element rather than apply pseudo-element styling to all <p> elements. In this case, the first letter of 

paragraphs with class="intro" will be displayed in red and in larger size. See illustration below:

<!DOCTYPE html>
<html>
<head>
<style>
p.intro::first-letter {
  color: #ff0000;
  font-size: 200%;
}  
</style>
</head>
<body>

<p class="intro">This is an introduction.</p>
<p>This is a paragraph with some text. A bit more text even.</p>

</body>
</html>


Multiple Pseudo-elements::

Several pseudo-elements can also be combined. In the example below, the first letter of a paragraph will be 

red, in an XX-large font size. The rest of the first line will be blue, and in small-caps. The rest of the 

paragraph will be the default font size and color. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
p::first-letter {
  color: #ff0000;
  font-size: xx-large;
}

p::first-line {
  color: #0000ff;
  font-variant: small-caps;
}
</style>
</head>
<body>

<p>You can combine the ::first-letter and ::first-line pseudo-elements to add a special effect to the first 

letter and the first line of a text!</p>

</body>
</html>



CSS - The ::before Pseudo-element::

The ::before pseudo-element can be used to insert some content before the content of an element. In the 

example below, and image (smiley.gif) is inserted before the content of each <h1> element:


<!DOCTYPE html>
<html>
<head>
<style>
h1::before {
  content: url(smiley.gif);
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>The ::before pseudo-element inserts content before the content of an element.</p>

<h1>This is a heading</h1>

</body>
</html>




CSS - The ::after Pseudo-element


The ::after pseudo-element can be used to insert some content after the content of an element. The example 

below shows the insertion of an image after the content of each <h1> element:


<!DOCTYPE html>
<html>
<head>
<style>
h1::after {
  content: url(smiley.gif);
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>The ::after pseudo-element inserts content after the content of an element.</p>

<h1>This is a heading</h1>

</body>
</html>



CSS - The ::marker Pseudo-element

The ::marker pseudo-element selects (styles) the markers of list of items. The example below shows styling 

of markers of list of items using ::marker pseudo-element:


<!DOCTYPE html>
<html>
<head>
<style>
::marker { 
  color: red;
  font-size: 23px;
}
</style>
</head>
<body>

<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

<ol>
  <li>First</li>
  <li>Second</li>
  <li>Third</li>
</ol>

</body>
</html>


NB: You don't have to style based on class here, the ::marker style will apply to all markers. 




CSS - The ::selection Pseudo-element::


The ::selection pseudo-element matches the portion of an element that is selected by a user. The properties 

that can be applied to ::selection include: color, background, cursor, and outline. The styling in the 

example below makes a selected text red on a yellow background:


<!DOCTYPE html>
<html>
<head>
<style>
::-moz-selection { /* Code for Firefox */
  color: red;
  background: yellow;
}

::selection {
  color: red;
  background: yellow;
}
</style>
</head>
<body>

<h1>Select some text on this page:</h1>

<p>This is a paragraph.</p>
<div>This is some text in a div element.</div>

<p><strong>Note:</strong> Firefox supports an alternative, the ::-moz-selection property.</p>

</body>
</html>




All CSS Pseudo Elements
Selector 	Example 	Example description
::after 	p::after 	Insert something after the content of each <p> element
::before 	p::before 	Insert something before the content of each <p> element
::first-letter 	p::first-letter 	Selects the first letter of each <p> element
::first-line 	p::first-line 	Selects the first line of each <p> element
::marker 	::marker 	Selects the markers of list items
::selection 	p::selection 	Selects the portion of an element that is selected by a user
All CSS Pseudo Classes
Selector 	Example 	Example description
:active 	a:active 	Selects the active link
:checked 	input:checked 	Selects every checked <input> element
:disabled 	input:disabled 	Selects every disabled <input> element
:empty 	p:empty 	Selects every <p> element that has no children
:enabled 	input:enabled 	Selects every enabled <input> element
:first-child 	p:first-child 	Selects every <p> elements that is the first child of its parent
:first-of-type 	p:first-of-type 	Selects every <p> element that is the first <p> element of its 

parent
:focus 	input:focus 	Selects the <input> element that has focus
:hover 	a:hover 	Selects links on mouse over
:in-range 	input:in-range 	Selects <input> elements with a value within a specified range
:invalid 	input:invalid 	Selects all <input> elements with an invalid value
:lang(language) 	p:lang(it) 	Selects every <p> element with a lang attribute value starting with 

"it"
:last-child 	p:last-child 	Selects every <p> elements that is the last child of its parent
:last-of-type 	p:last-of-type 	Selects every <p> element that is the last <p> element of its parent
:link 	a:link 	Selects all unvisited links
:not(selector) 	:not(p) 	Selects every element that is not a <p> element
:nth-child(n) 	p:nth-child(2) 	Selects every <p> element that is the second child of its parent
:nth-last-child(n) 	p:nth-last-child(2) 	Selects every <p> element that is the second child of its 

parent, counting from the last child
:nth-last-of-type(n) 	p:nth-last-of-type(2) 	Selects every <p> element that is the second <p> element of 

its parent, counting from the last child
:nth-of-type(n) 	p:nth-of-type(2) 	Selects every <p> element that is the second <p> element of 

its parent
:only-of-type 	p:only-of-type 	Selects every <p> element that is the only <p> element of its parent
:only-child 	p:only-child 	Selects every <p> element that is the only child of its parent
:optional 	input:optional 	Selects <input> elements with no "required" attribute
:out-of-range 	input:out-of-range 	Selects <input> elements with a value outside a specified range
:read-only 	input:read-only 	Selects <input> elements with a "readonly" attribute specified
:read-write 	input:read-write 	Selects <input> elements with no "readonly" attribute
:required 	input:required 	Selects <input> elements with a "required" attribute specified
:root 	root 	Selects the document's root element
:target 	#news:target 	Selects the current active #news element (clicked on a URL containing that 

anchor name)
:valid 	input:valid 	Selects all <input> elements with a valid value
:visited 	a:visited 	Selects all visited links






CSS Opacity


The opacity property quantifies the opacity or trasparency of an element.\


Transparent Image
Opacity of an image ranges from 0 to 1, with 0 being fully transparent and 1.0 meaning fully opaque. See 

example code below:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  opacity: 0.5;
}
</style>
</head>
<body>

<h1>Image Transparency</h1>
<p>The opacity property specifies the transparency of an element. The lower the value, the more 

transparent:</p>

<p>Image with 50% opacity:</p>
<img src="img_forest.jpg" alt="Forest" width="170" height="100">

</body>
</html>



Transparent Hover Effect

It is common for opacity property to be used alongside :hover selector to change the opacity of an image on 

mouse-over. See illustration of how to modify opacity of an image on mouseover below:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  opacity: 0.5;
}

img:hover {
  opacity: 1.0;
}
</style>
</head>
<body>

<h1>Image Transparency</h1>
<p>The opacity property is often used together with the :hover selector to change the opacity on mouse-

over:</p>
<img src="img_forest.jpg" alt="Forest" width="170" height="100">
<img src="img_mountains.jpg" alt="Mountains" width="170" height="100">
<img src="img_5terre.jpg" alt="Italy" width="170" height="100">

</body>
</html>



Note on example above: The CSS style shows what happens when a user hovers over one of the images. And in 

this example, we want the image to NOT be transparent when user mouses-over it. The CSS for this is thus 

opacity:1; upon hovering, and the pseudo class is set accordingly. 




Transparent Box

The opacity property used in adding transparency to an element is also inherited by the child elements. This 

can make text too transparent to be readable. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: #4CAF50;
  padding: 10px;
}

div.first {
  opacity: 0.1;
}

div.second {
  opacity: 0.3;
}

div.third {
  opacity: 0.6;
}
</style>
</head>
<body>

<h1>Transparent Box</h1>
<p>When using the opacity property to add transparency to the background of an element, all of its child 

elements become transparent as well. This can make the text inside a fully transparent element hard to 

read:</p>

<div class="first"><p>opacity 0.1</p></div>
<div class="second"><p>opacity 0.3</p></div>
<div class="third"><p>opacity 0.6</p></div>
<div><p>opacity 1 (default)</p></div>

</body>
</html>


Transparency using RGBA:::

The use of RGBA prevents the application of opacity to child elements. Once you specify color as RGBA, the 

opacity is only set for the background color and not the text. 

<!DOCTYPE html>
<html>
<head>
<style>
div {
  background: rgb(76, 175, 80);
  padding: 10px;
}

div.first {
  background: rgba(76, 175, 80, 0.1);
}

div.second {
  background: rgba(76, 175, 80, 0.3);
}

div.third {
  background: rgba(76, 175, 80, 0.6);
}
</style>
</head>
<body>

<h1>Transparent Box</h1>
<p>With opacity:</p>
<div style="opacity:0.1;"><p>10% opacity</p></div>
<div style="opacity:0.3;"><p>30% opacity</p></div>
<div style="opacity:0.6;"><p>60% opacity</p></div>
<div><p>opacity 1</p></div>

<p>With RGBA color values:</p>
<div class="first"><p>10% opacity</p></div>
<div class="second"><p>30% opacity</p></div>
<div class="third"><p>60% opacity</p></div>
<div><p>default</p></div>

<p>Notice how the text gets transparent as well as the background color when using the opacity property.</p>

</body>
</html>


Text in Transparent Box:::

In CSS, we can also create text in transparent box. The process involves: First, creating a <div> element 

(class="background") with a background image, and a border.

Then we create another <div> (class="transbox") inside the first <div>.

The <div class="transbox"> have a background color, and a border - the div is transparent.

Inside the transparent <div>, we add some text inside a <p> element. The example below shows how to insert 

text inside a transparent box:
 

<!DOCTYPE html>
<html>
<head>
<style>
div.background {
  background: url(klematis.jpg) repeat;
  border: 2px solid black;
}

div.transbox {
  margin: 30px;
  background-color: #ffffff;
  border: 1px solid black;
  opacity: 0.6;
}

div.transbox p {
  margin: 5%;
  font-weight: bold;
  color: #000000;
}
</style>
</head>
<body>

<div class="background">
  <div class="transbox">
    <p>This is some text that is placed in the transparent box.</p>
  </div>
</div>

</body>
</html>




CSS Navigation Bar

Navigation bars::

It is important for the audience of a website to find it easy to navigate. The CSS enables you to transform 

HTML menus into appealing navigation bars.


Navigation Bar= List of Links

A standard HTML is needed as a base for a navigation bar. In the examples in this chapter, navigation bar is 

built from standard HTML list. The use of <ul> and <li> elements in a navigation bar is reasonable since a 

navigation bar is essentially a list of links. 



See an example below of a plain HTML list as navigation menu:

<!DOCTYPE html>
<html>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<p>Note: We use href="#" for test links. In a real web site this would be URLs.</p>

</body>
</html>


We can then remove bullets, margins, and paddings from the list to make it look more appealing:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}
</style>
</head>
<body>

<p>In this example, we remove the bullets from the list, and its default padding and margin.</p>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>


NB: In the example above:

list-style-type: none; - Removes the bullets. A navigation bar does not need list markers
  
Set margin: 0; and padding: 0; to remove browser default settings

The code used above is the standard code used in both vertical and horizontal navigation bars. 



CSS Vertical Navigation Bar::


Vertical Navigation Bar:

To build a vertical nav bar, you can style <a> elements inside the list in addition to the code explained 

above. :


<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

li a {
  display: block;
  width: 60px;
  background-color: #dddddd;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<p>A background color is added to the links to show the link area.</p>
<p>Notice that the whole link area is clickable, not just the text.</p>

</body>
</html>


In the example above:  

display: block; - Displaying the links as block elements makes the whole link area clickable (not just the 

text), and it allows us to specify the width (and padding, margin, height, etc. if you want)
    
width: 60px; - Block elements take up the full width available by default. We want to specify a 60 pixels 

width


You can also set the width of <ul>, and remove the width of <a>, as they will take up the full width 

available when displayed as block elements. This will produce the same result as our previous example:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 60px;
} 

li a {
  display: block;
  background-color: #dddddd;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<p>A background color is added to the links to show the link area.</p>
<p>Notice that the whole link area is clickable, not just the text.</p>

</body>
</html>


Examples of Vertical Navigation Bars:::


To obtain a basic vertical navigation bar with a gray background color and change the background color of 

the links when the user moves the mouse over them:

<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #f1f1f1;
}

li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}

/* Change the link color on hover */
li a:hover {
  background-color: #555;
  color: white;
}
</style>
</head>
<body>

<h2>Vertical Navigation Bar</h2>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>



Active/Current Navigation Link:::

Add an "active" class to the current link to let the user know which page he/she is on:

<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #f1f1f1;
}

li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}

li a.active {
  background-color: #04AA6D;
  color: white;
}

li a:hover:not(.active) {
  background-color: #555;
  color: white;
}
</style>
</head>
<body>

<h2>Vertical Navigation Bar</h2>
<p>In this example, we create an "active" class with a green background color and a white text. The class is 

added to the "Home" link.</p>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>



Center Links & Add Borders


Adding text-align: center to <li> or <a> centers the links. To add border around the navbar, add border 

property to <ul>. To add borders inside the navbar, add border-bottom to all <li> elements except for the 

last one. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #f1f1f1;
  border: 1px solid #555;
}

li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}

li {
  text-align: center;
  border-bottom: 1px solid #555;
}

li:last-child {
  border-bottom: none;
}

li a.active {
  background-color: #04AA6D;
  color: white;
}

li a:hover:not(.active) {
  background-color: #555;
  color: white;
}
</style>
</head>
<body>

<h2>Vertical Navigation Bar</h2>
<p>In this example, we center the navigation links and add a border to the navigation bar.</p>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>



Full-height Fixed Vertical Navbar:::

To create a full-height sticky side navigation, apply the code below (it may not work properly on mobile 

devices):

<!DOCTYPE html>
<html>
<head>
<style>
body {
  margin: 0;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 25%;
  background-color: #f1f1f1;
  position: fixed;
  height: 100%;
  overflow: auto;
}

li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}

li a.active {
  background-color: #04AA6D;
  color: white;
}

li a:hover:not(.active) {
  background-color: #555;
  color: white;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<div style="margin-left:25%;padding:1px 16px;height:1000px;">
  <h2>Fixed Full-height Side Nav</h2>
  <h3>Try to scroll this area, and see how the sidenav sticks to the page</h3>
  <p>Notice that this div element has a left margin of 25%. This is because the side navigation is set to 

25% width. If you remove the margin, the sidenav will overlay/sit on top of this div.</p>
  <p>Also notice that we have set overflow:auto to sidenav. This will add a scrollbar when the sidenav is 

too long (for example if it has over 50 links inside of it).</p>
  <p>Some text..</p>
  <p>Some text..</p>
  <p>Some text..</p>
  <p>Some text..</p>
  <p>Some text..</p>
  <p>Some text..</p>
  <p>Some text..</p>
</div>

</body>
</html>




CSS Horizontal Navigation Bar::

You can create horizontal navigation bar using either inline or floating list items. 


Inline List Items

In addition to the standard code described above, you can specify <li> elements as inline to build 

horizontal navigation bar. Since <li> elements are block elements by default, styling them with display: 

inline; removes the line breaks before and after each list item to display them all on a single line. See 

illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

li {
  display: inline;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>





Floating List Items:::

Floating the <li> elements to the left and specifiying the navigation link layout creates a horizontal 

navigation bar. Overflow:hidden; when added to <ul> element prevents <li> elements from going outside the 

list. See the illustration below:

<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
}

li {
  float: left;
}

li a {
  display: block;
  padding: 8px;
  background-color: #dddddd;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<p><b>Note:</b> If a !DOCTYPE is not specified, floating items can produce unexpected results.</p>
<p>A background color is added to the links to show the link area. The whole link area is clickable, not 

just the text.</p>
<p><b>Note:</b> overflow:hidden is added to the ul element to prevent li elements from going outside of the 

list.</p>

</body>
</html>


In the example above, float:left; uses float to get block elements floating next to each other. 
display:block; allows us to specify  padding (and height, width, margins, etc. if you want)
    padding: 8px; - Specify some padding between each <a> element, to make them look good
    background-color: #dddddd; - Add a gray background-color to each <a> element


Tip: Add the background-color to <ul> instead of each <a> element if you want a full-width background color:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #dddddd;
}

li {
  float: left;
}

li a {
  display: block;
  padding: 8px;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<p>A background color is added to the list instead of each link to create a full-width background color.</p>
<p><b>Note:</b> overflow:hidden is added to the ul element to prevent li elements from going outside of the 

list.</p>

</body>
</html>




Horizontal Navigation Bar Examples

To create a basic horizontal navigation bar with a dark background color and change the background color of 

the links when the user moves the mouse over them:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #111;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>



Active/Current Navigation Link

Add an "active" class to the current link to let the user know which page he/she is on:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #111;
}

.active {
  background-color: #04AA6D;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>



Right-Align Links

Right-align links by floating the list items to the right (float:right;):

<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #111;
}

.active {
  background-color: #04AA6D;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li style="float:right"><a class="active" href="#about">About</a></li>
</ul>

</body>
</html>



Border Dividers

Add the border-right property to <li> to create link dividers:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
  border-right:1px solid #bbb;
}

li:last-child {
  border-right: none;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #111;
}

.active {
  background-color: #04AA6D;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li style="float:right"><a href="#about">About</a></li>
</ul>

</body>
</html>


Fixed Navigation Bar

Make the navigation bar stay at the top or the bottom of the page, even when the user scrolls the page:



Fixed top nav bar:

<!DOCTYPE html>
<html>
<head>
<style>
body {margin:0;}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
  position: fixed;
  top: 0;
  width: 100%;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #111;
}

.active {
  background-color: #04AA6D;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<div style="padding:20px;margin-top:30px;background-color:#1abc9c;height:1500px;">
  <h1>Fixed Top Navigation Bar</h1>
  <h2>Scroll this page to see the effect</h2>
  <h2>The navigation bar will stay at the top of the page while scrolling</h2>

  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
</div>

</body>
</html>



Fixed Bottom Navigation Bar:

<!DOCTYPE html>
<html>
<head>
<style>
body {margin:0;}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
  position: fixed;
  bottom: 0;
  width: 100%;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #111;
}

.active {
  background-color: #04AA6D;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<div style="padding:20px;background-color:#1abc9c;height:1500px;">
  <h1>Fixed Bottom Navigation Bar</h1>
  <h2>Scroll this page to see the effect</h2>
  <h2>The navigation bar will stay at the bottom of the page while scrolling</h2>

  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
  <p>Some text some text some text some text..</p>
</div>

</body>
</html>



Gray Horizontal Navbar

A gray horizontal bar with thin gray border is created as shown below:

<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  border: 1px solid #e7e7e7;
  background-color: #f3f3f3;
}

li {
  float: left;
}

li a {
  display: block;
  color: #666;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #ddd;
}

li a.active {
  color: white;
  background-color: #04AA6D;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  border: 1px solid #e7e7e7;
  background-color: #f3f3f3;
}

li {
  float: left;
}

li a {
  display: block;
  color: #666;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #ddd;
}

li a.active {
  color: white;
  background-color: #04AA6D;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>



Sticky Navbar

Add position: sticky; to <ul> to create a sticky navbar.

A sticky element toggles between relative and fixed, depending on the scroll position. It is positioned 

relative until a given offset position is met in the viewport - then it "sticks" in place (like 

position:fixed). Note that Internet Explorer do not support sticky positioning. Safari requires a -webkit- 

prefix (see example above). You must also specify at least one of top, right, bottom or left for sticky 

positioning to work. See illustration of the creation of sticky l


<!DOCTYPE html>
<html>
<head>
<style>
body {
  font-size: 28px;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
  position: -webkit-sticky; /* Safari */
  position: sticky;
  top: 0;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #111;
}

.active {
  background-color: #4CAF50;
}
</style>
</head>
<body>

<div class="header">
  <h2>Scroll Down</h2>
  <p>Scroll down to see the sticky effect.</p>
</div>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
</ul>

<h3>Sticky Navigation Bar Example</h3>
<p>The navbar will <strong>stick</strong> to the top when you reach its scroll position.</p>
<p><strong>Note:</strong> Internet Explorer do not support sticky positioning and Safari requires a -webkit- 

prefix.</p>
<p>Some text to enable scrolling. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
<p>Some text to enable scrolling. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
<p>Some text to enable scrolling. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
<p>Some text to enable scrolling. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
<p>Some text to enable scrolling. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
<p>Some text to enable scrolling. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
<p>Some text to enable scrolling. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>

</body>
</html>




Responsive Topnav

How to use CSS media queries to create a responsive top navigation is shown below:



<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {margin: 0;}

ul.topnav {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

ul.topnav li {float: left;}

ul.topnav li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

ul.topnav li a:hover:not(.active) {background-color: #111;}

ul.topnav li a.active {background-color: #04AA6D;}

ul.topnav li.right {float: right;}

@media screen and (max-width: 600px) {
  ul.topnav li.right, 
  ul.topnav li {float: none;}
}
</style>
</head>
<body>

<ul class="topnav">
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li class="right"><a href="#about">About</a></li>
</ul>

<div style="padding:0 16px;">
  <h2>Responsive Topnav Example</h2>
  <p>This example use media queries to stack the topnav vertically when the screen size is 600px or 

less.</p>
  <p>You will learn more about media queries and responsive web design later in our CSS Tutorial.</p>
  <h4>Resize the browser window to see the effect.</h4>
</div>

</body>
</html>




Responsive Sidenav

How to use CSS media queries to create a responsive side navigation.


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {margin: 0;}

ul.sidenav {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 25%;
  background-color: #f1f1f1;
  position: fixed;
  height: 100%;
  overflow: auto;
}

ul.sidenav li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}
 
ul.sidenav li a.active {
  background-color: #4CAF50;
  color: white;
}

ul.sidenav li a:hover:not(.active) {
  background-color: #555;
  color: white;
}

div.content {
  margin-left: 25%;
  padding: 1px 16px;
  height: 1000px;
}

@media screen and (max-width: 900px) {
  ul.sidenav {
    width: 100%;
    height: auto;
    position: relative;
  }
  
  ul.sidenav li a {
    float: left;
    padding: 15px;
  }
  
  div.content {margin-left: 0;}
}

@media screen and (max-width: 400px) {
  ul.sidenav li a {
    text-align: center;
    float: none;
  }
}
</style>
</head>
<body>

<ul class="sidenav">
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<div class="content">
  <h2>Responsive Sidenav Example</h2>
  <p>This example use media queries to transform the sidenav to a top navigation bar when the screen size is 

900px or less.</p>
  <p>We have also added a media query for screens that are 400px or less, which will vertically stack and 

center the navigation links.</p>
  <p>You will learn more about media queries and responsive web design later in our CSS Tutorial.</p>
  <h3>Resize the browser window to see the effect.</h3>
</div>

</body>
</html>




Dropdown Navbar

How to add a dropdown menu inside a navigation bar.


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a, .dropbtn {
  display: inline-block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover, .dropdown:hover .dropbtn {
  background-color: red;
}

li.dropdown {
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown-content a:hover {background-color: #f1f1f1;}

.dropdown:hover .dropdown-content {
  display: block;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li class="dropdown">
    <a href="javascript:void(0)" class="dropbtn">Dropdown</a>
    <div class="dropdown-content">
      <a href="#">Link 1</a>
      <a href="#">Link 2</a>
      <a href="#">Link 3</a>
    </div>
  </li>
</ul>

<h3>Dropdown Menu inside a Navigation Bar</h3>
<p>Hover over the "Dropdown" link to see the dropdown menu.</p>

</body>
</html>






CSS Dropdowns;

This section shows how to add hoverable dropdown with CSS:

Basic Dropdown:::
Create a dropdown box that appears when the user moves the mouse over an element,as shown below:


<!DOCTYPE html>
<html>
<head>
<style>
.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  padding: 12px 16px;
  z-index: 1;
}

.dropdown:hover .dropdown-content {
  display: block;
}
</style>
</head>
<body>

<h2>Hoverable Dropdown</h2>
<p>Move the mouse over the text below to open the dropdown content.</p>

<div class="dropdown">
  <span>Mouse over me</span>
  <div class="dropdown-content">
  <p>Hello World!</p>
  </div>
</div>

</body>
</html>


In the example above:

HTML:

Use <span> element to open the dropdown. You can also use <button> element

Use container element like <div> to create content of the drop-down and add whatever you want to include 

inside it. 

wrap a <div> element around elements to position drop-down correctly with CSS


css:

The .dropdown class uses position:relative, which is needed when we want the dropdown content to be placed 

right below the dropdown button (using position:absolute).

The .dropdown-content class holds the actual dropdown content. It is hidden by default, and will be 

displayed on hover (see below).

Note: Here, we have set the min-width to 160px. You can change it to suit your taste.

Tip: To make the width of drop-down content to be as wide as the dropdown button, set the width to 100% (and 

overflow:auto; to enable scroll on small screens)

To make dropdown menu look like a card, rather than a border, we have set CSS box-shadow property, not 

border.


The :hover selector is used to show the dropdown menu when the user moves the mouse over the dropdown 

button.



Dropdown Menu

Create a dropdown menu that allows the user to choose an option from a list as illustrated below:

<!DOCTYPE html>
<html>
<head>
<style>
.dropbtn {
  background-color: #4CAF50;
  color: white;
  padding: 16px;
  font-size: 16px;
  border: none;
  cursor: pointer;
}

.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

.dropdown-content a:hover {background-color: #f1f1f1}

.dropdown:hover .dropdown-content {
  display: block;
}

.dropdown:hover .dropbtn {
  background-color: #3e8e41;
}
</style>
</head>
<body>

<h2>Dropdown Menu</h2>
<p>Move the mouse over the button to open the dropdown menu.</p>

<div class="dropdown">
  <button class="dropbtn">Dropdown</button>
  <div class="dropdown-content">
  <a href="#">Link 1</a>
  <a href="#">Link 2</a>
  <a href="#">Link 3</a>
  </div>
</div>

<p><strong>Note:</strong> We use href="#" for test links. In a real web site this would be URLs.</p>

</body>
</html>





Right-aligned Dropdown Content


To make dropdown menu go from right to left instead of left to right, add right:0; in the styling as shown 

below:

<!DOCTYPE html>
<html>
<head>
<style>
.dropbtn {
  background-color: #4CAF50;
  color: white;
  padding: 16px;
  font-size: 16px;
  border: none;
  cursor: pointer;
}

.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  right: 0;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

.dropdown-content a:hover {background-color: #f1f1f1;}

.dropdown:hover .dropdown-content {
  display: block;
}

.dropdown:hover .dropbtn {
  background-color: #3e8e41;
}
</style>
</head>
<body>

<h2>Aligned Dropdown Content</h2>
<p>Determine whether the dropdown content should go from left to right or right to left with the left and 

right properties.</p>

<div class="dropdown" style="float:left;">
  <button class="dropbtn">Left</button>
  <div class="dropdown-content" style="left:0;">
  <a href="#">Link 1</a>
  <a href="#">Link 2</a>
  <a href="#">Link 3</a>
  </div>
</div>

<div class="dropdown" style="float:right;">
  <button class="dropbtn">Right</button>
  <div class="dropdown-content">
  <a href="#">Link 1</a>
  <a href="#">Link 2</a>
  <a href="#">Link 3</a>
  </div>
</div>

</body>
</html>



Dropdown Image

How to add an image and other content inside the dropdown box.


<!DOCTYPE html>
<html>
<head>
<style>
.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown:hover .dropdown-content {
  display: block;
}

.desc {
  padding: 15px;
  text-align: center;
}
</style>
</head>
<body>

<h2>Dropdown Image</h2>
<p>Move the mouse over the image below to open the dropdown content.</p>

<div class="dropdown">
  <img src="img_5terre.jpg" alt="Cinque Terre" width="100" height="50">
  <div class="dropdown-content">
  <img src="img_5terre.jpg" alt="Cinque Terre" width="300" height="200">
  <div class="desc">Beautiful Cinque Terre</div>
  </div>
</div>

</body>
</html>




Dropdown Navbar

How to add a dropdown menu inside a navigation bar:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a, .dropbtn {
  display: inline-block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover, .dropdown:hover .dropbtn {
  background-color: red;
}

li.dropdown {
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown-content a:hover {background-color: #f1f1f1;}

.dropdown:hover .dropdown-content {
  display: block;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li class="dropdown">
    <a href="javascript:void(0)" class="dropbtn">Dropdown</a>
    <div class="dropdown-content">
      <a href="#">Link 1</a>
      <a href="#">Link 2</a>
      <a href="#">Link 3</a>
    </div>
  </li>
</ul>

<h3>Dropdown Menu inside a Navigation Bar</h3>
<p>Hover over the "Dropdown" link to see the dropdown menu.</p>

</body>
</html>






CSS Image Gallery;


You can create an image gallery with CSS as illustrated below:

<!DOCTYPE html>
<html>
<head>
<style>
div.gallery {
  margin: 5px;
  border: 1px solid #ccc;
  float: left;
  width: 180px;
}

div.gallery:hover {
  border: 1px solid #777;
}

div.gallery img {
  width: 100%;
  height: auto;
}

div.desc {
  padding: 15px;
  text-align: center;
}
</style>
</head>
<body>

<div class="gallery">
  <a target="_blank" href="img_5terre.jpg">
    <img src="img_5terre.jpg" alt="Cinque Terre" width="600" height="400">
  </a>
  <div class="desc">Add a description of the image here</div>
</div>

<div class="gallery">
  <a target="_blank" href="img_forest.jpg">
    <img src="img_forest.jpg" alt="Forest" width="600" height="400">
  </a>
  <div class="desc">Add a description of the image here</div>
</div>

<div class="gallery">
  <a target="_blank" href="img_lights.jpg">
    <img src="img_lights.jpg" alt="Northern Lights" width="600" height="400">
  </a>
  <div class="desc">Add a description of the image here</div>
</div>

<div class="gallery">
  <a target="_blank" href="img_mountains.jpg">
    <img src="img_mountains.jpg" alt="Mountains" width="600" height="400">
  </a>
  <div class="desc">Add a description of the image here</div>
</div>

</body>
</html>


Responsive Image Gallery

How to use CSS media queries to create a responsive image gallery that will look good on desktops, tablets 

and smart phones.


<!DOCTYPE html>
<html>
<head>
<style>
div.gallery {
  border: 1px solid #ccc;
}

div.gallery:hover {
  border: 1px solid #777;
}

div.gallery img {
  width: 100%;
  height: auto;
}

div.desc {
  padding: 15px;
  text-align: center;
}

* {
  box-sizing: border-box;
}

.responsive {
  padding: 0 6px;
  float: left;
  width: 24.99999%;
}

@media only screen and (max-width: 700px) {
  .responsive {
    width: 49.99999%;
    margin: 6px 0;
  }
}

@media only screen and (max-width: 500px) {
  .responsive {
    width: 100%;
  }
}

.clearfix:after {
  content: "";
  display: table;
  clear: both;
}
</style>
</head>
<body>

<h2>Responsive Image Gallery</h2>

<h4>Resize the browser window to see the effect.</h4>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_5terre.jpg">
      <img src="img_5terre.jpg" alt="Cinque Terre" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
  </div>
</div>


<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_forest.jpg">
      <img src="img_forest.jpg" alt="Forest" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
  </div>
</div>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_lights.jpg">
      <img src="img_lights.jpg" alt="Northern Lights" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
  </div>
</div>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_mountains.jpg">
      <img src="img_mountains.jpg" alt="Mountains" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
  </div>
</div>

<div class="clearfix"></div>

<div style="padding:6px;">
  <p>This example use media queries to re-arrange the images on different screen sizes: for screens larger 

than 700px wide, it will show four images side by side, for screens smaller than 700px, it will show two 

images side by side. For screens smaller than 500px, the images will stack vertically (100%).</p>
  <p>You will learn more about media queries and responsive web design later in our CSS Tutorial.</p>
</div>

</body>
</html>



CSS Image Sprites


An image sprite is a collection of images put into a single image to reduce the number of server requests, 

save bandwidths and reduce the loading time of a page caused by multiple server requests. 



Simple Example: Image Sprites:::

Image sprites enables us to show just the part of the image we need. Within a composite of multiple images. 

See illustration below:

<!DOCTYPE html>
<html>
<head>
<style>
#home {
  width: 46px;
  height: 44px;
  background: url(img_navsprites.gif) 0 0;
}

#next {
  width: 43px;
  height: 44px;
  background: url(img_navsprites.gif) -91px 0;
}
</style>
</head>
<body>

<img id="home" src="img_trans.gif" width="1" height="1">
<img id="next" src="img_trans.gif" width="1" height="1">

</body>
</html>


In the example above,


    <img id="home" src="img_trans.gif"> - Only defines a small transparent image because the src attribute 

cannot be empty. The displayed image will be the background image we specify in CSS
    width: 46px; height: 44px; - Defines the portion of the image we want to use
    background: url(img_navsprites.gif) 0 0; - Defines the background image and its position (left 0px, top 

0px)






Image Sprites - Create a Navigation List

The illustration below shows the creation of navigation list using sprite image ("img_navsprites.gif"). An 

HTML list is used here because it  can be a list and supports background image as well. See the illustration 

below now:


<!DOCTYPE html>
<html>
<head>
<style>
#navlist {
  position: relative;
}

#navlist li {
  margin: 0;
  padding: 0;
  list-style: none;
  position: absolute;
  top: 0;
}

#navlist li, #navlist a {
  height: 44px;
  display: block;
}

#home {
  left: 0px;
  width: 46px;
  background: url('img_navsprites.gif') 0 0;
}

#prev {
  left: 63px;
  width: 43px;
  background: url('img_navsprites.gif') -47px 0;
}

#next {
  left: 129px;
  width: 43px;
  background: url('img_navsprites.gif') -91px 0;
}
</style>
</head>
<body>

<ul id="navlist">
  <li id="home"><a href="default.asp"></a></li>
  <li id="prev"><a href="css_intro.asp"></a></li>
  <li id="next"><a href="css_syntax.asp"></a></li>
</ul>

</body>
</html>


Explanation for the example above: 


    #navlist {position:relative;} - position is set to relative to allow absolute positioning inside it
    #navlist li {margin:0;padding:0;list-style:none;position:absolute;top:0;} - margin and padding are set 

to 0, list-style is removed, and all list items are absolute positioned
    #navlist li, #navlist a {height:44px;display:block;} - the height of all the images are 44px


Positioning and Styling each specific part:


    #home {left:0px;width:46px;} - Positioned all the way to the left, and the width of the image is 46px
    #home {background:url(img_navsprites.gif) 0 0;} - Defines the background image and its position (left 

0px, top 0px)
    #prev {left:63px;width:43px;} - Positioned 63px to the right (#home width 46px + some extra space 

between items), and the width is 43px.
    #prev {background:url('img_navsprites.gif') -47px 0;} - Defines the background image 47px to the right 

(#home width 46px + 1px line divider)
    #next {left:129px;width:43px;}- Positioned 129px to the right (start of #prev is 63px + #prev width 43px 

+ extra space), and the width is 43px.
    #next {background:url('img_navsprites.gif') -91px 0;} - Defines the background image 91px to the right 

(#home width 46px + 1px line divider + #prev width 43px + 1px line divider )



Image Sprites - Hover Effect:::

Here, we will add hover effect to the navigation list. Note that the :hover selector can be used on all 

elements including, but not limited to, links. 


<!DOCTYPE html>
<html>
<head>
<style>
#navlist {
  position: relative;
}

#navlist li {
  margin: 0;
  padding: 0;
  list-style: none;
  position: absolute;
  top: 0;
}

#navlist li, #navlist a {
  height: 44px;
  display: block;
}

#home {
  left: 0px;
  width: 46px;
  background: url('img_navsprites_hover.gif') 0 0;
}

#prev {
  left: 63px;
  width: 43px;
  background: url('img_navsprites_hover.gif') -47px 0;
}

#next {
  left: 129px;
  width: 43px;
  background: url('img_navsprites_hover.gif') -91px 0;
}

#home a:hover {
  background: url('img_navsprites_hover.gif') 0 -45px;
}

#prev a:hover {
  background: url('img_navsprites_hover.gif') -47px -45px;
}

#next a:hover {
  background: url('img_navsprites_hover.gif') -91px -45px;
}
</style>
</head>
<body>

<ul id="navlist">
  <li id="home"><a href="default.asp"></a></li>
  <li id="prev"><a href="css_intro.asp"></a></li>
  <li id="next"><a href="css_syntax.asp"></a></li>
</ul>

</body>
</html>


Explanation of the example above:

    #home a:hover {background: url('img_navsprites_hover.gif') 0 -45px;} - For all three hover images we 

specify the same background position, only 45px further down





CSS Attribute Selectors;


Style HTML Elements With Specific Attributes

You can style HTML elements with specifit attributes or attribute values. 



The [attribute] selector is used to select elements with a specified attribute.

The following example selects all <a> elements with a target attribute:


<!DOCTYPE html>
<html>
<head>
<style>
a[target] {
  background-color: yellow;
}
</style>
</head>
<body>

<h2>CSS [attribute] Selector</h2>
<p>The links with a target attribute gets a yellow background:</p>

<a href="https://www.w3schools.com">w3schools.com</a>
<a href="http://www.disney.com" target="_blank">disney.com</a>
<a href="http://www.wikipedia.org" target="_top">wikipedia.org</a>

</body>
</html>



CSS [attribute="value"] Selector

The [attribute="value"] selector is used to select elements with a specified attribute and value.

The following example selects all <a> elements with a target="_blank" attribute:


<!DOCTYPE html>
<html>
<head>
<style>
a[target=_blank] {
  background-color: yellow;
}
</style>
</head>
<body>

<h2>CSS [attribute="value"] Selector</h2>
<p>The link with target="_blank" gets a yellow background:</p>

<a href="https://www.w3schools.com">w3schools.com</a>
<a href="http://www.disney.com" target="_blank">disney.com</a>
<a href="http://www.wikipedia.org" target="_top">wikipedia.org</a>

</body>
</html>



CSS [attribute~="value"] Selector


The [attribute~="value"] selector is used to select elements with an attribute value containing a specified 

word.

The following example selects all elements with a title attribute that contains a space-separated list of 

words, one of which is "flower": 


<!DOCTYPE html>
<html>
<head>
<style>
[title~=flower] {
  border: 5px solid yellow;
}
</style>
</head>
<body>

<h2>CSS [attribute~="value"] Selector</h2>
<p>All images with the title attribute containing the word "flower" get a yellow border.</p>

<img src="klematis.jpg" title="klematis flower" width="150" height="113">
<img src="img_flwr.gif" title="flower" width="224" height="162">
<img src="img_tree.gif" title="tree" width="200" height="358">

</body>
</html>


The example above will match elements with title="flower", title="summer flower", and title="flower new", 

but not title="my-flower" or title="flowers".



CSS [attribute|="value"] Selector

The [attribute|="value"] selector is used to select elements with the specified attribute starting with the 

specified value.

The following example selects all elements with a class attribute value that begins with "top".

Note: The value has to be a whole word, either alone, like class="top", or followed by a hyphen( - ), like 

class="top-text"! 


See example below: 

<!DOCTYPE html>
<html>
<head>
<style>
[class|=top] {
  background: yellow;
}
</style>
</head>
<body>

<h2>CSS [attribute|="value"] Selector</h2>

<h1 class="top-header">Welcome</h1>
<p class="top-text">Hello world!</p>
<p class="topcontent">Are you learning CSS?</p>

</body>
</html>




CSS [attribute^="value"] Selector

The [attribute^="value"] selector is used to select elements whose attribute value begins with a specified 

value.

The following example selects all elements with a class attribute value that begins with "top":

Note: The value does not have to be a whole word! In this case topcontent and top-content are both selected.


<!DOCTYPE html>
<html>
<head>
<style>
[class^="top"] {
  background: yellow;
}
</style>
</head>
<body>

<h2>CSS [attribute^="value"] Selector</h2>

<h1 class="top-header">Welcome</h1>
<p class="top-text">Hello world!</p>
<p class="topcontent">Are you learning CSS?</p>

</body>
</html>



CSS [attribute$="value"] Selector

The [attribute$="value"] selector is used to select elements whose attribute value ends with a specified 

value.

The following example selects all elements with a class attribute value that ends with "test":

Note: The value does not have to be a whole word!  

<!DOCTYPE html>
<html>
<head>
<style> 
[class$="test"] {
  background: yellow;
}
</style>
</head>
<body>

<h2>CSS [attribute$="value"] Selector</h2>

<div class="first_test">The first div element.</div>
<div class="second">The second div element.</div>
<div class="my-test">The third div element.</div>
<p class="mytest">This is some text in a paragraph.</p>

</body>
</html>


CSS [attribute*="value"] Selector

The [attribute*="value"] selector is used to select elements whose attribute value contains a specified 

value.

The following example selects all elements with a class attribute value that contains "te":

Note: The value does not have to be a whole word!  


<!DOCTYPE html>
<html>
<head>
<style> 
[class*="te"] {
  background: yellow;
}
</style>
</head>
<body>

<h2>CSS [attribute*="value"] Selector</h2>

<div class="first_test">The first div element.</div>
<div class="second">The second div element.</div>
<div class="my-test">The third div element.</div>
<p class="mytest">This is some text in a paragraph.</p>

</body>
</html>


Styling Forms

The attribute selectors can be useful for styling forms without class or ID:


<!DOCTYPE html>
<html>
<head>
<style>
input[type=text] {
  width: 150px;
  display: block;
  margin-bottom: 10px;
  background-color: yellow;
}

input[type=button] {
  width: 120px;
  margin-left: 35px;
  display: block;
}
</style>
</head>
<body>

<h2>Styling Forms</h2>

<form name="input" action="" method="get">
  Firstname:<input type="text" name="Name" value="Peter" size="20">
  Lastname:<input type="text" name="Name" value="Griffin" size="20">
  <input type="button" value="Example Button">
</form>

</body>
</html>




All CSS Attribute Selectors
Selector 	Example 	Example description
[attribute] 	[target] 	Selects all elements with a target attribute
[attribute=value] 	[target=_blank] 	Selects all elements with target="_blank"
[attribute~=value] 	[title~=flower] 	Selects all elements with a title attribute containing the 

word "flower"
[attribute|=value] 	[lang|=en] 	Selects all elements with a lang attribute value starting with "en"
[attribute^=value] 	a[href^="https"] 	Selects every <a> element whose href attribute value begins 

with "https"
[attribute$=value] 	a[href$=".pdf"] 	Selects every <a> element whose href attribute value ends 

with ".pdf"
[attribute*=value] 	a[href*="w3schools"] 	Selects every <a> element whose href attribute value 

contains the substring "w3schools"




CSS Forms

CSS can enhance the looks of an HTML form. 


<!DOCTYPE html>
<html>
<style>
input[type=text], select {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
}

input[type=submit] {
  width: 100%;
  background-color: #4CAF50;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

input[type=submit]:hover {
  background-color: #45a049;
}

div {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
}
</style>
<body>

<h3>Using CSS to style an HTML Form</h3>

<div>
  <form action="/action_page.php">
    <label for="fname">First Name</label>
    <input type="text" id="fname" name="firstname" placeholder="Your name..">

    <label for="lname">Last Name</label>
    <input type="text" id="lname" name="lastname" placeholder="Your last name..">

    <label for="country">Country</label>
    <select id="country" name="country">
      <option value="australia">Australia</option>
      <option value="canada">Canada</option>
      <option value="usa">USA</option>
    </select>
  
    <input type="submit" value="Submit">
  </form>
</div>

</body>
</html>



Styling Input Fields

Use the width property to determine the width of the input field:


<!DOCTYPE html>
<html>
<head>
<style> 
input {
  width: 100%;
}
</style>
</head>
<body>

<h2>A full-width input field</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname">
</form>

</body>
</html>


The example above applies to all <input> elements. If you only want to style a specific input type, you can 

use attribute selectors:

    input[type=text] - will only select text fields
    input[type=password] - will only select password fields
    input[type=number] - will only select number fields
    etc..


Padded Inputs

Use the padding property to add space inside the text field.

Tip: When you have many inputs after each other, you might also want to add some margin, to add more space 

outside of them:

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
}
</style>
</head>
<body>

<h2>Padded input fields</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname">
</form>

</body>
</html>



Note that we have set the box-sizing property to border-box. This makes sure that the padding and eventually 

borders are included in the total width and height of the elements. 


Bordered Inputs

Use the border property to change the border size and color, and use the border-radius property to add 

rounded corners:

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 2px solid red;
  border-radius: 4px;
}
</style>
</head>
<body>

<h2>Input fields with borders</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname">
</form>

</body>
</html>


use border-bottom property is you only want a bottom border, as shown below:

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: none;
  border-bottom: 2px solid red;
}
</style>
</head>
<body>

<h2>Input fields with bottom border</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname">
</form>

</body>
</html>




Colored Inputs

Use the background-color property to add a background color to the input, and the color property to change 

the text color: 

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: none;
  background-color: #3CBC8D;
  color: white;
}
</style>
</head>
<body>

<h2>Input fields with color</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname" value="John">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname" value="Doe">
</form>

</body>
</html>




Focused Inputs

By default, some browsers will add a blue outline around the input when it gets focus (clicked on). You can 

remove this behavior by adding outline: none; to the input.

Use the :focus selector to do something with the input field when it gets focus:


<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 1px solid #555;
  outline: none;
}

input[type=text]:focus {
  background-color: lightblue;
}
</style>
</head>
<body>

<h2>Input fields with color on :focus</h2>

<p>Here, the input field gets a color when it gets focus (clicked on):</p>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname" value="John">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname" value="Doe">
</form>

</body>
</html>



To change to a lightblue line during focus:


<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 3px solid #ccc;
  -webkit-transition: 0.5s;
  transition: 0.5s;
  outline: none;
}

input[type=text]:focus {
  border: 3px solid #555;
}
</style>
</head>
<body>

<h2>Input fields with black border on :focus</h2>

<p>Here, the input field gets a black border color when it gets focus (clicked on). We have also added the 

CSS transition property to animate the border color (takes 0.5 seconds to change the color on focus):</p>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname" value="John">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname" value="Doe">
</form>

</body>
</html>



Input with icon/image

If you want an icon inside the input, use the background-image property and position it with the 

background-position property. Also notice that we add a large left padding to reserve the space of the icon:

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  box-sizing: border-box;
  border: 2px solid #ccc;
  border-radius: 4px;
  font-size: 16px;
  background-color: white;
  background-image: url('searchicon.png');
  background-position: 10px 10px; 
  background-repeat: no-repeat;
  padding: 12px 20px 12px 40px;
}
</style>
</head>
<body>

<h2>Input field with an icon inside</h2>

<form>
  <input type="text" name="search" placeholder="Search..">
</form>

</body>
</html>



Animated Search Input

In this example we use the CSS transition property to animate the width of the search input when it gets 

focus. You will learn more about the transition property later, in our CSS Transitions chapter.

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 130px;
  box-sizing: border-box;
  border: 2px solid #ccc;
  border-radius: 4px;
  font-size: 16px;
  background-color: white;
  background-image: url('searchicon.png');
  background-position: 10px 10px; 
  background-repeat: no-repeat;
  padding: 12px 20px 12px 40px;
  transition: width 0.4s ease-in-out;
}

input[type=text]:focus {
  width: 100%;
}
</style>
</head>
<body>

<h2>Animate width of search input</h2>

<form>
  <input type="text" name="search" placeholder="Search..">
</form>

</body>
</html>



Styling Textareas

Tip: Use the resize property to prevent textareas from being resized (disable the "grabber" in the bottom 

right corner):

<!DOCTYPE html>
<html>
<head>
<style> 
textarea {
  width: 100%;
  height: 150px;
  padding: 12px 20px;
  box-sizing: border-box;
  border: 2px solid #ccc;
  border-radius: 4px;
  background-color: #f8f8f8;
  font-size: 16px;
  resize: none;
}
</style>
</head>
<body>

<h2>Styling textarea</h2>

<p><strong>Tip:</strong> Use the resize property to prevent textareas from being resized (disable the 

"grabber" in the bottom right corner):</p>

<form>
  <textarea>Some text...</textarea>
</form>

</body>
</html>




Styling Select Menus

See illustration below:


<!DOCTYPE html>
<html>
<head>
<style> 
select {
  width: 100%;
  padding: 16px 20px;
  border: none;
  border-radius: 4px;
  background-color: #f1f1f1;
}
</style>
</head>
<body>

<h2>Styling a select menu</h2>

<form>
  <select id="country" name="country">
  <option value="au">Australia</option>
  <option value="ca">Canada</option>
  <option value="usa">USA</option>
  </select>
</form>

</body>
</html>



Styling Input Buttons

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=button], input[type=submit], input[type=reset] {
  background-color: #4CAF50;
  border: none;
  color: white;
  padding: 16px 32px;
  text-decoration: none;
  margin: 4px 2px;
  cursor: pointer;
}
</style>
</head>
<body>

<h2>Styling form buttons</h2>

<input type="button" value="Button">
<input type="reset" value="Reset">
<input type="submit" value="Submit">

</body>
</html>


See CSS Buttons tutorial here: https://www.w3schools.com/css/css3_buttons.asp

Responsive Form

Resize the browser window to see the effect. When the screen is less than 600px wide, make the two columns 

stack on top of each other instead of next to each other.

Advanced: The following example use media queries to create a responsive form. You will learn more about 

this in a later chapter.



<!DOCTYPE html>
<html>
<head>
<style>
* {
  box-sizing: border-box;
}

input[type=text], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  resize: vertical;
}

label {
  padding: 12px 12px 12px 0;
  display: inline-block;
}

input[type=submit] {
  background-color: #4CAF50;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  float: right;
}

input[type=submit]:hover {
  background-color: #45a049;
}

.container {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
}

.col-25 {
  float: left;
  width: 25%;
  margin-top: 6px;
}

.col-75 {
  float: left;
  width: 75%;
  margin-top: 6px;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Responsive layout - when the screen is less than 600px wide, make the two columns stack on top of each 

other instead of next to each other */
@media screen and (max-width: 600px) {
  .col-25, .col-75, input[type=submit] {
    width: 100%;
    margin-top: 0;
  }
}
</style>
</head>
<body>

<h2>Responsive Form</h2>
<p>Resize the browser window to see the effect. When the screen is less than 600px wide, make the two 

columns stack on top of each other instead of next to each other.</p>

<div class="container">
  <form action="/action_page.php">
  <div class="row">
    <div class="col-25">
      <label for="fname">First Name</label>
    </div>
    <div class="col-75">
      <input type="text" id="fname" name="firstname" placeholder="Your name..">
    </div>
  </div>
  <div class="row">
    <div class="col-25">
      <label for="lname">Last Name</label>
    </div>
    <div class="col-75">
      <input type="text" id="lname" name="lastname" placeholder="Your last name..">
    </div>
  </div>
  <div class="row">
    <div class="col-25">
      <label for="country">Country</label>
    </div>
    <div class="col-75">
      <select id="country" name="country">
        <option value="australia">Australia</option>
        <option value="canada">Canada</option>
        <option value="usa">USA</option>
      </select>
    </div>
  </div>
  <div class="row">
    <div class="col-25">
      <label for="subject">Subject</label>
    </div>
    <div class="col-75">
      <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea>
    </div>
  </div>
  <br>
  <div class="row">
    <input type="submit" value="Submit">
  </div>
  </form>
</div>

</body>
</html>





CSS Counters


They are CSS-maintained variables whose values can be incremental by CSS rules (to track the number of times 

they are used).  You can also use counters to adjust appearance of content based on its placement in the 

document.


Automatic Numbering With Counters

CSS counters are like "variables". The variable values can be incremented by CSS rules (which will track how 

many times they are used).

To work with CSS counters we will use the following properties:

    counter-reset - Creates or resets a counter
    counter-increment - Increments a counter value
    content - Inserts generated content
    counter() or counters() function - Adds the value of a counter to an element

To use a CSS counter, it must first be created with counter-reset.


To illustrate, the example below creates a counter for the page (in the body selector), increments the 

counter value for each <h2> element and adds "Section <value of the counter>:" to the beginning of each <h2> 

element:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  counter-reset: section;
}

h2::before {
  counter-increment: section;
  content: "Section " counter(section) ": ";
}
</style>
</head>
<body>

<h1>Using CSS Counters</h1>

<h2>HTML Tutorial</h2>
<h2>CSS Tutorial</h2>
<h2>JavaScript Tutorial</h2>
<h2>Python Tutorial</h2>
<h2>SQL Tutorial</h2>

</body>
</html>


In the example above, this is what the outcome looks like:


Using CSS Counters

Section 1: HTML Tutorial
Section 2: CSS Tutorial
Section 3: JavaScript Tutorial
Section 4: Python Tutorial
Section 5: SQL Tutorial

And when you highlight, the 'Section 1' through 5 is not highlighted as it is automatically generated from 

CSS. 





Nesting Counters

The following example creates one counter for the page (section) and one counter for each <h1> element 

(subsection). The "section" counter will be counted for each <h1> element with "Section <value of the 

section counter>.", and the "subsection" counter will be counted for each <h2> element with "<value of the 

section counter>.<value of the subsection counter>":


<!DOCTYPE html>
<html>
<head>
<style>
body {
  counter-reset: section;
}

h1 {
  counter-reset: subsection;
}

h1::before {
  counter-increment: section;
  content: "Section " counter(section) ". ";
}

h2::before {
  counter-increment: subsection;
  content: counter(section) "." counter(subsection) " ";
}
</style>
</head>
<body>


<h1>HTML/CSS Tutorials</h1>
<h2>HTML</h2>
<h2>CSS</h2>
<h2>Bootstrap</h2>
<h2>W3.CSS</h2>

<h1>Scripting Tutorials</h1>
<h2>JavaScript</h2>
<h2>jQuery</h2>
<h2>React</h2>

<h1>Programming Tutorials</h1>
<h2>Python</h2>
<h2>Java</h2>
<h2>C++</h2>

</body>
</html>


The nested counters above are displayed like this:

Section 1. HTML/CSS Tutorials

1.1 HTML
1.2 CSS
1.3 Bootstrap
1.4 W3.CSS

Section 2. Scripting Tutorials

2.1 JavaScript
2.2 jQuery
2.3 React

Section 3. Programming Tutorials

3.1 Python
3.2 Java
3.3 C++



A counter can also be useful to make outlined lists because a new instance of a counter is automatically 

created in child elements. Here we use the counters() function to insert a string between different levels 

of nested counters:

<!DOCTYPE html>
<html>
<head>
<style>
ol {
  counter-reset: section;
  list-style-type: none;
}

li::before {
  counter-increment: section;
  content: counters(section,".") " ";
}
</style>
</head>
<body>

<ol>
  <li>item</li>
  <li>item   
  <ol>
    <li>item</li>
    <li>item</li>
    <li>item
    <ol>
      <li>item</li>
      <li>item</li>
      <li>item</li>
    </ol>
    </li>
    <li>item</li>
  </ol>
  </li>
  <li>item</li>
  <li>item</li>
</ol>

<ol>
  <li>item</li>
  <li>item</li>
</ol>

</body>
</html>


The counter above is rendered as shown below:


    1 item
    2 item
        2.1 item
        2.2 item
        2.3 item
            2.3.1 item
            2.3.2 item
            2.3.3 item
        2.4 item
    3 item
    4 item

    1 item
    2 item


CSS Counter Properties
Property 	Description
content 	Used with the ::before and ::after pseudo-elements, to insert generated content
counter-increment 	Increments one or more counter values
counter-reset 	Creates or resets one or more counters
counter() 	Returns the current value of the named counter






CSS Website Layout

Website Layout

A website is often divided into headers, menus, content and a footer:

There are tons of different layout designs to choose from. However, the structure above, is one of the most 

common, and we will take a closer look at it in this tutorial.


Header

A header is usually located at the top of the website (or right below a top navigation menu). It often 

contains a logo or the website name:


<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS Website Layout</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {
  margin: 0;
}

/* Style the header */
.header {
  background-color: #f1f1f1;
  padding: 20px;
  text-align: center;
}
</style>
</head>
<body>

<div class="header">
  <h1>Header</h1>
</div>

</body>
</html>



Navigation Bar


A navigation bar contains a list of links to help visitors navigating through your website:


<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS Website Layout</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
}

/* Style the header */
.header {
  background-color: #f1f1f1;
  padding: 20px;
  text-align: center;
}

/* Style the top navigation bar */
.topnav {
  overflow: hidden;
  background-color: #333;
}

/* Style the topnav links */
.topnav a {
  float: left;
  display: block;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

/* Change color on hover */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}
</style>
</head>
<body>

<div class="header">
  <h1>Header</h1>
</div>

<div class="topnav">
  <a href="#">Link</a>
  <a href="#">Link</a>
  <a href="#">Link</a>
</div>

</body>
</html>



Content

The layout in this section, often depends on the target users. The most common layout is one (or combining 

them) of the following:

    1-column (often used for mobile browsers)
    2-column (often used for tablets and laptops)
    3-column layout (only used for desktops)

We will create a 3-column layout, and change it to a 1-column layout on smaller screens:


<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS Website Layout</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
}

/* Style the header */
.header {
  background-color: #f1f1f1;
  padding: 20px;
  text-align: center;
}

/* Style the top navigation bar */
.topnav {
  overflow: hidden;
  background-color: #333;
}

/* Style the topnav links */
.topnav a {
  float: left;
  display: block;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

/* Change color on hover */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}

/* Create three equal columns that floats next to each other */
.column {
  float: left;
  width: 33.33%;
  padding: 15px;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Responsive layout - makes the three columns stack on top of each other instead of next to each other */
@media screen and (max-width:600px) {
  .column {
    width: 100%;
  }
}
</style>
</head>
<body>

<div class="header">
  <h1>Header</h1>
  <p>Resize the browser window to see the responsive effect.</p>
</div>

<div class="topnav">
  <a href="#">Link</a>
  <a href="#">Link</a>
  <a href="#">Link</a>
</div>

<div class="row">
  <div class="column">
    <h2>Column</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas sit amet pretium urna. Vivamus 

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque vehicula, risus eget aliquam 

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent scelerisque tortor sed accumsan 

convallis.</p>
  </div>
  
  <div class="column">
    <h2>Column</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas sit amet pretium urna. Vivamus 

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque vehicula, risus eget aliquam 

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent scelerisque tortor sed accumsan 

convallis.</p>
  </div>
  
  <div class="column">
    <h2>Column</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas sit amet pretium urna. Vivamus 

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque vehicula, risus eget aliquam 

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent scelerisque tortor sed accumsan 

convallis.</p>
  </div>
</div>

</body>
</html>


Tip: To create a 2-column layout, change the width to 50%. To create a 4-column layout, use 25%, etc.
Tip: See CSS Media Queries chapter to learn how the @media rule works

Tip: A more modern way of creating column layouts, is to use CSS Flexbox. However, it is not supported in 

Internet Explorer 10 and earlier versions. If you require IE6-10 support, use floats (as shown above). 



Unequal Columns

The main content is the biggest and the most important part of your site.

It is common with unequal column widths, so that most of the space is reserved for the main content. The 

side content (if any) is often used as an alternative navigation or to specify information relevant to the 

main content. Change the widths as you like, only remember that it should add up to 100% in total:


<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS Website Layout</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
}

/* Style the header */
.header {
  background-color: #f1f1f1;
  padding: 20px;
  text-align: center;
}

/* Style the top navigation bar */
.topnav {
  overflow: hidden;
  background-color: #333;
}

/* Style the topnav links */
.topnav a {
  float: left;
  display: block;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

/* Change color on hover */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}

/* Create three unequal columns that floats next to each other */
.column {
  float: left;
  padding: 10px;
}

/* Left and right column */
.column.side {
  width: 25%;
}

/* Middle column */
.column.middle {
  width: 50%;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Responsive layout - makes the three columns stack on top of each other instead of next to each other */
@media screen and (max-width: 600px) {
  .column.side, .column.middle {
    width: 100%;
  }
}
</style>
</head>
<body>

<div class="header">
  <h1>Header</h1>
  <p>Resize the browser window to see the responsive effect.</p>
</div>

<div class="topnav">
  <a href="#">Link</a>
  <a href="#">Link</a>
  <a href="#">Link</a>
</div>

<div class="row">
  <div class="column side">
    <h2>Side</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit..</p>
  </div>
  
  <div class="column middle">
    <h2>Main Content</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas sit amet pretium urna. Vivamus 

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque vehicula, risus eget aliquam 

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent scelerisque tortor sed accumsan 

convallis.</p>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas sit amet pretium urna. Vivamus 

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque vehicula, risus eget aliquam 

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent scelerisque tortor sed accumsan 

convallis.</p>
  </div>
  
  <div class="column side">
    <h2>Side</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit..</p>
  </div>
</div>
  
</body>
</html>


Footer

The footer is placed at the bottom of your page. It often contains information like copyright and contact 

info:



<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS Website Layout</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
}

/* Style the header */
.header {
  background-color: #f1f1f1;
  padding: 20px;
  text-align: center;
}

/* Style the top navigation bar */
.topnav {
  overflow: hidden;
  background-color: #333;
}

/* Style the topnav links */
.topnav a {
  float: left;
  display: block;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

/* Change color on hover */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}

/* Create three unequal columns that floats next to each other */
.column {
  float: left;
  padding: 10px;
}

/* Left and right column */
.column.side {
  width: 25%;
}

/* Middle column */
.column.middle {
  width: 50%;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Responsive layout - makes the three columns stack on top of each other instead of next to each other */
@media screen and (max-width: 600px) {
  .column.side, .column.middle {
    width: 100%;
  }
}

/* Style the footer */
.footer {
  background-color: #f1f1f1;
  padding: 10px;
  text-align: center;
}
</style>
</head>
<body>

<div class="header">
  <h1>Header</h1>
  <p>Resize the browser window to see the responsive effect.</p>
</div>

<div class="topnav">
  <a href="#">Link</a>
  <a href="#">Link</a>
  <a href="#">Link</a>
</div>

<div class="row">
  <div class="column side">
    <h2>Side</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit..</p>
  </div>
  
  <div class="column middle">
    <h2>Main Content</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas sit amet pretium urna. Vivamus 

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque vehicula, risus eget aliquam 

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent scelerisque tortor sed accumsan 

convallis.</p>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas sit amet pretium urna. Vivamus 

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque vehicula, risus eget aliquam 

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent scelerisque tortor sed accumsan 

convallis.</p>
  </div>
  
  <div class="column side">
    <h2>Side</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit..</p>
  </div>
</div>

<div class="footer">
  <p>Footer</p>
</div>
  
</body>
</html>


Responsive Website Layout

By using some of the CSS code above, we have created a responsive website layout, which varies between two 

columns and full-width columns depending on screen width:


<!DOCTYPE html>
<html>
<head>
<style>
* {
  box-sizing: border-box;
}

body {
  font-family: Arial;
  padding: 10px;
  background: #f1f1f1;
}

/* Header/Blog Title */
.header {
  padding: 30px;
  text-align: center;
  background: white;
}

.header h1 {
  font-size: 50px;
}

/* Style the top navigation bar */
.topnav {
  overflow: hidden;
  background-color: #333;
}

/* Style the topnav links */
.topnav a {
  float: left;
  display: block;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

/* Change color on hover */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}

/* Create two unequal columns that floats next to each other */
/* Left column */
.leftcolumn {   
  float: left;
  width: 75%;
}

/* Right column */
.rightcolumn {
  float: left;
  width: 25%;
  background-color: #f1f1f1;
  padding-left: 20px;
}

/* Fake image */
.fakeimg {
  background-color: #aaa;
  width: 100%;
  padding: 20px;
}

/* Add a card effect for articles */
.card {
  background-color: white;
  padding: 20px;
  margin-top: 20px;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Footer */
.footer {
  padding: 20px;
  text-align: center;
  background: #ddd;
  margin-top: 20px;
}

/* Responsive layout - when the screen is less than 800px wide, make the two columns stack on top of each 

other instead of next to each other */
@media screen and (max-width: 800px) {
  .leftcolumn, .rightcolumn {   
    width: 100%;
    padding: 0;
  }
}

/* Responsive layout - when the screen is less than 400px wide, make the navigation links stack on top of 

each other instead of next to each other */
@media screen and (max-width: 400px) {
  .topnav a {
    float: none;
    width: 100%;
  }
}
</style>
</head>
<body>

<div class="header">
  <h1>My Website</h1>
  <p>Resize the browser window to see the effect.</p>
</div>

<div class="topnav">
  <a href="#">Link</a>
  <a href="#">Link</a>
  <a href="#">Link</a>
  <a href="#" style="float:right">Link</a>
</div>

<div class="row">
  <div class="leftcolumn">
    <div class="card">
      <h2>TITLE HEADING</h2>
      <h5>Title description, Dec 7, 2017</h5>
      <div class="fakeimg" style="height:200px;">Image</div>
      <p>Some text..</p>
      <p>Sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do 

eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud 

exercitation ullamco.</p>
    </div>
    <div class="card">
      <h2>TITLE HEADING</h2>
      <h5>Title description, Sep 2, 2017</h5>
      <div class="fakeimg" style="height:200px;">Image</div>
      <p>Some text..</p>
      <p>Sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do 

eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud 

exercitation ullamco.</p>
    </div>
  </div>
  <div class="rightcolumn">
    <div class="card">
      <h2>About Me</h2>
      <div class="fakeimg" style="height:100px;">Image</div>
      <p>Some text about me in culpa qui officia deserunt mollit anim..</p>
    </div>
    <div class="card">
      <h3>Popular Post</h3>
      <div class="fakeimg"><p>Image</p></div>
      <div class="fakeimg"><p>Image</p></div>
      <div class="fakeimg"><p>Image</p></div>
    </div>
    <div class="card">
      <h3>Follow Me</h3>
      <p>Some text..</p>
    </div>
  </div>
</div>

<div class="footer">
  <h2>Footer</h2>
</div>

</body>
</html>




CSS Units



CSS has several different units for expressing a length.

Many CSS properties take "length" values, such as width, margin, padding, font-size, etc.

Length is a number followed by a length unit, such as 10px, 2em, etc.

<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  font-size: 60px;
}

p {
  font-size: 25px;
  line-height: 50px;
}
</style>
</head>
<body>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>

</body>
</html>






Note: A whitespace cannot appear between the number and the unit. However, if the value is 0, the unit can 

be omitted.

For some CSS properties, negative lengths are allowed.

There are two types of length units: absolute and relative.



Absolute Lengths

The absolute length units are fixed and a length expressed in any of these will appear as exactly that size.

Absolute length units are not recommended for use on screen, because screen sizes vary so much. However, 

they can be used if the output medium is known, such as for print layout.



Unit 	Description
cm 	centimeters
mm 	millimeters
in 	inches (1in = 96px = 2.54cm)
px * 	pixels (1px = 1/96th of 1in)
pt 	points (1pt = 1/72 of 1in)
pc 	picas (1pc = 12 pt) 


Pixels (px) are relative to the viewing device. For low-dpi devices, 1px is one device pixel (dot) of the 

display. For printers and high resolution screens 1px implies multiple device pixels.


Relative Lengths

Relative length units specify a length relative to another length property. Relative length units scales 

better between different rendering mediums.
Unit 	Description 	
em 	Relative to the font-size of the element (2em means 2 times the size of the current font) 	
ex 	Relative to the x-height of the current font (rarely used) 	
ch 	Relative to width of the "0" (zero) 	
rem 	Relative to font-size of the root element 	
vw 	Relative to 1% of the width of the viewport* 	
vh 	Relative to 1% of the height of the viewport* 	
vmin 	Relative to 1% of viewport's* smaller dimension 	
vmax 	Relative to 1% of viewport's* larger dimension 	
% 	Relative to the parent element


Tip: The em and rem units are practical in creating perfectly scalable layout!
* Viewport = the browser window size. If the viewport is 50cm wide, 1vw = 0.5cm.


NB: Always confirm browser support for the units you choose. 




What is Specificity?

If there are two or more conflicting CSS rules that point to the same element, the browser follows some 

rules to determine which one is most specific and therefore wins out.

Think of specificity as a score/rank that determines which style declarations are ultimately applied to an 

element.

The universal selector (*) has low specificity, while ID selectors are highly specific! 

Note: Specificity is a common reason why your CSS-rules don't apply to some elements, although you think 

they should.



Specificity Hierarchy

Each and every selector has its place in the hierarchy. There four categories which define the specificity 

level of a selector:


Inline styles - An inline style is attached directly to the element to be styled. Example: <h1 style="color: 

#ffffff;">.

IDs - An ID is a unique identifier for the page elements, such as #navbar.

Classes, attributes and pseudo-classes - This category includes .classes, [attributes] and pseudo-classes 

such as :hover, :focus etc.

Elements and pseudo-elements - This category includes element names and pseudo-elements, such as h1, div, 

:before and :after.


You need to memorize how to calculate specificity! This gives you better control over the elements. 

Start at 0, add 1000 for style attribute, add 100 for each ID, add 10 for each attribute, class or pseudo-

class, add 1 for each element name or pseudo-element.

Consider these three code fragments:


Example
A: h1
B: #content h1
C: <div id="content"><h1 style="color: #ffffff">Heading</h1></div>

The specificity of A is 1 (one element)
The specificity of B is 101 (one ID reference and one element)
The specificity of C is 1000 (inline styling)

Since 1 < 101 < 1000, the third rule (C) has a greater level of specificity, and therefore will be applied.



Specificity Rules

Equal specificity: the latest rule counts - If the same rule is written twice into the external style sheet, 

then the lower rule in the style sheet is closer to the element to be styled, and therefore will be applied:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {background-color: yellow;}
h1 {background-color: red;}
</style>
</head>
<body>

<h1>This is heading 1</h1>

</body>
</html>


the latter rule is always applied.

ID selectors have a higher specificity than attribute selectors - Look at the following three code lines:


<!DOCTYPE html>
<html>
<head>
<style>
div#a {background-color: green;}
#a {background-color: yellow;}
div[id=a] {background-color: blue;}
</style>
</head>
<body>

<div id="a">This is a div</div>

</body>
</html>


the first rule is more specific than the other two, and will be applied.

Contextual selectors are more specific than a single element selector - The embedded style sheet is closer 

to the element to be styled (than the external style sheet. So in the following situation, the latter rule 

will be applied.


Example
From external CSS file:
#content h1 {background-color: red;}

In HTML file:
<style>
#content h1 {
  background-color: yellow;
}
</style>



A class selector beats any number of element selectors - a class selector such as .intro beats h1, p, div, 

etc:


<!DOCTYPE html>
<html>
<head>
<style>
.intro {background-color: yellow;}
h1 {background-color: red;}
</style>
</head>
<body>

<h1 class="intro">This is a heading</h1>

</body>
</html>


The universal selector and inherited values have a specificity of 0 - *, body * and similar have a zero 

specificity. Inherited values also have a specificity of 0.





CSS The !important Rule

The !important rule in CSS is used to add more importance to a property/value than normal.

In fact, if you use the !important rule, it will override ALL previous styling rules for that specific 

property on that element!

Let us look at an example:


<!DOCTYPE html>
<html>
<head>
<style>
#myid {
  background-color: blue;
}

.myclass {
  background-color: gray;
}

p {
  background-color: red !important;
}
</style>
</head>
<body>

<p>This is some text in a paragraph.</p>

<p class="myclass">This is some text in a paragraph.</p>

<p id="myid">This is some text in a paragraph.</p>

</body>
</html>


In the example above, all three paragraphs will get a red background color, even though the ID selector and 

the class selector has a higher specificity. The !important rule overrides the background-color property in 

both cases.



Important About !important

The only way to override an !important rule is to include another !important rule on a declaration with the 

same (or higher) specificity in the source code - and here the problem starts! This makes the CSS code 

confusing and the debugging will be hard, especially if you have a large style sheet!

Here we have created a simple example. It is not very clear, when you look at the CSS source code, which 

color is considered most important:


<!DOCTYPE html>
<html>
<head>
<style>
#myid {
  background-color: blue !important;
}

.myclass {
  background-color: gray !important;
}

p {
  background-color: red !important;
}
</style>
</head>
<body>

<p>This is some text in a paragraph.</p>

<p class="myclass">This is some text in a paragraph.</p>

<p id="myid">This is some text in a paragraph.</p>

</body>
</html>


Tip: It is good to know about the !important rule, you might see it in some CSS source code. However, do not 

use it unless you absolutely have to.



Maybe One or Two Fair Uses of !important

You can use !important if you have to override a style that cannot be overridden in any other way such as 

when you are working in a content management system (CMS) and cannot edit the CSS code. In that case, you 

can set some custom styles to override some of the CMS styles. Another way to use !important is: Assume you 

want a special look for all buttons on a page. Here, buttons are styled with a gray background color, white 

text, and some padding and border, as shown below:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #8c8c8c; 
  color: white;
  padding: 5px;
  border: 1px solid black; 
}
</style>
</head>
<body>

<p>Standard button: <a class="button" href="default.asp">CSS Tutorial</a></p>

<p>Standard button: <a class="button" href="/html/">HTML Tutorial</a></p>

</body>
</html>



The look of a button can sometimes change if we put it inside another element with higher specificity, and 

the properties gets in conflict. Here is an example of this (the links inside myDiv have yellow background 

and written in red):


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #8c8c8c; 
  color: white;
  padding: 5px;
  border: 1px solid black; 
}

#myDiv a {
  color: red;
  background-color: yellow;  
}
</style>
</head>
<body>

<p>Standard button: <a class="button" href="default.asp">CSS Tutorial</a></p>

<div id="myDiv">
<p>A link text inside myDiv: <a href="/html/">HTML Tutorial</a></p>
<p>A link button inside myDiv: <a href="/html/" class="button">HTML Tutorial</a></p>
</div>

</body>
</html>


To "force" all buttons to have the same look, no matter what, we can add the !important rule to the 

properties of the button, like this (only the "HTML Tutorial" button has a yellow background with a red 

font):

<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #8c8c8c !important; 
  color: white !important;
  padding: 5px !important;
  border: 1px solid black !important; 
}

#myDiv a {
  color: red;
  background-color: yellow;  
}
</style>
</head>
<body>

<p>Standard button: <a class="button" href="default.asp">CSS Tutorial</a></p>

<div id="myDiv">
<p>A link text inside myDiv: <a href="/html/">HTML Tutorial</a></p>
<p>A link button inside myDiv: <a href="/html/" class="button">HTML Tutorial</a></p>
</div>

</body>
</html>






CSS Math Functions

The CSS math functions allow mathematical expressions to be used as property values. Here, we will explain 

the calc(), max() and min() functions.


The calc() Function

The calc() function performs a calculation to be used as the property value.

CSS Syntax
calc(expression)
Value 	Description
expression 	Required. A mathematical expression. The result will be used as the value.
The following operators can be used: + - * /

See illustration below:

<!DOCTYPE html>
<html>
<head>
<style>
#div1 {
  position: absolute;
  left: 50px;
  width: calc(100% - 100px);
  border: 1px solid black;
  background-color: yellow;
  padding: 5px;
}
</style>
</head>
<body>

<h1>The calc() Function</h1>

<p>Create a div that stretches across the window, with a 50px gap between both sides of the div and the 

edges of the window:</p>

<div id="div1">Some text...</div>

</body>
</html>


The max() Function

The max() function uses the largest value, from a comma-separated list of values, as the property value.

CSS Syntax
max(value1, value2, ...)


Value 	Description
value1, value2, ... 	Required. A list of comma-separated values - where the largest value is chosen


<!DOCTYPE html>
<html>
<head>
<style>
#div1 {
  background-color: yellow;
  height: 100px;
  width: max(50%, 300px);
}
</style>
</head>
<body>

<h1>The max() Function</h1>

<p>Use max() to set the width of #div1 to whichever value is largest, 50% or 300px:</p>

<div id="div1">Some text...</div>

<p>Resize the browser window to see the effect.</p>

</body>
</html>


The min() Function

The min() function uses the smallest value, from a comma-separated list of values, as the property value.

CSS Syntax
min(value1, value2, ...)

Value 	Description
value1, value2, ... 	Required. A list of comma-separated values - where the smallest value is chosen

Let us look at an example:


<!DOCTYPE html>
<html>
<head>
<style>
#div1 {
  background-color: yellow;
  height: 100px;
  width: min(50%, 300px);
}
</style>
</head>
<body>

<h1>The min() Function</h1>

<p>Use min() to set the width of #div1 to whichever value is smallest, 50% or 300px:</p>

<div id="div1">Some text...</div>

<p>Resize the browser window to see the effect.</p>

</body>
</html>






CSS ADVANCED
 




css Rounded Corners;

This enables you to give any element a rounded corner. 


CSS border-radius Property

The CSS border-radius property defines the radius of an element's corners. This property allows you to add 

rounded corners to elements! You can have create rounded corners for an element with a specified background 

color, with a border, and with a background image. See illustration below:

<!DOCTYPE html>
<html>
<head>
<style> 
#rcorners1 {
  border-radius: 25px;
  background: #73AD21;
  padding: 20px; 
  width: 200px;
  height: 150px;  
}

#rcorners2 {
  border-radius: 25px;
  border: 2px solid #73AD21;
  padding: 20px; 
  width: 200px;
  height: 150px;  
}

#rcorners3 {
  border-radius: 25px;
  background: url(paper.gif);
  background-position: left top;
  background-repeat: repeat;
  padding: 20px; 
  width: 200px;
  height: 150px;  
}
</style>
</head>
<body>

<h1>The border-radius Property</h1>

<p>Rounded corners for an element with a specified background color:</p>
<p id="rcorners1">Rounded corners!</p>
<p>Rounded corners for an element with a border:</p>
<p id="rcorners2">Rounded corners!</p>
<p>Rounded corners for an element with a background image:</p>
<p id="rcorners3">Rounded corners!</p>

</body>
</html>



Note that: In the example above, the border-radius property is actually a shorthand property for the 

border-top-left-radius, border-top-right-radius, border-bottom-right-radius and border-bottom-left-radius 

properties.



CSS border-radius - Specify Each Corner::

You can specify 1-4 border-radius properties for an element. These include:


Four values - border-radius: 15px 50px 30px 5px; (first value applies to top-left corner, second value 

applies to top-right corner, third value applies to bottom-right corner, and fourth value applies to 

bottom-left corner): 

Three values - border-radius: 15px 50px 30px; (first value applies to top-left corner, second value applies 

to top-right and bottom-left corners, and third value applies to bottom-right corner):

Two values - border-radius: 15px 50px; (first value applies to top-left and bottom-right corners, and the 

second value applies to top-right and bottom-left corners):

One value - border-radius: 15px; (the value applies to all four corners, which are rounded equally:



See example code illustrating this principle below:


<!DOCTYPE html>
<html>
<head>
<style> 
#rcorners1 {
  border-radius: 15px 50px 30px 5px;
  background: #73AD21;
  padding: 20px; 
  width: 200px;
  height: 150px; 
}

#rcorners2 {
  border-radius: 15px 50px 30px;
  background: #73AD21;
  padding: 20px; 
  width: 200px;
  height: 150px; 
}

#rcorners3 {
  border-radius: 15px 50px;
  background: #73AD21;
  padding: 20px; 
  width: 200px;
  height: 150px; 
} 

#rcorners4 {
  border-radius: 15px;
  background: #73AD21;
  padding: 20px; 
  width: 200px;
  height: 150px; 
} 
</style>
</head>
<body>

<h1>The border-radius Property</h1>

<p>Four values - border-radius: 15px 50px 30px 5px:</p>
<p id="rcorners1"></p>

<p>Three values - border-radius: 15px 50px 30px:</p>
<p id="rcorners2"></p>

<p>Two values - border-radius: 15px 50px:</p>
<p id="rcorners3"></p>

<p>One value - border-radius: 15px:</p>
<p id="rcorners4"></p>

</body>
</html>


Elliptical corners can also be created as shown below:

<!DOCTYPE html>
<html>
<head>
<style> 
#rcorners1 {
  border-radius: 50px / 15px;
  background: #73AD21;
  padding: 20px; 
  width: 200px;
  height: 150px; 
}

#rcorners2 {
  border-radius: 15px / 50px;
  background: #73AD21;
  padding: 20px; 
  width: 200px;
  height: 150px; 
}

#rcorners3 {
  border-radius: 50%;
  background: #73AD21;
  padding: 20px; 
  width: 200px;
  height: 150px;
} 
</style>
</head>
<body>

<h1>The border-radius Property</h1>

<p>Elliptical border - border-radius: 50px / 15px:</p>
<p id="rcorners1"></p>

<p>Elliptical border - border-radius: 15px / 50px:</p>
<p id="rcorners2"></p>

<p>Ellipse border - border-radius: 50%:</p>
<p id="rcorners3"></p>

</body>
</html>



CSS Rounded Corners Properties
Property 	Description
border-radius 	A shorthand property for setting all the four border-*-*-radius properties
border-top-left-radius 	Defines the shape of the border of the top-left corner
border-top-right-radius 	Defines the shape of the border of the top-right corner
border-bottom-right-radius 	Defines the shape of the border of the bottom-right corner
border-bottom-left-radius 	Defines the shape of the border of the bottom-left corner




CSS Border Images;

The CSS border-image property allows you to set the image to be used as the border around an element. 



CSS border-image Property

The CSS border-image property allows you to specify an image to be used instead of the normal border around 

an element.

The property has three parts:

    The image to use as the border
    Where to slice the image
    Define whether the middle sections should be repeated or stretched


The border-image property takes the image and slices it into nine sections, like a tic-tac-toe board. It 

then places the corners at the corners, and the middle sections are repeated or stretched as you specify.

Note: For border-image to work, the element also needs the border property set!

Here, the middle sections of the image are repeated to create the border:

See code below (30 round repeat the image):

<!DOCTYPE html>
<html>
<head>
<style> 
#borderimg { 
  border: 10px solid transparent;
  padding: 15px;
  border-image: url(border.png) 30 round;
}
</style>
</head>
<body>

<h1>The border-image Property</h1>

<p>Here, the middle sections of the image are repeated to create the border:</p>
<p id="borderimg">border-image: url(border.png) 30 round;</p>

<p>Here is the original image:</p><img src="border.png">
<p><strong>Note:</strong> Internet Explorer 10, and earlier versions, do not support the border-image 

property.</p>

</body>
</html>


Another example illustrating how the middle section of the image is stretched (30 stretch streches the 

image):


<!DOCTYPE html>
<html>
<head>
<style> 
#borderimg { 
  border: 10px solid transparent;
  padding: 15px;
  border-image: url(border.png) 30 stretch;
}
</style>
</head>
<body>

<h1>The border-image Property</h1>

<p>Here, the middle sections of the image are stretched to create the border:</p>
<p id="borderimg">border-image: url(border.png) 30 stretch;</p>

<p>Here is the original image:</p><img src="border.png">
<p><strong>Note:</strong> Internet Explorer 10, and earlier versions, do not support the border-image 

property.</p>

</body>
</html>



Tip: The border-image property is actually a shorthand property for the border-image-source, border-image-

slice, border-image-width, border-image-outset and border-image-repeat properties.




CSS border-image - Different Slice Values

Different slice values completely changes the look of the border:


<!DOCTYPE html>
<html>
<head>
<style>
#borderimg1 {
  border: 10px solid transparent;
  padding: 15px;
  border-image: url(border.png) 50 round;
}

#borderimg2 {
  border: 10px solid transparent;
  padding: 15px;
  border-image: url(border.png) 20% round;
}

#borderimg3 {
  border: 10px solid transparent;
  padding: 15px;
  border-image: url(border.png) 30% round;
}
</style>
</head>
<body>

<h1>The border-image Property</h1>

<p id="borderimg1">border-image: url(border.png) 50 round;</p>
<p id="borderimg2">border-image: url(border.png) 20% round;</p>
<p id="borderimg3">border-image: url(border.png) 30% round;</p>

<p><strong>Note:</strong> Internet Explorer 10, and earlier versions, do not support the border-image 

property.</p>

</body>
</html>


CSS Border Image Properties
Property 	Description
border-image 	A shorthand property for setting all the border-image-* properties
border-image-source 	Specifies the path to the image to be used as a border
border-image-slice 	Specifies how to slice the border image
border-image-width 	Specifies the widths of the border image
border-image-outset 	Specifies the amount by which the border image area extends beyond the border box
border-image-repeat 	Specifies whether the border image should be repeated, rounded or stretched



CSS Multiple Backgrounds




In this chapter you will learn how to add multiple background images to one element.

You will also learn about the following properties:

    background-size
    background-origin
    background-clip

CSS Multiple Backgrounds

CSS allows you to add multiple background images for an element, through the background-image property.

The different background images are separated by commas, and the images are stacked on top of each other, 

where the first image is closest to the viewer.

The following example has two background images, the first image is a flower (aligned to the bottom and 

right) and the second image is a paper background (aligned to the top-left corner):


<!DOCTYPE html>
<html>
<head>
<style> 
#example1 {
  background-image: url(img_flwr.gif), url(paper.gif);
  background-position: right bottom, left top;
  background-repeat: no-repeat, repeat;
  padding: 15px;
}
</style>
</head>
<body>

<h1>Multiple Backgrounds</h1>
<p>The following div element has two background images:</p>

<div id="example1">
  <h1>Lorem Ipsum Dolor</h1>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

</body>
</html>




Multiple background images can be specified using either the individual background properties (as above) or 

the background shorthand property.

The following example uses the background shorthand property (same result as example above):

<!DOCTYPE html>
<html>
<head>
<style> 
#example1 {
  background: url(img_flwr.gif) right bottom no-repeat, url(paper.gif) left top repeat;
  padding: 15px;
}
</style>
</head>
<body>

<div id="example1">
  <h1>Lorem Ipsum Dolor</h1>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

</body>
</html>




CSS Background Size

The CSS background-size property allows you to specify the size of background images.

The size can be specified in lengths, percentages, or by using one of the two keywords: contain or cover.

The following example resizes a background image to much smaller than the original image (using pixels). See 

the code below:


<!DOCTYPE html>
<html>
<head>
<style>
#example1 {
  border: 1px solid black;
  background: url(img_flwr.gif);
  background-size: 100px 80px;
  background-repeat: no-repeat;
  padding: 15px;
}

#example2 {
  border: 1px solid black;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
  padding: 15px;
}
</style>
</head>
<body>

<h1>The background-size Property</h1>

<p>Resized background-image:</p>
<div id="example1">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

<p>Original size of the background-image:</p>
<div id="example2">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

</body>
</html>




The two other possible values for background-size are contain and cover.

The contain keyword scales the background image to be as large as possible (but both its width and its 

height must fit inside the content area). As such, depending on the proportions of the background image and 

the background positioning area, there may be some areas of the background which are not covered by the 

background image.

The cover keyword scales the background image so that the content area is completely covered by the 

background image (both its width and height are equal to or exceed the content area). As such, some parts of 

the background image may not be visible in the background positioning area.

The following example illustrates the use of contain and cover:

<!DOCTYPE html>
<html>
<head>
<style>
.div1 {
  border: 1px solid black;
  height: 120px;
  width: 150px;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
  background-size: contain;
}

.div2 {
  border: 1px solid black;
  height: 120px;
  width: 150px;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
  background-size: cover;
}

.div3 {
  border: 1px solid black;
  height: 120px;
  width: 150px;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
}
</style>
</head>
<body>

<h1>The background-size Property</h1>

<h2>background-size: contain:</h2>
<div class="div1">
<p>Lorem ipsum dolor sit amet.</p>
</div>

<h2>background-size: cover:</h2>
<div class="div2">
<p>Lorem ipsum dolor sit amet.</p>
</div>

<h2>No background-size defined:</h2>
<div class="div3">
<p>Lorem ipsum dolor sit amet.</p>
</div>

<p>Original image:</p>
<img src="img_flwr.gif" alt="Flowers" width="224" height="162">

</body>
</html>




Define Sizes of Multiple Background Images

The background-size property also accepts multiple values for background size (using a comma-separated 

list), when working with multiple backgrounds.

The following example has three background images specified, with different background-size value for each 

image:



<!DOCTYPE html>
<html>
<head>
<style> 
#example1 {
  background: url(img_tree.gif) left top no-repeat, url(img_flwr.gif) right bottom no-repeat, url(paper.gif) 

left top repeat;
  padding: 15px;
  background-size: 50px, 130px, auto;
}
</style>
</head>
<body>

<div id="example1">
  <h1>Lorem Ipsum Dolor</h1>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

</body>
</html>





Full Size Background Image

Now we want to have a background image on a website that covers the entire browser window at all times.

The requirements are as follows:

    Fill the entire page with the image (no white space)
    Scale image as needed
    Center image on page
    Do not cause scrollbars

The following example shows how to do it; Use the <html> element (the <html> element is always at least the 

height of the browser window). Then set a fixed and centered background on it. Then adjust its size with the 

background-size property:



<!DOCTYPE html>
<html>
<head>
<style> 
html { 
  background: url(img_man.jpg) no-repeat center fixed; 
  background-size: cover;
}

body { 
  color: white; 
}
</style>
</head>
<body>

<h1>Full Page Background Image</h1>
<p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation 

ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>

</body>
</html>



Hero Image

You could also use different background properties on a <div> to create a hero image (a large image with 

text), and place it where you want.


<!DOCTYPE html>
<html>
<head>
<style> 
html { 
  background: url(img_man.jpg) no-repeat center fixed; 
  background-size: cover;
}

body { 
  color: white; 
}
</style>
</head>
<body>

<h1>Full Page Background Image</h1>
<p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation 

ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>

</body>
</html>




The CSS background-origin property specifies where the background image is positioned.

The property takes three different values:

    border-box - the background image starts from the upper left corner of the border
    padding-box - (default) the background image starts from the upper left corner of the padding edge
    content-box - the background image starts from the upper left corner of the content

The following example illustrates the background-origin property:

<!DOCTYPE html>
<html>
<head>
<style>
#example1 {
  border: 10px solid black;
  padding: 35px;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
}

#example2 {
  border: 10px solid black;
  padding: 35px;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
  background-origin: border-box;
}

#example3 {
  border: 10px solid black;
  padding: 35px;
  background: url(img_flwr.gif);
  background-repeat: no-repeat;
  background-origin: content-box;
}
</style>
</head>
<body>

<h1>The background-origin Property</h1>

<p>No background-origin (padding-box is default):</p>
<div id="example1">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

<p>background-origin: border-box:</p>
<div id="example2">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

<p>background-origin: content-box:</p>
<div id="example3">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
  <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip 

ex ea commodo consequat.</p>
</div>

</body>
</html>


CSS background-clip Property

The CSS background-clip property specifies the painting area of the background.

The property takes three different values:

    border-box - (default) the background is painted to the outside edge of the border
    padding-box - the background is painted to the outside edge of the padding
    content-box - the background is painted within the content box

The following example illustrates the background-clip property:

<!DOCTYPE html>
<html>
<head>
<style>
#example1 {
  border: 10px dotted black;
  padding: 35px;
  background: yellow;
}

#example2 {
  border: 10px dotted black;
  padding: 35px;
  background: yellow;
  background-clip: padding-box;
}

#example3 {
  border: 10px dotted black;
  padding: 35px;
  background: yellow;
  background-clip: content-box;
}
</style>
</head>
<body>

<h1>The background-clip Property</h1>

<p>No background-clip (border-box is default):</p>
<div id="example1">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
</div>

<p>background-clip: padding-box:</p>
<div id="example2">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
</div>

<p>background-clip: content-box:</p>
<div id="example3">
  <h2>Lorem Ipsum Dolor</h2>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut 

laoreet dolore magna aliquam erat volutpat.</p>
</div>

</body>
</html>




CSS Advanced Background Properties
Property 	Description
background 	A shorthand property for setting all the background properties in one declaration
background-clip 	Specifies the painting area of the background
background-image 	Specifies one or more background images for an element
background-origin 	Specifies where the background image(s) is/are positioned
background-size 	Specifies the size of the background image(s)



CSS Colors


RGBA Colors

RGBA color values are an extension of RGB color values with an alpha channel - which specifies the opacity 

for a color.

An RGBA color value is specified with: rgba(red, green, blue, alpha). The alpha parameter is a number 

between 0.0 (fully transparent) and 1.0 (fully opaque). See the example below for the definition of RGBA 

colors:


<!DOCTYPE html>
<html>
<head>
<style>
#p1 {background-color:rgba(255,0,0,0.3);}
#p2 {background-color:rgba(0,255,0,0.3);}
#p3 {background-color:rgba(0,0,255,0.3);}
#p4 {background-color:rgba(192,192,192,0.3);}
#p5 {background-color:rgba(255,255,0,0.3);}
#p6 {background-color:rgba(255,0,255,0.3);}
</style>
</head>
<body>

<h1>Define Colors With RGBA Values</h1>

<p id="p1">Red</p>
<p id="p2">Green</p>
<p id="p3">Blue</p>
<p id="p4">Grey</p>
<p id="p5">Yellow</p>
<p id="p6">Cerise</p>

</body>
</html>



HSL Colors

HSL stands for Hue, Saturation and Lightness.

An HSL color value is specified with: hsl(hue, saturation, lightness).

    Hue is a degree on the color wheel (from 0 to 360):
        0 (or 360) is red
        120 is green
        240 is blue
    Saturation is a percentage value: 100% is the full color.
    Lightness is also a percentage; 0% is dark (black) and 100% is white.
The example below shows the definition of HSL colors:


<!DOCTYPE html>
<html>
<head>
<style>
#p1 {background-color:hsl(120,100%,50%);}
#p2 {background-color:hsl(120,100%,75%);}
#p3 {background-color:hsl(120,100%,25%);}
#p4 {background-color:hsl(120,60%,70%);}
#p5 {background-color:hsl(290,100%,50%);}
#p6 {background-color:hsl(290,60%,70%);}
</style>
</head>
<body>

<h1>Define Colors With HSL Values</h1>

<p id="p1">Green</p>
<p id="p2">Light green</p>
<p id="p3">Dark green</p>
<p id="p4">Pastel green</p>
<p id="p5">Violet</p>
<p id="p6">Pastel violet</p>

</body>
</html>



HSLA Colors

HSLA color values are an extension of HSL color values with an alpha channel - which specifies the opacity 

for a color.

An HSLA color value is specified with: hsla(hue, saturation, lightness, alpha), where the alpha parameter 

defines the opacity. The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (fully opaque).

See the example below for different HSLA colors:

<!DOCTYPE html>
<html>
<head>
<style>
#p1 {background-color:hsla(120,100%,50%,0.3);}
#p2 {background-color:hsla(120,100%,75%,0.3);}
#p3 {background-color:hsla(120,100%,25%,0.3);}
#p4 {background-color:hsla(120,60%,70%,0.3);}
#p5 {background-color:hsla(290,100%,50%,0.3);}
#p6 {background-color:hsla(290,60%,70%,0.3);}
</style>
</head>
<body>

<h1>Define Colors With HSLA Values</h1>

<p id="p1">Green</p>
<p id="p2">Light green</p>
<p id="p3">Dark green</p>
<p id="p4">Pastel green</p>
<p id="p5">Violet</p>
<p id="p6">Pastel violet</p>

</body>
</html>




Opacity

The CSS opacity property sets the opacity for the whole element (both background color and text will be 

opaque/transparent).

The opacity property value must be a number between 0.0 (fully transparent) and 1.0 (fully opaque). 

The texts above will also be transparent. See example below for elements with specified opacity:


<!DOCTYPE html>
<html>
<head>
<style>
#p1 {background-color:rgb(255,0,0);opacity:0.6;}
#p2 {background-color:rgb(0,255,0);opacity:0.6;}
#p3 {background-color:rgb(0,0,255);opacity:0.6;}
#p4 {background-color:rgb(192,192,192);opacity:0.6;}
#p5 {background-color:rgb(255,255,0);opacity:0.6;}
#p6 {background-color:rgb(255,0,255);opacity:0.6;}
</style>
</head>
<body>

<h1>Define Colors With Opacity</h1>

<p id="p1">Red</p>
<p id="p2">Green</p>
<p id="p3">Blue</p>
<p id="p4">Grey</p>
<p id="p5">Yellow</p>
<p id="p6">Cerise</p>

</body>
</html>







CSS Color Keywords

In this section, transparent, currentcolor, and inherit keywords will be explained.

The transparent Keyword

The transparent keyword is used to make a color transparent. This is often used to make a transparent 

background color for an element. In the example below, Here, the background color of the <div> element will 

be fully transparent, and the background image will show through:



<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-image: url("paper.gif");
}

div.ex1 { 
  background-color: lightgreen;
  border: 2px solid black;
  padding: 15px;
}

div.ex2 { 
  background-color: transparent;
  border: 2px solid black;
  padding: 15px;
} 
</style>
</head>
<body>

<h2>The transparent Keyword</h2>

<div class="ex1">This div has a light green background.</div>
<br>
<div class="ex2">This div has a transparent background.</div>

</body>
</html>


Note: The transparent keyword is equivalent to rgba(0,0,0,0). RGBA color values are an extension of RGB 

color values with an alpha channel - which specifies the opacity for a color. Read more in our CSS RGB 

chapter and in our CSS Colors chapter.




The currentcolor Keyword

The currentcolor keyword is like a variable that holds the current value of the color property of an 

element.

This keyword can be useful if you want a specific color to be consistent in an element or a page. In the 

example below, the border color of <div> element will be blue since the text color of the <div> element is 

blue:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  color: blue;
  border: 10px solid currentcolor;
  padding: 15px;  
}
</style>
</head>
<body>

<h2>The currentcolor Keyword</h2>

<p>The currentcolor keyword refers to the current value of the color property of an element.</p>

<div>
This div element has a blue text color and a blue border.
</div>

</body>
</html>



In this example the <div>'s background color is set to the current color value of the body element:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  color: purple;
}

div {
  background-color: currentcolor;
  padding: 15px;
}

div p {
  color: white;
}
</style>
</head>
<body>

<h2>The currentcolor Keyword</h2>

<p>This is some text in the body part...</p>

<div>
<p>This div's background color is set to the current color value of the body element.</p>
</div>

</body>
</html>



In this example the <div>'s border color and shadow color is set to the current color value of the body 

element:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  color: green;
}

div { 
  box-shadow: 0px 0px 15px currentcolor;
  border: 5px solid currentcolor;
  padding: 15px;
}
</style>
</head>
<body>

<h2>The currentcolor Keyword</h2>

<p>This is some text in the body part...</p>

<div>
<p>This div's border color and shadow color is set to the current color value of the body element.</p>
</div>

</body>
</html>




The inherit Keyword

The inherit keyword specifies that a property should inherit its value from its parent element.

The inherit keyword can be used for any CSS property, and on any HTML element.


In this example the <span>'s border settings will be inherited from the parent element:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 2px solid red;
}

span {
  border: inherit;
}
</style>
</head>
<body>

<h2>The inherit Keyword</h2>

<div>Here, the <span>span element's</span> border settings will be inherited from the parent element.</div>
<br>

<div style="border:2px dotted blue;">Here, the <span>span element's</span> border settings will also be 

inherited from the parent element.</div>

</body>
</html>





CSS Gradients


The CSS gradients enable you to display smooth transitions between two of many specified colors. The three 

types of gradients that can be defined in CSS include:



    Linear Gradients (goes down/up/left/right/diagonally)
    Radial Gradients (defined by their center)
    Conic Gradients (rotated around a center point)




CSS Linear Gradients

To create a linear gradient you must define at least two color stops. Color stops are the colors you want to 

render smooth transitions among. You can also set a starting point and a direction (or an angle) along with 

the gradient effect.
Syntax
background-image: linear-gradient(direction, color-stop1, color-stop2, ...); 


Direction - Top to Bottom (this is default)

The following example shows a linear gradient that starts at the top. It starts red, transitioning to 

yellow:

<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: linear-gradient(red, yellow);
}
</style>
</head>
<body>

<h1>Linear Gradient - Top to Bottom</h1>
<p>This linear gradient starts red at the top, transitioning to yellow at the bottom:</p>

<div id="grad1"></div>

</body>
</html>




Direction - Left to Right

The following example shows a linear gradient that starts from the left. It starts red, transitioning to 

yellow:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: linear-gradient(to right, red , yellow);
}
</style>
</head>
<body>

<h1>Linear Gradient - Left to Right</h1>
<p>This linear gradient starts red at the left, transitioning to yellow (to the right):</p>

<div id="grad1"></div>

</body>
</html>



Direction - Diagonal

You can make a gradient diagonally by specifying both the horizontal and vertical starting positions.

The following example shows a linear gradient that starts at top left (and goes to bottom right). It starts 

red, transitioning to yellow:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: linear-gradient(to bottom right, red, yellow);
}
</style>
</head>
<body>

<h1>Linear Gradient - Diagonal</h1>
<p>This linear gradient starts red at top left, transitioning to yellow (at bottom right):</p>

<div id="grad1"></div>

</body>
</html>




Using Angles

If you want more control over the direction of the gradient, you can define an angle, instead of the 

predefined directions (to bottom, to top, to right, to left, to bottom right, etc.). A value of 0deg is 

equivalent to "to top". A value of 90deg is equivalent to "to right". A value of 180deg is equivalent to "to 

bottom".
Syntax
background-image: linear-gradient(angle, color-stop1, color-stop2);

The following example shows how to use angles on linear gradients:



<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 100px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: linear-gradient(0deg, red, yellow);
}

#grad2 {
  height: 100px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: linear-gradient(90deg, red, yellow);
}

#grad3 {
  height: 100px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: linear-gradient(180deg, red, yellow);
}

#grad4 {
  height: 100px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: linear-gradient(-90deg, red, yellow);
}
</style>
</head>
<body>

<h1>Linear Gradients - Using Different Angles</h1>

<div id="grad1" style="text-align:center;">0deg</div><br>
<div id="grad2" style="text-align:center;">90deg</div><br>
<div id="grad3" style="text-align:center;">180deg</div><br>
<div id="grad4" style="text-align:center;">-90deg</div>

</body>
</html>


Using Multiple Color Stops

The following example shows a linear gradient (from top to bottom) with multiple color stops:

<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: linear-gradient(red, yellow, green);
}

#grad2 {
  height: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: linear-gradient(red, orange, yellow, green, blue, indigo, violet);
}

#grad3 {
  height: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: linear-gradient(red 10%, green 85%, blue 90%);
}
</style>
</head>
<body>

<h1>Linear Gradients - Multiple Color Stops</h1>
<p><strong>Note:</strong> Color stops are spaced evenly when no percents are specified.</p>

<h2>3 Color Stops (evenly spaced):</h2>
<div id="grad1"></div>

<h2>7 Color Stops (evenly spaced):</h2>
<div id="grad2"></div>

<h2>3 Color Stops (not evenly spaced):</h2>
<div id="grad3"></div>

</body>
</html>



The following example shows how to create a linear gradient (from left to right) with the color of the 

rainbow and some text:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 55px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: linear-gradient(to right, red, orange, yellow, green, blue, indigo, violet);
}
</style>
</head>
<body>

<div id="grad1" style="text-align:center;margin:auto;color:#888888;font-size:40px;font-weight:bold">
Rainbow Background
</div>

</body>
</html>




Using Transparency

CSS gradients also support transparency, which can be used to create fading effects.

To add transparency, we use the rgba() function to define the color stops. The last parameter in the rgba() 

function can be a value from 0 to 1, and it defines the transparency of the color: 0 indicates full 

transparency, 1 indicates full color (no transparency).

The following example shows a linear gradient that starts from the left. It starts fully transparent, 

transitioning to full color red:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  background-image: linear-gradient(to right, rgba(255,0,0,0), rgba(255,0,0,1));
}
</style>
</head>
<body>

<h1>Linear Gradient - Transparency</h1>
<p>To add transparency, we use the rgba() function to define the color stops. The last parameter in the 

rgba() function can be a value from 0 to 1, and it defines the transparency of the color: 0 indicates full 

transparency, 1 indicates full color (no transparency).</p>

<div id="grad1"></div>

</body>
</html>




Repeating a linear-gradient

The repeating-linear-gradient() function is used to repeat linear gradients:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: repeating-linear-gradient(red, yellow 10%, green 20%);
}

#grad2 {
  height: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: repeating-linear-gradient(45deg,red,yellow 7%,green 10%);
}

#grad3 {
  height: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: repeating-linear-gradient(190deg,red,yellow 7%,green 10%);
}

#grad4 {
  height: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: repeating-linear-gradient(90deg,red,yellow 7%,green 10%);
}
</style>
</head>
<body>

<h1>Repeating Linear Gradient</h1>

<div id="grad1"></div>

<p>A repeating gradient on 45deg axe starting red and finishing green:</p>
<div id="grad2"></div>

<p>A repeating gradient on 190deg axe starting red and finishing green:</p>
<div id="grad3"></div>

<p>A repeating gradient on 90deg axe starting red and finishing green:</p>
<div id="grad4"></div>

</body>
</html>




CSS Radial Gradients::


CSS Radial Gradients

A radial gradient is defined by its center.

To create a radial gradient you must also define at least two color stops.
Syntax
background-image: radial-gradient(shape size at position, start-color, ..., last-color);



By default, shape is ellipse, size is farthest-corner, and position is center.

Radial Gradient - Evenly Spaced Color Stops (this is default)

The following example shows a radial gradient with evenly spaced color stops:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 150px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: radial-gradient(red, yellow, green);
}
</style>
</head>
<body>

<h1>Radial Gradient - Evenly Spaced Color Stops</h1>

<div id="grad1"></div>

</body>
</html>



Radial Gradient - Differently Spaced Color Stops

The following example shows a radial gradient with differently spaced color stops:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 150px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: radial-gradient(red 5%, yellow 15%, green 60%);
}
</style>
</head>
<body>

<h1>Radial Gradient - Differently Spaced Color Stops</h1>

<div id="grad1"></div>

</body>
</html>



Set Shape

The shape parameter defines the shape. It can take the value circle or ellipse. The default value is 

ellipse.

The following example shows a radial gradient with the shape of a circle:




<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 150px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: radial-gradient(red, yellow, green);
}

#grad2 {
  height: 150px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: radial-gradient(circle, red, yellow, green);
}
</style>
</head>
<body>

<h1>Radial Gradient - Shapes</h1>

<h2>Ellipse (this is default):</h2>
<div id="grad1"></div>

<h2><strong>Circle:</strong></h2>
<div id="grad2"></div>

</body>
</html>




Use of Different Size Keywords

The size parameter defines the size of the gradient. It can take four values:

    closest-side
    farthest-side
    closest-corner
    farthest-corner

The example below show radial gradients with different size keywords:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 150px;
  width: 150px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: radial-gradient(closest-side at 60% 55%, red, yellow, black);
}

#grad2 {
  height: 150px;
  width: 150px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: radial-gradient(farthest-side at 60% 55%, red, yellow, black);
}

#grad3 {
  height: 150px;
  width: 150px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: radial-gradient(closest-corner at 60% 55%, red, yellow, black);
}

#grad4 {
  height: 150px;
  width: 150px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: radial-gradient(farthest-corner at 60% 55%, red, yellow, black);
}
</style>
</head>
<body>

<h1>Radial Gradients - Different size keywords</h1>

<h2>closest-side:</h2>
<div id="grad1"></div>

<h2>farthest-side:</h2>
<div id="grad2"></div>

<h2>closest-corner:</h2>
<div id="grad3"></div>

<h2>farthest-corner (default):</h2>
<div id="grad4"></div>

</body>
</html>




Repeating a radial-gradient

The repeating-radial-gradient() function is used to repeat radial gradients. The example below shows 

repeating radial gradient:

<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 150px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: repeating-radial-gradient(red, yellow 10%, green 15%);
}
</style>
</head>
<body>

<h1>Repeating Radial Gradient</h1>

<div id="grad1"></div>

</body>
</html>




CSS Conic Gradients
CSS Conic Gradients

A conic gradient is a gradient with color transitions rotated around a center point.

To create a conic gradient you must define at least two colors.


Syntax

background-image: conic-gradient([from angle] [at position,] color [degree], color [degree], ...);

By default, angle is 0deg and position is center.

If no degree is specified, the colors will be spread equally around the center point.



Conic Gradient: Three Colors

The following example shows a conic gradient with three colors. The example below shows a conic gradient 

with three colors:

<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: conic-gradient(red, yellow, green);
}
</style>
</head>
<body>

<h1>Conic Gradient - Three Colors</h1>

<div id="grad1"></div>

</body>
</html>




Conic Gradient: Five Colors

The following example shows a conic gradient with five colors. The example below shows a conic gradient with 

five colors:

<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: conic-gradient(red, yellow, green, blue, black);
}
</style>
</head>
<body>

<h1>Conic Gradient - Five Colors</h1>

<div id="grad1"></div>

</body>
</html>



Conic Gradient: Three Colors and Degrees

The following example shows a conic gradient with three colors and a degree for each color. A conic gradient 

with three colors and a degree for each color is shown in the example below:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: conic-gradient(red 45deg, yellow 90deg, green 210deg);
}
</style>
</head>
<body>

<h1>Conic Gradient - Defined degree for each color</h1>

<div id="grad1"></div>

</body>
</html>



Create Pie Charts

Just add border-radius: 50% to make the conic gradient look like a pie:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: conic-gradient(red, yellow, green, blue, black);
  border-radius: 50%;
}
</style>
</head>
<body>

<h1>Conic Gradient - Pie Chart</h1>

<div id="grad1"></div>

</body>
</html>


Example below shows a pie chart with defined degrees for all the colors:

<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: conic-gradient(red 0deg, red 90deg, yellow 90deg, yellow 180deg, green 180deg, green 

270deg, blue 270deg);
  border-radius: 50%;
}
</style>
</head>
<body>

<h1>Conic Gradient - Pie Chart</h1>

<div id="grad1"></div>

</body>
</html>



Conic Gradient With Specified From Angle

The [from angle] specifies an angle that the entire conic gradient is rotated by.

The following example shows a conic gradient with a from angle of 90deg:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: conic-gradient(from 90deg, red, yellow, green);
  border-radius: 50%;
}
</style>
</head>
<body>

<h1>Conic Gradient - With a from angle</h1>

<div id="grad1"></div>

</body>
</html>




Conic Gradient With Specified Center Position

The [at position] specifies the center of the conic gradient.

The following example shows a conic gradient with a center position of 60% 45%:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: conic-gradient(at 60% 45%, red, yellow, green);
  border-radius: 50%;
}
</style>
</head>
<body>

<h1>Conic Gradient - With a specified center position</h1>

<div id="grad1"></div>

</body>
</html>




Repeating a Conic Gradient

The repeating-conic-gradient() function is used to repeat conic gradients. The example below shows the 

repeating conic gradient:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: repeating-conic-gradient(red 10%, yellow 20%);
  border-radius: 50%;
}
</style>
</head>
<body>

<h1>Repeating a Conic Gradient</h1>

<div id="grad1"></div>

</body>
</html>



Here is a repeating conic gradient with defined color-starts and color-stops:


<!DOCTYPE html>
<html>
<head>
<style>
#grad1 {
  height: 200px;
  width: 200px;
  background-color: red; /* For browsers that do not support gradients */
  background-image: repeating-conic-gradient(red 0deg 10deg, yellow 10deg 20deg, blue 20deg 30deg);
  border-radius: 50%;
}
</style>
</head>
<body>

<h1>Repeating a Conic Gradient with color-starts and -stops</h1>

<div id="grad1"></div>

</body>
</html>


CSS Gradient Functions

The following table lists the CSS gradient functions:
Function 	Description
conic-gradient() 	Creates a conic gradient. Define at least two colors (around a center point)
linear-gradient() 	Creates a linear gradient. Define at least two colors (top to bottom)
radial-gradient() 	Creates a radial gradient. Define at least two colors (center to edges)
repeating-conic-gradient() 	Repeats a conic gradient
repeating-linear-gradient() 	Repeats a linear gradient
repeating-radial-gradient() 	Repeats a radial gradient







CSS Shadow Effects

CSS Shadow Effects

With CSS you can add shadow to text and to elements.

In these chapters you will learn about the following properties:

    text-shadow
    box-shadow


CSS Text Shadow

The CSS text-shadow property applies shadow to text.

In its simplest use, you only specify the horizontal shadow (2px) and the vertical shadow (2px):


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-shadow: 2px 2px;
}
</style>
</head>
<body>

<h1>Text-shadow effect!</h1>

</body>
</html>


You can then add color to the shadow effect:

<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-shadow: 2px 2px red;
}
</style>
</head>
<body>

<h1>Text-shadow effect!</h1>

</body>
</html>


Then, add a blur effect to the shadow (blur effect is 5px in this case):


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-shadow: 2px 2px 5px red;
}
</style>
</head>
<body>

<h1>Text-shadow effect!</h1>

</body>
</html>




In the example below, you will have a white text with a black shadow:

<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  color: white;
  text-shadow: 2px 2px 4px #000000;
}
</style>
</head>
<body>

<h1>Text-shadow effect!</h1>

</body>
</html>



The example below shows red neon glow shadow (shadow is 3px and there is not vertical and horizontal text 

shadow, hence the 0 0 3px):

<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-shadow: 0 0 3px #FF0000;
}
</style>
</head>
<body>

<h1>Text-shadow with red neon glow!</h1>

</body>
</html>


Multiple Shadows

To add more than one shadow to the text, you can add a comma-separated list of shadows.

The following example shows a red and blue neon glow shadow:
Text shadow effect!



<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  text-shadow: 0 0 3px #FF0000, 0 0 5px #0000FF;
}
</style>
</head>
<body>

<h1>Text-shadow with red and blue neon glow!</h1>

</body>
</html>



The following example shows a white text with black, blue, and darkblue shadow:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  color: white;
  text-shadow: 1px 1px 2px black, 0 0 25px blue, 0 0 5px darkblue;
}
</style>
</head>
<body>

<h1>Text-shadow effect!</h1>

</body>
</html>



You can also use the text-shadow property to create a plain border around some text (without shadows)[In 

this case, a black border is added around the text]:


<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  color: yellow;
  text-shadow: -1px 0 black, 0 1px black, 1px 0 black, 0 -1px black;
}
</style>
</head>
<body>

<h1>Border around text!</h1>

</body>
</html>


CSS Box Shadow::

The CSS box-shadow property applies shadow to elements.

In its simplest use, you only specify the horizontal shadow and the vertical shadow:


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 300px;
  height: 100px;
  padding: 15px;
  background-color: yellow;
  box-shadow: 10px 10px;
}
</style>
</head>
<body>

<h1>The box-shadow Property</h1>

<div>This is a div element with a box-shadow</div>

</body>
</html>


You can then add a color to the shadow:

<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 300px;
  height: 100px;
  padding: 15px;
  background-color: yellow;
  box-shadow: 10px 10px grey;
}
</style>
</head>
<body>

<div>This is a div element with a box-shadow</div>

</body>
</html>




Next, add a blur effect to the shadow:

<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 300px;
  height: 100px;
  padding: 15px;
  background-color: yellow;
  box-shadow: 10px 10px 5px grey;
}
</style>
</head>
<body>

<div>This is a div element with a box-shadow</div>

</body>
</html>



A paper-like card can be created as shown below:

<!DOCTYPE html>
<html>
<head>
<style>
div.card {
  width: 250px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  text-align: center;
}

div.header {
  background-color: #4CAF50;
  color: white;
  padding: 10px;
  font-size: 40px;
}

div.container {
  padding: 10px;
}
</style>
</head>
<body>

<h2>Cards</h2>

<p>The box-shadow property can be used to create paper-like cards:</p>

<div class="card">
  <div class="header">
    <h1>1</h1>
  </div>

  <div class="container">
    <p>January 1, 2016</p>
  </div>
</div>

</body>
</html>


You can also create a paper-like card with an image using the box-shadow property as shown below:

<!DOCTYPE html>
<html>
<head>
<style>
div.polaroid {
  width: 250px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  text-align: center;
}

div.container {
  padding: 10px;
}
</style>
</head>
<body>

<h2>Polaroid Images / Cards</h2>

<p>The box-shadow property can be used to create paper-like cards:</p>

<div class="polaroid">
  <img src="rock600x400.jpg" alt="Norway" style="width:100%">
  <div class="container">
    <p>Hardanger, Norway</p>
  </div>
</div>

</body>
</html>



CSS Shadow Properties

The following table lists the CSS shadow properties:
Property 	Description
box-shadow 	Adds one or more shadows to an element
text-shadow 	Adds one or more shadows to a text 






CSS Text Effects

CSS Text Overflow, Word Wrap, Line Breaking Rules, and Writing Modes

In this chapter you will learn about the following properties:

    text-overflow
    word-wrap
    word-break
    writing-mode


CSS Text Overflow

The CSS text-overflow property specifies how overflowed content that is not displayed should be signaled to 

the user.

It can be clipped:

This is some long text that will not fit in the box

or it can be rendered as an ellipsis (...):

This is some long text that will not fit in the box

The CSS code is as follows:


<!DOCTYPE html>
<html>
<head>
<style> 
p.test1 {
  white-space: nowrap; 
  width: 200px; 
  border: 1px solid #000000;
  overflow: hidden;
  text-overflow: clip;
}

p.test2 {
  white-space: nowrap; 
  width: 200px; 
  border: 1px solid #000000;
  overflow: hidden;
  text-overflow: ellipsis;
}
</style>
</head>
<body>

<h1>The text-overflow Property</h1>
<p>The following two paragraphs contains a long text that will not fit in the box.</p>

<h2>text-overflow: clip:</h2>
<p class="test1">This is some long text that will not fit in the box</p>

<h2>text-overflow: ellipsis:</h2>
<p class="test2">This is some long text that will not fit in the box</p>

</body>
</html>


The following example shows how you can display the overflowed content when hovering over the element:



<!DOCTYPE html>
<html>
<head>
<style> 
div.test {
  white-space: nowrap; 
  width: 200px; 
  overflow: hidden; 
  border: 1px solid #000000;
}

div.test:hover {
  overflow: visible;
}
</style>
</head>
<body>

<p>Hover over the two divs below, to see the entire text.</p>
<div class="test" style="text-overflow:ellipsis;">This is some long text that will not fit in the box</div>
<br>
<div class="test" style="text-overflow:clip;">This is some long text that will not fit in the box</div>

</body>
</html>



CSS Word Wrapping

The CSS word-wrap property allows long words to be able to be broken and wrap onto the next line. 

If a word is too long to fit within an area, it expands outside. The word-wrap property allows you to force 

the text to wrap - even if it means splitting it in the middle of a word. The CSS code you need to allow 

long words to be able to be broken and wrap onto the next line is as shown below:

<!DOCTYPE html>
<html>
<head>
<style> 
p.test {
  width: 11em; 
  border: 1px solid #000000;
  word-wrap: break-word;
}
</style>
</head>
<body>

<h1>The word-wrap Property</h1>

<p class="test">This paragraph contains a very long word: thisisaveryveryveryveryveryverylongword. The long 

word will break and wrap to the next line.</p>

</body>
</html>



CSS Word Breaking

The CSS word-break property specifies line breaking rules . See the CSS code to do that below (where lines 

break at hyphens):


<!DOCTYPE html>
<html>
<head>
<style> 
p.test1 {
  width: 140px; 
  border: 1px solid #000000;
  word-break: keep-all;
}

p.test2 {
  width: 140px; 
  border: 1px solid #000000;
  word-break: break-all;
}
</style>
</head>
<body>

<h1>The word-break Property</h1>

<p class="test1">This paragraph contains some text. This line will-break-at-hyphens.</p>

<p class="test2">This paragraph contains some text. The lines will break at any character.</p>

</body>
</html>




CSS Writing Mode

The CSS writing-mode property specifies whether lines of text are laid out horizontally or vertically.

Some text with a span element with a vertical-rl writing-mode.

The following example shows some different writing modes:


<!DOCTYPE html>
<html>
<head>
<style> 
p.test1 {
  writing-mode: horizontal-tb; 
}

span.test2 {
  writing-mode: vertical-rl; 
}

p.test2 {
  writing-mode: vertical-rl; 
}
</style>
</head>
<body>
<h1>The writing-mode Property</h1>

<p class="test1">Some text with default writing-mode.</p>

<p>Some text with a span element with a <span class="test2">vertical-rl</span> writing-mode.</p>

<p class="test2">Some text with writing-mode: vertical-rl.</p>

</body>
</html>



CSS Text Effect Properties

The following table lists the CSS text effect properties:
Property 	Description
text-align-last 	Specifies how to align the last line of a text
text-justify 	Specifies how justified text should be aligned and spaced
text-overflow 	Specifies how overflowed content that is not displayed should be signaled to the user
word-break 	Specifies line breaking rules for non-CJK scripts
word-wrap 	Allows long words to be able to be broken and wrap onto the next line
writing-mode 	Specifies whether lines of text are laid out horizontally or vertically





css Web Fonts


The CSS @font-face Rule

Web fonts allow Web designers to use fonts that are not installed on the user's computer.

When you have found/bought the font you wish to use, just include the font file on your web server, and it 

will be automatically downloaded to the user when needed.

Your "own" fonts are defined within the CSS @font-face rule.


Different Font Formats

TrueType Fonts (TTF)

TrueType is a font standard developed in the late 1980s, by Apple and Microsoft. TrueType is the most common 

font format for both the Mac OS and Microsoft Windows operating systems.

OpenType Fonts (OTF)

OpenType is a format for scalable computer fonts. It was built on TrueType, and is a registered trademark of 

Microsoft. OpenType fonts are used commonly today on the major computer platforms.

The Web Open Font Format (WOFF)

WOFF is a font format for use in web pages. It was developed in 2009, and is now a W3C Recommendation. WOFF 

is essentially OpenType or TrueType with compression and additional metadata. The goal is to support font 

distribution from a server to a client over a network with bandwidth constraints.

The Web Open Font Format (WOFF 2.0)

TrueType/OpenType font that provides better compression than WOFF 1.0.

SVG Fonts/Shapes

SVG fonts allow SVG to be used as glyphs when displaying text. The SVG 1.1 specification define a font 

module that allows the creation of fonts within an SVG document. You can also apply CSS to SVG documents, 

and the @font-face rule can be applied to text in SVG documents.

Embedded OpenType Fonts (EOT)

EOT fonts are a compact form of OpenType fonts designed by Microsoft for use as embedded fonts on web pages.





Check CSS web fonts on W3Schools to see browser support for various font formats.


Using The Font You Want

In the @font-face rule; first define a name for the font (e.g. myFirstFont) and then point to the font file.

Tip: Always use lowercase letters for the font URL. Uppercase letters can give unexpected results in IE.

To use the font for an HTML element, refer to the name of the font (myFirstFont) through the font-family 

property:


<!DOCTYPE html>
<html>
<head>
<style> 
@font-face {
   font-family: myFirstFont;
   src: url(sansation_light.woff);
}

* {
   font-family: myFirstFont;
}
</style>
</head>
<body>

<h1>The @font-face Rule</h1>

<div>
With CSS, websites can use fonts other than the pre-selected "web-safe" fonts.
</div>

</body>
</html>


Using Bold Text

You must add another @font-face rule containing descriptors for bold text:

The file "sansation_bold.woff" is another font file, that contains the bold characters for the Sansation 

font.

Browsers will use this whenever a piece of text with the font-family "myFirstFont" should render as bold.

This way you can have many @font-face rules for the same font.

See same chapter in W3Schools for CSS Font descriptors (Using a custom font is of no use in my work for 

now).








CSS 2D Transforms


CSS 2D Transforms

CSS transforms allow you to move, rotate, scale, and skew elements. You will learn about C SS transform 

property in this chapter. And in the next chapter you will learn about 3D transforms in CSS. 


CSS 2D Transforms Methods

With the CSS transform property you can use the following 2D transformation methods:

    translate()
    rotate()
    scaleX()
    scaleY()
    scale()
    skewX()
    skewY()
    skew()
    matrix()


The translate() Method

The translate() method moves an element from its current position (according to the parameters given for the 

X-axis and the Y-axis).

The following example moves the <div> element 50 pixels to the right, and 100 pixels down from its current 

position:



<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 300px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
  transform: translate(50px,100px);
}
</style>
</head>
<body>

<h1>The translate() Method</h1>
<p>The translate() method moves an element from its current position:</p>

<div>
This div element is moved 50 pixels to the right, and 100 pixels down from its current position.
</div>

</body>
</html>




The rotate() Method

The rotate() method rotates an element clockwise or counter-clockwise according to a given degree.

The following example rotates the <div> element clockwise with 20 degrees:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 300px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
}

div#myDiv {
  transform: rotate(20deg);
}
</style>
</head>
<body>

<h1>The rotate() Method</h1>

<p>The rotate() method rotates an element clockwise or counter-clockwise.</p>

<div>
This a normal div element.
</div>

<div id="myDiv">
This div element is rotated clockwise 20 degrees.
</div>

</body>
</html>



Using negative values will rotate the element counter-clockwise.

The following example rotates the <div> element counter-clockwise with 20 degrees:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 300px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
}

div#myDiv {
  transform: rotate(-20deg);
}
</style>
</head>
<body>

<h1>The rotate() Method</h1>

<p>The rotate() method rotates an element clockwise or counter-clockwise.</p>

<div>
This a normal div element.
</div>

<div id="myDiv">
This div element is rotated counter-clockwise with 20 degrees.
</div>

</body>
</html>





The scale() Method
Scale

The scale() method increases or decreases the size of an element (according to the parameters given for the 

width and height).

The following example increases the <div> element to be two times of its original width, and three times of 

its original height: 


<!DOCTYPE html>
<html>
<head>
<style>
div {
  margin: 150px;
  width: 200px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
  transform: scale(2,3);
}
</style>
</head>
<body>

<h1>The scale() Method</h1>

<p>The scale() method increases or decreases the size of an element.</p>

<div>
This div element is two times of its original width, and three times of its original height.
</div>

</body>
</html>



The following example decreases the <div> element to be half of its original width and height: 



<!DOCTYPE html>
<html>
<head>
<style>
div {
  margin: 150px;
  width: 200px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
  transform: scale(0.5,0.5);
}
</style>
</head>
<body>

<h1>The scale() Method</h1>

<p>The scale() method increases or decreases the size of an element.</p>

<div>
This div element is decreased to be half of its original width and height.
</div>

</body>
</html>




The scaleX() Method

The scaleX() method increases or decreases the width of an element.

The following example increases the <div> element to be two times of its original width: 


<!DOCTYPE html>
<html>
<head>
<style>
div {
  margin: 150px;
  width: 200px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
  transform: scaleX(2);
}
</style>
</head>
<body>

<h1>The scaleX() Method</h1>

<p>The scaleX() method increases or decreases the width of an element.</p>

<div>
This div element is two times of its original width.
</div>

</body>
</html>



The following example decreases the <div> element to be half of its original width: 


<!DOCTYPE html>
<html>
<head>
<style>
div {
  margin: 150px;
  width: 200px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
  transform: scaleX(0.5);
}
</style>
</head>
<body>

<h1>The scaleX() Method</h1>

<p>The scaleX() method increases or decreases the width of an element.</p>

<div>
This div element is half of its original width.
</div>

</body>
</html>




The scaleY() Method

The scaleY() method increases or decreases the height of an element.

The following example increases the <div> element to be three times of its original height: 


<!DOCTYPE html>
<html>
<head>
<style>
div {
  margin: 150px;
  width: 200px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
  transform: scaleY(3);
}
</style>
</head>
<body>

<h1>The scaleY() Method</h1>

<p>The scaleY() method increases or decreases the height of an element.</p>

<div>
This div element is three times of its original height.
</div>

</body>
</html>




The following example decreases the <div> element to be half of its original height: 


<!DOCTYPE html>
<html>
<head>
<style>
div {
  margin: 150px;
  width: 200px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
  transform: scaleY(0.5);
}
</style>
</head>
<body>

<h1>The scaleY() Method</h1>

<p>The scaleY() method increases or decreases the height of an element.</p>

<div>
This div element is half of its original height.
</div>

</body>
</html>



The skewX() Method

The skewX() method skews an element along the X-axis by the given angle.

The following example skews the <div> element 20 degrees along the X-axis:

<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 300px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
}

div#myDiv {
  transform: skewX(20deg);
}
</style>
</head>
<body>

<h1>The skewX() Method</h1>

<p>The skewX() method skews an element along the X-axis by the given angle.</p>

<div>
This a normal div element.
</div>

<div id="myDiv">
This div element is skewed 20 degrees along the X-axis.
</div>

</body>
</html>






The skewY() Method

The skewY() method skews an element along the Y-axis by the given angle.

The following example skews the <div> element 20 degrees along the Y-axis:



<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 300px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
}

div#myDiv {
  transform: skewY(20deg);
}
</style>
</head>
<body>

<h1>The skewY() Method</h1>

<p>The skewY() method skews an element along the Y-axis by the given angle.</p>

<div>
This a normal div element.
</div>

<div id="myDiv">
This div element is skewed 20 degrees along the Y-axis.
</div>

</body>
</html>




The skew() Method

The skew() method skews an element along the X and Y-axis by the given angles.

The following example skews the <div> element 20 degrees along the X-axis, and 10 degrees along the Y-axis:



<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 300px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
}

div#myDiv {
  transform: skew(20deg,10deg);
}
</style>
</head>
<body>

<h1>The skew() Method</h1>
<p>The skew() method skews an element into a given angle.</p>

<div>
This a normal div element.
</div>

<div id="myDiv">
This div element is skewed 20 degrees along the X-axis, and 10 degrees along the Y-axis.
</div>

</body>
</html>



If the second parameter is not specified, it has a zero value. So, the following example skews the <div> 

element 20 degrees along the X-axis:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 300px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
}

div#myDiv {
  transform: skew(20deg);
}
</style>
</head>
<body>

<h1>The skew() Method</h1>

<p>The skew() method skews an element into a given angle.</p>

<div>
This a normal div element.
</div>

<div id="myDiv">
This div element is skewed 20 degrees along the X-axis.
</div>

</body>
</html>



The matrix() Method
Rotate

The matrix() method combines all the 2D transform methods into one.

The matrix() method take six parameters, containing mathematic functions, which allows you to rotate, scale, 

move (translate), and skew elements.

The parameters are as follow: matrix(scaleX(),skewY(),skewX(),scaleY(),translateX(),translateY())


See the illustration of the matrix method below:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 300px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
}

div#myDiv1 {
  transform: matrix(1, -0.3, 0, 1, 0, 0);
}

div#myDiv2 {
  transform: matrix(1, 0, 0.5, 1, 150, 0);
}
</style>
</head>
<body>

<h1>The matrix() Method</h1>

<p>The matrix() method combines all the 2D transform methods into one.</p>

<div>
This a normal div element.
</div>

<div id="myDiv1">
Using the matrix() method.
</div>

<div id="myDiv2">
Another use of the matrix() method.
</div>

</body>
</html>



CSS Transform Properties

The following table lists all the 2D transform properties:
Property 	Description
transform 	Applies a 2D or 3D transformation to an element
transform-origin 	Allows you to change the position on transformed elements



CSS 2D Transform Methods
Function 	Description
matrix(n,n,n,n,n,n) 	Defines a 2D transformation, using a matrix of six values
translate(x,y) 	Defines a 2D translation, moving the element along the X- and the Y-axis
translateX(n) 	Defines a 2D translation, moving the element along the X-axis
translateY(n) 	Defines a 2D translation, moving the element along the Y-axis
scale(x,y) 	Defines a 2D scale transformation, changing the elements width and height
scaleX(n) 	Defines a 2D scale transformation, changing the element's width
scaleY(n) 	Defines a 2D scale transformation, changing the element's height
rotate(angle) 	Defines a 2D rotation, the angle is specified in the parameter
skew(x-angle,y-angle) 	Defines a 2D skew transformation along the X- and the Y-axis
skewX(angle) 	Defines a 2D skew transformation along the X-axis
skewY(angle) 	Defines a 2D skew transformation along the Y-axis

NB: Confirm the browser support before using transform property



CSS 3D Transforms

CSS 3D Transforms

CSS also supports 3D transformations.


You will learn about CSS 3d transform property in this chapter.




CSS 3D Transforms Methods

With the CSS transform property you can use the following 3D transformation methods:

    rotateX()
    rotateY()
    rotateZ()


The rotateX() Method
Rotate X

The rotateX() method rotates an element around its X-axis at a given degree. See illustration below:



<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 300px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
}

#myDiv {
  transform: rotateX(150deg);
}
</style>
</head>
<body>

<h1>The rotateX() Method</h1>

<p>The rotateX() method rotates an element around its X-axis at a given degree.</p>

<div>
This a normal div element.
</div>

<div id="myDiv">
This div element is rotated 150 degrees.
</div>

</body>
</html>



The rotateY() Method
Rotate Y

The rotateY() method rotates an element around its Y-axis at a given degree. See the example below:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 300px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
}

#myDiv {
  transform: rotateY(150deg);
}
</style>
</head>
<body>

<h1>The rotateY() Method</h1>

<p>The rotateY() method rotates an element around its Y-axis at a given degree.</p>

<div>
This a normal div element.
</div>

<div id="myDiv">
This div element is rotated 150 degrees.
</div>

</body>
</html>


 
The rotateZ() Method

The rotateZ() method rotates an element around its Z-axis at a given degree:


<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 300px;
  height: 100px;
  background-color: yellow;
  border: 1px solid black;
}

#myDiv {
  transform: rotateZ(90deg);
}
</style>
</head>
<body>

<h1>The rotateZ() Method</h1>

<p>The rotateZ() method rotates an element around its Z-axis at a given degree.</p>

<div>
This a normal div element.
</div>

<div id="myDiv">
This div element is rotated 90 degrees.
</div>

</body>
</html>



CSS Transform Properties

The following table lists all the 3D transform properties:
Property 	Description
transform 	Applies a 2D or 3D transformation to an element
transform-origin 	Allows you to change the position on transformed elements
transform-style 	Specifies how nested elements are rendered in 3D space
perspective 	Specifies the perspective on how 3D elements are viewed
perspective-origin 	Specifies the bottom position of 3D elements
backface-visibility 	Defines whether or not an element should be visible when not facing the screen



CSS 3D Transform Methods
Function 	Description
matrix3d
(n,n,n,n,n,n,n,n,n,n,n,n,n,n,n,n) 	Defines a 3D transformation, using a 4x4 matrix of 16 values
translate3d(x,y,z) 	Defines a 3D translation
translateX(x) 	Defines a 3D translation, using only the value for the X-axis
translateY(y) 	Defines a 3D translation, using only the value for the Y-axis
translateZ(z) 	Defines a 3D translation, using only the value for the Z-axis
scale3d(x,y,z) 	Defines a 3D scale transformation
scaleX(x) 	Defines a 3D scale transformation by giving a value for the X-axis
scaleY(y) 	Defines a 3D scale transformation by giving a value for the Y-axis
scaleZ(z) 	Defines a 3D scale transformation by giving a value for the Z-axis
rotate3d(x,y,z,angle) 	Defines a 3D rotation
rotateX(angle) 	Defines a 3D rotation along the X-axis
rotateY(angle) 	Defines a 3D rotation along the Y-axis
rotateZ(angle) 	Defines a 3D rotation along the Z-axis
perspective(n) 	Defines a perspective view for a 3D transformed element





CSS Transitions

CSS transitions allows you to change property values smoothly, over a given duration. Always check the 

browser compatibility before using any of these properties.


In this chapter you will learn about the following properties:

    transition
    transition-delay
    transition-duration
    transition-property
    transition-timing-function


How to Use CSS Transitions?

To create a transition effect, you must specify two things:

    the CSS property you want to add an effect to
    the duration of the effect

Note: If the duration part is not specified, the transition will have no effect, because the default value 

is 0.

The following example shows a 100px * 100px red <div> element. The <div> element has also specified a 

transition effect for the width property, with a duration of 2 seconds:

Example

div {
  width: 100px;
  height: 100px;
  background: red;
  transition: width 2s;
} 



The transition effect will start when the specified CSS property (width) changes value.

Now, let us specify a new value for the width property when a user mouses over the <div> element:


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background: red;
  transition: width 2s;
}

div:hover {
  width: 300px;
}
</style>
</head>
<body>

<h1>The transition Property</h1>

<p>Hover over the div element below, to see the transition effect:</p>
<div></div>

</body>
</html>



Notice that when the cursor mouses out of the element, it will gradually change back to its original style.


Change Several Property Values

The following example adds a transition effect for both the width and height property, with a duration of 2 

seconds for the width and 4 seconds for the height:



<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background: red;
  transition: width 2s, height 4s;
}

div:hover {
  width: 300px;
  height: 300px;
}
</style>
</head>
<body>

<h1>The transition Property</h1>

<p>Hover over the div element below, to see the transition effect:</p>

<div></div>

</body>
</html>


Specify the Speed Curve of the Transition

The transition-timing-function property specifies the speed curve of the transition effect.

The transition-timing-function property can have the following values:

    ease - specifies a transition effect with a slow start, then fast, then end slowly (this is default)
    linear - specifies a transition effect with the same speed from start to end
    ease-in - specifies a transition effect with a slow start
    ease-out - specifies a transition effect with a slow end
    ease-in-out - specifies a transition effect with a slow start and end
    cubic-bezier(n,n,n,n) - lets you define your own values in a cubic-bezier function

The following example shows some of the different speed curves that can be used:



<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background: red;
  transition: width 2s;
}

#div1 {transition-timing-function: linear;}
#div2 {transition-timing-function: ease;}
#div3 {transition-timing-function: ease-in;}
#div4 {transition-timing-function: ease-out;}
#div5 {transition-timing-function: ease-in-out;}

div:hover {
  width: 300px;
}
</style>
</head>
<body>

<h1>The transition-timing-function Property</h1>

<p>Hover over the div elements below, to see the different speed curves:</p>

<div id="div1">linear</div><br>
<div id="div2">ease</div><br>
<div id="div3">ease-in</div><br>
<div id="div4">ease-out</div><br>
<div id="div5">ease-in-out</div><br>

</body>
</html>



Delay the Transition Effect

The transition-delay property specifies a delay (in seconds) for the transition effect.

The following example has a 1 second delay before starting:



<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background: red;
  transition: width 3s;
  transition-delay: 1s;
}

div:hover {
  width: 300px;
}
</style>
</head>
<body>

<h1>The transition-delay Property</h1>

<p>Hover over the div element below, to see the transition effect:</p>

<div></div>

<p><b>Note:</b> The transition effect has a 1 second delay before starting.</p>

</body>
</html>



Transition + Transformation

The following example adds a transition effect to the transformation:


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background: red;
  transition: width 2s, height 2s, transform 2s;
}

div:hover {
  width: 300px;
  height: 300px;
  transform: rotate(180deg);
}
</style>
</head>
<body>

<h1>Transition + Transform</h1>

<p>Hover over the div element below:</p>

<div></div>

</body>
</html>



More Transition Examples

The CSS transition properties can be specified one by one, like this:


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background: red;
  transition-property: width;
  transition-duration: 2s;
  transition-timing-function: linear;
  transition-delay: 1s;
}

div:hover {
  width: 300px;
}
</style>
</head>
<body>

<h1>The transition Properties Specified One by One</h1>

<p>Hover over the div element below, to see the transition effect:</p>

<div></div>

<p><b>Note:</b> The transition effect has a 1 second delay before starting.</p>

</body>
</html>


You can also specify the CSS transition properties by using the shorthand property transition:

<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background: red;
  transition: width 2s linear 1s;
}

div:hover {
  width: 300px;
}
</style>
</head>
<body>

<h1>Using The transition Shorthand Property</h1>

<p>Hover over the div element below, to see the transition effect:</p>

<div></div>

<p><b>Note:</b> The transition effect has a 1 second delay before starting.</p>

</body>
</html>



CSS Transition Properties

The following table lists all the CSS transition properties:
Property 	Description
transition 	A shorthand property for setting the four transition properties into a single property
transition-delay 	Specifies a delay (in seconds) for the transition effect
transition-duration 	Specifies how many seconds or milliseconds a transition effect takes to complete
transition-property 	Specifies the name of the CSS property the transition effect is for
transition-timing-function 	Specifies the speed curve of the transition effect





CSS Animations


CSS animations enable animations to be added to HTML elements without using Javascript or Flash. Always 

remember to check browser support before using any of the CSS animation properties.


In this chapter you will learn about the following properties:

    @keyframes
    animation-name
    animation-duration
    animation-delay
    animation-iteration-count
    animation-direction
    animation-timing-function
    animation-fill-mode
    animation


What are CSS Animations?

An animation lets an element gradually change from one style to another.

You can change as many CSS properties you want, as many times as you want.

To use CSS animation, you must first specify some keyframes for the animation.

Keyframes hold what styles the element will have at certain times.



<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  animation-name: example;
  animation-duration: 4s;
}

@keyframes example {
  from {background-color: red;}
  to {background-color: yellow;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<div></div>

<p><b>Note:</b> When an animation is finished, it goes back to its original style.</p>

</body>
</html>



Note: The animation-duration property defines how long an animation should take to complete. If the 

animation-duration property is not specified, no animation will occur, because the default value is 0s (0 

seconds). 

In the example above we have specified when the style will change by using the keywords "from" and "to" 

(which represents 0% (start) and 100% (complete)).

It is also possible to use percent. By using percent, you can add as many style changes as you like.

The following example will change the background-color of the <div> element when the animation is 25% 

complete, 50% complete, and again when the animation is 100% complete:



<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 100px;
  height: 100px;
  background-color: red;
  animation-name: example;
  animation-duration: 4s;
}

@keyframes example {
  0%   {background-color: red;}
  25%  {background-color: yellow;}
  50%  {background-color: blue;}
  100% {background-color: green;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<div></div>

<p><b>Note:</b> When an animation is finished, it goes back to its original style.</p>

</body>
</html>




The following example will change both the background-color and the position of the <div> element when the 

animation is 25% complete, 50% complete, and again when the animation is 100% complete:



<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  animation-name: example;
  animation-duration: 4s;
}

@keyframes example {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<div></div>

<p><b>Note:</b> When an animation is finished, it goes back to its original style.</p>

</body>
</html>


The following example will change both the background-color and the position of the <div> element when the 

animation is 25% complete, 50% complete, when animation is 75% complete, and again when the animation is 

100% complete:


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  animation-name: example;
  animation-duration: 4s;
}

@keyframes example {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<div></div>

<p><b>Note:</b> When an animation is finished, it goes back to its original style.</p>

</body>
</html>


Delay an Animation

The animation-delay property specifies a delay for the start of an animation.

The following example has a 2 seconds delay before starting the animation:


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  animation-name: example;
  animation-duration: 4s;
  animation-delay: 2s;
}

@keyframes example {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>The animation-delay property specifies a delay for the start of an animation. The following example has a 

2 seconds delay before starting the animation:</p>

<div></div>

</body>
</html>


Negative values are also allowed. If using negative values, the animation will start as if it had already 

been playing for N seconds.

In the following example, the animation will start as if it had already been playing for 2 seconds (i.e. it 

begins at a state it should have normally been at exactly 2s after it starts):


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  animation-name: example;
  animation-duration: 4s;
  animation-delay: -2s;
}

@keyframes example {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>Using negative values in the animation-delay property: Here, the animation will start as if it had 

already been playing for 2 seconds:</p>

<div></div>

</body>
</html>



Set How Many Times an Animation Should Run

The animation-iteration-count property specifies the number of times an animation should run.

The following example will run the animation 3 times before it stops:


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  animation-name: example;
  animation-duration: 4s;
  animation-iteration-count: 3;
}

@keyframes example {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>The animation-iteration-count property specifies the number of times an animation should run. The 

following example will run the animation 3 times before it stops:</p>

<div></div>

</body>
</html>


The following example uses the value "infinite" to make the animation continue for ever:


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  animation-name: example;
  animation-duration: 4s;
  animation-iteration-count: infinite;
}

@keyframes example {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>The animation-iteration-count property can be set to infinite to let the animation run for ever:</p>

<div></div>

</body>
</html>



Run Animation in Reverse Direction or Alternate Cycles

The animation-direction property specifies whether an animation should be played forwards, backwards or in 

alternate cycles.

The animation-direction property can have the following values:

    normal - The animation is played as normal (forwards). This is default
    reverse - The animation is played in reverse direction (backwards)
    alternate - The animation is played forwards first, then backwards
    alternate-reverse - The animation is played backwards first, then forwards

The following example will run the animation in reverse direction (backwards):


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  animation-name: example;
  animation-duration: 4s;
  animation-direction: reverse;  
}

@keyframes example {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>The animation-direction property specifies whether an animation should be played forwards, backwards or 

in alternate cycles. The following example will run the animation in reverse direction (backwards):</p>

<div></div>

</body>
</html>



The following example uses the value "alternate" to make the animation run forwards first, then backwards:

<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  animation-name: example;
  animation-duration: 4s;
  animation-iteration-count: 2;
  animation-direction: alternate;  
}

@keyframes example {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>The animation-direction property specifies whether an animation should be played forwards, backwards or 

in alternate cycles. The following example uses the value "alternate" to make the animation run forwards 

first, then backwards:</p>

<div></div>

</body>
</html>


The following example uses the value "alternate-reverse" to make the animation run backwards first, then 

forwards:

<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  animation-name: example;
  animation-duration: 4s;
  animation-iteration-count: 2;
  animation-direction: alternate-reverse;  
}

@keyframes example {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>The animation-direction property specifies whether an animation should be played forwards, backwards or 

in alternate cycles. The following example uses the value "alternate-reverse" to make the animation run 

backwards first, then forwards:</p>

<div></div>

</body>
</html>






Specify the Speed Curve of the Animation

The animation-timing-function property specifies the speed curve of the animation.

The animation-timing-function property can have the following values:

    ease - Specifies an animation with a slow start, then fast, then end slowly (this is default)
    linear - Specifies an animation with the same speed from start to end
    ease-in - Specifies an animation with a slow start
    ease-out - Specifies an animation with a slow end
    ease-in-out - Specifies an animation with a slow start and end
    cubic-bezier(n,n,n,n) - Lets you define your own values in a cubic-bezier function



The following example shows some of the different speed curves that can be used:

<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 50px;
  background-color: red;
  font-weight: bold;
  position: relative;
  animation: mymove 5s infinite;
}

#div1 {animation-timing-function: linear;}
#div2 {animation-timing-function: ease;}
#div3 {animation-timing-function: ease-in;}
#div4 {animation-timing-function: ease-out;}
#div5 {animation-timing-function: ease-in-out;}

@keyframes mymove {
  from {left: 0px;}
  to {left: 300px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>The animation-timing-function property specifies the speed curve of the animation. The following example 

shows some of the different speed curves that can be used:</p>

<div id="div1">linear</div>
<div id="div2">ease</div>
<div id="div3">ease-in</div>
<div id="div4">ease-out</div>
<div id="div5">ease-in-out</div>

</body>
</html>



Specify the fill-mode For an Animation

CSS animations do not affect an element before the first keyframe is played or after the last keyframe is 

played. The animation-fill-mode property can override this behavior.

The animation-fill-mode property specifies a style for the target element when the animation is not playing 

(before it starts, after it ends, or both).

The animation-fill-mode property can have the following values:

    none - Default value. Animation will not apply any styles to the element before or after it is executing
    forwards - The element will retain the style values that is set by the last keyframe (depends on 

animation-direction and animation-iteration-count)
    backwards - The element will get the style values that is set by the first keyframe (depends on 

animation-direction), and retain this during the animation-delay period
    both - The animation will follow the rules for both forwards and backwards, extending the animation 

properties in both directions

The following example lets the <div> element retain the style values from the last keyframe when the 

animation ends:


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background: red;
  position: relative;
  animation-name: example;
  animation-duration: 3s;  
  animation-fill-mode: forwards;
}

@keyframes example {
  from {top: 0px;}
  to {top: 200px; background-color: blue;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>Let the div element retain the style values set by the last keyframe when the animation ends:</p>

<div></div>

</body>
</html>




The following example lets the <div> element get the style values set by the first keyframe before the 

animation starts (during the animation-delay period):

<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background: red;
  position: relative;
  animation-name: example;
  animation-duration: 3s;  
  animation-delay: 2s;
  animation-fill-mode: backwards;
}

@keyframes example {
  from {top: 0px; background-color: yellow;}
  to {top: 200px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>Let the div element get the style values set by the first keyframe before the animation starts (during 

the animation-delay period):</p>

<div></div>

</body>
</html>




The following example lets the <div> element get the style values set by the first keyframe before the 

animation starts, and retain the style values from the last keyframe when the animation ends:


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background: red;
  position: relative;
  animation-name: example;
  animation-duration: 3s;  
  animation-delay: 2s;
  animation-fill-mode: both;
}

@keyframes example {
  from {top: 0px; background-color: yellow;}
  to {top: 200px; background-color: blue;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>Let the div element get the style values set by the first keyframe before the animation starts, and 

retain the style values from the last keyframe when the animation ends:</p>

<div></div>

</body>
</html>



Animation Shorthand Property

The example below uses six of the animation properties:


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  animation-name: example;
  animation-duration: 5s;
  animation-timing-function: linear;
  animation-delay: 2s;
  animation-iteration-count: infinite;
  animation-direction: alternate;
}

@keyframes example {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>This example uses six of the animation properties:</p>

<div></div>

</body>
</html>


The same animation effect as above can be achieved by using the shorthand animation property:

<!DOCTYPE html>
<html>
<head>
<style> 
div {
  width: 100px;
  height: 100px;
  background-color: red;
  position: relative;
  animation: myfirst 5s linear 2s infinite alternate;
}

@keyframes myfirst {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}
</style>
</head>
<body>

<h1>CSS Animation</h1>

<p>This example uses the shorthand animation property:</p>

<div></div>

</body>
</html>



CSS Animation Properties

The following table lists the @keyframes rule and all the CSS animation properties:
Property 	Description
@keyframes 	Specifies the animation code
animation 	A shorthand property for setting all the animation properties
animation-delay 	Specifies a delay for the start of an animation
animation-direction 	Specifies whether an animation should be played forwards, backwards or in alternate 

cycles
animation-duration 	Specifies how long time an animation should take to complete one cycle
animation-fill-mode 	Specifies a style for the element when the animation is not playing (before it 

starts, after it ends, or both)
animation-iteration-count 	Specifies the number of times an animation should be played
animation-name 	Specifies the name of the @keyframes animation
animation-play-state 	Specifies whether the animation is running or paused
animation-timing-function 	Specifies the speed curve of the animation





CSS Tooltip

This section shows how you can create tooltips for elements on  your webpage


Basic Tooltip

Create a tooltip that appears when the user moves the mouse over an element:



<!DOCTYPE html>
<html>
<style>
.tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted black;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;

  /* Position the tooltip */
  position: absolute;
  z-index: 1;
}

.tooltip:hover .tooltiptext {
  visibility: visible;
}
</style>
<body style="text-align:center;">

<h2>Basic Tooltip</h2>

<p>Move the mouse over the text below:</p>

<div class="tooltip">Hover over me
  <span class="tooltiptext">Tooltip text</span>
</div>

<p>Note that the position of the tooltip text isn't very good. Go back to the tutorial and continue reading 

on how to position the tooltip in a desirable way.</p>

</body>
</html>


Example Explained

HTML: Use a container element (like <div>) and add the "tooltip" class to it. When the user mouse over this 

<div>, it will show the tooltip text.

The tooltip text is placed inside an inline element (like <span>) with class="tooltiptext".

CSS: The tooltip class use position:relative, which is needed to position the tooltip text 

(position:absolute). Note: See examples below on how to position the tooltip.

The tooltiptext class holds the actual tooltip text. It is hidden by default, and will be visible on hover 

(see below). We have also added some basic styles to it: 120px width, black background color, white text 

color, centered text, and 5px top and bottom padding.

The CSS border-radius property is used to add rounded corners to the tooltip text.

The :hover selector is used to show the tooltip text when the user moves the mouse over the <div> with 

class="tooltip".



Positioning Tooltips

In this example, the tooltip is placed to the right (left:105%) of the "hoverable" text (<div>). Also note 

that top:-5px is used to place it in the middle of its container element. We use the number 5 because the 

tooltip text has a top and bottom padding of 5px. If you increase its padding, also increase the value of 

the top property to ensure that it stays in the middle (if this is something you want). The same applies if 

you want the tooltip placed to the left.

The right tooltip is shown below: 

<!DOCTYPE html>
<html>
<style>
.tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted black;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;
  
  /* Position the tooltip */
  position: absolute;
  z-index: 1;
  top: -5px;
  left: 105%;
}

.tooltip:hover .tooltiptext {
  visibility: visible;
}
</style>
<body style="text-align:center;">

<h2>Right Tooltip</h2>
<p>Move the mouse over the text below:</p>

<div class="tooltip">Hover over me
  <span class="tooltiptext">Tooltip text</span>
</div>

</body>
</html>



The left Tooltip is shown below:

<!DOCTYPE html>
<html>
<style>
.tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted black;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;
  
  /* Position the tooltip */
  position: absolute;
  z-index: 1;
  top: -5px;
  right: 105%;
}

.tooltip:hover .tooltiptext {
  visibility: visible;
}
</style>
<body style="text-align:center;">

<h2>Left Tooltip</h2>
<p>Move the mouse over the text below:</p>

<div class="tooltip">Hover over me
  <span class="tooltiptext">Tooltip text</span>
</div>

</body>
</html>



If you want the tooltip to appear on top or on the bottom, see examples below. Note that we use the margin-

left property with a value of minus 60 pixels. This is to center the tooltip above/below the hoverable text. 

It is set to the half of the tooltip's width (120/2 = 60).



<!DOCTYPE html>
<html>
<style>
.tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted black;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;
  
  /* Position the tooltip */
  position: absolute;
  z-index: 1;
  bottom: 100%;
  left: 50%;
  margin-left: -60px;
}

.tooltip:hover .tooltiptext {
  visibility: visible;
}
</style>
<body style="text-align:center;">

<h2>Top Tooltip</h2>
<p>Move the mouse over the text below:</p>

<div class="tooltip">Hover over me
  <span class="tooltiptext">Tooltip text</span>
</div>

</body>
</html>



See illustration below on how to insert bottom tooltip on your HTML element:


<!DOCTYPE html>
<html>
<style>
.tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted black;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;
  
  /* Position the tooltip */
  position: absolute;
  z-index: 1;
  top: 100%;
  left: 50%;
  margin-left: -60px;
}

.tooltip:hover .tooltiptext {
  visibility: visible;
}
</style>
<body style="text-align:center;">

<h2>Bottom Tooltip</h2>
<p>Move the mouse over the text below:</p>

<div class="tooltip">Hover over me
  <span class="tooltiptext">Tooltip text</span>
</div>

</body>
</html>


Tooltip Arrows

To create an arrow that should appear from a specific side of the tooltip, add "empty" content after 

tooltip, with the pseudo-element class ::after together with the content property. The arrow itself is 

created using borders. This will make the tooltip look like a speech bubble.

This example demonstrates how to add an arrow to the bottom of the tooltip:


<!DOCTYPE html>
<html>
<style>
.tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted black;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;
  position: absolute;
  z-index: 1;
  bottom: 150%;
  left: 50%;
  margin-left: -60px;
}

.tooltip .tooltiptext::after {
  content: "";
  position: absolute;
  top: 100%;
  left: 50%;
  margin-left: -5px;
  border-width: 5px;
  border-style: solid;
  border-color: black transparent transparent transparent;
}

.tooltip:hover .tooltiptext {
  visibility: visible;
}
</style>
<body style="text-align:center;">

<h2>Top Tooltip w/ Bottom Arrow</h2>

<div class="tooltip">Hover over me
  <span class="tooltiptext">Tooltip text</span>
</div>

</body>
</html>


The explanation to the example above:


Position the arrow inside the tooltip: top: 100% will place the arrow at the bottom of the tooltip. left: 

50% will center the arrow.

Note: The border-width property specifies the size of the arrow. If you change this, also change the 

margin-left value to the same. This will keep the arrow centered.

The border-color is used to transform the content into an arrow. We set the top border to black, and the 

rest to transparent. If all sides were black, you would end up with a black square box.

This example demonstrates how to add an arrow to the top of the tooltip. Notice that we set the bottom 

border color this time:


To add top arrow (A bottom tooltip with arrow pointing up), use the code below: 



<!DOCTYPE html>
<html>
<style>
.tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted black;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;
  position: absolute;
  z-index: 1;
  top: 150%;
  left: 50%;
  margin-left: -60px;
}

.tooltip .tooltiptext::after {
  content: "";
  position: absolute;
  bottom: 100%;
  left: 50%;
  margin-left: -5px;
  border-width: 5px;
  border-style: solid;
  border-color: transparent transparent black transparent;
}

.tooltip:hover .tooltiptext {
  visibility: visible;
}
</style>
<body style="text-align:center;">

<h2>Bottom Tooltip w/ Top Arrow</h2>

<div class="tooltip">Hover over me
  <span class="tooltiptext">Tooltip text</span>
</div>

</body>
</html>



To add left arrow (a tooltip on the right with an arrow facing the left side of the element or text with 

tooltip), use the code below:


<!DOCTYPE html>
<html>
<style>
.tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted black;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;
  position: absolute;
  z-index: 1;
  top: -5px;
  left: 110%;
}

.tooltip .tooltiptext::after {
  content: "";
  position: absolute;
  top: 50%;
  right: 100%;
  margin-top: -5px;
  border-width: 5px;
  border-style: solid;
  border-color: transparent black transparent transparent;
}
.tooltip:hover .tooltiptext {
  visibility: visible;
}
</style>
<body style="text-align:center;">

<h2>Right Tooltip w/ Left Arrow</h2>

<div class="tooltip">Hover over me
  <span class="tooltiptext">Tooltip text</span>
</div>

</body>
</html>




To add an arrow pointing to the right of the tooltip, use the code below:


<!DOCTYPE html>
<html>
<style>
.tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted black;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;
  position: absolute;
  z-index: 1;
  top: -5px;
  right: 110%;
}

.tooltip .tooltiptext::after {
  content: "";
  position: absolute;
  top: 50%;
  left: 100%;
  margin-top: -5px;
  border-width: 5px;
  border-style: solid;
  border-color: transparent transparent transparent black;
}
.tooltip:hover .tooltiptext {
  visibility: visible;
}
</style>
<body style="text-align:center;">

<h2>Left Tooltip w/ Right Arrow</h2>

<div class="tooltip">Hover over me
  <span class="tooltiptext">Tooltip text</span>
</div>

</body>
</html>



Fade In Tooltips (Animation)

If you want to fade in the tooltip text when it is about to be visible, you can use the CSS transition 

property together with the opacity property, and go from being completely invisible to 100% visible, in a 

number of specified seconds (1 second in the example below):


<!DOCTYPE html>
<html>
<style>
.tooltip {
  position: relative;
  display: inline-block;
  border-bottom: 1px dotted black;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;
  position: absolute;
  z-index: 1;
  bottom: 100%;
  left: 50%;
  margin-left: -60px;
  
  /* Fade in tooltip - takes 1 second to go from 0% to 100% opac: */
  opacity: 0;
  transition: opacity 1s;
}

.tooltip:hover .tooltiptext {
  visibility: visible;
  opacity: 1;
}
</style>
<body style="text-align:center;">

<h2>Fade In Tooltip on Hover</h2>
<p>When you move the mouse over the text below, the tooltip text will fade in and take 1 second to go from 

completely invisible to visible.</p>

<div class="tooltip">Hover over me
  <span class="tooltiptext">Tooltip text</span>
</div>

</body>
</html>







CSS Styling Images



Rounded Images

Use the border-radius property to create rounded images:


A rounded image is shown below:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  border-radius: 8px;
}
</style>
</head>
<body>

<h2>Rounded Image</h2>

<p>Use the border-radius property to create rounded images:</p>

<img src="paris.jpg" alt="Paris" width="300" height="300">

</body>
</html>


 A circled image is shown below:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  border-radius: 50%;
}
</style>
</head>
<body>

<h2>Circled Image</h2>

<p>Use the border-radius property to create circled images:</p>

<img src="paris.jpg" alt="Paris" width="300" height="300">

</body>
</html>



Thumbnail Images

Use the border property to create thumbnail images.


Thumbnail image is created as shown below:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
  width: 150px;
}
</style>
</head>
<body>

<h2>Thumbnail Image</h2>

<p>Use the border property to create thumbnail images:</p>

<img src="paris.jpg" alt="Paris" style="width:150px">

</body>
</html>



Thumbnail image as link is shown below:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
  width: 150px;
}

img:hover {
  box-shadow: 0 0 2px 1px rgba(0, 140, 186, 0.5);
}
</style>
</head>
<body>

<h2>Thumbnail Image as Link</h2>

<p>Use the border property to create thumbnail images. Wrap an anchor around the image to use it as a 

link.</p>
<p>Hover over the image and click on it to see the effect.</p>

<a target="_blank" href="paris.jpg">
  <img src="paris.jpg" alt="Paris" style="width:150px">
</a>

</body>
</html>




Responsive Images

Responsive images will automatically adjust to fit the size of the screen.

Resize the browser window to see the effect:


If you want an image to scale down if it has to, but never scale up to be larger than its original size, add 

the following (max-width: 100%; height:auto;):


<!DOCTYPE html>
<html>
<head>
<style>
img {
  max-width: 100%;
  height: auto;
}
</style>
</head>
<body>

<h2>Responsive Image</h2>

<p>Responsive images will automatically adjust to fit the size of the screen.</p>
<p>Resize the browser window to see the effect:</p>

<img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">

</body>
</html>




Center an Image

To center an image, set left and right margin to auto and make it into a block element:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
</head>
<body>

<h2>Center an Image</h2>

<p>To center an image, set left and right margin to auto, and make it into a block element.</p>

<img src="paris.jpg" alt="Paris" style="width:50%">

</body>
</html>



Polaroid Images / Cards

This is an image with a text underneath enclosed in a border. See the code below:

<!DOCTYPE html>
<html>
<head>
<style>
body {margin:25px;}

div.polaroid {
  width: 80%;
  background-color: white;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  margin-bottom: 25px;
}

div.container {
  text-align: center;
  padding: 10px 20px;
}
</style>
</head>
<body>

<h2>Responsive Polaroid Images / Cards</h2>

<div class="polaroid">
  <img src="img_5terre.jpg" alt="5 Terre" style="width:100%">
  <div class="container">
  <p>Cinque Terre</p>
  </div>
</div>

<div class="polaroid">
  <img src="lights600x400.jpg" alt="Norther Lights" style="width:100%">
  <div class="container">
  <p>Northern Lights</p>
  </div>
</div>

</body>
</html>



Transparent Image

The opacity property can take a value from 0.0 - 1.0. The lower value, the more transparent:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  opacity: 0.5;
}
</style>
</head>
<body>

<h1>Image Transparency</h1>

<p>The opacity property specifies the transparency of an element. The lower the value, the more 

transparent:</p>

<p>Image with 50% opacity:</p>
<img src="img_forest.jpg" alt="Forest" width="170" height="100">

</body>
</html>



Image Text

How to position text in an image:


Top left image position:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.topleft {
  position: absolute;
  top: 8px;
  left: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>

<p>Add some text to an image in the top left corner:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="topleft">Top Left</div>
</div>

</body>
</html>


Top right image position:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.topright {
  position: absolute;
  top: 8px;
  right: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>

<p>Add some text to an image in the top right corner:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="topright">Top Right</div>
</div>

</body>
</html>


Bottom left image position:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.bottomleft {
  position: absolute;
  bottom: 8px;
  left: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>

<p>Add some text to an image in the bottom left corner:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="bottomleft">Bottom Left</div>
</div>

</body>
</html>



Bottom right image position:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.bottomright {
  position: absolute;
  bottom: 8px;
  right: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>

<p>Add some text to an image in the bottom right corner:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="bottomright">Bottom Right</div>
</div>

</body>
</html>




Center image position:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.center {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Image Text</h2>

<p>Center text in image:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="center">Centered</div>
</div>

</body>
</html>




Image Filters

The CSS filter property adds visual effects (like blur and saturation) to an element.

Note: The filter property is not supported in Internet Explorer or Edge 12.



Example

Change the color of all images to black and white (100% gray):
img {
  filter: grayscale(100%);
} 


<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 33%;
  height: auto;
  float: left; 
  max-width: 235px;
}

.blur {filter: blur(4px);}
.brightness {filter: brightness(250%);}
.contrast {filter: contrast(180%);}
.grayscale {filter: grayscale(100%);}
.huerotate {filter: hue-rotate(180deg);}
.invert {filter: invert(100%);}
.opacity {filter: opacity(50%);}
.saturate {filter: saturate(7);}
.sepia {filter: sepia(100%);}
.shadow {filter: drop-shadow(8px 8px 10px green);}
</style>
</head>
<body>

<h2>Image Filters</h2>

<p><strong>Note:</strong> The filter property is not supported in Internet Explorer or Edge 12.</p>

<img src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="blur" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="brightness" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="contrast" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="grayscale" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="huerotate" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="invert" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="opacity" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="saturate" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="sepia" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="shadow" src="pineapple.jpg" alt="Pineapple" width="300" height="300">

</body>
</html>


Image Hover Overlay

Create an overlay effect on hover:


Image with Fade in text:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 50%;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .5s ease;
  background-color: #008CBA;
}

.container:hover .overlay {
  opacity: 1;
}

.text {
  color: white;
  font-size: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
</style>
</head>
<body>

<h2>Fade in Overlay</h2>

<div class="container">
  <img src="img_avatar.png" alt="Avatar" class="image">
  <div class="overlay">
    <div class="text">Hello World</div>
  </div>
</div>

</body>
</html>



Image that fades-in a box:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 50%;
}

.image {
  opacity: 1;
  display: block;
  width: 100%;
  height: auto;
  transition: .5s ease;
  backface-visibility: hidden;
}

.middle {
  transition: .5s ease;
  opacity: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%)
}

.container:hover .image {
  opacity: 0.3;
}

.container:hover .middle {
  opacity: 1;
}

.text {
  background-color: #4CAF50;
  color: white;
  font-size: 16px;
  padding: 16px 32px;
}
</style>
</head>
<body>

<h2>Fade in a Box</h2>

<div class="container">
  <img src="img_avatar.png" alt="Avatar" class="image" style="width:100%">
  <div class="middle">
    <div class="text">John Doe</div>
  </div>
</div>
  
</body>
</html>



Image with text that slides-in from the top:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 50%;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  bottom: 100%;
  left: 0;
  right: 0;
  background-color: #008CBA;
  overflow: hidden;
  width: 100%;
  height: 0;
  transition: .5s ease;
}

.container:hover .overlay {
  bottom: 0;
  height: 100%;
}

.text {
  white-space: nowrap; 
  color: white;
  font-size: 20px;
  position: absolute;
  overflow: hidden;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
</style>
</head>
<body>

<h2>Slide in Overlay from the Top</h2>

<div class="container">
  <img src="img_avatar.png" alt="Avatar" class="image">
  <div class="overlay">
    <div class="text">Hello World</div>
  </div>
</div>
 
</body>
</html>



Image with overlay that slides-in from bottom:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 50%;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: #008CBA;
  overflow: hidden;
  width: 100%;
  height: 0;
  transition: .5s ease;
}

.container:hover .overlay {
  height: 100%;
}

.text {
  white-space: nowrap; 
  color: white;
  font-size: 20px;
  position: absolute;
  overflow: hidden;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
</style>
</head>
<body>

<h2>Slide in Overlay from the Bottom</h2>

<div class="container">
  <img src="img_avatar.png" alt="Avatar" class="image">
  <div class="overlay">
    <div class="text">Hello World</div>
  </div>
</div>

</body>
</html>


Image with overlay that slides-in from the left:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 50%;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: #008CBA;
  overflow: hidden;
  width: 0;
  height: 100%;
  transition: .5s ease;
}

.container:hover .overlay {
  width: 100%;
}

.text {
  white-space: nowrap; 
  color: white;
  font-size: 20px;
  position: absolute;
  overflow: hidden;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
</style>
</head>
<body>

<h2>Slide in Overlay from the Left</h2>

<div class="container">
  <img src="img_avatar.png" alt="Avatar" class="image">
  <div class="overlay">
    <div class="text">Hello World</div>
  </div>
</div>

</body>
</html>



Image with overlay that slides-in from right:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 50%;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  bottom: 0;
  left: 100%;
  right: 0;
  background-color: #008CBA;
  overflow: hidden;
  width: 0;
  height: 100%;
  transition: .5s ease;
}

.container:hover .overlay {
  width: 100%;
  left: 0;
}

.text {
  white-space: nowrap; 
  color: white;
  font-size: 20px;
  position: absolute;
  overflow: hidden;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
</style>
</head>
<body>

<h2>Slide in Overlay from the Right</h2>

<div class="container">
  <img src="img_avatar.png" alt="Avatar" class="image">
  <div class="overlay">
    <div class="text">Hello World</div>
  </div>
</div>

</body>
</html>




Create an image that will flip when you move the mouse pointer over it:

<!DOCTYPE html>
<html>
<head>
<style>
img:hover {
  transform: scaleX(-1);
}
</style>
</head>
<body>

<h2>Flip an Image</h2>
<p>Move your mouse over the image.</p>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>




Responsive Image Gallery

CSS can be used to create image galleries. This example use media queries to re-arrange the images on 

different screen sizes. Resize the browser window to see the effect:


<!DOCTYPE html>
<html>
<head>
<style>
div.gallery {
  border: 1px solid #ccc;
}

div.gallery:hover {
  border: 1px solid #777;
}

div.gallery img {
  width: 100%;
  height: auto;
}

div.desc {
  padding: 15px;
  text-align: center;
}

* {
  box-sizing: border-box;
}

.responsive {
  padding: 0 6px;
  float: left;
  width: 24.99999%;
}

@media only screen and (max-width: 700px) {
  .responsive {
    width: 49.99999%;
    margin: 6px 0;
  }
}

@media only screen and (max-width: 500px) {
  .responsive {
    width: 100%;
  }
}

.clearfix:after {
  content: "";
  display: table;
  clear: both;
}
</style>
</head>
<body>

<h2>Responsive Image Gallery</h2>

<h4>Resize the browser window to see the effect.</h4>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_5terre.jpg">
      <img src="img_5terre.jpg" alt="Cinque Terre" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
  </div>
</div>


<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_forest.jpg">
      <img src="img_forest.jpg" alt="Forest" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
  </div>
</div>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_lights.jpg">
      <img src="img_lights.jpg" alt="Northern Lights" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
  </div>
</div>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_mountains.jpg">
      <img src="img_mountains.jpg" alt="Mountains" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
  </div>
</div>

<div class="clearfix"></div>

<div style="padding:6px;">
  <p>This example use media queries to re-arrange the images on different screen sizes: for screens larger 

than 700px wide, it will show four images side by side, for screens smaller than 700px, it will show two 

images side by side. For screens smaller than 500px, the images will stack vertically (100%).</p>
  <p>You will learn more about media queries and responsive web design later in our CSS Tutorial.</p>
</div>

</body>
</html>



Image Modal (Advanced)

This is an example to demonstrate how CSS and JavaScript can work together.

First, use CSS to create a modal window (dialog box), and hide it by default.

Then, use a JavaScript to show the modal window and to display the image inside the modal, when a user 

clicks on the image:


<!DOCTYPE html>
<html>
<head>
<style>
#myImg {
  border-radius: 5px;
  cursor: pointer;
  transition: 0.3s;
}

#myImg:hover {opacity: 0.7;}

/* The Modal (background) */
.modal {
  display: none; /* Hidden by default */
  position: fixed; /* Stay in place */
  z-index: 1; /* Sit on top */
  padding-top: 100px; /* Location of the box */
  left: 0;
  top: 0;
  width: 100%; /* Full width */
  height: 100%; /* Full height */
  overflow: auto; /* Enable scroll if needed */
  background-color: rgb(0,0,0); /* Fallback color */
  background-color: rgba(0,0,0,0.9); /* Black w/ opacity */
}

/* Modal Content (image) */
.modal-content {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
}

/* Caption of Modal Image */
#caption {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
  text-align: center;
  color: #ccc;
  padding: 10px 0;
  height: 150px;
}

/* Add Animation */
.modal-content, #caption {  
  animation-name: zoom;
  animation-duration: 0.6s;
}

@keyframes zoom {
  from {transform: scale(0.1)} 
  to {transform: scale(1)}
}

/* The Close Button */
.close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  transition: 0.3s;
}

.close:hover,
.close:focus {
  color: #bbb;
  text-decoration: none;
  cursor: pointer;
}

/* 100% Image Width on Smaller Screens */
@media only screen and (max-width: 700px){
  .modal-content {
    width: 100%;
  }
}
</style>
</head>
<body>

<h2>Image Modal</h2>

<p>Here, we use CSS to create a modal (dialog box) that is hidden by default.</p>
<p>We use JavaScript to trigger the modal and to display the current image inside the modal when it is 

clicked on. Also note that we use the value from the image's "alt" attribute as an image caption text inside 

the modal.</p>
<p>Don't worry if you do not understand the code right away. When you are done with CSS, go to our 

JavaScript Tutorial to learn more.</p>

<img id="myImg" src="img_lights.jpg" alt="Northern Lights, Norway" width="300" height="200">

<!-- The Modal -->
<div id="myModal" class="modal">
  <span class="close">&times;</span>
  <img class="modal-content" id="img01">
  <div id="caption"></div>
</div>

<script>
// Get the modal
var modal = document.getElementById('myModal');

// Get the image and insert it inside the modal - use its "alt" text as a caption
var img = document.getElementById('myImg');
var modalImg = document.getElementById("img01");
var captionText = document.getElementById("caption");
img.onclick = function(){
  modal.style.display = "block";
  modalImg.src = this.src;
  captionText.innerHTML = this.alt;
}

// Get the <span> element that closes the modal
var span = document.getElementsByClassName("close")[0];

// When the user clicks on <span> (x), close the modal
span.onclick = function() { 
  modal.style.display = "none";
}
</script>

</body>
</html>




CSS Image Reflection (confirm browser support for image reflection):


The box-reflect property is used to create an image reflection.

The value of the box-reflect property can be: below, above, left , or right.


Here is an example of image reflection:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  -webkit-box-reflect: below;
}
</style>
</head>
<body>

<h1>CSS Image Reflection</h1>

<p>Show the reflection below the image:</p>
<img src="img_tree.png">

</body>
</html>



Image reflection to the right:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  -webkit-box-reflect: right;
}
</style>
</head>
<body>

<h1>CSS Image Reflection</h1>

<p>Show the reflection to the right of the image:</p>
<img src="img_tree.png">

</body>
</html>



CSS Reflection Offset

To specify the gap between the image and the reflection, add the size of the gap to the box-reflect 

property.


<!DOCTYPE html>
<html>
<head>
<style>
img {
  -webkit-box-reflect: below 20px;
}
</style>
</head>
<body>

<h1>CSS Image Reflection</h1>

<p>Show the reflection below the image, with a 20 pixels offset:</p>
<img src="img_tree.png">

</body>
</html>



CSS Reflection With Gradient

We can also create a fade-out effect on the reflection.


<!DOCTYPE html>
<html>
<head>
<style>
img {
  -webkit-box-reflect: below 0px linear-gradient(to bottom, rgba(0,0,0,0.0), rgba(0,0,0,0.4));
}
</style>
</head>
<body>

<h1>CSS Image Reflection</h1>

<p>Show the reflection with gradient (to make a fade-out effect):</p>
<img src="img_tree.png">

</body>
</html>





CSS The object-fit Property


The CSS object-fit property is used to specify how an <img> or <video> should be resized to fit its 

container.


This property tells the content to fill the container in a variety of ways; such as "preserve that aspect 

ratio" or "stretch up and take up as much space as possible".


Squishing an image to fit a container 200*300 pixels (with the destruction of the orginal aspect ratio)

<!DOCTYPE html>
<html>
<head>
<style>
img {
  width:200px;
  height:300px;
}
</style>
</head>
<body>

<h2>Image</h2>
<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>

Object-fit can help you modify your preferences for aspect ratio



The object-fit property can take one of the following values:

    fill - This is default. The image is resized to fill the given dimension. If necessary, the image will 

be stretched or squished to fit
    contain - The image keeps its aspect ratio, but is resized to fit within the given dimension
    cover - The image keeps its aspect ratio and fills the given dimension. The image will be clipped to fit
    none - The image is not resized
    scale-down - the image is scaled down to the smallest version of none or contain



Using object-fit: cover;

If we use object-fit: cover; the image keeps its aspect ratio and fills the given dimension. The image will 

be clipped to fit:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: cover;
}
</style>
</head>
<body>

<h2>Using object-fit: cover</h2>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>



Using object-fit: contain;

If we use object-fit: contain; the image keeps its aspect ratio, but is resized to fit within the given 

dimension:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: contain;
}
</style>
</head>
<body>

<h2>Using object-fit: contain</h2>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>



Using object-fit: fill;

If we use object-fit: fill; the image is resized to fill the given dimension. If necessary, the image will 

be stretched or squished to fit:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: fill;
}
</style>
</head>
<body>

<h2>Using object-fit: fill</h2>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>



Using object-fit: none;

If we use object-fit: none; the image is not resized:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: none;
}
</style>
</head>
<body>

<h2>Using object-fit: none</h2>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>


Using object-fit: scale-down;

If we use object-fit: scale-down; the image is scaled down to the smallest version of none or contain:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: scale-down;
}
</style>
</head>
<body>

<h2>Using object-fit: scale-down</h2>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>



Another Example

Here we have two images and we want them to fill the width of 50% of the browser window and 100% of the 

height.

In the following example we do NOT use object-fit, so when we resize the browser window, the aspect ratio of 

the images will be destroyed:


<!DOCTYPE html>
<html>
<body>

<h2>Not Using object-fit</h2>

<p>Here we use do not use "object-fit", so when we resize the browser window, the aspect ratio of the images 

will be destroyed:</p>

<div style="width:100%;height:400px;">
  <img src="rock600x400.jpg" alt="Norway" style="float:left;width:50%;height:100%;">
  <img src="paris.jpg" alt="Paris" style="float:left;width:50%;height:100%;">
</div>

</body>
</html>


In the next example, we use object-fit: cover;, so when we resize the browser window, the aspect ratio of 

the images is preserved:


<!DOCTYPE html>
<html>
<body>

<h2>Using object-fit</h2>

<p>Here we use "object-fit: cover;", so when we resize the browser window, the aspect ratio of the images is 

preserved:</p>

<div style="width:100%;height:400px;">
  <img src="rock600x400.jpg" alt="Norway" style="float:left;width:50%;height:100%;object-fit:cover;">
  <img src="paris.jpg" alt="Paris" style="float:left;width:50%;height:100%;object-fit:cover;">
</div>

</body>
</html>




CSS object-fit More Examples

The following example demonstrates all the possible values of the object-fit property in one example:


<!DOCTYPE html>
<html>
<head>
<style>
.fill {object-fit: fill;}
.contain {object-fit: contain;}
.cover {object-fit: cover;}
.scale-down {object-fit: scale-down;}
.none {object-fit: none;}
</style>
</head>
<body>

<h1>The object-fit Property</h1>

<h2>No object-fit:</h2>
<img src="paris.jpg" alt="Paris" style="width:200px;height:300px">

<h2>object-fit: fill (this is default):</h2>
<img class="fill" src="paris.jpg" alt="Paris" style="width:200px;height:300px">

<h2>object-fit: contain:</h2>
<img class="contain" src="paris.jpg" alt="Paris" style="width:200px;height:300px">

<h2>object-fit: cover:</h2>
<img class="cover" src="paris.jpg" alt="Paris" style="width:200px;height:300px">

<h2>object-fit: scale-down:</h2>
<img class="scale-down" src="paris.jpg" alt="Paris" style="width:200px;height:300px">

<h2>object-fit: none:</h2>
<img class="none" src="paris.jpg" alt="Paris" style="width:200px;height:300px">

</body>
</html>



CSS Object-* Properties

The following table lists the CSS object-* properties:
Property 	Description
object-fit 	Specifies how an <img> or <video> should be resized to fit its container
object-position 	Specifies how an <img> or <video> should be positioned with x/y coordinates inside 

its "own content box"








...........


CSS The object-position Property

The CSS object-position property is used to specify how an <img> or <video> should be positioned within its 

container.



Using the object-position Property

Let's say that the part of the image that is shown, is not positioned as we want. To position the image, we 

will use the object-position property.

Here we will use the object-position property to position the image so that the great old building is in 

center:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: cover;
  object-position: 80% 100%;
}
</style>
</head>
<body>

<h2>Using object-position</h2>

<p>Here we will use the object-position property to position the image so that the great old building is in 

center:</p>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>



Here we will use the object-position property to position the image so that the famous Eiffel Tower is in 

center:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: cover;
  object-position: 15% 100%;
}
</style>
</head>
<body>

<h2>Using object-position</h2>

<p>Here we will use the object-position property to position the image so that the famous Eiffel Tower is in 

center:</p>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>



CSS Object-* Properties

The following table lists the CSS object-* properties:
Property 	Description
object-fit 	Specifies how an <img> or <video> should be resized to fit its container
object-posititon 	Specifies how an <img> or <video> should be positioned with x/y coordinates inside 

its "own content box"







CSS Buttons

This chapter is about styling buttons in CSS. A basic button styling is shown below:

<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}
</style>
</head>
<body>

<h2>CSS Buttons</h2>

<button>Default Button</button>
<a href="#" class="button">Link Button</a>
<button class="button">Button</button>
<input type="button" class="button" value="Input Button">

</body>
</html>



Button colors

Use the background-color property to change the background color of a button:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.button2 {background-color: #008CBA;} /* Blue */
.button3 {background-color: #f44336;} /* Red */ 
.button4 {background-color: #e7e7e7; color: black;} /* Gray */ 
.button5 {background-color: #555555;} /* Black */
</style>
</head>
<body>

<h2>Button Colors</h2>

<p>Change the background color of a button with the background-color property:</p>

<button class="button">Green</button>
<button class="button button2">Blue</button>
<button class="button button3">Red</button>
<button class="button button4">Gray</button>
<button class="button button5">Black</button>

</body>
</html>


Button sizes:

Use the font-size property to change the font size of a button:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  margin: 4px 2px;
  cursor: pointer;
}

.button1 {font-size: 10px;}
.button2 {font-size: 12px;}
.button3 {font-size: 16px;}
.button4 {font-size: 20px;}
.button5 {font-size: 24px;}
</style>
</head>
<body>

<h2>Button Sizes</h2>

<p>Change the font size of a button with the font-size property:</p>

<button class="button button1">10px</button>
<button class="button button2">12px</button>
<button class="button button3">16px</button>
<button class="button button4">20px</button>
<button class="button button5">24px</button>

</body>
</html>


Use the padding property to change the padding of a button:

<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.button1 {padding: 10px 24px;}
.button2 {padding: 12px 28px;}
.button3 {padding: 14px 40px;}
.button4 {padding: 32px 16px;}
.button5 {padding: 16px;}
</style>
</head>
<body>

<h2>Button Padding</h2>

<p>Change the padding of a button with the padding property:</p>

<button class="button button1">10px 24px</button>
<button class="button button2">12px 28px</button>
<button class="button button3">14px 40px</button>
<button class="button button4">32px 16px</button>
<button class="button button5">16px</button>

</body>
</html>



Rounded Buttons
Use the border-radius property to add rounded corners to a button:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.button1 {border-radius: 2px;}
.button2 {border-radius: 4px;}
.button3 {border-radius: 8px;}
.button4 {border-radius: 12px;}
.button5 {border-radius: 50%;}
</style>
</head>
<body>

<h2>Rounded Buttons</h2>

<p>Add rounded corners to a button with the border-radius property:</p>

<button class="button button1">2px</button>
<button class="button button2">4px</button>
<button class="button button3">8px</button>
<button class="button button4">12px</button>
<button class="button button5">50%</button>

</body>
</html>



Colored Button Borders

Use the border property to add a colored border to a button:

<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.button1 {
  background-color: white; 
  color: black; 
  border: 2px solid #4CAF50;
}

.button2 {
  background-color: white; 
  color: black; 
  border: 2px solid #008CBA;
}

.button3 {
  background-color: white; 
  color: black; 
  border: 2px solid #f44336;
}

.button4 {
  background-color: white;
  color: black;
  border: 2px solid #e7e7e7;
}

.button5 {
  background-color: white;
  color: black;
  border: 2px solid #555555;
}
</style>
</head>
<body>

<h2>Colored Button Borders</h2>

<p>Use the border property to add a border to the button:</p>

<button class="button button1">Green</button>
<button class="button button2">Blue</button>
<button class="button button3">Red</button>
<button class="button button4">Gray</button>
<button class="button button5">Black</button>

</body>
</html>




Hoverable Buttons

Use the :hover selector to change the style of a button when you move the mouse over it.

Tip: Use the transition-duration property to determine the speed of the "hover" effect:



<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  transition-duration: 0.4s;
  cursor: pointer;
}

.button1 {
  background-color: white; 
  color: black; 
  border: 2px solid #4CAF50;
}

.button1:hover {
  background-color: #4CAF50;
  color: white;
}

.button2 {
  background-color: white; 
  color: black; 
  border: 2px solid #008CBA;
}

.button2:hover {
  background-color: #008CBA;
  color: white;
}

.button3 {
  background-color: white; 
  color: black; 
  border: 2px solid #f44336;
}

.button3:hover {
  background-color: #f44336;
  color: white;
}

.button4 {
  background-color: white;
  color: black;
  border: 2px solid #e7e7e7;
}

.button4:hover {background-color: #e7e7e7;}

.button5 {
  background-color: white;
  color: black;
  border: 2px solid #555555;
}

.button5:hover {
  background-color: #555555;
  color: white;
}
</style>
</head>
<body>

<h2>Hoverable Buttons</h2>

<p>Use the :hover selector to change the style of the button when you move the mouse over it.</p>
<p><strong>Tip:</strong> Use the transition-duration property to determine the speed of the "hover" 

effect:</p>

<button class="button button1">Green</button>
<button class="button button2">Blue</button>
<button class="button button3">Red</button>
<button class="button button4">Gray</button>
<button class="button button5">Black</button>

</body>
</html>



Shadow Buttons

Use the box-shadow property to add shadows to a button:

<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
  -webkit-transition-duration: 0.4s; /* Safari */
  transition-duration: 0.4s;
}

.button1 {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2), 0 6px 20px 0 rgba(0,0,0,0.19);
}

.button2:hover {
  box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24),0 17px 50px 0 rgba(0,0,0,0.19);
}
</style>
</head>
<body>

<h2>Shadow Buttons</h2>

<p>Use the box-shadow property to add shadows to the button:</p>

<button class="button button1">Shadow Button</button>
<button class="button button2">Shadow on Hover</button>

</body>
</html>



Disabled Buttons

Use the opacity property to add transparency to a button (creates a "disabled" look).

Tip: You can also add the cursor property with a value of "not-allowed", which will display a "no parking 

sign" when you mouse over the button:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.disabled {
  opacity: 0.6;
  cursor: not-allowed;
}
</style>
</head>
<body>

<h2>Disabled Button</h2>

<p>Use the opacity property to add some transparency to a button (make it look disabled):</p>

<button class="button">Normal Button</button>
<button class="button disabled">Disabled Button</button>

</body>
</html>



Button Width

By default, the size of the button is determined by its text content (as wide as its content). Use the width 

property to change the width of a button:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.button1 {width: 250px;}
.button2 {width: 50%;}
.button3 {width: 100%;}
</style>
</head>
<body>

<h2>Set Button Widths</h2>

<p>Use the width property to change the width of the button:</p>

<button class="button button1">250px</button><br>
<button class="button button2">50%</button><br>
<button class="button button3">100%</button>

<p><strong>Tip:</strong> Use pixels if you want to set a fixed width and use percent for responsive buttons 

(e.g. 50% of its parent element). Resize the browser window to see the effect.</p>

</body>
</html>


Button Groups (resembles a navigation bar)

Remove margins and add float:left to each button to create a button group:



<!DOCTYPE html>
<html>
<head>
<style>
.btn-group .button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  cursor: pointer;
  float: left;
}

.btn-group .button:hover {
  background-color: #3e8e41;
}
</style>
</head>
<body>

<h2>Button Groups</h2>

<p>Remove margins and float the buttons to create a button group:</p>

<div class="btn-group">
  <button class="button">Button</button>
  <button class="button">Button</button>
  <button class="button">Button</button>
  <button class="button">Button</button>
</div>

<p style="clear:both"><br>Remember to clear floats after, or else will this p element also float next to the 

buttons.</p>

</body>
</html>



Bordered Button Group (similar to navbar with borders)

Use the border property to create a bordered button group:

<!DOCTYPE html>
<html>
<head>
<style>
.btn-group .button {
  background-color: #4CAF50; /* Green */
  border: 1px solid green;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  cursor: pointer;
  float: left;
}

.btn-group .button:not(:last-child) {
  border-right: none; /* Prevent double borders */
}

.btn-group .button:hover {
  background-color: #3e8e41;
}
</style>
</head>
<body>

<h2>Bordered Button Group</h2>

<p>Add borders to create a bordered button group:</p>

<div class="btn-group">
  <button class="button">Button</button>
  <button class="button">Button</button>
  <button class="button">Button</button>
  <button class="button">Button</button>
</div>

<p style="clear:both"><br>Remember to clear floats after, or else will this p element also float next to the 

buttons.</p>

</body>
</html>


Vertical Button Group

Use display:block instead of float:left to group the buttons below each other, instead of side by side:

<!DOCTYPE html>
<html>
<head>
<style>
.btn-group .button {
  background-color: #4CAF50; /* Green */
  border: 1px solid green;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  font-size: 16px;
  cursor: pointer;
  width: 150px;
  display: block;
}

.btn-group .button:not(:last-child) {
  border-bottom: none; /* Prevent double borders */
}

.btn-group .button:hover {
  background-color: #3e8e41;
}
</style>
</head>
<body>

<h2>Vertical Button Group</h2>

<div class="btn-group">
  <button class="button">Button</button>
  <button class="button">Button</button>
  <button class="button">Button</button>
  <button class="button">Button</button>
</div>

</body>
</html>



Button on Image:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 100%;
  max-width: 400px;
}

.container img {
  width: 100%;
  height: auto;
}

.container .btn {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  background-color: #f1f1f1;
  color: black;
  font-size: 16px;
  padding: 16px 30px;
  border: none;
  cursor: pointer;
  border-radius: 5px;
  text-align: center;
}

.container .btn:hover {
  background-color: black;
  color: white;
}
</style>
</head>
<body>

<h2>Button on Image</h2>

<p>Add a button on an image:</p>

<div class="container">
  <img src="img_lights.jpg" alt="Snow" style="width:100%">
  <button class="btn">Button</button>
</div>

</body>
</html>



Animated Buttons
Example

Add an arrow on hover:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  display: inline-block;
  border-radius: 4px;
  background-color: #f4511e;
  border: none;
  color: #FFFFFF;
  text-align: center;
  font-size: 28px;
  padding: 20px;
  width: 200px;
  transition: all 0.5s;
  cursor: pointer;
  margin: 5px;
}

.button span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}

.button span:after {
  content: '\00bb';
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.button:hover span {
  padding-right: 25px;
}

.button:hover span:after {
  opacity: 1;
  right: 0;
}
</style>
</head>
<body>

<h2>Animated Button</h2>

<button class="button" style="vertical-align:middle"><span>Hover </span></button>

</body>
</html>







Add a "pressed" effect on click:

<!DOCTYPE html>
<html>
<head>
<style>
.button {
  display: inline-block;
  padding: 15px 25px;
  font-size: 24px;
  cursor: pointer;
  text-align: center;
  text-decoration: none;
  outline: none;
  color: #fff;
  background-color: #4CAF50;
  border: none;
  border-radius: 15px;
  box-shadow: 0 9px #999;
}

.button:hover {background-color: #3e8e41}

.button:active {
  background-color: #3e8e41;
  box-shadow: 0 5px #666;
  transform: translateY(4px);
}
</style>
</head>
<body>

<h2>Animated Button - "Pressed Effect"</h2>

<button class="button">Click Me</button>

</body>
</html>




Fade in on hover:

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.button {
  background-color: #f4511e;
  border: none;
  color: white;
  padding: 16px 32px;
  text-align: center;
  font-size: 16px;
  margin: 4px 2px;
  opacity: 0.6;
  transition: 0.3s;
  display: inline-block;
  text-decoration: none;
  cursor: pointer;
}

.button:hover {opacity: 1}
</style>
</head>
<body>

<h2>Animated Button - Fade in Effect</h2>

<button class="button">Hover Over Me</button>

</body>
</html>



Add a "ripple" effect on click:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  position: relative;
  background-color: #4CAF50;
  border: none;
  font-size: 28px;
  color: #FFFFFF;
  padding: 20px;
  width: 200px;
  text-align: center;
  transition-duration: 0.4s;
  text-decoration: none;
  overflow: hidden;
  cursor: pointer;
}

.button:after {
  content: "";
  background: #f1f1f1;
  display: block;
  position: absolute;
  padding-top: 300%;
  padding-left: 350%;
  margin-left: -20px !important;
  margin-top: -120%;
  opacity: 0;
  transition: all 0.8s
}

.button:active:after {
  padding: 0;
  margin: 0;
  opacity: 1;
  transition: 0s
}
</style>
</head>
<body>

<h2>Animated Button - Ripple Effect</h2>

<button class="button">Click Me</button>

</body>
</html>



.................
CSS Pagination


This chapter will show you how to create responsive pagination in CSS.



Simple Pagination

If you have a website with lots of pages, you may wish to add some sort of pagination to each page:


<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
}
</style>
</head>
<body>

<h2>Simple Pagination</h2>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>



Active and Hoverable Pagination

Highlight the current page with an .active class, and use the :hover selector to change the color of each 

page link when moving the mouse over them:


<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<h2>Active and Hoverable Pagination</h2>

<p>Move the mouse over the numbers.</p>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a class="active" href="#">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>




Rounded Active and Hoverable Buttons

Add the border-radius property if you want a rounded "active" and "hover" button:

<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border-radius: 5px;
}

.pagination a:hover:not(.active) {
  background-color: #ddd;
  border-radius: 5px;
}
</style>
</head>
<body>

<h2>Rounded Active and Hover Buttons</h2>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#" class="active">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>



Hoverable Transition Effect

Add the transition property to the page links to create a transition effect on hover:

<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  transition: background-color .3s;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<h2>Transition Effect on Hover</h2>

<p>Move the mouse over the numbers.</p>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#" class="active">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>




Bordered Pagination

Use the border property to add borders to the pagination:


<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  transition: background-color .3s;
  border: 1px solid #ddd;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border: 1px solid #4CAF50;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<h2>Pagination with Borders</h2>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#" class="active">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>



Rounded Borders

Tip: Add rounded borders to your first and last link in the pagination:


<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  border: 1px solid #ddd;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border: 1px solid #4CAF50;
}

.pagination a:hover:not(.active) {background-color: #ddd;}

.pagination a:first-child {
  border-top-left-radius: 5px;
  border-bottom-left-radius: 5px;
}

.pagination a:last-child {
  border-top-right-radius: 5px;
  border-bottom-right-radius: 5px;
}
</style>
</head>
<body>

<h2>Pagination with Rounded Borders</h2>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a class="active" href="#">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>



Space Between Links

Tip: Add the margin property if you do not want to group the page links:


<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  transition: background-color .3s;
  border: 1px solid #ddd;
  margin: 0 4px;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border: 1px solid #4CAF50;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<h2>Pagination with Margins</h2>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#" class="active">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>



Pagination Size

Change the size of the pagination with the font-size property:

<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  transition: background-color .3s;
  border: 1px solid #ddd;
  font-size: 22px;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border: 1px solid #4CAF50;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<h2>Pagination Size</h2>

<p>Change the font-size property to make the pagination smaller or bigger.</p>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#" class="active">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>



Centered Pagination

To center the pagination, wrap a container element (like <div>) around it with text-align:center


<!DOCTYPE html>
<html>
<head>
<style>
.center {
  text-align: center;
}

.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  transition: background-color .3s;
  border: 1px solid #ddd;
  margin: 0 4px;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border: 1px solid #4CAF50;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<h2>Centered Pagination</h2>

<div class="center">
  <div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#" class="active">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
  </div>
</div>

</body>
</html>



More Examples:


Next/Previous buttons and Navigation pagination:


<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  transition: background-color .3s;
  border: 1px solid #ddd;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border: 1px solid #4CAF50;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<p>Next/Previous buttons:</p>
<div class="pagination">
  <a href="#">?</a>
  <a href="#">?</a>
</div>

<p>Navigation pagination:</p>
<div class="pagination">
  <a href="#" class="active">Home</a>
  <a href="#">Link 1</a>
  <a href="#">Link 2</a>
  <a href="#">Link 3</a>
</div>

</body>
</html>




Breadcrumbs

Another variation of pagination is so-called "breadcrumbs":

<!DOCTYPE html>
<html>
<head>
<style>
ul.breadcrumb {
  padding: 8px 16px;
  list-style: none;
  background-color: #eee;
}

ul.breadcrumb li {display: inline;}

ul.breadcrumb li+li:before {
  padding: 8px;
  color: black;
  content: "/\00a0";
}

ul.breadcrumb li a {color: green;}
</style>
</head>
<body>

<h2>Breadcrumb Pagination</h2>

<ul class="breadcrumb">
  <li><a href="#">Home</a></li>
  <li><a href="#">Pictures</a></li>
  <li><a href="#">Summer 15</a></li>
  <li>Italy</li>
</ul>

</body>
</html>





..........

CSS Multiple Columns


CSS Multi-column Layout

The CSS multi-column layout allows easy definition of multiple columns of text - just like in newspapers:


CSS Multi-column Properties (Verify browser support for each property)

In this chapter you will learn about the following multi-column properties:

    column-count
    column-gap
    column-rule-style
    column-rule-width
    column-rule-color
    column-rule
    column-span
    column-width



CSS Create Multiple Columns

The column-count property specifies the number of columns an element should be divided into.

The following example will divide the text in the <div> element into 3 columns:  


<!DOCTYPE html>
<html>
<head>
<style>
.newspaper {
  column-count: 3;
}
</style>
</head>
<body>

<h1>Create Multiple Columns</h1>

<div class="newspaper">
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet 

dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper 

suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in 

vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et 

accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait 

nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod 

mazim placerat facer possim assum.
</div>

</body>
</html>



CSS Specify the Gap Between Columns

The column-gap property specifies the gap between the columns.

The following example specifies a 40 pixels gap between the columns:


<!DOCTYPE html>
<html>
<head>
<style>
.newspaper {
  column-count: 3;
  column-gap: 40px;
}
</style>
</head>
<body>

<h1>Specify the Gap Between Columns</h1>

<div class="newspaper">
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet 

dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper 

suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in 

vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et 

accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait 

nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod 

mazim placerat facer possim assum. 
</div>

</body>
</html>



CSS Column Rules

The column-rule-style property specifies the style of the rule between columns:


<!DOCTYPE html>
<html>
<head>
<style>
.newspaper {
  column-count: 3;
  column-gap: 40px;
  column-rule-style: solid;
}
</style>
</head>
<body>

<h1>Add a Rule Between the Columns</h1>

<div class="newspaper">
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet 

dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper 

suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in 

vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et 

accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait 

nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod 

mazim placerat facer possim assum.
</div>

</body>
</html>




The column-rule-width property specifies the width of the rule between columns:


<!DOCTYPE html>
<html>
<head>
<style> 
.newspaper {
  column-count: 3;
  column-gap: 40px;
  column-rule-style: solid;
  column-rule-width: 1px;
}
</style>
</head>
<body>

<h1>Set the Rule Width</h1>

<div class="newspaper">
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet 

dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper 

suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in 

vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et 

accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait 

nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod 

mazim placerat facer possim assum.
</div>

</body>
</html>


The column-rule-color property specifies the color of the rule between columns:

<!DOCTYPE html>
<html>
<head>
<style>
.newspaper {
  column-count: 3;
  column-gap: 40px;
  column-rule-style: solid;
  column-rule-width: 1px;
  column-rule-color: lightblue;
}
</style>
</head>
<body>

<h1>Set the Rule Color</h1>

<div class="newspaper">
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet 

dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper 

suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in 

vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et 

accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait 

nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod 

mazim placerat facer possim assum.
</div>

</body>
</html>





The column-rule property is a shorthand property for setting all the column-rule-* properties above.

The following example sets the width, style, and color of the rule between columns:


<!DOCTYPE html>
<html>
<head>
<style>
.newspaper {
  column-count: 3;
  column-gap: 40px;
  column-rule: 1px solid lightblue;
}
</style>
</head>
<body>

<h1>Use the column-rule Shorthand Property</h1>

<div class="newspaper">
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet 

dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper 

suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in 

vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et 

accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait 

nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod 

mazim placerat facer possim assum.
</div>

</body>
</html>


Specify How Many Columns an Element Should Span

The column-span property specifies how many columns an element should span across.

The following example specifies that the <h2> element should span across all columns:


<!DOCTYPE html>
<html>
<head>
<style> 
.newspaper {
  column-count: 3;
  column-gap: 40px;
  column-rule: 1px solid lightblue;
}

h2 {
  column-span: all;
}
</style>
</head>
<body>

<div class="newspaper">
<h2>Lorem Ipsum Dolor Sit Amet</h2>
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet 

dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper 

suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in 

vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et 

accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait 

nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod 

mazim placerat facer possim assum.
</div>

</body>
</html>



Specify The Column Width

The column-width property specifies a suggested, optimal width for the columns.

The following example specifies that the suggested, optimal width for the columns should be 100px:

<!DOCTYPE html>
<html>
<head>
<style> 
.newspaper {
  column-width: 100px;
}
</style>
</head>
<body>

<h1>Specify The Column Width</h1>

<div class="newspaper">
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet 

dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper 

suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in 

vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et 

accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait 

nulla facilisi. Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod 

mazim placerat facer possim assum.
</div>

</body>
</html>


CSS Multi-columns Properties

The following table lists all the multi-columns properties: 
Property 	Description
column-count 	Specifies the number of columns an element should be divided into
column-fill 	Specifies how to fill columns
column-gap 	Specifies the gap between the columns
column-rule 	A shorthand property for setting all the column-rule-* properties
column-rule-color 	Specifies the color of the rule between columns
column-rule-style 	Specifies the style of the rule between columns
column-rule-width 	Specifies the width of the rule between columns
column-span 	Specifies how many columns an element should span across
column-width 	Specifies a suggested, optimal width for the columns
columns 	A shorthand property for setting column-width and column-count




CSS User Interface

In this chapter you will learn about the following CSS user interface properties (confirm browser support 

for a property before using it):

    resize
    outline-offset


CSS Resizing

The resize property specifies if (and how) an element should be resizable by the user.



The following example lets the user resize only the width of a <div> element:

<!DOCTYPE html>
<html>
<head>
<style> 
div {
  border: 2px solid;
  padding: 20px; 
  width: 300px;
  resize: horizontal;
  overflow: auto;
}
</style>
</head>
<body>

<h1>The resize Property</h1>

<div>
  <p>Let the user resize only the width of this div element.</p>
  <p>To resize: Click and drag the bottom right corner of this div element.</p>
</div>

</body>
</html>




The following example lets the user resize only the height of a <div> element:

<!DOCTYPE html>
<html>
<head>
<style> 
div {
  border: 2px solid;
  padding: 20px; 
  width: 300px;
  resize: vertical;
  overflow: auto;
}
</style>
</head>
<body>

<h1>The resize Property</h1>

<div>
  <p>Let the user resize only the height of this div element.</p>
  <p>To resize: Click and drag the bottom right corner of this div element.</p>
</div>

</body>
</html>



The following example lets the user resize both the height and width of a <div> element:


<!DOCTYPE html>
<html>
<head>
<style> 
div {
  border: 2px solid;
  padding: 20px; 
  width: 300px;
  resize: both;
  overflow: auto;
}
</style>
</head>
<body>

<h1>The resize Property</h1>

<div>
  <p>Let the user resize both the height and the width of this div element.</p>
  <p>To resize: Click and drag the bottom right corner of this div element.</p>
</div>

</body>
</html>


In many browsers, <textarea> is resizable by default. Here, we have used the resize property to disable the 

resizability:

<!DOCTYPE html>
<html>
<head>
<style> 
textarea#test {
   resize: none;
}
</style>
</head>
<body>

<h1>The resize Property</h1>

<p>In many browsers, textarea elements are resizable by default. In this example, we have used the resize 

property to disable the resizability:</p>

<textarea id="test">Textarea - Not resizable</textarea>
<br><br>

<textarea>Textarea - Resizable (default)</textarea>

</body>
</html>



CSS Outline Offset

The outline-offset property adds space between an outline and the edge or border of an element.


Note: Outline differs from borders! Unlike border, the outline is drawn outside the element's border, and 

may overlap other content. Also, the outline is NOT a part of the element's dimensions; the element's total 

width and height is not affected by the width of the outline.


The following example uses the outline-offset property to add space between the border and the outline:



<!DOCTYPE html>
<html>
<head>
<style> 
div.ex1 {
  margin: 20px;
  border: 1px solid black;
  outline: 4px solid red;
  outline-offset: 15px;
} 

div.ex2 {
  margin: 10px;
  border: 1px solid black;
  outline: 5px dashed blue;
  outline-offset: 5px;
} 
</style>
</head>
<body>
<h1>The outline-offset Property</h1>

<div class="ex1">This div has a 4 pixels solid red outline 15 pixels outside the border edge.</div>
<br>

<div class="ex2">This div has a 5 pixels dashed blue outline 5 pixels outside the border edge.</div>

</body>
</html>



CSS User Interface Properties

The following table lists all the user interface properties:
Property 	Description
outline-offset 	Adds space between an outline and the edge or border of an element
resize 	Specifies whether or not an element is resizable by the user




CSS Variables 


css variables - The var() Function::


CSS Variables

The var() function is used to insert the value of a CSS variable.

CSS variables have access to the DOM, which means that you can create variables with local or global scope, 

change the variables with JavaScript, and change the variables based on media queries.

A good way to use CSS variables is when it comes to the colors of your design. Instead of copy and paste the 

same colors over and over again, you can place them in variables.



The Traditional Way

The following example shows the traditional way of defining some colors in a style sheet (by defining the 

colors to use, for each specific element):


<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: #1e90ff;
}

h2 {
  border-bottom: 2px solid #1e90ff;
}

.container {
  color: #1e90ff;
  background-color: #ffffff;
  padding: 15px;
}

button {
  background-color: #ffffff;
  color: #1e90ff;
  border: 1px solid #1e90ff;
  padding: 5px;
}
</style>
</head>
<body>

<h1>The Traditional Way</h1>

<div class="container">
  <h2>Lorem Ipsum</h2>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>
    <button>Yes</button>
    <button>No</button>
  </p>
</div>

</body>
</html>



Syntax of the var() Function

The var() function is used to insert the value of a CSS variable.

The syntax of the var() function is as follows:
var(--name, value)
Value 	Description
name 	Required. The variable name (must start with two dashes)
value 	Optional. The fallback value (used if the variable is not found)

Note: The variable name must begin with two dashes (--) and it is case sensitive!



How var() Works

First of all: CSS variables can have a global or local scope.

Global variables can be accessed/used through the entire document, while local variables can be used only 

inside the selector where it is declared.

To create a variable with global scope, declare it inside the :root selector. The :root selector matches the 

document's root element.

To create a variable with local scope, declare it inside the selector that is going to use it.

The following example is equal to the example above, but here we use the var() function.

First, we declare two global variables (--blue and --white). Then, we use the var() function to insert the 

value of the variables later in the style sheet:



<!DOCTYPE html>
<html>
<head>
<style>
:root {
  --blue: #1e90ff;
  --white: #ffffff; 
}

body {
  background-color: var(--blue);
}

h2 {
  border-bottom: 2px solid var(--blue);
}

.container {
  color: var(--blue);
  background-color: var(--white);
  padding: 15px;
}

button {
  background-color: var(--white);
  color: var(--blue);
  border: 1px solid var(--blue);
  padding: 5px;
}
</style>
</head>
<body>

<h1>Using the var() Function</h1>

<div class="container">
  <h2>Lorem Ipsum</h2>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>
    <button>Yes</button>
    <button>No</button>
  </p>
</div>

</body>
</html>



Advantages of using var() are:

    makes the code easier to read (more understandable)
    makes it much easier to change the color values

To change the blue and white color to a softer blue and white, you just need to change the two variable 

values:


<!DOCTYPE html>
<html>
<head>
<style>
:root {
  --blue: #6495ed;
  --white: #faf0e6; 
}

body {
  background-color: var(--blue);
}

h2 {
  border-bottom: 2px solid var(--blue);
}

.container {
  color: var(--blue);
  background-color: var(--white);
  padding: 15px;
}

button {
  background-color: var(--white);
  color: var(--blue);
  border: 1px solid var(--blue);
  padding: 5px;
}
</style>
</head>
<body>

<h1>Using the var() Function</h1>

<div class="container">
  <h2>Lorem Ipsum</h2>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>
    <button>Yes</button>
    <button>No</button>
  </p>
</div>

</body>
</html>


BROWSER SUPPORT: PLEASE CONFIRM BROWSER SUPPORT FOR THE var() FUNCTION BEFORE USE.



CSS var() Function
Property 	Description
var() 	Inserts the value of a CSS variable





CSS Overriding Variables::


Override Global Variable With Local Variable

From the previous page we have learned that global variables can be accessed/used through the entire 

document, while local variables can be used only inside the selector where it is declared.

Look at the example from the previous page:


<!DOCTYPE html>
<html>
<head>
<style>
:root {
  --blue: #1e90ff;
  --white: #ffffff; 
}

body {
  background-color: var(--blue);
}

h2 {
  border-bottom: 2px solid var(--blue);
}

.container {
  color: var(--blue);
  background-color: var(--white);
  padding: 15px;
}

button {
  background-color: var(--white);
  color: var(--blue);
  border: 1px solid var(--blue);
  padding: 5px;
}
</style>
</head>
<body>

<h1>Using the var() Function</h1>

<div class="container">
  <h2>Lorem Ipsum</h2>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>
    <button>Yes</button>
    <button>No</button>
  </p>
</div>

</body>
</html>



Sometimes we want the variables to change only in a specific section of the page.

Assume we want a different color of blue for button elements. Then, we can re-declare the --blue variable 

inside the button selector. When we use var(--blue) inside this selector, it will use the local --blue 

variable value declared here.

We see that the local --blue variable will override the global --blue variable for the button elements:



<!DOCTYPE html>
<html>
<head>
<style>
:root {
  --blue: #1e90ff;
  --white: #ffffff; 
}

body {
  background-color: var(--blue);
}

h2 {
  border-bottom: 2px solid var(--blue);
}

.container {
  color: var(--blue);
  background-color: var(--white);
  padding: 15px;
}

button {
  --blue: #0000ff; /* local variable will override global */
  background-color: var(--white);
  color: var(--blue);
  border: 1px solid var(--blue);
  padding: 5px;
}
</style>
</head>
<body>

<h1>Override Global Variable With Local Variable</h1>

<div class="container">
  <h2>Lorem Ipsum</h2>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>
    <button>Yes</button>
    <button>No</button>
  </p>
</div>

</body>
</html>



Add a New Local Variable

If a variable is to be used only one single place, we could also have declared a new local variable, like 

this:



<!DOCTYPE html>
<html>
<head>
<style>
:root {
  --blue: #1e90ff;
  --white: #ffffff; 
}

body {
  background-color: var(--blue);
}

h2 {
  border-bottom: 2px solid var(--blue);
}

.container {
  color: var(--blue);
  background-color: var(--white);
  padding: 15px;
}

button {
  --button-blue: #0000ff; /* new local variable */
  background-color: var(--white);
  color: var(--button-blue);
  border: 1px solid var(--button-blue);
  padding: 5px;
}
</style>
</head>
<body>

<h1>New Local Variable</h1>

<div class="container">
  <h2>Lorem Ipsum</h2>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>
    <button>Yes</button>
    <button>No</button>
  </p>
</div>

</body>
</html>


PLEASE CONFIRM THE BROWSER VERSION COMPATIBILITY WITH THE var() FUNCTION

CSS var() Function
Property 	Description
var() 	Inserts the value of a CSS variable




CSS Change Variables With JavaScript::


Change Variables With JavaScript

CSS variables have access to the DOM, which means that you can change them with JavaScript.

Here is an example of how you can create a script to display and change the --blue variable from the example 

used in the previous pages. 


<!DOCTYPE html>
<html>
<head>
<style>
:root {
  --blue: #1e90ff;
  --white: #ffffff; 
}

body {
  background-color: var(--blue);
}

h2 {
  border-bottom: 2px solid var(--blue);
}

.container {
  color: var(--blue);
  background-color: var(--white);
  padding: 15px;
}

.container button  {
  background-color: var(--white);
  color: var(--blue);
  border: 1px solid var(--blue);
  padding: 5px;
}
</style>

<script>
// Get the root element
var r = document.querySelector(':root');

// Create a function for getting a variable value
function myFunction_get() {
  // Get the styles (properties and values) for the root
  var rs = getComputedStyle(r);
  // Alert the value of the --blue variable
  alert("The value of --blue is: " + rs.getPropertyValue('--blue'));
}

// Create a function for setting a variable value
function myFunction_set() {
  // Set the value of variable --blue to another value (in this case "lightblue")
  r.style.setProperty('--blue', 'lightblue');
}
</script>
</head>
<body>

<h1>Get and Change CSS Variable With JavaScript</h1>

<div class="container">
  <h2>Lorem Ipsum</h2>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam semper diam at erat pulvinar, at 

pulvinar felis blandit.</p>
  <p>
    <button>Yes</button>
    <button>No</button>
  </p>
</div>
<br>

<button type="button" onclick="myFunction_get()">Get CSS Variable with JavaScript</button>
<button type="button" onclick="myFunction_set()">Change CSS Variable with JavaScript</button>

</body>
</html>


Using Variables in Media Queries

Now we want to change a variable value inside a media query.

Tip: Media Queries are about defining different style rules for different devices (screens, tablets, mobile 

phones, etc.). You can learn more Media Queries in our Media Queries Chapter.

Here, we first declare a new local variable named --fontsize for the .container class. We set its value to 

25 pixels. Then we use it in the .container class further down. Then, we create a @media rule that says 

"When the browser's width is 450px or wider, change the --fontsize variable value of the .container class to 

50px."

Here is the complete example:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
/* Variable declarations */ 
:root {
  --blue: #1e90ff;
  --white: #ffffff; 
}

.container {
  --fontsize: 25px;
}

/* Styles */ 
body {
  background-color: var(--blue);
}

h2 {
  border-bottom: 2px solid var(--blue);
}

.container {
  color: var(--blue);
  background-color: var(--white);
  padding: 15px;
  font-size: var(--fontsize);
}

@media screen and (min-width: 450px) {
  .container {
    --fontsize: 50px;
  }
}
</style>
</head>
<body>

<h1>Using Variables in Media Queries</h1>

<div class="container">
  <h2>Lorem Ipsum</h2>
  <p>When the browser's width is less than 450px, the font-size of this div is 25px. When it is 450px or 

wider, set the --fontsize variable value to 50px. Resize the browser window to see the effect.</p>
</div>

</body>
</html>




Here is another example where we also change the value of the --blue variable in the @media rule:

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
/* Variable declarations */ 
:root {
  --blue: #1e90ff;
  --white: #ffffff; 
}

.container {
  --fontsize: 25px;
}

/* Styles */ 
body {
  background-color: var(--blue);
}

h2 {
  border-bottom: 2px solid var(--blue);
}

.container {
  color: var(--blue);
  background-color: var(--white);
  padding: 15px;
  font-size: var(--fontsize);
}

@media screen and (min-width: 450px) {
  .container {
    --fontsize: 50px;
  }
  :root {
    --blue: lightblue;
  }
}
</style>
</head>
<body>

<h1>Using Variables in Media Queries</h1>

<div class="container">
  <h2>Lorem Ipsum</h2>
  <p>When the browser's width is 450px or wider, set the --fontsize variable value to 50px and the --blue 

variable value to lightblue. Resize the browser window to see the effect.</p>
</div>

</body>
</html>



,,,,,,,,,,,,,
CSS Box Sizing

The CSS box-sizing property allows us to include the padding and border in an element's total width and 

height.


Without the CSS box-sizing Property

By default, the width and height of an element is calculated like this:

width + padding + border = actual width of an element
height + padding + border = actual height of an element

This means: When you set the width/height of an element, the element often appears bigger than you have set 

(because the element's border and padding are added to the element's specified width/height).

Two <div> elements with the same specified width and height can have different sizes if one has padding 

specified. This is the consequence of the two equations above on the actual width and height of an element 

respectively. See the illustration  of this problem in the code below:

 
<!DOCTYPE html>
<html>
<head>
<style> 
.div1 {
  width: 300px;
  height: 100px;
  border: 1px solid blue;
}

.div2 {
  width: 300px;
  height: 100px;  
  padding: 50px;
  border: 1px solid red;
}
</style>
</head>
<body>

<h1>Without box-sizing</h1>

<div class="div1">This div is smaller (width is 300px and height is 100px).</div>
<br>
<div class="div2">This div is bigger (width is also 300px and height is 100px).</div>

</body>
</html>


The box-sizing property solves this problem.


With the CSS box-sizing Property

The box-sizing property allows us to include the padding and border in an element's total width and height.

If you set box-sizing: border-box; on an element, padding and border are included in the width and height. 

Here is the same example as above, with box-sizing: border-box; added to both <div> elements:

<!DOCTYPE html>
<html>
<head>
<style> 
.div1 {
  width: 300px;
  height: 100px;
  border: 1px solid blue;
  box-sizing: border-box;
}

.div2 {
  width: 300px;
  height: 100px;  
  padding: 50px;
  border: 1px solid red;
  box-sizing: border-box;
}
</style>
</head>
<body>

<h1>With box-sizing</h1>

<div class="div1">Both divs are the same size now!</div>
<br>
<div class="div2">Hooray!</div>

</body>
</html>



Since the result of using the box-sizing: border-box; is so much better, many developers want all elements 

on their pages to work this way.

The code below ensures that all elements are sized in this more intuitive way. Many browsers already use 

box-sizing: border-box; for many form elements (but not all - which is why inputs and text areas look 

different at width: 100%;).

Applying this to all elements is safe and wise:


<!DOCTYPE html>
<html>
<head>
<style>
body {
  margin: 0;
}

* {
  box-sizing: border-box;
} 

input, textarea {
  width: 100%;
}
</style>
</head>
<body>

<form action="/action_page.php">
  First name:<br>
  <input type="text" name="firstname" value="Mickey"><br>
  Last name:<br>
  <input type="text" name="lastname" value="Mouse"><br>
  Comments:<br>
  <textarea name="message" rows="5" cols="30">
  </textarea>
  <br><br>
  <input type="submit" value="Submit">
</form> 

<p><strong>Tip:</strong> Try to remove the box-sizing property from the style element and look what happens.
Notice that the width of input, textarea, and submit button will go outside of the screen.</p>

</body>
</html>



CSS Box Sizing Property
Property 	Description
box-sizing 	Defines how the width and height of an element are calculated: should they include padding 

and borders, or not



................

CSS Media Queries

CSS3 Introduced Media Queries (check to confirm browser version support for @media queries)

Media queries in CSS3 extended the CSS2 media types idea: Instead of looking for a type of device, they look 

at the capability of the device.

Media queries can be used to check many things, such as:

    width and height of the viewport
    width and height of the device
    orientation (is the tablet/phone in landscape or portrait mode?)
    resolution

Using media queries are a popular technique for delivering a tailored style sheet to desktops, laptops, 

tablets, and mobile phones (such as iPhone and Android phones).




Media Query Syntax

A media query consists of a media type and can contain one or more expressions, which resolve to either true 

or false.
@media not|only mediatype and (expressions) {
  CSS-Code;
}



The result of the query is true if the specified media type matches the type of device the document is being 

displayed on and all expressions in the media query are true. When a media query is true, the corresponding 

style sheet or style rules are applied, following the normal cascading rules.

Unless you use the not or only operators, the media type is optional and the all type will be implied.

You can also have different stylesheets for different media:
<link rel="stylesheet" media="mediatype and|not|only (expressions)" href="print.css">


CSS3 Media Types
Value 	Description
all 	Used for all media type devices
print 	Used for printers
screen 	Used for computer screens, tablets, smart-phones etc.
speech 	Used for screenreaders that "reads" the page out loud




Media Queries Simple Examples

One way to use media queries is to have an alternate CSS section right inside your style sheet.

The following example changes the background-color to lightgreen if the viewport is 480 pixels wide or wider 

(if the viewport is less than 480 pixels, the background-color will be pink):

<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: pink;
}

@media screen and (min-width: 480px) {
  body {
    background-color: lightgreen;
  }
}
</style>
</head>
<body>

<h1>Resize the browser window to see the effect!</h1>
<p>The media query will only apply if the media type is screen and the viewport is 480px wide or wider.</p>

</body>
</html>


The following example shows a menu that will float to the left of the page if the viewport is 480 pixels 

wide or wider (if the viewport is less than 480 pixels, the menu will be on top of the content):

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
.wrapper {overflow: auto;}

#main {margin-left: 4px;}

#leftsidebar {
  float: none;
  width: auto;
}

#menulist {
  margin: 0;
  padding: 0;
}

.menuitem {
  background: #CDF0F6;
  border: 1px solid #d4d4d4;
  border-radius: 4px;
  list-style-type: none;
  margin: 4px;
  padding: 2px;
}

@media screen and (min-width: 480px) {
  #leftsidebar {width: 200px; float: left;}
  #main {margin-left: 216px;}
}
</style>
</head>
<body>

<div class="wrapper">
  <div id="leftsidebar">
    <ul id="menulist">
      <li class="menuitem">Menu-item 1</li>
      <li class="menuitem">Menu-item 2</li>
      <li class="menuitem">Menu-item 3</li>
      <li class="menuitem">Menu-item 4</li>
      <li class="menuitem">Menu-item 5</li>
    </ul>
  </div>
  
  <div id="main">
    <h1>Resize the browser window to see the effect!</h1>
    <p>This example shows a menu that will float to the left of the page if the viewport is 480 pixels wide 

or wider. If the viewport is less than 480 pixels, the menu will be on top of the content.</p>
  </div>
</div>

</body>
</html>




.................


CSS Media Queries - Examples


CSS Media Queries - More Examples

Let us look at some more examples of using media queries.

Media queries are a popular technique for delivering a tailored style sheet to different devices. To 

demonstrate a simple example, we can change the background color for different devices:

<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: tan;
  color: black;
}

/* On screens that are 992px wide or less, the background color is blue */
@media screen and (max-width: 992px) {
  body {
    background-color: blue;
    color: white;
  }
}

/* On screens that are 600px wide or less, the background color is olive */
@media screen and (max-width: 600px) {
  body {
    background-color: olive;
    color: white;
  }
}
</style>
</head>
<body>

<h1>Resize the browser window to see the effect!</h1>
<p>By default, the background color of the document is "tan". If the screen size is 992px or less, the color 

will change to "blue". If it is 600px or less, it will change to "olive".</p>

</body>
</html>



The reason why 992px and 600px were used is because they are the "typical breakpoints" for devices. Learn 

more about this concept under responsive web design tutorial.



Media Queries For Menus

In this example, we use media queries to create a responsive navigation menu, that varies in design on 

different screen sizes.

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

/* Style the top navigation bar */
.topnav {
  overflow: hidden;
  background-color: #333;
}

/* Style the topnav links */
.topnav a {
  float: left;
  display: block;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

/* Change color on hover */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}

/* On screens that are 600px wide or less, make the menu links stack on top of each other instead of next to 

each other */
@media screen and (max-width: 600px) {
  .topnav a {
    float: none;
    width: 100%;
  }
}
</style>
</head>
<body>

<h2>Responsive navigation menu</h2>
<p>Resize the browser window to see the effect: When the screen is less than 600px, the navigation menu will 

be displayed vertically instead of horizontally.</p>

<div class="topnav">
  <a href="#">Link</a>
  <a href="#">Link</a>
  <a href="#">Link</a>
</div>

</body>
</html>


Media Queries For Columns

A common use of media queries, is to create a flexible layout. In this example, we create a layout that 

varies between four, two and full-width columns, depending on different screen sizes:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

/* Create four equal columns that floats next to each other */
.column {
  float: left;
  width: 25%;
  padding: 20px;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* On screens that are 992px wide or less, go from four columns to two columns */
@media screen and (max-width: 992px) {
  .column {
    width: 50%;
  }
}

/* On screens that are 600px wide or less, make the columns stack on top of each other instead of next to 

each other */
@media screen and (max-width: 600px) {
  .column {
    width: 100%;
  }
}
</style>
</head>
<body>

<h2>Responsive Four Column Layout</h2>
<p><strong>Resize the browser window to see the responsive effect.</strong> On screens that are 992px wide 

or less, the columns will resize from four columns to two columns. On screens that are 600px wide or less, 

the columns will stack on top of each other instead of next to eachother.</p>

<div class="row">
  <div class="column" style="background-color:#aaa;">
    <h2>Column 1</h2>
    <p>Some text..</p>
  </div>
  
  <div class="column" style="background-color:#bbb;">
    <h2>Column 2</h2>
    <p>Some text..</p>
  </div>
  
  <div class="column" style="background-color:#ccc;">
    <h2>Column 3</h2>
    <p>Some text..</p>
  </div>
  
  <div class="column" style="background-color:#ddd;">
    <h2>Column 4</h2>
    <p>Some text..</p>
  </div>
</div>

</body>
</html>


Tip: A more modern way of creating column layouts, is to use CSS Flexbox (see example below). However, it is 

not supported in Internet Explorer 10 and earlier versions. If you require IE6-10 support, use floats (as 

shown above). See the flexbox alternative to media queries as shown below:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

/* Container for flexboxes */
.row {
  display: flex;
  flex-wrap: wrap;
}

/* Create four equal columns */
.column {
  flex: 25%;
  padding: 20px;
}

/* On screens that are 992px wide or less, go from four columns to two columns */
@media screen and (max-width: 992px) {
  .column {
    flex: 50%;
  }
}

/* On screens that are 600px wide or less, make the columns stack on top of each other instead of next to 

each other */
@media screen and (max-width: 600px) {
  .row {
    flex-direction: column;
  }
}
</style>
</head>
<body>

<h2>Responsive Four Column Layout with Flex</h2>
<p><strong>Resize the browser window to see the responsive effect.</strong> On screens that are 992px wide 

or less, the columns will resize from four columns to two columns. On screens that are 600px wide or less, 

the columns will stack on top of each other instead of next to eachother.</p>

<div class="row">
  <div class="column" style="background-color:#aaa;">
    <h2>Column 1</h2>
    <p>Some text..</p>
  </div>
  
  <div class="column" style="background-color:#bbb;">
    <h2>Column 2</h2>
    <p>Some text..</p>
  </div>
  
  <div class="column" style="background-color:#ccc;">
    <h2>Column 3</h2>
    <p>Some text..</p>
  </div>
  
  <div class="column" style="background-color:#ddd;">
    <h2>Column 4</h2>
    <p>Some text..</p>
  </div>
</div>

</body>
</html>



Hide Elements With Media Queries

Another common use of media queries, is to hide elements on different screen sizes:

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
div.example {
  background-color: yellow;
  padding: 20px;
}

@media screen and (max-width: 600px) {
  div.example {
    display: none;
  }
}
</style>
</head>
<body>

<h2>Hide elements on different screen sizes</h2>

<div class="example">Example DIV.</div>

<p>When the browser's width is 600px wide or less, hide the div element. Resize the browser window to see 

the effect.</p>

</body>
</html>



Change Font Size With Media Queries

You can also use media queries to change the font size of an element on different screen sizes:

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
div.example {
  background-color: lightgrey;
  padding: 20px;
}

@media screen and (min-width: 600px) {
  div.example {
    font-size: 80px;
  }
}

@media screen and (max-width: 600px) {
  div.example {
    font-size: 30px;
  }
}
</style>
</head>
<body>

<h2>Change the font size of an element on different screen sizes</h2>

<div class="example">Example DIV.</div>

<p>When the browser's width is 600px wide or less, set the font-size of DIV to 30px. When it is 601px or 

wider, set the font-size to 80px. Resize the browser window to see the effect.</p>

</body>
</html>



Flexible Image Gallery

In this example, we use media queries together with flexbox to create a responsive image gallery:



<!DOCTYPE html>
<html>
<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial;
}

.header {
  text-align: center;
  padding: 32px;
}

.row {
  display: flex;
  flex-wrap: wrap;
  padding: 0 4px;
}

/* Create four equal columns that sits next to each other */
.column {
  flex: 25%;
  max-width: 25%;
  padding: 0 4px;
}

.column img {
  margin-top: 8px;
  vertical-align: middle;
}

/* Responsive layout - makes a two column-layout instead of four columns */
@media screen and (max-width: 800px) {
  .column {
    flex: 50%;
    max-width: 50%;
  }
}

/* Responsive layout - makes the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 600px) {
  .column {
    flex: 100%;
    max-width: 100%;
  }
}
</style>
<body>

<!-- Header -->
<div class="header">
  <h1>Responsive Image Grid</h1>
  <p>Resize the browser window to see the responsive effect.</p>
</div>

<!-- Photo Grid -->
<div class="row"> 
  <div class="column">
    <img src="/w3images/wedding.jpg" style="width:100%">
    <img src="/w3images/rocks.jpg" style="width:100%">
    <img src="/w3images/falls2.jpg" style="width:100%">
    <img src="/w3images/paris.jpg" style="width:100%">
    <img src="/w3images/nature.jpg" style="width:100%">
    <img src="/w3images/mist.jpg" style="width:100%">
    <img src="/w3images/paris.jpg" style="width:100%">
  </div>
  
  <div class="column">
    <img src="/w3images/underwater.jpg" style="width:100%">
    <img src="/w3images/ocean.jpg" style="width:100%">
    <img src="/w3images/wedding.jpg" style="width:100%">
    <img src="/w3images/mountainskies.jpg" style="width:100%">
    <img src="/w3images/rocks.jpg" style="width:100%">
    <img src="/w3images/underwater.jpg" style="width:100%">
  </div> 
   
  <div class="column">
    <img src="/w3images/wedding.jpg" style="width:100%">
    <img src="/w3images/rocks.jpg" style="width:100%">
    <img src="/w3images/falls2.jpg" style="width:100%">
    <img src="/w3images/paris.jpg" style="width:100%">
    <img src="/w3images/nature.jpg" style="width:100%">
    <img src="/w3images/mist.jpg" style="width:100%">
    <img src="/w3images/paris.jpg" style="width:100%">
  </div>
  
  <div class="column">
    <img src="/w3images/underwater.jpg" style="width:100%">
    <img src="/w3images/ocean.jpg" style="width:100%">
    <img src="/w3images/wedding.jpg" style="width:100%">
    <img src="/w3images/mountainskies.jpg" style="width:100%">
    <img src="/w3images/rocks.jpg" style="width:100%">
    <img src="/w3images/underwater.jpg" style="width:100%">
  </div>
</div>

</body>
</html>




Flexible Website

In this example, we use media queries together with flexbox to create a responsive website, containing a 

flexible navigation bar and flexible content. See the example below:

<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

/* Style the body */
body {
  font-family: Arial;
  margin: 0;
}

/* Header/logo Title */
.header {
  padding: 60px;
  text-align: center;
  background: #1abc9c;
  color: white;
}

/* Style the top navigation bar */
.navbar {
  display: flex;
  background-color: #333;
}

/* Style the navigation bar links */
.navbar a {
  color: white;
  padding: 14px 20px;
  text-decoration: none;
  text-align: center;
}

/* Change color on hover */
.navbar a:hover {
  background-color: #ddd;
  color: black;
}

/* Column container */
.row {  
  display: flex;
  flex-wrap: wrap;
}

/* Create two unequal columns that sits next to each other */
/* Sidebar/left column */
.side {
  flex: 30%;
  background-color: #f1f1f1;
  padding: 20px;
}

/* Main column */
.main {
  flex: 70%;
  background-color: white;
  padding: 20px;
}

/* Fake image, just for this example */
.fakeimg {
  background-color: #aaa;
  width: 100%;
  padding: 20px;
}

/* Footer */
.footer {
  padding: 20px;
  text-align: center;
  background: #ddd;
}

/* Responsive layout - when the screen is less than 700px wide, make the two columns stack on top of each 

other instead of next to each other */
@media screen and (max-width: 700px) {
  .row, .navbar {   
    flex-direction: column;
  }
}
</style>
</head>
<body>

<!-- Note -->
<div style="background:yellow;padding:5px">
  <h4 style="text-align:center">Resize the browser window to see the responsive effect.</h4>
</div>

<!-- Header -->
<div class="header">
  <h1>My Website</h1>
  <p>With a <b>flexible</b> layout.</p>
</div>

<!-- Navigation Bar -->
<div class="navbar">
  <a href="#">Link</a>
  <a href="#">Link</a>
  <a href="#">Link</a>
  <a href="#">Link</a>
</div>

<!-- The flexible grid (content) -->
<div class="row">
  <div class="side">
    <h2>About Me</h2>
    <h5>Photo of me:</h5>
    <div class="fakeimg" style="height:200px;">Image</div>
    <p>Some text about me in culpa qui officia deserunt mollit anim..</p>
    <h3>More Text</h3>
    <p>Lorem ipsum dolor sit ame.</p>
    <div class="fakeimg" style="height:60px;">Image</div><br>
    <div class="fakeimg" style="height:60px;">Image</div><br>
    <div class="fakeimg" style="height:60px;">Image</div>
  </div>
  <div class="main">
    <h2>TITLE HEADING</h2>
    <h5>Title description, Dec 7, 2017</h5>
    <div class="fakeimg" style="height:200px;">Image</div>
    <p>Some text..</p>
    <p>Sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do 

eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud 

exercitation ullamco.</p>
    <br>
    <h2>TITLE HEADING</h2>
    <h5>Title description, Sep 2, 2017</h5>
    <div class="fakeimg" style="height:200px;">Image</div>
    <p>Some text..</p>
    <p>Sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do 

eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud 

exercitation ullamco.</p>
  </div>
</div>

<!-- Footer -->
<div class="footer">
  <h2>Footer</h2>
</div>

</body>
</html>



Orientation: Portrait / Landscape

Media queries can also be used to change layout of a page depending on the orientation of the browser.

You can have a set of CSS properties that will only apply when the browser window is wider than its height, 

a so called "Landscape" orientation: 


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {
  background-color: lightgreen;
}

@media only screen and (orientation: landscape) {
  body {
    background-color: lightblue;
  }
}
</style>
</head>
<body>

<p>Resize the browser window. When the width of this document is larger than the height, the background 

color is "lightblue", otherwise it is "lightgreen".</p>

</body>
</html>




Min Width to Max Width

You can also use the (max-width: ..) and (min-width: ..) values to set a minimum width and a maximum width.

For example, when the browser's width is between 600 and 900px, change the appearance of a <div> element:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
@media screen and (max-width: 900px) and (min-width: 600px) {
  div.example {
    font-size: 50px;
    padding: 50px;
    border: 8px solid black;
    background: yellow;
  }
}
</style>
</head>
<body>

<h2>Change the appearance of DIV on different screen sizes</h2>

<div class="example">Example DIV.</div>

<p>When the browser's width is between 600 and 900px, change the appearance of DIV. 
<strong>Resize the browser window to see the effect</strong>.</p>

</body>
</html>


Using an additional value: In the example below, we add an additional media query to our already existing 

one using a comma (this will behave like an OR operator):

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
@media screen and (max-width: 900px) and (min-width: 600px), (min-width: 1100px) {
  div.example{
    font-size: 50px;
    padding: 50px;
    border: 8px solid black;
    background: yellow;
  }
}
</style>
</head>
<body>

<h2>Change the appearance of DIV on different screen sizes</h2>

<div class="example">Example DIV.</div>

<p>When the browser's width is between 600 and 900px OR above 1100px, change the appearance of DIV. 
<strong>Resize the browser window to see the effect</strong>.</p>

</body>
</html>



Check CSS @media reference to learn more about the use of the media rule. More on @media rule will come 

under CSS RWD.




............

CSS Flexbox


CSS Flexbox Layout Module::

Before the Flexbox Layout module, there were four layout modes:

    Block, for sections in a webpage
    Inline, for text
    Table, for two-dimensional table data
    Positioned, for explicit position of an element

The Flexible Box Layout Module, makes it easier to design flexible responsive layout structure without using 

float or positioning.




Flexbox Elements

To start using the Flexbox model, you need to first define a flex container. The element below represents a 

flex container (the blue area) with three flex items. 

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  margin: 10px;
  padding: 20px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>Create a Flex Container</h1>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

<p>A Flexible Layout must have a parent element with the <em>display</em> property set to <em>flex</em>.</p>

<p>Direct child elements(s) of the flexible container automatically becomes flexible items.</p>

</body>
</html>




CSS Flex Container::

Parent Element (Container)

Like we specified in the previous chapter, this is a flex container (the blue area) with three flex items:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  margin: 10px;
  padding: 20px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>Create a Flex Container</h1>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

<p>A Flexible Layout must have a parent element with the <em>display</em> property set to <em>flex</em>.</p>

<p>Direct child elements(s) of the flexible container automatically becomes flexible items.</p>

</body>
</html>


The flex container properties are:

    flex-direction
    flex-wrap
    flex-flow
    justify-content
    align-items
    align-content


The flex-direction Property

The flex-direction property defines in which direction the container wants to stack the flex items.

Example

The column value stacks the flex items vertically (from top to bottom):

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  flex-direction: column;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The flex-direction Property</h1>

<p>The "flex-direction: column;" stacks the flex items vertically (from top to bottom):</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>



Example

The column-reverse value stacks the flex items vertically (but from bottom to top):


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  flex-direction: column-reverse;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The flex-direction Property</h1>

<p>The "flex-direction: column-reverse;" stacks the flex items vertically (but from bottom to top):</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>



Example

The row value stacks the flex items horizontally (from left to right):

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  flex-direction: row;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The flex-direction Property</h1>

<p>The "flex-direction: row;" stacks the flex items horizontally (from left to right):</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>



Example

The row-reverse value stacks the flex items horizontally (but from right to left):

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  flex-direction: row-reverse;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The flex-direction Property</h1>

<p>The "flex-direction: row-reverse;" stacks the flex items horizontally (but from right to left):</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>



The flex-wrap Property

The flex-wrap property specifies whether the flex items should wrap or not.

The examples below have 12 flex items, to better demonstrate the flex-wrap property.


Example

The wrap value specifies that the flex items will wrap if necessary (wrap keeps the items within the 

container when the window size change):


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  flex-wrap: wrap;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The flex-wrap Property</h1>

<p>The "flex-wrap: wrap;" specifies that the flex items will wrap if necessary:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
  <div>7</div>
  <div>8</div>
  <div>9</div>  
  <div>10</div>
  <div>11</div>
  <div>12</div>  
</div>

<p>Try resizing the browser window.</p>

</body>
</html>



Example

The nowrap value specifies that the flex items will not wrap (this is default):


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  flex-wrap: nowrap;
  background-color: DodgerBlue;
}

.flex-container>div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The flex-wrap Property</h1>

<p>The "flex-wrap: nowrap;" specifies that the flex items will not wrap (this is default):</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
  <div>7</div>
  <div>8</div>
  <div>9</div>  
  <div>10</div>
  <div>11</div>
  <div>12</div>  
</div>

<p>Try resizing the browser window.</p>

</body>
</html>




Example

The wrap-reverse value specifies that the flexible items will wrap if necessary, in reverse order:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  flex-wrap: wrap-reverse;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The flex-wrap Property</h1>

<p>The "flex-wrap: wrap-reverse;" specifies that the flex items will wrap if necessary, in reverse 

order:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
  <div>7</div>
  <div>8</div>
  <div>9</div>  
  <div>10</div>
  <div>11</div>
  <div>12</div>  
</div>

<p>Try resizing the browser window.</p>

</body>
</html>



The flex-flow Property

The flex-flow property is a shorthand property for setting both the flex-direction and flex-wrap properties.


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  flex-flow: row wrap;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>
<h1>The flex-flow Property</h1>

<p>The flex-flow property is a shorthand property for the flex-direction and the flex-wrap properties.</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
  <div>7</div>
  <div>8</div>
  <div>9</div>  
  <div>10</div>
  <div>11</div>
  <div>12</div>  
</div>

<p>Try resizing the browser window.</p>

</body>
</html>



The justify-content Property

The justify-content property is used to align the flex items:

Example

The center value aligns the flex items at the center of the container:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  justify-content: center;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The justify-content Property</h1>

<p>The "justify-content: center;" aligns the flex items at the center of the container:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>




Example

The flex-start value aligns the flex items at the beginning of the container (this is default):


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  justify-content: flex-start;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The justify-content Property</h1>

<p>The "justify-content: flex-start;" aligns the flex items at the beginning of the container (this is 

default):</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>



Example

The flex-end value aligns the flex items at the end of the container:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  justify-content: flex-end;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The justify-content Property</h1>

<p>The "justify-content: flex-end;" aligns the flex items at the end of the container:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>



Example

The space-around value displays the flex items with space before, between, and after the lines:

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  justify-content: space-around;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The justify-content Property</h1>

<p>The "justify-content: space-around;" displays the flex items with space before, between, and after the 

lines:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>



Example

The space-between value displays the flex items with space between the lines:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  justify-content: space-between;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The justify-content Property</h1>

<p>The "justify-content: space-between;" displays the flex items with space between the lines:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>



The align-items Property

The align-items property is used to align the flex items. In these examples we use a 200 pixels high 

container, to better demonstrate the align-items property.


Example

The center value aligns the flex items in the middle of the container:

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 200px;
  align-items: center;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-items Property</h1>

<p>The "align-items: center;" aligns the flex items in the middle of the container:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>



Example

The flex-start value aligns the flex items at the top of the container:

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 200px;
  align-items: flex-start;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-items Property</h1>

<p>The "align-items: flex-start;" aligns the flex items at the top of the container:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>



Example

The flex-end value aligns the flex items at the bottom of the container:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 200px;
  align-items: flex-end;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-items Property</h1>

<p>The "align-items: flex-end;" aligns the flex items at the bottom of the container:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>



Example

The stretch value stretches the flex items to fill the container (this is default):

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 200px;
  align-items: stretch;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-items Property</h1>

<p>The "align-items: stretch;" stretches the flex items to fill the container (this is default):</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
</div>

</body>
</html>




Example

The baseline value aligns the flex items such as their baselines aligns:

Note: the example uses different font-size to demonstrate that the items gets aligned by the text baseline:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 200px;
  align-items: baseline;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>
<h1>The align-items Property</h1>

<p>The "align-items: baseline;" aligns the flex items such as their baselines aligns:</p>

<div class="flex-container">
  <div><h1>1</h1></div>
  <div><h6>2</h6></div>
  <div><h3>3</h3></div>  
  <div><small>4</small></div>  
</div>

</body>
</html>



The align-content Property

The align-content property is used to align the flex lines. In these examples we use a 600 pixels high 

container, with the flex-wrap property set to wrap, to better demonstrate the align-content property.


Example

The space-between value displays the flex lines with equal space between them:

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: space-between;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-content Property</h1>

<p>The "align-content: space-between;" displays the flex lines with equal space between them:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
  <div>7</div>
  <div>8</div>
  <div>9</div>  
  <div>10</div>
  <div>11</div>
  <div>12</div>  
</div>

</body>
</html>




Example

The space-around value displays the flex lines with space before, between, and after them:

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: space-around;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-content Property</h1>

<p>The "align-content: space-around;" displays the flex lines with space before, between, and after 

them:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
  <div>7</div>
  <div>8</div>
  <div>9</div>  
  <div>10</div>
  <div>11</div>
  <div>12</div>  
</div>

</body>
</html>



Example

The stretch value stretches the flex lines to take up the remaining space (this is default):


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: stretch;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-content Property</h1>

<p>The "align-content: stretch;" stretches the flex lines to take up the remaining space (this is 

default):</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
  <div>7</div>
  <div>8</div>
  <div>9</div>  
  <div>10</div>
  <div>11</div>
  <div>12</div>  
</div>

</body>
</html>



Example

The center value displays display the flex lines in the middle of the container:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: center;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-content Property</h1>

<p>The "align-content: center;" displays the flex lines in the middle of the container:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
  <div>7</div>
  <div>8</div>
  <div>9</div>  
  <div>10</div>
  <div>11</div>
  <div>12</div>  
</div>

</body>
</html>


Example

The flex-start value displays the flex lines at the start of the container:

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: flex-start;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-content Property</h1>

<p>The "align-content: flex-start;" displays the flex lines at the start of the container:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
  <div>7</div>
  <div>8</div>
  <div>9</div>  
  <div>10</div>
  <div>11</div>
  <div>12</div>  
</div>

</body>
</html>



Example

The flex-end value displays the flex lines at the end of the container: 


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: flex-end;
  background-color: DodgerBlue;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-content Property</h1>

<p>The "align-content: flex-end;" displays the flex lines at the end of the container:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
  <div>7</div>
  <div>8</div>
  <div>9</div>  
  <div>10</div>
  <div>11</div>
  <div>12</div>  
</div>

</body>
</html>





Perfect Centering

In the following example we will solve a very common style problem: perfect centering.

SOLUTION: Set both the justify-content and align-items properties to center, and the flex item will be 

perfectly centered:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 300px;
  background-color: DodgerBlue;
}

.flex-container>div {
  background-color: #f1f1f1;
  color: white;
  width: 100px;
  height: 100px;
}
</style>
</head>
<body>

<h1>Perfect Centering</h1>

<p>A flex container with both the justify-content and the align-items properties set to <em>center</em> will 

align the item(s) in the center (in both axis).</p>

<div class="flex-container">
  <div></div>
</div>

</body>
</html>




The CSS Flexbox Container Properties

The following table lists all the CSS Flexbox Container properties:
Property 	Description
align-content 	Modifies the behavior of the flex-wrap property. It is similar to align-items, but instead 

of aligning flex items, it aligns flex lines
align-items 	Vertically aligns the flex items when the items do not use all available space on the 

cross-axis
display 	Specifies the type of box used for an HTML element
flex-direction 	Specifies the direction of the flexible items inside a flex container
flex-flow 	A shorthand property for flex-direction and flex-wrap
flex-wrap 	Specifies whether the flex items should wrap or not, if there is not enough room for them on 

one flex line
justify-content 	Horizontally aligns the flex items when the items do not use all available space on 

the main-axis



CSS Flex Items::

Child Elements (Items)

The direct child elements of a flex container automatically becomes flexible (flex) items. The element above 

represents four blue flex items inside a grey flex container.


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  background-color: #f1f1f1;
}

.flex-container > div {
  background-color: DodgerBlue;
  color: white;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>Flexible Items</h1>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div> 
  <div>4</div>
</div>

<p>All direct children of a flexible container becomes flexible items.</p>

</body>
</html>





The flex item properties are:

    order
    flex-grow
    flex-shrink
    flex-basis
    flex
    align-self



The order Property

The order property specifies the order of the flex items. The first flex item in the code does not have to 

appear as the first item in the layout. The order value must be a number, default value is 0.


Example

The order property can change the order of the flex items:

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  align-items: stretch;
  background-color: #f1f1f1;
}

.flex-container>div {
  background-color: DodgerBlue;
  color: white;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The order Property</h1>

<p>Use the order property to sort the flex items as you like:</p>

<div class="flex-container">
  <div style="order: 3">1</div>
  <div style="order: 2">2</div>
  <div style="order: 4">3</div> 
  <div style="order: 1">4</div>
</div>

</body>
</html>



The flex-grow Property

The flex-grow property specifies how much a flex item will grow relative to the rest of the flex items. The 

value must be a number, default value is 0.


Example

Make the third flex item grow eight times faster than the other flex items:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  align-items: stretch;
  background-color: #f1f1f1;
}

.flex-container > div {
  background-color: DodgerBlue;
  color: white;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The flex-grow Property</h1>

<p>Make the third flex item grow eight times faster than the other flex items:</p>

<div class="flex-container">
  <div style="flex-grow: 1">1</div>
  <div style="flex-grow: 1">2</div>
  <div style="flex-grow: 8">3</div>
</div>

</body>
</html>




The flex-shrink Property

The flex-shrink property specifies how much a flex item will shrink relative to the rest of the flex items. 

The value must be a number, default value is 1.


Example

Do not let the third flex item shrink as much as the other flex items:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  align-items: stretch;
  background-color: #f1f1f1;
}

.flex-container>div {
  background-color: DodgerBlue;
  color: white;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The flex-shrink Property</h1>

<p>Do not let the third flex item shrink as much as the other flex items:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div style="flex-shrink: 0">3</div>
  <div>4</div>
  <div>5</div>
  <div>6</div>
  <div>7</div>
  <div>8</div>
  <div>9</div>
  <div>10</div>
</div>

</body>
</html>



The flex-basis Property

The flex-basis property specifies the initial length of a flex item.


Example

Set the initial length of the third flex item to 200 pixels:

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  align-items: stretch;
  background-color: #f1f1f1;
}

.flex-container > div {
  background-color: DodgerBlue;
  color: white;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The flex-basis Property</h1>

<p>Set the initial length of the third flex item to 200 pixels:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div style="flex-basis:200px">3</div>
  <div>4</div>
</div>

</body>
</html>



The flex Property

The flex property is a shorthand property for the flex-grow, flex-shrink, and flex-basis properties.


Example

Make the third flex item not growable (0), not shrinkable (0), and with an initial length of 200 pixels:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  align-items: stretch;
  background-color: #f1f1f1;
}

.flex-container>div {
  background-color: DodgerBlue;
  color: white;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The flex Property</h1>

<p>Make the third flex item not growable (0), not shrinkable (0), and with an initial length of 200 

pixels:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div style="flex: 0 0 200px">3</div>
  <div>4</div>
</div>

</body>
</html>



The align-self Property

The align-self property specifies the alignment for the selected item inside the flexible container.

The align-self property overrides the default alignment set by the container's align-items property.

In these examples we use a 200 pixels high container, to better demonstrate the align-self property:


Example

Align the third flex item in the middle of the container:


<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 200px;
  background-color: #f1f1f1;
}

.flex-container > div {
  background-color: DodgerBlue;
  color: white;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-self Property</h1>

<p>The "align-self: center;" aligns the selected flex item in the middle of the container:</p>

<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div style="align-self: center">3</div>
  <div>4</div>
</div>

<p>The align-self property overrides the align-items property of the container.</p>

</body>
</html>



Example

Align the second flex item at the top of the container, and the third flex item at the bottom of the 

container:

<!DOCTYPE html>
<html>
<head>
<style>
.flex-container {
  display: flex;
  height: 200px;
  background-color: #f1f1f1;
}

.flex-container > div {
  background-color: DodgerBlue;
  color: white;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-self Property</h1>

<p>The "align-self: flex-start;" aligns the selected flex item at the top of the container.</p>
<p>The "align-self: flex-end;" aligns the selected flex item at the bottom of the container.</p>

<div class="flex-container">
  <div>1</div>
  <div style="align-self: flex-start">2</div>
  <div style="align-self: flex-end">3</div>
  <div>4</div>
</div>

<p>The align-self property overrides the align-items property of the container.</p>

</body>
</html>




The CSS Flexbox Items Properties

The following table lists all the CSS Flexbox Items properties:
Property 	Description
align-self 	Specifies the alignment for a flex item (overrides the flex container's align-items 

property)
flex 	A shorthand property for the flex-grow, flex-shrink, and the flex-basis properties
flex-basis 	Specifies the initial length of a flex item
flex-grow 	Specifies how much a flex item will grow relative to the rest of the flex items inside the 

same container
flex-shrink 	Specifies how much a flex item will shrink relative to the rest of the flex items inside the 

same container
order 	Specifies the order of the flex items inside the same container




CSS Flex Responsive


Responsive Flexbox

You learned from the CSS Media Queries chapter that you can use media queries to create different layouts 

for different screen sizes and devices.

For example, if you want to create a two-column layout for most screen sizes, and a one-column layout for 

small screen sizes (such as phones and tablets), you can change the flex-direction from row to column at a 

specific breakpoint (800px in the example below):


<!DOCTYPE html>
<html>
<head>
<style>
* {
  box-sizing: border-box;
}

.flex-container {
  display: flex;
  flex-direction: row;
  font-size: 30px;
  text-align: center;
}

.flex-item-left {
  background-color: #f1f1f1;
  padding: 10px;
  flex: 50%;
}

.flex-item-right {
  background-color: dodgerblue;
  padding: 10px;
  flex: 50%;
}

/* Responsive layout - makes a one column-layout instead of two-column layout */
@media (max-width: 800px) {
  .flex-container {
    flex-direction: column;
  }
}
</style>
</head>
<body>

<h1>Responsive Flexbox</h1>

<p>The "flex-direction: row;" stacks the flex items horizontally (from left to right).</p>
<p>The "flex-direction: column;" stacks the flex items vertically (from top to bottom).</p>
<p><b>Resize the browser window to see that the direction changes when the 
screen size is 800px wide or smaller.</b></p>

<div class="flex-container">
  <div class="flex-item-left">1</div>
  <div class="flex-item-right">2</div>
</div>

</body>
</html>



Another way is to change the percentage of the flex property of the flex items to create different layouts 

for different screen sizes. Note that we also have to include flex-wrap: wrap; on the flex container for 

this example to work:

<!DOCTYPE html>
<html>
<head>
<style>
* {
  box-sizing: border-box;
}

.flex-container {
  display: flex;
  flex-wrap: wrap;
  font-size: 30px;
  text-align: center;
}

.flex-item-left {
  background-color: #f1f1f1;
  padding: 10px;
  flex: 50%;
}

.flex-item-right {
  background-color: dodgerblue;
  padding: 10px;
  flex: 50%;
}

/* Responsive layout - makes a one column-layout instead of a two-column layout */
@media (max-width: 800px) {
  .flex-item-right, .flex-item-left {
    flex: 100%;
  }
}
</style>
</head>
<body>

<h1>Responsive Flexbox</h1>

<p>In this example, we change the percentage of flex to create different layouts for different screen 

sizes.</p>
<p><b>Resize the browser window to see that the direction changes when the 
screen size is 800px wide or smaller.</b></p>

<div class="flex-container">
  <div class="flex-item-left">1</div>
  <div class="flex-item-right">2</div>
</div>

</body>
</html>



Responsive Image Gallery using Flexbox

Use flexbox to create a responsive image gallery that varies between four, two or full-width images, 

depending on screen size:

<!DOCTYPE html>
<html>
<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial;
}

.header {
  text-align: center;
  padding: 32px;
}

.row {
  display: flex;
  flex-wrap: wrap;
  padding: 0 4px;
}

/* Create four equal columns that sits next to each other */
.column {
  flex: 25%;
  max-width: 25%;
  padding: 0 4px;
}

.column img {
  margin-top: 8px;
  vertical-align: middle;
}

/* Responsive layout - makes a two column-layout instead of four columns */
@media (max-width: 800px) {
  .column {
    flex: 50%;
    max-width: 50%;
  }
}

/* Responsive layout - makes the two columns stack on top of each other instead of next to each other */
@media (max-width: 600px) {
  .column {
    flex: 100%;
    max-width: 100%;
  }
}
</style>
<body>

<!-- Header -->
<div class="header">
  <h1>Responsive Image Gallery</h1>
  <p>Resize the browser window to see the responsive effect.</p>
</div>

<!-- Photo Grid -->
<div class="row"> 
  <div class="column">
    <img src="/w3images/wedding.jpg" style="width:100%">
    <img src="/w3images/rocks.jpg" style="width:100%">
    <img src="/w3images/falls2.jpg" style="width:100%">
    <img src="/w3images/paris.jpg" style="width:100%">
    <img src="/w3images/nature.jpg" style="width:100%">
    <img src="/w3images/mist.jpg" style="width:100%">
    <img src="/w3images/paris.jpg" style="width:100%">
  </div>
  
  <div class="column">
    <img src="/w3images/underwater.jpg" style="width:100%">
    <img src="/w3images/ocean.jpg" style="width:100%">
    <img src="/w3images/wedding.jpg" style="width:100%">
    <img src="/w3images/mountainskies.jpg" style="width:100%">
    <img src="/w3images/rocks.jpg" style="width:100%">
    <img src="/w3images/underwater.jpg" style="width:100%">
  </div> 
   
  <div class="column">
    <img src="/w3images/wedding.jpg" style="width:100%">
    <img src="/w3images/rocks.jpg" style="width:100%">
    <img src="/w3images/falls2.jpg" style="width:100%">
    <img src="/w3images/paris.jpg" style="width:100%">
    <img src="/w3images/nature.jpg" style="width:100%">
    <img src="/w3images/mist.jpg" style="width:100%">
    <img src="/w3images/paris.jpg" style="width:100%">
  </div>
  
  <div class="column">
    <img src="/w3images/underwater.jpg" style="width:100%">
    <img src="/w3images/ocean.jpg" style="width:100%">
    <img src="/w3images/wedding.jpg" style="width:100%">
    <img src="/w3images/mountainskies.jpg" style="width:100%">
    <img src="/w3images/rocks.jpg" style="width:100%">
    <img src="/w3images/underwater.jpg" style="width:100%">
  </div>
</div>

</body>
</html>



Responsive Website using Flexbox

Use flexbox to create a responsive website, containing a flexible navigation bar and flexible content:


<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

/* Style the body */
body {
  font-family: Arial;
  margin: 0;
}

/* Header/logo Title */
.header {
  padding: 60px;
  text-align: center;
  background: #1abc9c;
  color: white;
}

/* Style the top navigation bar */
.navbar {
  display: flex;
  background-color: #333;
}

/* Style the navigation bar links */
.navbar a {
  color: white;
  padding: 14px 20px;
  text-decoration: none;
  text-align: center;
}

/* Change color on hover */
.navbar a:hover {
  background-color: #ddd;
  color: black;
}

/* Column container */
.row {  
  display: flex;
  flex-wrap: wrap;
}

/* Create two unequal columns that sits next to each other */
/* Sidebar/left column */
.side {
  flex: 30%;
  background-color: #f1f1f1;
  padding: 20px;
}

/* Main column */
.main {
  flex: 70%;
  background-color: white;
  padding: 20px;
}

/* Fake image, just for this example */
.fakeimg {
  background-color: #aaa;
  width: 100%;
  padding: 20px;
}

/* Footer */
.footer {
  padding: 20px;
  text-align: center;
  background: #ddd;
}

/* Responsive layout - when the screen is less than 700px wide, make the two columns stack on top of each 

other instead of next to each other */
@media screen and (max-width: 700px) {
  .row, .navbar {   
    flex-direction: column;
  }
}
</style>
</head>
<body>

<!-- Note -->
<div style="background:yellow;padding:5px">
  <h4 style="text-align:center">Resize the browser window to see the responsive effect.</h4>
</div>

<!-- Header -->
<div class="header">
  <h1>My Website</h1>
  <p>With a <b>flexible</b> layout.</p>
</div>

<!-- Navigation Bar -->
<div class="navbar">
  <a href="#">Link</a>
  <a href="#">Link</a>
  <a href="#">Link</a>
  <a href="#">Link</a>
</div>

<!-- The flexible grid (content) -->
<div class="row">
  <div class="side">
    <h2>About Me</h2>
    <h5>Photo of me:</h5>
    <div class="fakeimg" style="height:200px;">Image</div>
    <p>Some text about me in culpa qui officia deserunt mollit anim..</p>
    <h3>More Text</h3>
    <p>Lorem ipsum dolor sit ame.</p>
    <div class="fakeimg" style="height:60px;">Image</div><br>
    <div class="fakeimg" style="height:60px;">Image</div><br>
    <div class="fakeimg" style="height:60px;">Image</div>
  </div>
  <div class="main">
    <h2>TITLE HEADING</h2>
    <h5>Title description, Dec 7, 2017</h5>
    <div class="fakeimg" style="height:200px;">Image</div>
    <p>Some text..</p>
    <p>Sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do 

eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud 

exercitation ullamco.</p>
    <br>
    <h2>TITLE HEADING</h2>
    <h5>Title description, Sep 2, 2017</h5>
    <div class="fakeimg" style="height:200px;">Image</div>
    <p>Some text..</p>
    <p>Sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do 

eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud 

exercitation ullamco.</p>
  </div>
</div>

<!-- Footer -->
<div class="footer">
  <h2>Footer</h2>
</div>

</body>
</html>



.........


Responsive Web Design - Introduction

What is Responsive Web Design?

Responsive web design makes your web page look good on all devices.

Responsive web design uses only HTML and CSS.

Responsive web design is not a program or a JavaScript.



Designing For The Best Experience For All Users

Web pages can be viewed using many different devices: desktops, tablets, and phones. Your web page should 

look good, and be easy to use, regardless of the device.

Web pages should not leave out information to fit smaller devices, but rather adapt its content to fit any 

device.

It is called responsive web design when you use CSS and HTML to resize, hide, shrink, enlarge, or move the 

content to make it look good on any screen.

Don't worry if you don't understand the example below, we will break down the code, step-by-step, in the 

next chapters.


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* {
  box-sizing: border-box;
}

.row::after {
  content: "";
  clear: both;
  display: table;
}

[class*="col-"] {
  float: left;
  padding: 15px;
}

html {
  font-family: "Lucida Sans", sans-serif;
}

.header {
  background-color: #9933cc;
  color: #ffffff;
  padding: 15px;
}

.menu ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.menu li {
  padding: 8px;
  margin-bottom: 7px;
  background-color: #33b5e5;
  color: #ffffff;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.menu li:hover {
  background-color: #0099cc;
}

.aside {
  background-color: #33b5e5;
  padding: 15px;
  color: #ffffff;
  text-align: center;
  font-size: 14px;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.footer {
  background-color: #0099cc;
  color: #ffffff;
  text-align: center;
  font-size: 12px;
  padding: 15px;
}

/* For mobile phones: */
[class*="col-"] {
  width: 100%;
}

@media only screen and (min-width: 600px) {
  /* For tablets: */
  .col-s-1 {width: 8.33%;}
  .col-s-2 {width: 16.66%;}
  .col-s-3 {width: 25%;}
  .col-s-4 {width: 33.33%;}
  .col-s-5 {width: 41.66%;}
  .col-s-6 {width: 50%;}
  .col-s-7 {width: 58.33%;}
  .col-s-8 {width: 66.66%;}
  .col-s-9 {width: 75%;}
  .col-s-10 {width: 83.33%;}
  .col-s-11 {width: 91.66%;}
  .col-s-12 {width: 100%;}
}
@media only screen and (min-width: 768px) {
  /* For desktop: */
  .col-1 {width: 8.33%;}
  .col-2 {width: 16.66%;}
  .col-3 {width: 25%;}
  .col-4 {width: 33.33%;}
  .col-5 {width: 41.66%;}
  .col-6 {width: 50%;}
  .col-7 {width: 58.33%;}
  .col-8 {width: 66.66%;}
  .col-9 {width: 75%;}
  .col-10 {width: 83.33%;}
  .col-11 {width: 91.66%;}
  .col-12 {width: 100%;}
}
</style>
</head>
<body>

<div class="header">
  <h1>Chania</h1>
</div>

<div class="row">
  <div class="col-3 col-s-3 menu">
    <ul>
      <li>The Flight</li>
      <li>The City</li>
      <li>The Island</li>
      <li>The Food</li>
    </ul>
  </div>

  <div class="col-6 col-s-9">
    <h1>The City</h1>
    <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two 

parts, the old town and the modern city.</p>
  </div>

  <div class="col-3 col-s-12">
    <div class="aside">
      <h2>What?</h2>
      <p>Chania is a city on the island of Crete.</p>
      <h2>Where?</h2>
      <p>Crete is a Greek island in the Mediterranean Sea.</p>
      <h2>How?</h2>
      <p>You can reach Chania airport from all over Europe.</p>
    </div>
  </div>
</div>

<div class="footer">
  <p>Resize the browser window to see how the content respond to the resizing.</p>
</div>

</body>
</html>





Responsive Web Design - The Viewport

What is The Viewport?

The viewport is the user's visible area of a web page.

The viewport varies with the device, and will be smaller on a mobile phone than on a computer screen.

Before tablets and mobile phones, web pages were designed only for computer screens, and it was common for 

web pages to have a static design and a fixed size.

Then, when we started surfing the internet using tablets and mobile phones, fixed size web pages were too 

large to fit the viewport. To fix this, browsers on those devices scaled down the entire web page to fit the 

screen.

This was not perfect!! But a quick fix.




Setting The Viewport

HTML5 introduced a method to let web designers take control over the viewport, through the <meta> tag.

You should include the following <meta> viewport element in all your web pages:



<meta name="viewport" content="width=device-width, initial-scale=1.0">


This gives the browser instructions on how to control the page's dimensions and scaling.

The width=device-width part sets the width of the page to follow the screen-width of the device (which will 

vary depending on the device).

The initial-scale=1.0 part sets the initial zoom level when the page is first loaded by the browser.

Here is an example of a web page without the viewport meta tag, and the same web page with the viewport meta 

tag:


Size Content to The Viewport

Users are used to scroll websites vertically on both desktop and mobile devices - but not horizontally!

So, if the user is forced to scroll horizontally, or zoom out, to see the whole web page it results in a 

poor user experience.

Some additional rules to follow:

1. Do NOT use large fixed width elements - For example, if an image is displayed at a width wider than the 

viewport it can cause the viewport to scroll horizontally. Remember to adjust this content to fit within the 

width of the viewport.

2. Do NOT let the content rely on a particular viewport width to render well - Since screen dimensions and 

width in CSS pixels vary widely between devices, content should not rely on a particular viewport width to 

render well.

3. Use CSS media queries to apply different styling for small and large screens - Setting large absolute CSS 

widths for page elements will cause the element to be too wide for the viewport on a smaller device. 

Instead, consider using relative width values, such as width: 100%. Also, be careful of using large absolute 

positioning values. It may cause the element to fall outside the viewport on small devices.




Responsive Web Design - Grid-View

What is a Grid-View?

Many web pages are based on a grid-view, which means that the page is divided into columns:

Using a grid-view is very helpful when designing web pages. It makes it easier to place elements on the 

page.


A responsive grid-view often has 12 columns, and has a total width of 100%, and will shrink and expand as 

you resize the browser window.


Building a Responsive Grid-View

Lets start building a responsive grid-view.

First ensure that all HTML elements have the box-sizing property set to border-box. This makes sure that the 

padding and border are included in the total width and height of the elements.

Add the following code in your CSS:
* {
  box-sizing: border-box;
}


Read more about the box-sizing property in our CSS Box Sizing chapter.

The following example shows a simple responsive web page, with two columns:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* {
  box-sizing: border-box;
}

.header {
  border: 1px solid red;
  padding: 15px;
}

.menu {
  width: 25%;
  float: left;
  padding: 15px;
  border: 1px solid red;
}

.main {
  width: 75%;
  float: left;
  padding: 15px;
  border: 1px solid red;
}
</style>
</head>
<body>

<div class="header">
  <h1>Chania</h1>
</div>

<div class="menu">
  <ul>
    <li>The Flight</li>
    <li>The City</li>
    <li>The Island</li>
    <li>The Food</li>
  </ul>
</div>

<div class="main">
  <h1>The City</h1>
  <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two 

parts, the old town and the modern city.</p>
  <p>Resize the browser window to see how the content respond to the resizing.</p>
</div>

</body>
</html>



The example above is fine if the web page only contains two columns.

However, we want to use a responsive grid-view with 12 columns, to have more control over the web page.

First we must calculate the percentage for one column: 100% / 12 columns = 8.33%.

Then we make one class for each of the 12 columns, class="col-" and a number defining how many columns the 

section should span:



<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* {
  box-sizing: border-box;
}

.header {
  border: 1px solid red;
  padding: 15px;
}

.row::after {
  content: "";
  clear: both;
  display: table;
}

[class*="col-"] {
  float: left;
  padding: 15px;
  border: 1px solid red;
}

.col-1 {width: 8.33%;}
.col-2 {width: 16.66%;}
.col-3 {width: 25%;}
.col-4 {width: 33.33%;}
.col-5 {width: 41.66%;}
.col-6 {width: 50%;}
.col-7 {width: 58.33%;}
.col-8 {width: 66.66%;}
.col-9 {width: 75%;}
.col-10 {width: 83.33%;}
.col-11 {width: 91.66%;}
.col-12 {width: 100%;}
</style>
</head>
<body>

<div class="header">
  <h1>Chania</h1>
</div>

<div class="row">

<div class="col-3">
  <ul>
    <li>The Flight</li>
    <li>The City</li>
    <li>The Island</li>
    <li>The Food</li>
  </ul>
</div>

<div class="col-9">
  <h1>The City</h1>
  <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two 

parts, the old town and the modern city.</p>
  <p>Resize the browser window to see how the content respond to the resizing.</p>
</div>

</div>

</body>
</html>



To make all these columns should be floating to the left, and have a padding of 15px, the required CSS is:


CSS:
[class*="col-"] {
  float: left;
  padding: 15px;
  border: 1px solid red;
}



Each row should be wrapped in a <div>. The number of columns inside a row should always add up to 12:
HTML:
<div class="row">
  <div class="col-3">...</div> <!-- 25% -->
  <div class="col-9">...</div> <!-- 75% -->
</div>


The columns inside a row are all floating to the left, and are therefore taken out of the flow of the page, 

and other elements will be placed as if the columns do not exist. To prevent this, we will add a style that 

clears the flow:
CSS:
.row::after {
  content: "";
  clear: both;
  display: table;
}


We also want to add some styles and colors to make it look better:

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* {
  box-sizing: border-box;
}

.row::after {
  content: "";
  clear: both;
  display: table;
}

[class*="col-"] {
  float: left;
  padding: 15px;
}

.col-1 {width: 8.33%;}
.col-2 {width: 16.66%;}
.col-3 {width: 25%;}
.col-4 {width: 33.33%;}
.col-5 {width: 41.66%;}
.col-6 {width: 50%;}
.col-7 {width: 58.33%;}
.col-8 {width: 66.66%;}
.col-9 {width: 75%;}
.col-10 {width: 83.33%;}
.col-11 {width: 91.66%;}
.col-12 {width: 100%;}

html {
  font-family: "Lucida Sans", sans-serif;
}

.header {
  background-color: #9933cc;
  color: #ffffff;
  padding: 15px;
}

.menu ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.menu li {
  padding: 8px;
  margin-bottom: 7px;
  background-color: #33b5e5;
  color: #ffffff;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.menu li:hover {
  background-color: #0099cc;
}
</style>
</head>
<body>

<div class="header">
  <h1>Chania</h1>
</div>

<div class="row">
  <div class="col-3 menu">
    <ul>
      <li>The Flight</li>
      <li>The City</li>
      <li>The Island</li>
      <li>The Food</li>
    </ul>
  </div>

  <div class="col-9">
    <h1>The City</h1>
    <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two 

parts, the old town and the modern city.</p>
    <p>Resize the browser window to see how the content respond to the resizing.</p>
  </div>
</div>

</body>
</html>


Notice that the webpage in the example does not look good when you resize the browser window to a very small 

width. In the next chapter you will learn how to fix that.




Responsive Web Design - Media Queries


What is a Media Query?

Media query is a CSS technique introduced in CSS3.

It uses the @media rule to include a block of CSS properties only if a certain condition is true.


Example

If the browser window is 600px or smaller, the background color will be lightblue:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {
  background-color: lightgreen;
}

@media only screen and (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
</style>
</head>
<body>

<p>Resize the browser window. When the width of this document is 600 pixels or less, the background-color is 

"lightblue", otherwise it is "lightgreen".</p>

</body>
</html>



Add a Breakpoint

Earlier in this tutorial we made a web page with rows and columns, and it was responsive, but it did not 

look good on a small screen.

Media queries can help with that. We can add a breakpoint where certain parts of the design will behave 

differently on each side of the breakpoint.


Use a media query to add a breakpoint at 768px:


Example

When the screen (browser window) gets smaller than 768px, each column should have a width of 100%:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* {
  box-sizing: border-box;
}

.row::after {
  content: "";
  clear: both;
  display: block;
}

[class*="col-"] {
  float: left;
  padding: 15px;
}

html {
  font-family: "Lucida Sans", sans-serif;
}

.header {
  background-color: #9933cc;
  color: #ffffff;
  padding: 15px;
}

.menu ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.menu li {
  padding: 8px;
  margin-bottom: 7px;
  background-color: #33b5e5;
  color: #ffffff;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.menu li:hover {
  background-color: #0099cc;
}

.aside {
  background-color: #33b5e5;
  padding: 15px;
  color: #ffffff;
  text-align: center;
  font-size: 14px;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.footer {
  background-color: #0099cc;
  color: #ffffff;
  text-align: center;
  font-size: 12px;
  padding: 15px;
}

/* For desktop: */
.col-1 {width: 8.33%;}
.col-2 {width: 16.66%;}
.col-3 {width: 25%;}
.col-4 {width: 33.33%;}
.col-5 {width: 41.66%;}
.col-6 {width: 50%;}
.col-7 {width: 58.33%;}
.col-8 {width: 66.66%;}
.col-9 {width: 75%;}
.col-10 {width: 83.33%;}
.col-11 {width: 91.66%;}
.col-12 {width: 100%;}

@media only screen and (max-width: 768px) {
  /* For mobile phones: */
  [class*="col-"] {
    width: 100%;
  }
}
</style>
</head>
<body>

<div class="header">
  <h1>Chania</h1>
</div>

<div class="row">
  <div class="col-3 menu">
    <ul>
    <li>The Flight</li>
    <li>The City</li>
    <li>The Island</li>
    <li>The Food</li>
    </ul>
  </div>

  <div class="col-6">
    <h1>The City</h1>
    <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two 

parts, the old town and the modern city.</p>
  </div>

  <div class="col-3 right">
    <div class="aside">
      <h2>What?</h2>
      <p>Chania is a city on the island of Crete.</p>
      <h2>Where?</h2>
      <p>Crete is a Greek island in the Mediterranean Sea.</p>
      <h2>How?</h2>
      <p>You can reach Chania airport from all over Europe.</p>
    </div>
  </div>
</div>

<div class="footer">
  <p>Resize the browser window to see how the content respond to the resizing.</p>
</div>

</body>
</html>



Always Design for Mobile First

Mobile First means designing for mobile before designing for desktop or any other device (This will make the 

page display faster on smaller devices).

This means that we must make some changes in our CSS.

Instead of changing styles when the width gets smaller than 768px, we should change the design when the 

width gets larger than 768px. This will make our design Mobile First:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* {
  box-sizing: border-box;
}

.row::after {
  content: "";
  clear: both;
  display: table;
}

[class*="col-"] {
  float: left;
  padding: 15px;
}

html {
  font-family: "Lucida Sans", sans-serif;
}

.header {
  background-color: #9933cc;
  color: #ffffff;
  padding: 15px;
}

.menu ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.menu li {
  padding: 8px;
  margin-bottom: 7px;
  background-color: #33b5e5;
  color: #ffffff;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.menu li:hover {
  background-color: #0099cc;
}

.aside {
  background-color: #33b5e5;
  padding: 15px;
  color: #ffffff;
  text-align: center;
  font-size: 14px;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.footer {
  background-color: #0099cc;
  color: #ffffff;
  text-align: center;
  font-size: 12px;
  padding: 15px;
}

/* For mobile phones: */
[class*="col-"] {
  width: 100%;
}

@media only screen and (min-width: 768px) {
  /* For desktop: */
  .col-1 {width: 8.33%;}
  .col-2 {width: 16.66%;}
  .col-3 {width: 25%;}
  .col-4 {width: 33.33%;}
  .col-5 {width: 41.66%;}
  .col-6 {width: 50%;}
  .col-7 {width: 58.33%;}
  .col-8 {width: 66.66%;}
  .col-9 {width: 75%;}
  .col-10 {width: 83.33%;}
  .col-11 {width: 91.66%;}
  .col-12 {width: 100%;}
}
</style>
</head>
<body>

<div class="header">
  <h1>Chania</h1>
</div>

<div class="row">
  <div class="col-3 menu">
    <ul>
      <li>The Flight</li>
      <li>The City</li>
      <li>The Island</li>
      <li>The Food</li>
    </ul>
  </div>

  <div class="col-6">
    <h1>The City</h1>
    <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two 

parts, the old town and the modern city.</p>
  </div>

  <div class="col-3 right">
    <div class="aside">
      <h2>What?</h2>
      <p>Chania is a city on the island of Crete.</p>
      <h2>Where?</h2>
      <p>Crete is a Greek island in the Mediterranean Sea.</p>
      <h2>How?</h2>
      <p>You can reach Chania airport from all over Europe.</p>
    </div>
  </div>
</div>

<div class="footer">
  <p>Resize the browser window to see how the content respond to the resizing.</p>
</div>

</body>
</html>



Another Breakpoint

You can add as many breakpoints as you like.

We will also insert a breakpoint between tablets and mobile phones.


We do this by adding one more media query (at 600px), and a set of new classes for devices larger than 600px 

(but smaller than 768px):


Example

Note that the two sets of classes are almost identical, the only difference is the name (col- and col-s-):


 /* For mobile phones: */
[class*="col-"] {
  width: 100%;
}

@media only screen and (min-width: 600px) {
  /* For tablets: */
  .col-s-1 {width: 8.33%;}
  .col-s-2 {width: 16.66%;}
  .col-s-3 {width: 25%;}
  .col-s-4 {width: 33.33%;}
  .col-s-5 {width: 41.66%;}
  .col-s-6 {width: 50%;}
  .col-s-7 {width: 58.33%;}
  .col-s-8 {width: 66.66%;}
  .col-s-9 {width: 75%;}
  .col-s-10 {width: 83.33%;}
  .col-s-11 {width: 91.66%;}
  .col-s-12 {width: 100%;}
}

@media only screen and (min-width: 768px) {
  /* For desktop: */
  .col-1 {width: 8.33%;}
  .col-2 {width: 16.66%;}
  .col-3 {width: 25%;}
  .col-4 {width: 33.33%;}
  .col-5 {width: 41.66%;}
  .col-6 {width: 50%;}
  .col-7 {width: 58.33%;}
  .col-8 {width: 66.66%;}
  .col-9 {width: 75%;}
  .col-10 {width: 83.33%;}
  .col-11 {width: 91.66%;}
  .col-12 {width: 100%;}
} 


It might seem odd that we have two sets of identical classes, but it gives us the opportunity in HTML, to 

decide what will happen with the columns at each breakpoint:

HTML Example

For desktop:

The first and the third section will both span 3 columns each. The middle section will span 6 columns.

For tablets:

The first section will span 3 columns, the second will span 9, and the third section will be displayed below 

the first two sections, and it will span 12 columns:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* {
  box-sizing: border-box;
}

.row::after {
  content: "";
  clear: both;
  display: table;
}

[class*="col-"] {
  float: left;
  padding: 15px;
}

html {
  font-family: "Lucida Sans", sans-serif;
}

.header {
  background-color: #9933cc;
  color: #ffffff;
  padding: 15px;
}

.menu ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.menu li {
  padding: 8px;
  margin-bottom: 7px;
  background-color: #33b5e5;
  color: #ffffff;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.menu li:hover {
  background-color: #0099cc;
}

.aside {
  background-color: #33b5e5;
  padding: 15px;
  color: #ffffff;
  text-align: center;
  font-size: 14px;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.footer {
  background-color: #0099cc;
  color: #ffffff;
  text-align: center;
  font-size: 12px;
  padding: 15px;
}

/* For mobile phones: */
[class*="col-"] {
  width: 100%;
}

@media only screen and (min-width: 600px) {
  /* For tablets: */
  .col-s-1 {width: 8.33%;}
  .col-s-2 {width: 16.66%;}
  .col-s-3 {width: 25%;}
  .col-s-4 {width: 33.33%;}
  .col-s-5 {width: 41.66%;}
  .col-s-6 {width: 50%;}
  .col-s-7 {width: 58.33%;}
  .col-s-8 {width: 66.66%;}
  .col-s-9 {width: 75%;}
  .col-s-10 {width: 83.33%;}
  .col-s-11 {width: 91.66%;}
  .col-s-12 {width: 100%;}
}
@media only screen and (min-width: 768px) {
  /* For desktop: */
  .col-1 {width: 8.33%;}
  .col-2 {width: 16.66%;}
  .col-3 {width: 25%;}
  .col-4 {width: 33.33%;}
  .col-5 {width: 41.66%;}
  .col-6 {width: 50%;}
  .col-7 {width: 58.33%;}
  .col-8 {width: 66.66%;}
  .col-9 {width: 75%;}
  .col-10 {width: 83.33%;}
  .col-11 {width: 91.66%;}
  .col-12 {width: 100%;}
}
</style>
</head>
<body>

<div class="header">
  <h1>Chania</h1>
</div>

<div class="row">
  <div class="col-3 col-s-3 menu">
    <ul>
      <li>The Flight</li>
      <li>The City</li>
      <li>The Island</li>
      <li>The Food</li>
    </ul>
  </div>

  <div class="col-6 col-s-9">
    <h1>The City</h1>
    <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two 

parts, the old town and the modern city.</p>
  </div>

  <div class="col-3 col-s-12">
    <div class="aside">
      <h2>What?</h2>
      <p>Chania is a city on the island of Crete.</p>
      <h2>Where?</h2>
      <p>Crete is a Greek island in the Mediterranean Sea.</p>
      <h2>How?</h2>
      <p>You can reach Chania airport from all over Europe.</p>
    </div>
  </div>
</div>

<div class="footer">
  <p>Resize the browser window to see how the content respond to the resizing.</p>
</div>

</body>
</html>



Typical Device Breakpoints

There are tons of screens and devices with different heights and widths, so it is hard to create an exact 

breakpoint for each device. To keep things simple you could target five groups:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
.example {
  padding: 20px;
  color: white;
}
/* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {
  .example {background: red;}
}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {
  .example {background: green;}
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
  .example {background: blue;}
} 

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {
  .example {background: orange;}
} 

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
  .example {background: pink;}
}
</style>
</head>
<body>

<h2>Typical Media Query Breakpoints</h2>
<p class="example">Resize the browser window to see how the background color of this paragraph changes on 

different screen sizes.</p>

</body>
</html>





Orientation: Portrait / Landscape

Media queries can also be used to change layout of a page depending on the orientation of the browser.

You can have a set of CSS properties that will only apply when the browser window is wider than its height, 

a so called "Landscape" orientation: 



Example

The web page will have a lightblue background if the orientation is in landscape mode:

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {
  background-color: lightgreen;
}

@media only screen and (orientation: landscape) {
  body {
    background-color: lightblue;
  }
}
</style>
</head>
<body>

<p>Resize the browser window. When the width of this document is larger than the height, the background 

color is "lightblue", otherwise it is "lightgreen".</p>

</body>
</html>



Hide Elements With Media Queries

Another common use of media queries, is to hide elements on different screen sizes:
I will be hidden on small screens.

Example


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
div.example {
  background-color: yellow;
  padding: 20px;
}

@media screen and (max-width: 600px) {
  div.example {
    display: none;
  }
}
</style>
</head>
<body>

<h2>Hide elements on different screen sizes</h2>

<div class="example">Example DIV.</div>

<p>When the browser's width is 600px wide or less, hide the div element. Resize the browser window to see 

the effect.</p>

</body>
</html>



Change Font Size With Media Queries

You can also use media queries to change the font size of an element on different screen sizes:

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
div.example {
  background-color: lightgrey;
  padding: 20px;
}

@media screen and (min-width: 600px) {
  div.example {
    font-size: 80px;
  }
}

@media screen and (max-width: 600px) {
  div.example {
    font-size: 30px;
  }
}
</style>
</head>
<body>

<h2>Change the font size of an element on different screen sizes</h2>

<div class="example">Example DIV.</div>

<p>When the browser's width is 600px wide or less, set the font-size of DIV to 30px. When it is 601px or 

wider, set the font-size to 80px. Resize the browser window to see the effect.</p>

</body>
</html>



CSS @media Reference

For a full overview of all the media types and features/expressions, please look at the @media rule in our 

CSS reference here: https://www.w3schools.com/cssref/css3_pr_mediaquery.asp




.....


Responsive Web Design - Images

Using The width Property

If the width property is set to a percentage and the height property is set to "auto", the image will be 

responsive and scale up and down:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
img {
  width: 100%;
  height: auto;
}
</style>
</head>
<body>

<img src="img_chania.jpg" width="460" height="345">
<p>Resize the browser window to see how the image will scale.</p>

</body>
</html>


Notice that in the example above, the image can be scaled up to be larger than its original size. A better 

solution, in many cases, will be to use the max-width property instead.


Using The max-width Property

If the max-width property is set to 100%, the image will scale down if it has to, but never scale up to be 

larger than its original size:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
img {
  max-width: 100%;
  height: auto;
}
</style>
</head>
<body>

<img src="img_chania.jpg" width="460" height="345">
<p>Resize the browser window to see how the image will scale when the width is less than 460px.</p>

</body>
</html>


Add an Image to The Example Web Page

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* {
  box-sizing: border-box;
}

img {
  width: 100%;
  height: auto;
}

.row:after {
  content: "";
  clear: both;
  display: table;
}

[class*="col-"] {
  float: left;
  padding: 15px;
  width: 100%;
}

@media only screen and (min-width: 600px) {
  .col-s-1 {width: 8.33%;}
  .col-s-2 {width: 16.66%;}
  .col-s-3 {width: 25%;}
  .col-s-4 {width: 33.33%;}
  .col-s-5 {width: 41.66%;}
  .col-s-6 {width: 50%;}
  .col-s-7 {width: 58.33%;}
  .col-s-8 {width: 66.66%;}
  .col-s-9 {width: 75%;}
  .col-s-10 {width: 83.33%;}
  .col-s-11 {width: 91.66%;}
  .col-s-12 {width: 100%;}
}

@media only screen and (min-width: 768px) {
  .col-1 {width: 8.33%;}
  .col-2 {width: 16.66%;}
  .col-3 {width: 25%;}
  .col-4 {width: 33.33%;}
  .col-5 {width: 41.66%;}
  .col-6 {width: 50%;}
  .col-7 {width: 58.33%;}
  .col-8 {width: 66.66%;}
  .col-9 {width: 75%;}
  .col-10 {width: 83.33%;}
  .col-11 {width: 91.66%;}
  .col-12 {width: 100%;}
}

html {
  font-family: "Lucida Sans", sans-serif;
}

.header {
  background-color: #9933cc;
  color: #ffffff;
  padding: 15px;
}

.menu ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.menu li {
  padding: 8px;
  margin-bottom: 7px;
  background-color :#33b5e5;
  color: #ffffff;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.menu li:hover {
  background-color: #0099cc;
}

.aside {
  background-color: #33b5e5;
  padding: 15px;
  color: #ffffff;
  text-align: center;
  font-size: 14px;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.footer {
  background-color: #0099cc;
  color: #ffffff;
  text-align: center;
  font-size: 12px;
  padding: 15px;
}
</style>
</head>
<body>

<div class="header">
  <h1>Chania</h1>
</div>

<div class="row">
  <div class="col-3 col-s-3 menu">
    <ul>
      <li>The Flight</li>
      <li>The City</li>
      <li>The Island</li>
      <li>The Food</li>
    </ul>
  </div>

  <div class="col-6 col-s-9">
    <h1>The City</h1>
    <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two 

parts, the old town and the modern city.</p>
    <img src="img_chania.jpg" width="460" height="345">
  </div>

  <div class="col-3 col-s-12">
    <div class="aside">
      <h2>What?</h2>
      <p>Chania is a city on the island of Crete.</p>
      <h2>Where?</h2>
      <p>Crete is a Greek island in the Mediterranean Sea.</p>
      <h2>How?</h2>
      <p>You can reach Chania airport from all over Europe.</p>
    </div>
  </div>
</div>

<div class="footer">
  <p>Resize the browser window to see how the content respond to the resizing.</p>
</div>

</body>
</html>



Background Images

Background images can also respond to resizing and scaling.

Here we will show three different methods:

1. If the background-size property is set to "contain", the background image will scale, and try to fit the 

content area. However, the image will keep its aspect ratio (the proportional relationship between the 

image's width and height):

The CSS code for background-size: contain; is shown below:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
div {
  width: 100%;
  height: 400px;
  background-image: url('img_flowers.jpg');
  background-repeat: no-repeat;
  background-size: contain;
  border: 1px solid red;
}
</style>
</head>
<body>

<p>Resize the browser window to see the effect.</p>

<div></div>

</body>
</html>



2. If the background-size property is set to "100% 100%", the background image will stretch to cover the 

entire content area. The CSS code for this is as shown below:

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
div {
  width: 100%;
  height: 400px;
  background-image: url('img_flowers.jpg');
  background-size: 100% 100%;
  border: 1px solid red;
}
</style>
</head>
<body>

<p>Resize the browser window to see the effect.</p>

<div></div>

</body>
</html>


3. If the background-size property is set to "cover", the background image will scale to cover the entire 

content area. Notice that the "cover" value keeps the aspect ratio, and some part of the background image 

may be clipped. The CSS code for this option is as shown below:

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
div {
  width: 100%;
  height: 400px;
  background-image: url('img_flowers.jpg');
  background-size: cover;
  border: 1px solid red;
}
</style>
</head>
<body>

<p>Resize the browser window to see the effect.</p>

<div></div>

</body>
</html>


Different Images for Different Devices

A large image can be perfect on a big computer screen, but useless on a small device. Why load a large image 

when you have to scale it down anyway? To reduce the load, or for any other reasons, you can use media 

queries to display different images on different devices.

Here is one large image and one smaller image that will be displayed on different devices:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
/* For width smaller than 400px: */
body {
  background-repeat: no-repeat;
  background-image: url('img_smallflower.jpg'); 
}

/* For width 400px and larger: */
@media only screen and (min-width: 400px) {
  body { 
     background-image: url('img_flowers.jpg'); 
  }
}
</style>
</head>
<body>

<p style="margin-top:360px;">Resize the browser width and the background image will change at 400px.</p>

</body>
</html>


You can use the media query min-device-width, instead of min-width, which checks the device width, instead 

of the browser width. Then the image will not change when you resize the browser window: 

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
/* For device width smaller than 400px: */
body {
  background-repeat: no-repeat;
  background-image: url('img_smallflower.jpg'); 
}

/* For device width 400px and larger: */
@media only screen and (min-device-width: 400px) {
  body { 
     background-image: url('img_flowers.jpg'); 
  }
}
</style>
</head>
<body>

</body>
</html>


The HTML <picture> Element

The HTML <picture> element gives web developers more flexibility in specifying image resources.

The most common use of the <picture> element will be for images used in responsive designs. Instead of 

having one image that is scaled up or down based on the viewport width, multiple images can be designed to 

more nicely fill the browser viewport.

The <picture> element works similar to the <video> and <audio> elements. You set up different sources, and 

the first source that fits the preferences is the one being used:

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<picture>
  <source srcset="img_smallflower.jpg" media="(max-width: 400px)">
  <source srcset="img_flowers.jpg">
  <img src="img_flowers.jpg" alt="Flowers" style="width:auto;">
</picture>

<p>Resize the browser width and the background image will change at 400px.</p>

</body>
</html>



The srcset attribute is required, and defines the source of the image.

The media attribute is optional, and accepts the media queries you find in CSS @media rule available here: 

https://www.w3schools.com/cssref/css3_pr_mediaquery.asp .

You should also define an <img> element for browsers that do not support the <picture> element.



............

Responsive Web Design - Videos

Using The width Property

If the width property is set to 100%, the video player will be responsive and scale up and down:

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
video {
  width: 100%;
  height: auto;
}
</style>
</head>
<body>

<video width="400" controls>
  <source src="mov_bbb.mp4" type="video/mp4">
  <source src="mov_bbb.ogg" type="video/ogg">
  Your browser does not support HTML5 video.
</video>

<p>Resize the browser window to see how the size of the video player will scale.</p>

</body>
</html>



Notice that in the example above, the video player can be scaled up to be larger than its original size. A 

better solution, in many cases, will be to use the max-width property instead.


Using The max-width Property

If the max-width property is set to 100%, the video player will scale down if it has to, but never scale up 

to be larger than its original size:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
video {
  max-width: 100%;
  height: auto;
}
</style>
</head>
<body>

<video width="400" controls>
  <source src="mov_bbb.mp4" type="video/mp4">
  <source src="mov_bbb.ogg" type="video/ogg">
  Your browser does not support HTML5 video.
</video>

<p>Resize the browser window to see how the size of the video player will scale when the width is less than 

400px.</p>

</body>
</html>




Add a Video to the Example Web Page

We want to add a video in our example web page. The video will be resized to always take up all the 

available space:


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* {
  box-sizing: border-box;
}

video {
  width: 100%;
  height: auto;
}

.row:after {
  content: "";
  clear: both;
  display: table;
}

[class*="col-"] {
  float: left;
  padding: 15px;
  width: 100%;
}

@media only screen and (min-width: 600px) {
  .col-s-1 {width: 8.33%;}
  .col-s-2 {width: 16.66%;}
  .col-s-3 {width: 25%;}
  .col-s-4 {width: 33.33%;}
  .col-s-5 {width: 41.66%;}
  .col-s-6 {width: 50%;}
  .col-s-7 {width: 58.33%;}
  .col-s-8 {width: 66.66%;}
  .col-s-9 {width: 75%;}
  .col-s-10 {width: 83.33%;}
  .col-s-11 {width: 91.66%;}
  .col-s-12 {width: 100%;}
}

@media only screen and (min-width: 768px) {
  .col-1 {width: 8.33%;}
  .col-2 {width: 16.66%;}
  .col-3 {width: 25%;}
  .col-4 {width: 33.33%;}
  .col-5 {width: 41.66%;}
  .col-6 {width: 50%;}
  .col-7 {width: 58.33%;}
  .col-8 {width: 66.66%;}
  .col-9 {width: 75%;}
  .col-10 {width: 83.33%;}
  .col-11 {width: 91.66%;}
  .col-12 {width: 100%;}
}

html {
  font-family: "Lucida Sans", sans-serif;
}

.header {
  background-color: #9933cc;
  color: #ffffff;
  padding: 15px;
}

.menu ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.menu li {
  padding: 8px;
  margin-bottom: 7px;
  background-color: #33b5e5;
  color: #ffffff;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.menu li:hover {
  background-color: #0099cc;
}

.aside {
  background-color: #33b5e5;
  padding: 15px;
  color: #ffffff;
  text-align: center;
  font-size: 14px;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

.footer {
  background-color: #0099cc;
  color: #ffffff;
  text-align: center;
  font-size: 12px;
  padding: 15px;
}
</style>
</head>
<body>

<div class="header">
  <h1>Chania</h1>
</div>

<div class="row">
  <div class="col-3 col-s-3 menu">
    <ul>
      <li>The Flight</li>
      <li>The City</li>
      <li>The Island</li>
      <li>The Food</li>
    </ul>
  </div>

  <div class="col-6 col-s-9">
    <h1>The City</h1>
    <p>Chania is the capital of the Chania region on the island of Crete. The city can be divided in two 

parts, the old town and the modern city.</p>
    <video width="400" controls>
      <source src="mov_bbb.mp4" type="video/mp4">
      <source src="mov_bbb.ogg" type="video/ogg">
      Your browser does not support HTML5 video.
    </video>
  </div>

  <div class="col-3 col-s-12">
    <div class="aside">
      <h2>What?</h2>
      <p>Chania is a city on the island of Crete.</p>
      <h2>Where?</h2>
      <p>Crete is a Greek island in the Mediterranean Sea.</p>
      <h2>How?</h2>
      <p>You can reach Chania airport from all over Europe.</p>
    </div>
  </div>
</div>

<div class="footer">
  <p>Resize the browser window to see how the content respond to the resizing.</p>
</div>

</body>
</html>






...................................
RWD Frameworks


There are many free CSS frameworks for Responsive Design. Some of them are:

W3.CSS: https://www.w3schools.com/w3css/default.asp  
Bootstrap (uses HTML, CSS and JQuery): https://www.w3schools.com/bootstrap/bootstrap_ver.asp
 

..............
RWD Templates

Check here for useful responsive web design templates: https://www.w3schools.com/css/css_rwd_templates.asp



.......................................

CSS Grid Layout Module

An example of CSS grid layout module is shown in the html code below:

<!DOCTYPE html>
<html>
<head>
<style>
.item1 { grid-area: header; }
.item2 { grid-area: menu; }
.item3 { grid-area: main; }
.item4 { grid-area: right; }
.item5 { grid-area: footer; }

.grid-container {
  display: grid;
  grid-template-areas:
    'header header header header header header'
    'menu main main main right right'
    'menu footer footer footer footer footer';
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>Grid Layout</h1>

<p>This grid layout contains six columns and three rows:</p>

<div class="grid-container">
  <div class="item1">Header</div>
  <div class="item2">Menu</div>
  <div class="item3">Main</div>  
  <div class="item4">Right</div>
  <div class="item5">Footer</div>
</div>

</body>
</html>


Grid Layout

The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to 

design web pages without having to use floats and positioning.

Browser Support

The grid properties are supported in all modern browsers.



Grid Elements


A grid layout consists of a parent element, with one or more child elements.


<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  background-color: #2196F3;
  padding: 10px;
}
.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 20px;
  font-size: 30px;
  text-align: center;
}
</style>
</head>
<body>

<h1>Grid Elements</h1>

<p>A Grid Layout must have a parent element with the <em>display</em> property set to <em>grid</em> or 

<em>inline-grid</em>.</p>

<p>Direct child element(s) of the grid container automatically becomes grid items.</p>

<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>  
  <div class="grid-item">4</div>
  <div class="grid-item">5</div>
  <div class="grid-item">6</div>  
  <div class="grid-item">7</div>
  <div class="grid-item">8</div>
  <div class="grid-item">9</div>  
</div>

</body>
</html>





Display Property

An HTML element becomes a grid container when its display property is set to grid or inline-grid.

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  background-color: #2196F3;
  padding: 10px;
}

.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 20px;
  font-size: 30px;
  text-align: center;
}
</style>
</head>
<body>

<h1>display: grid</h1>

<p>Use display: grid; to make a block-level grid container:</p>

<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>  
  <div class="grid-item">4</div>
  <div class="grid-item">5</div>
  <div class="grid-item">6</div>  
  <div class="grid-item">7</div>
  <div class="grid-item">8</div>
  <div class="grid-item">9</div>  
</div>

</body>
</html>


The inline-grid version is shown below:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: inline-grid;
  grid-template-columns: auto auto auto;
  background-color: #2196F3;
  padding: 10px;
}

.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 20px;
  font-size: 30px;
  text-align: center;
}
</style>
</head>
<body>

<h1>display: inline-grid</h1>

<p>Use display: inline-grid; to make an inline grid container:</p>

<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>  
  <div class="grid-item">4</div>
  <div class="grid-item">5</div>
  <div class="grid-item">6</div>  
  <div class="grid-item">7</div>
  <div class="grid-item">8</div>
  <div class="grid-item">9</div>  
</div>

</body>
</html>


All direct children of the grid container automatically become grid items.


Grid Columns

The vertical lines of grid items are called columns.


Grid Rows

The horizontal lines of grid items are called rows.



Grid Gaps

The spaces between each column/row are called gaps. The spaces between grid rows are called Row Gaps while 

the spaces between columns are called Column Gaps.

You can adjust the gap size by using one of the following properties:

    grid-column-gap
    grid-row-gap
    grid-gap



Example

The grid-column-gap property sets the gap between the columns:
 

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-column-gap: 50px;
  grid-template-columns: auto auto auto;
  background-color: #2196F3;
  padding: 10px;
}

.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 20px;
  font-size: 30px;
  text-align: center;
}
</style>
</head>
<body>

<h1>The grid-column-gap Property</h1>

<p>Use the <em>grid-column-gap</em> property to adjust the space between the columns:</p>

<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>  
  <div class="grid-item">4</div>
  <div class="grid-item">5</div>
  <div class="grid-item">6</div>  
  <div class="grid-item">7</div>
  <div class="grid-item">8</div>
  <div class="grid-item">9</div>  
</div>

</body>
</html>



Example

The grid-row-gap property sets the gap between the rows:


<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-row-gap: 50px;
  grid-template-columns: auto auto auto;
  background-color: #2196F3;
  padding: 10px;
}

.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 20px;
  font-size: 30px;
  text-align: center;
}
</style>
</head>
<body>

<h1>The grid-row-gap Property</h1>

<p>Use the <em>grid-row-gap</em> property to adjust the space between the rows:</p>

<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>  
  <div class="grid-item">4</div>
  <div class="grid-item">5</div>
  <div class="grid-item">6</div>  
  <div class="grid-item">7</div>
  <div class="grid-item">8</div>
  <div class="grid-item">9</div>  
</div>

</body>
</html>


Example

The grid-gap property is a shorthand property for the grid-row-gap and the grid-column-gap properties:


<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-gap: 50px 100px;
  grid-template-columns: auto auto auto;
  background-color: #2196F3;
  padding: 10px;
}

.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 20px;
  font-size: 30px;
  text-align: center;
}
</style>
</head>
<body>

<h1>The grid-gap Property</h1>

<p>Use the <em>grid-gap</em> shorthand property to adjust the space between the columns and rows.</p>

<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>  
  <div class="grid-item">4</div>
  <div class="grid-item">5</div>
  <div class="grid-item">6</div>  
  <div class="grid-item">7</div>
  <div class="grid-item">8</div>
  <div class="grid-item">9</div>  
</div>

</body>
</html>



Example

The grid-gap property can also be used to set both the row gap and the column gap in one value:


<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-gap: 50px;
  grid-template-columns: auto auto auto;
  background-color: #2196F3;
  padding: 10px;
}

.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 20px;
  font-size: 30px;
  text-align: center;
}
</style>
</head>
<body>

<h1>The grid-gap Property:</h1>

<p>Use the <em>grid-gap</em> shorthand property to adjust the space between the columns and rows:</p>

<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>  
  <div class="grid-item">4</div>
  <div class="grid-item">5</div>
  <div class="grid-item">6</div>  
  <div class="grid-item">7</div>
  <div class="grid-item">8</div>
  <div class="grid-item">9</div>  
</div>

</body>
</html>



Grid Lines

The lines between columns are called column lines.

The lines between rows are called row lines.

Refer to line numbers when placing a grid item in a grid container:


Example

Place a grid item at column line 1, and let it end on column line 3:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}

.item1 {
  grid-column-start: 1;
  grid-column-end: 3;
}
</style>
</head>
<body>

<h1>Grid Lines</h1>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
  <div class="item7">7</div>
  <div class="item8">8</div>  
</div>

<p>You can refer to line numbers when placing grid items.</p>

</body>
</html>


Example

Place a grid item at row line 1, and let it end on row line 3:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}

.item1 {
  grid-row-start: 1;
  grid-row-end: 3;
}
</style>
</head>
<body>

<h1>Grid Lines</h1>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
  <div class="item7">7</div>
  <div class="item8">8</div>  
</div>

<p>You can refer to line numbers when placing grid items.</p>

</body>
</html>



All CSS Grid Properties
Property 	Description
column-gap 	Specifies the gap between the columns
gap 	A shorthand property for the row-gap and the column-gap properties
grid 	A shorthand property for the grid-template-rows, grid-template-columns, grid-template-areas, grid-

auto-rows, grid-auto-columns, and the grid-auto-flow properties
grid-area 	Either specifies a name for the grid item, or this property is a shorthand property for the 

grid-row-start, grid-column-start, grid-row-end, and grid-column-end properties
grid-auto-columns 	Specifies a default column size
grid-auto-flow 	Specifies how auto-placed items are inserted in the grid
grid-auto-rows 	Specifies a default row size
grid-column 	A shorthand property for the grid-column-start and the grid-column-end properties
grid-column-end 	Specifies where to end the grid item
grid-column-gap 	Specifies the size of the gap between columns
grid-column-start 	Specifies where to start the grid item
grid-gap 	A shorthand property for the grid-row-gap and grid-column-gap properties
grid-row 	A shorthand property for the grid-row-start and the grid-row-end properties
grid-row-end 	Specifies where to end the grid item
grid-row-gap 	Specifies the size of the gap between rows
grid-row-start 	Specifies where to start the grid item
grid-template 	A shorthand property for the grid-template-rows, grid-template-columns and grid-areas 

properties
grid-template-areas 	Specifies how to display columns and rows, using named grid items
grid-template-columns 	Specifies the size of the columns, and how many columns in a grid layout
grid-template-rows 	Specifies the size of the rows in a grid layout
row-gap 	Specifies the gap between the grid rows




CSS Grid Container

Grid Container

To make an HTML element behave as a grid container, you have to set the display property to grid or inline-

grid.

Grid containers consist of grid items, placed inside columns and rows.


The grid-template-columns Property

The grid-template-columns property defines the number of columns in your grid layout, and it can define the 

width of each column.

The value is a space-separated-list, where each value defines the width of the respective column.

If you want your grid layout to contain 4 columns, specify the width of the 4 columns, or "auto" if all 

columns should have the same width.



Example

Make a grid with 4 columns:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The grid-template-columns Property</h1>

<p>You can use the <em>grid-template-columns</em> property to specify the number of columns in your grid 

layout.</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
  <div>7</div>
  <div>8</div>
</div>

</body>
</html>


Note: If you have more than 4 items in a 4 columns grid, the grid will automatically add a new row to put 

the items in.



The grid-template-columns property can also be used to specify the size (width) of the columns.

Example

Set a size for the 4 columns:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: 80px 200px auto 30px;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The grid-template-columns Property</h1>

<p>Use the <em>grid-template-columns</em> property to specify the size of each column.</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
  <div>7</div>
  <div>8</div>
</div>

</body>
</html>




The grid-template-rows Property

The grid-template-rows property defines the height of each row.

The value is a space-separated-list, where each value defines the height of the respective row:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  grid-template-rows: 80px 200px;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The grid-template-rows Property</h1>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

<p>Use the <em>grid-template-rows</em> property to specify the size (height) of each row.</p>

</body>
</html>


The justify-content Property

The justify-content property is used to align the whole grid inside the container. See example below:
Note: The grid's total width has to be less than the container's width for the justify-content property to 

have any effect. 

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  justify-content: space-evenly;
  grid-template-columns: 50px 50px 50px; /*Make the grid smaller than the container*/
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The justify-content Property</h1>

<p>Use the <em>justify-content</em> property to align the grid inside the container.</p>

<p>The value "space-evenly" will give the columns equal amount of space between, and around them:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>


The example with space-around for justify-content property is as shown below:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  justify-content: space-around;
  grid-template-columns: 50px 50px 50px; /*Make the grid smaller than the container*/
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The justify-content Property</h1>

<p>Use the <em>justify-content</em> property to align the grid inside the container.</p>

<p>The value "space-around" will give the columns equal amount of space around them:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>


See below for space-between option for justify-content property is as shown below:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  justify-content: space-between;
  grid-template-columns: 50px 50px 50px; /*Make the grid smaller than the container*/
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The justify-content Property</h1>

<p>Use the <em>justify-content</em> property to align the grid inside the container.</p>

<p>The value "space-between" will give the columns equal amount of space between them:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>





To justify contents to the center:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  justify-content: center;
  grid-template-columns: 50px 50px 50px; /*Make the grid smaller than the container*/
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The justify-content Property</h1>

<p>Use the <em>justify-content</em> property to align the grid inside the container.</p>

<p>The value "center" will align the grid in the middle of the container:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>


<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  justify-content: center;
  grid-template-columns: 50px 50px 50px; /*Make the grid smaller than the container*/
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The justify-content Property</h1>

<p>Use the <em>justify-content</em> property to align the grid inside the container.</p>

<p>The value "center" will align the grid in the middle of the container:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>




To justify content to be at the start of a container:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  justify-content: start;
  grid-template-columns: 50px 50px 50px; /*Make the grid smaller than the container*/
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The justify-content Property</h1>

<p>Use the <em>justify-content</em> property to align the grid inside the container.</p>

<p>The value "start" will align the grid at the beginning of the container:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>





To justify content of container at the end of the container:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  justify-content: end;
  grid-template-columns: 50px 50px 50px; /*Make the grid smaller than the container*/
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The justify-content Property</h1>

<p>Use the <em>justify-content</em> property to align the grid inside the container.</p>

<p>The value "end" will align the grid at the end of the container:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>


The align-content Property

The align-content property is used to vertically align the whole grid inside the container. The the example 

of align-content vertically inside the grid to center below:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  height: 400px;
  align-content: center;
  grid-template-columns: auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-content Property</h1>

<p>Use the <em>align-content</em> property to vertically align the grid inside the container.</p>

<p>The value "center" will align the rows in the middle of the container:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>








Note: The grid's total height has to be less than the container's height for the align-content property to 

have any effect.


To align grid contents vertically inside the grid such that the rows have equal amount of space between 

them, set align-content to space-evenly:


<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  height: 400px;
  align-content: space-evenly;
  grid-template-columns: auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-content Property</h1>

<p>Use the <em>align-content</em> property to vertically align the grid inside the container.</p>

<p>The value "space-evenly" will give the rows equal amount of space between, and around them:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>


To align contents of grid container vertically such that each row has equal amount of space around them (in 

a way similar to an invisible thick border):

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  height: 400px;
  align-content: space-around;
  grid-template-columns: auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-content Property</h1>

<p>Use the <em>align-content</em> property to vertically align the grid inside the container.</p>

<p>The value "space-around" will give the rows equal amount of space around them:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>




To make space between the rows to be equal:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  height: 400px;
  align-content: space-between;
  grid-template-columns: auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-content Property</h1>

<p>Use the <em>align-content</em> property to vertically align the grid inside the container.</p>

<p>The value "space-between" will give the rows equal amount of space between them:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>


To align content of a container vertically to be at the beginning of a container:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  height: 400px;
  align-content: start;
  grid-template-columns: auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-content Property</h1>

<p>Use the <em>align-content</em> property to vertically align the grid inside the container.</p>

<p>The value "start" will align the rows at the beginning of the container:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>


To align content vertically at the end of the container, set the align-content:end; as shown below:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  height: 400px;
  align-content: end;
  grid-template-columns: auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The align-content Property</h1>

<p>Use the <em>align-content</em> property to vertically align the grid inside the container.</p>

<p>The value "end" will align the rows at the end of the container:</p>

<div class="grid-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>  
  <div>4</div>
  <div>5</div>
  <div>6</div>  
</div>

</body>
</html>





CSS Grid Item

Child Elements (Items)

A grid container contains grid items.

By default, a container has one grid item for each column, in each row, but you can style the grid items so 

that they will span multiple columns and/or rows.




The grid-column Property:

The grid-column property defines on which column(s) to place an item.

You define where the item will start, and where the item will end.


Note: The grid-column property is a shorthand property for the grid-column-start and the grid-column-end 

properties.

To place an item, you can refer to line numbers, or use the keyword "span" to define how many columns the 

item will span.





Example

Make "item1" start on column 1 and end before column 5:


<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}

.item1 {
  grid-column: 1 / 5;
}
</style>
</head>
<body>

<h1>The grid-column Property</h1>

<p>Use the <em>grid-column</em> property to specify where to place an item.</p>
<p>Item1 will start on column 1 and end before column 5:</p>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
  <div class="item7">7</div>
  <div class="item8">8</div>  
  <div class="item9">9</div>
  <div class="item10">10</div>
  <div class="item11">11</div>
  <div class="item12">12</div>
  <div class="item13">13</div>
  <div class="item14">14</div>
  <div class="item15">15</div>
</div>

</body>
</html>


Example

Make "item1" start on column 1 and span 3 columns:


<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}

.item1 {
  grid-column: 1 / span 3;
}
</style>
</head>
<body>

<h1>The grid-column Property</h1>

<p>Use the <em>grid-column</em> property to specify where to place an item.</p>
<p>Item1 will start on column-line 1 and span 3 columns:</p>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
  <div class="item7">7</div>
  <div class="item8">8</div>  
  <div class="item9">9</div>
  <div class="item10">10</div>
  <div class="item11">11</div>
  <div class="item12">12</div>
  <div class="item13">13</div>
  <div class="item14">14</div>
  <div class="item15">15</div>
  <div class="item16">16</div>
</div>

</body>
</html>



Example

Make "item2" start on column 2 and span 3 columns:


<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}

.item2 {
  grid-column: 2 / span 3;
}
</style>
</head>
<body>

<h1>The grid-column Property</h1>

<p>Use the <em>grid-column</em> property to specify where to place an item.</p>
<p>Item2 will start on column line 2 and span 3 columns:</p>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
  <div class="item7">7</div>
  <div class="item8">8</div>  
  <div class="item9">9</div>
  <div class="item10">10</div>
  <div class="item11">11</div>
  <div class="item12">12</div>
  <div class="item13">13</div>
  <div class="item14">14</div>
  <div class="item15">15</div>
  <div class="item16">16</div>
</div>

</body>
</html>



The grid-row Property:

The grid-row property defines on which row to place an item.

You define where the item will start, and where the item will end.



Note: The grid-row property is a shorthand property for the grid-row-start and the grid-row-end properties.

To place an item, you can refer to line numbers, or use the keyword "span" to define how many rows the item 

will span:


Example

Make "item1" start on row-line 1 and end on row-line 4:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}

.item1 {
  grid-row: 1 / 4;
}
</style>
</head>
<body>

<h1>The grid-row Property</h1>

<p>Use the <em>grid-row</em> property to specify where to place an item.</p>
<p>Item1 will start on row-line 1 and end on row-line 4:</p>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
  <div class="item7">7</div>
  <div class="item8">8</div>  
  <div class="item9">9</div>
  <div class="item10">10</div>
  <div class="item11">11</div>
  <div class="item12">12</div>
  <div class="item13">13</div>
  <div class="item14">14</div>
  <div class="item15">15</div>
  <div class="item16">16</div>
</div>

</body>
</html>


Example

Make "item1" start on row 1 and span 2 rows:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}

.item1 {
  grid-row: 1 / span 2;
}
</style>
</head>
<body>

<h1>The grid-row Property</h1>

<p>Use the <em>grid-row</em> property to specify where to place an item.</p>
<p>Item1 will start on row 1 and span 2 rows:</p>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
  <div class="item7">7</div>
  <div class="item8">8</div>  
  <div class="item9">9</div>
  <div class="item10">10</div>
  <div class="item11">11</div>
  <div class="item12">12</div>
  <div class="item13">13</div>
  <div class="item14">14</div>
  <div class="item15">15</div>
  <div class="item16">16</div>
  <div class="item17">17</div>
</div>

</body>
</html>




The grid-area Property

The grid-area property can be used as a shorthand property for the grid-row-start, grid-column-start, grid-

row-end and the grid-column-end properties respectively.


Example

Make "item8" start on row-line 1 and column-line 2, and end on row-line 5 and column line 6:

<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}

.item8 {
  grid-area: 1 / 2 / 5 / 6;
}
</style>
</head>
<body>

<h1>The grid-area Property</h1>

<p>You can use the <em>grid-area</em> property to specify where to place an item.</p>

<p>The syntax is:</p>
<p>grid-row-start / grid-column-start / grid-row-end / grid-column-end.</p>

<p>Item8 will start on row-line 1 and column-line 2, and end on row-line 5 column-line 6:</p>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
  <div class="item7">7</div>
  <div class="item8">8</div>  
  <div class="item9">9</div>
  <div class="item10">10</div>
  <div class="item11">11</div>
  <div class="item12">12</div>
  <div class="item13">13</div>
  <div class="item14">14</div>
  <div class="item15">15</div>
</div>

</body>
</html>



Example

Make "item8" start on row-line 2 and column-line 1, and span 2 rows and 3 columns:


<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}

.item8 {
  grid-area: 2 / 1 / span 2 / span 3;
}
</style>
</head>
<body>

<h1>The grid-area Property</h1>

<p>You can use the <em>grid-area</em> property to specify where to place an item.</p>

<p>The syntax is grid-row-start / grid-column-start / grid-row-end / grid-column-end.</p>

<p>Item8 will start on row-line 2 and column-line 1, and span 2 rows and 3 columns:</p>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
  <div class="item7">7</div>
  <div class="item8">8</div>  
  <div class="item9">9</div>
  <div class="item10">10</div>
  <div class="item11">11</div>
  <div class="item12">12</div>
  <div class="item13">13</div>
</div>

</body>
</html>



Naming Grid Items

The grid-area property can also be used to assign names to grid items.

Named grid items can be referred to by the grid-template-areas property of the grid container.



Example

Item1 gets the name "myArea" and spans all five columns in a five columns grid layout:


<!DOCTYPE html>
<html>
<head>
<style>
.item1 {
  grid-area: myArea;
}

.grid-container {
  display: grid;
  grid-template-areas: 'myArea myArea myArea myArea myArea';
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The grid-area Property</h1>

<p>You can use the <em>grid-area</em> property to name grid items.</p>

<p>You can refer to the name when you set up the grid layout, by using the <em>grid-template-areas</em> 

property on the grid container.</p>

<p>Item1, is called "myArea" and will take up the place of all five columns:</p>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
</div>

</body>
</html>





Each row is defined by apostrophes (' ')

The columns in each row is defined inside the apostrophes, separated by a space.

Note: A period sign represents a grid item with no name.



Example

Let "myArea" span two columns in a five columns grid layout (period signs represent items with no name):

<!DOCTYPE html>
<html>
<head>
<style>
.item1 {
  grid-area: myArea;
}

.grid-container {
  display: grid;
  grid-template-areas: 'myArea myArea . . .';
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The grid-area Property</h1>

<p>You can use the <em>grid-area</em> property to name grid items.</p>

<p>You can refer to the name when you set up the grid layout, by using the <em>grid-template-areas</em> 

property on the grid container.</p>

<p>Item1, is called "myArea" and will take up the place of two columns (out of five):</p>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
  <div class="item7">7</div>
  <div class="item8">8</div>
  <div class="item9">9</div>
</div>

</body>
</html>




To define two rows, define the column of the second row inside another set of apostrophes:


Example

Make "item1" span two columns and two rows:


<!DOCTYPE html>
<html>
<head>
<style>
.item1 {
  grid-area: myArea;
}

.grid-container {
  display: grid;
  grid-template-areas: 'myArea myArea . . .' 'myArea myArea . . .';
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The grid-area Property</h1>

<p>You can use the <em>grid-area</em> property to name grid items.</p>

<p>You can refer to the name when you set up the grid layout, by using the <em>grid-template-areas</em> 

property on the grid container.</p>

<p>Item1, is called "myArea" and will take up the place of two columns (out of five), and will span two 

rows:</p>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
  <div class="item7">7</div>
</div>

</body>
</html>



Example

Name all items, and make a ready-to-use webpage template:

<!DOCTYPE html>
<html>
<head>
<style>
.item1 { grid-area: header; }
.item2 { grid-area: menu; }
.item3 { grid-area: main; }
.item4 { grid-area: right; }
.item5 { grid-area: footer; }

.grid-container {
  display: grid;
  grid-template-areas:
    'header header header header header header'
    'menu main main main right right'
    'menu footer footer footer footer footer';
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>
</head>
<body>

<h1>The grid-area Property</h1>

<p>You can use the <em>grid-area</em> property to name grid items.</p>

<p>You can refer to the name when you set up the grid layout, by using the <em>grid-template-areas</em> 

property on the grid container.</p>

<p>This grid layout contains six columns and three rows:</p>

<div class="grid-container">
  <div class="item1">Header</div>
  <div class="item2">Menu</div>
  <div class="item3">Main</div>  
  <div class="item4">Right</div>
  <div class="item5">Footer</div>
</div>

</body>
</html>



The Order of the Items

The Grid Layout allows us to position the items anywhere we like.

The first item in the HTML code does not have to appear as the first item in the grid.


<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}

.item1 { grid-area: 1 / 3 / 2 / 4; }
.item2 { grid-area: 2 / 3 / 3 / 4; }
.item3 { grid-area: 1 / 1 / 2 / 2; }
.item4 { grid-area: 1 / 2 / 2 / 3; }
.item5 { grid-area: 2 / 1 / 3 / 2; }
.item6 { grid-area: 2 / 2 / 3 / 3; }
</style>
</head>
<body>

<h1>Sort the Items</h1>

<p>The grid items do not have to be displayed in the same order as they are written in the HTML code.</p>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
</div>

</body>
</html>



You can re-arrange the order for certain screen sizes, by using media queries ( and also span accordingly):


<!DOCTYPE html>
<html>
<head>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  grid-gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}

@media only screen and (max-width: 500px) {
  .item1 { grid-area: 1 / span 3 / 2 / 4; }
  .item2 { grid-area: 3 / 3 / 4 / 4; }
  .item3 { grid-area: 2 / 1 / 3 / 2; }
  .item4 { grid-area: 2 / 2 / span 2 / 3; }
  .item5 { grid-area: 3 / 1 / 4 / 2; }
  .item6 { grid-area: 2 / 3 / 3 / 4; }
}
</style>
</head>
<body>

<h1>Re-arange the Order on Small Devices</h1>

<p>Resize the window to 500 pixels see the effect.</p>

<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>  
  <div class="item4">4</div>
  <div class="item5">5</div>
  <div class="item6">6</div>
</div>

</body>
</html>





CSS Templates

You will find four examples of some CSS templates shown below. EAch of the templates were generated using 

float, flexbox and grid. This will give you the chance to compare the three methods of creating a webpage:


CSS Layout Templates

You will find some responsive starter templates generated with CSS here: 

https://www.w3schools.com/css/css_templates.asp

You are free to modify, save, share, and use them in all your projects. 


Check Sass tutorial here: https://www.w3schools.com/sass/default.php

Access the full list of CSS references here: https://www.w3schools.com/cssref/default.asp


















- - - - - - - - - - - - - - - - - -  - - - - - - - - - - - -  - - - - - - -- - - - - - - - -  - - - - - - - - - - -  - - - - - --  - - - - - - - - -- - - - -- - - -- - - - - -- 
CSS References
