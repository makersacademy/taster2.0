THIS ARTICLE IS UNDER CONSTRUCTION

Please note, as with all Makers Academy materials, there may be subtle errors in the following materials. Please try to approach those as challenges on which to polish your debugging skills - pull requests always welcome.

CSS Pill
================

We strongly advise you to also take those quick pills:
- [:pill: html](https://github.com/makersacademy/course/blob/master/pills/html.md "html")
- [:pill: html5](https://github.com/makersacademy/course/blob/master/pills/html5.md "html5")

CSS Syntax
================

There are few denomination to know:

A **rule** is a consist of a selector and a block of declaration(s)

A **selector** is the element you will target and style

A **declaration** is a combination of property and value (it always end with a semi-colon)

A **property** is behaviour of a declaration (background-color, width, etc)

A **value** is how the behaviour of the declaration will act (background-color: blue, width: 500px;, etc)


![css syntax image](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/css_syntax.png)

Element inspector
================

I will let you discover this awesome tool, you can not develop a static website without it (or you will do it in twice the time)

![inspect element](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/inspect_element.png)

**On the left :**
the website

**On the right :**
the above part
This is your DOM, refer to [this pill :pill:](http://code.tutsplus.com/tutorials/the-30-css-selectors-you-must-memorize--net-16048 "css selectors") if you do not remember what is the DOM.                                                                                
The thing is that you can pass on hover the DOM and it will highlight the part you are on on the left side of the screen (the website)

the below part
This is your CSS toolbox, you can play with the declarations and see directly how it is displayed on the left part of your screen in order to be efficient, and understand more how things are reacting !

You have many many more tools in this inspect element, but we will not cover them here ! Play around you'll love it.

Introduction and inheritance
================

CSS stands for Cascading Style Sheets. The cascading part means that there is an inheritance structure. A rule underneath an another one will take it over.

For example, if you do something like:

```css

h1 {
  color: blue;
}

h1 {
  color: red;
}

```

The color of the h1 will be ? red

Other example :

```css

div > h1 {
  color: blue;
}

h1 {
  color: red;
}

```

The color of the h1 will be ? blue

So what is this strange selector " > " ? this is a selector and it means that it will target all the descendant h1 inside a div.
This rule is more precise, so that means that the rule will take over.

>**Notice:** In order to priorities some rules from an another one, you can:                                                
1) Put an element under an another one                                                                                     
2) Target more specifically an element with an selector or by doing a suite of classes, IDs, etc (explore, you will learn by doing)


We previously introduced the concept of inheritancce, now we will see how to manage them with the different selectors:

CSS Selectors
================

We previously seen the " > " selector you can see a list of the 30 css selectors [ here](http://code.tutsplus.com/tutorials/the-30-css-selectors-you-must-memorize--net-16048 "css selectors"):

We will cover here the most used:

####The star selector " * ":

This will select all the elements of the DOM:

```css

* {
  margin: 0;
}

```

####The tag element selector :

In order to target a specific tag, you can only mention it as we did it in the example above:

```css

h1 {
  color: blue;
}

p {
  width: 700px;
}

```

####The class selector " . ":

Remember, during the lecture, we've seen that we could make a bridge between the HTML and CSS file !

if we have this HTML code:

```html

<p class="this_is_my_class_selector">
  Something
</p>
```

in order to style this paragraph, you will need to target it like that in the CSS file:

```css

p.this_is_my_class_selector {
  width: 600px;
}

or

.this_is_my_class_selector {
  width: 600px;
}

```

####The ID selector " # ":

It works exactly in the same way as the class selector:


```html

<p id="this_is_my_id_selector">
  Something
</p>
```

in order to style this paragraph, you will need to target it like that in the CSS file:

```css

p#this_is_my_class_selector {
  width: 600px;
}

or

#his_is_my_class_selector {
  width: 600px;
}

```
So, what is the differences between ID and Classes ?

An ID is can be used only once, a class can be re-used as much as you need.
In order to make a better difference, think about your website, it will have many blocks that will looks exactly the same.
For example, a paragraph can always have the same style. To do that properly, you will style one time the paragraph, with the same class and it will looks the same on all your website.

####The comma selector " , ":

This will help you to define the same CSS rules to multiple different element.

For example, if I want that all of my input and textarea have the same width, I can do something like:

```css

input, textarea {
  width: 600px;
}

```

####The plus selector " + ":

The plus selector will help you to target the element that goes directly after the previous one.

```css

.first_element + .second_element {
  font-size: 22px;
}

```

####Combine them !

```css
div#form input.input, textarea, p > button {
  border: 6px solid red;
}
```

This will give a red border of 6px to:

the input, textarea and the button inside of the paragraph if all those selector are inside a div that has the ID "form".

CSS Proprieties
================

**background-color:** background color of the block selected;

```css
p.warning-notice {
  background-color: red;
}
```

**color:** font color of the block;


```css
p {
  color: green;
}
```

**font:** There are several properties describing what font should be used;

```css
body {
  font-family: Arial, Helvetica, Sans-Serif; // in priority order
  font-size: 18px;
  font-style: italic;
  font-weight: bold;
}
```

**text-align:** Determines how children are aligned horizontally (not just text, any children);

```css
#menu {
  text-align: right;
}
```


**border:** border of the block element targeted;

```css
li.menu-item {
  border: 1px solid black;
}
```

**width and height:** size of the block targeted;

```css
.photo {
  width: 200px;
  height: 100px;
}
```

There is way way more CSS proprieties, [you can find them here](http://www.htmldog.com/reference/cssproperties/ "css proprieties"):

The box model:
================

![css box model](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/box_model.png)

This will help you to place your elements.

598x198 : This is width and height of the element (let's say it is a paragraph).
padding 16px: Your paragraph has a 16px padding on top bottom left and right.
margin-top & margin-bottom 30px: Your paragraph will be placed at 30px from the block above and below.
margin-left & margin-right 40px: Your paragraph will be placed at 40px from the block on the left and on the right.

![css box model](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/boxmodelannot.png)

```css
div {
    width: 320px;
    padding: 10px;
    border: 5px solid gray;
    margin: 0;
}
```
Here is the math:
320px (width)
+ 20px (left + right padding)
+ 10px (left + right border)
+ 0px (left + right margin)
= 350px

Or you can use a simple declaration:

```css
div {
    width: 350px;
    padding: 10px;
    border: 5px solid gray;
    margin: 0;
    -moz-box-sizing: border-box;
        box-sizing: border-box;
}
```
Here is the math:
350px (width)
+ 20px (left + right padding)
+ 10px (left + right border)
+ 0px (left + right margin)
= 350px

WTF?

The box-sizing: border-box; declaration takes the border and the padding in count when you set a width !
Now the full block will have a width of 350px.
It is way easy to manage such a block.

Positioning
================

Positioning is the aim of CSS, without it, our pages will be a succession of blocks.

>A block-level element occupies the entire "line" by default, so other elements are positioned above and below it, whereas an inline element flows with other elements, leaving them on their left and on the right.
Evgeny

In order to position your blocks, you can attribute them two differents properties:

####Display

The difference between **block** and **inline**:

a <p> can be a block, they will be usally displayed one after the other

a <a> will generally be an inline element inside of a <p>

You also have a common value for this property, display: inline-block;

This will help you to give a width and height to your inline element.

display: none; is used to hide an element (You will see more in the Javascript Part)

####Position

position: relative; This set the block in a relative position. That means it will be positioned after the lat relative block.

position: absolute; This means it is "floating" inside the last relative block.

position: fixed; This will float on the page where you ask me to be, you can scroll the window, it will follow.

[Checkout this super quick tutorial that will helps you to understand everything.](http://learnlayout.com/ "learn layout"):

Tips&Tricks:
================

####Comments

A CSS comment can be written in two differents ways:

1 line comment:

```css

.first_element + .second_element {
  font-size: 22px; //inline comment (maximum 1 line)
}

```
Multiple line comment:

```css
/*
I can write a comment in this line
this one as well
again ..
*/
.first_element + .second_element {
  font-size: 22px;
}

```

####Do not start with a number :

```css

.1-first_element  {
  font-size: 22px;
}

```

This will not work...

####Where I am?

If you have trouble to localize your block or understand its behaviour, write a border: 1px solid black;
This little meanless trick will save you a lot of time for the beginning.

####Logic :

```css

div.fluid_center  {
  width: 200px;
  margin-left: calc(50% - 200px);
}

```

This will center the .fluid_width div block in the middle.
It has a width of 200px and it is at 50% of the left side of the page.

####Vendor prefix

-webkit- for Chrome
-moz- for Firefox
-o- for Opera
-ms- for IE
