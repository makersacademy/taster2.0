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

> For the geekest, open the element inspector, go to the network tab, reload the page and see if it is loading the page correctly.

### Section 2: Create the blocks ! (1h30)

>Write meaningful "classes" and "IDs" in order to let anybody understanding what you are styling.
Do not write classes like:
  .x or .y, etc
Prefer:
  .menu .menu__ul .menu__li

1. Let's start by the menu, It needs to be:
  - On the top, right
  - Needs to be a block that push other elements underneath
  - It has the "monospace" font
  - The link (make it open in a new tab)

2. Go on with the article:
  - Is relatively positioned after the menu
  - The width is about 80vw (learn about vw and vh units)
  - In order to put the picture on the right and the text on the left, you can float: left; the text.

3. The footer
  - Can be in position: fixed;
  - the text is centered by default

([take this pill :pill:](https://github.com/makersacademy/taster2.0/blob/master/assets/pills/css.md "Taster v1") if you have some trouble)

To not loose your mind with CSS, you need to be careful and not write on top on the other rules.
That's why, we recommend you to code the structure of your page first and after to make it pretty.

[Next challenge, be Agile!](https://github.com/makersacademy/taster2.0/blob/master/challenge_3.md "Challenge 3")
