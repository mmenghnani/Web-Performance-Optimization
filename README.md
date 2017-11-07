## Website Performance Optimization portfolio project

Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed! In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

To get started, check out the repository and inspect the code.

### Getting started

#### Part 1: Optimize PageSpeed Insights score for index.html

1) Added async attribute to all the JS files
2) Added media="print" for the CSS.
3) Inlined the style.css file
4) Inlined the both the other JS scripts
5) Moved the font link below the footer
6) Compressed the profile pic and the pizzeria pic


#### Part 2: Optimize Frames per Second in pizza.html

Main.js changes
1) In the function changePizzaSizes,
    a) Brought the declaration of dx,newwidth and randomPizzaContainer outside the loop
    b) Instead of using querySelectorAll, I am using getElementById now.
2) In the function updatePositions,
    a) Brought the declaration of items,scrollTop and scrollTopNew outside the loop
    b) Instead of using querySelectorAll, I am using getElementsByClassName now.
3) Decreased the number of iterations for the loop generating sliding pizza from 200 to 100.

HTML changes
1) Inlined the style.css for pizza.html to unblock critical rendering path


