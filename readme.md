THIS ARTICLE IS UNDER CONSTRUCTION

Please note, as with all Makers Academy materials, there may be subtle errors in the following materials. Please try to approach those as challenges on which to polish your debugging skills - pull requests always welcome.

Taster 2.0
================
Taster 2.0 is a new version of [Taster v1](https://github.com/makersacademy/Taster/blob/master/post.md "Taster v1")
The version 2.0 is a bit longer and will be run during a full week end course.


Learning Objectives
================

1. Make the difference between
  - HTML
  - CSS
  - JS
  - OOP

2. Introduction
  - HTML
  - CSS
  - JS
  - Responsive Web-Design
  - Agile Methodology

3. Knowledges about
  - Web server
  - Domain name
  - Hostings
  - Framework
  - Libraries
  - Good practices
  - The different ays to create a website

You will end up by having a great overview and answers on:
  - How the web is working ?
  - What are the different possibilities ?
  - How everything is related and work together ?

###You will end up with your first website !!!

Notices
================

###Good Practice
DO NOT COPY PASTE !!!
If you do so, you will never really memorized all the tags and how they are working together !

As Evgeny wrote in Taster v1:
>You're strongly encouraged to type in all code instead of copy-pasting it. This will really help your understanding of how everything works.
We can't stress this enough. Copy and Paste is the DEVIL!! Even though at times you will be copying chunks of code, the simple process of typing it yourself will help you learn. Trust us. You can't cut corners.

###Organization
We strongly advice you to start a makersacademy directory somewhere in your computer
In order to keep all your work organize and from the experience we have now, you can organize this directory with this structure:
- makersacademy
  - Taster
    - HTML Challenge
  - Pre-course
  - week 1
  - week 2
  - ...

Let's code !!!

Challenge 1 - Structure your app - (about 1h30)
================

Now that you understood:
  - What is HTML ?
  - Why is it essential to know how to play with it ?

Look what we will build today !

![hello world image](https://raw.githubusercontent.com/makersacademy/taster2.0/master/Challenges/Challenge_2/assets/images/Challenge%202.png)

### Section 1: Hello World ! (20 min)
Let's start by simply reproducing the picture bellow !

![hello world image](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/HTML%20Challenge/Hello%20world.png)

To do so you will need to:

1. Open your text editor ([Atom](https://atom.io/ "Atom.io") or [Sublime Text  3](https://www.sublimetext.com/3 "Sublime text 3"))

2. Create an index.html file

3. Create a title

4. Make your title becoming a link that goes anywhere you want

5. Right click on your index.html file and open it with your web browser

> **Good practices:**
Indent your code

> **Bonus challenge:**
Open the link in an another tab - you can check: "attributes on html links" on google

Show off ! You just created your first html page !

We will soon push it live, but you've just learnt something essential, you first work locally and when you've got the result you expected, you can push it live !

### Section 2: The first real step (30min)

The first thing you really start with is actually not coding.

1. Take a paper, a pen, and draft the website with all of its element
  - The menu
  - The article (title, text and picture)
  - The footer
  - The background image
2. Talk about it with your pair
2. Name those elements with the right tags
4. Talk about it with your pair

You can do something like that but way more simple.

![hello world image](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/HTML%20Challenge/mockup%20example.gif)

### Section 3: Code the HTML structure of your website (30min)

Now you can code what you've put on the paper

1. Go back on your text editor, delete the inside of the body
2. Start coding what you've put on paper

> **Good practices:**
Indent your code
Write attributes


If you have trouble remembering all the tags we've seen during the course, [take this pill :pill:](https://github.com/makersacademy/taster2.0/blob/master/assets/pills/html.md "Taster v2"), Glups

Hum... There is a little issue right ? Every elements are below the other ...

Should we style it to make it pretty !?

Challenge 2 - Make it pretty !
================

### Section 1: Make the bridge ! (15 min)

As you've seen during the lecture, we need to make some links between the HTML pages and the CSS pages.

1. We need to tell the HTML page where is the stylesheet

If you want to be sure that the link is correctly done, put something like that in your css file:

```css

body {
  background: lightblue;
}

```

### Section 2: Create the blocks ! (1h30)

1. Let's start by the menu, It needs to be:
  - On the top, right
  - Needs to be a block that push other elements underneath
  - It has the "monospace" font
  - The link (make it open in a new tab)

Write meaningful classes and Ids in order to let a non coder person understanding what you are styling.

For example:

Do not write classes like :
  .x or .y, etc

Prefer:
  .menu .menu__ul .menu__li

3. Go on with the article and then the footer

([take this pill :pill:](https://github.com/makersacademy/course/blob/master/pills/css.md "Taster v1") if you have some trouble)

To not loose your mind with CSS, you need to be careful and not write on top on the other rules.
That's why, we recommend you to code the structure of your page first and after to make it pretty.

Challenge 3 - Be agile !
================
