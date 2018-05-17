## Website Performance Optimization portfolio project

The challenge was to optimize this online portfolio for speed! In particular, to optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).


### Getting started

#### Part 1: Optimize PageSpeed Insights score for index.html

1) Added async attribute to all the JS files
2) Added media="print" for the CSS.
3) Inlined the style.css file
4) Inlined the both the other JS scripts
5) Moved the font link below the footer
6) Compressed the profile pic and the pizzeria pic

Pagespeed Insights Scores
1) index.html - Mobile(90),Desktop(90)
2) project-2048.html - Mobile(95),Desktop(97)
3) project-mobile.html - Mobile(95),Desktop(97)
4) project-webperf.html - Mobile(96),Desktop(97)


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
1) Inlined the style.css for pizza.html

Time to resize pizza




![image](https://user-images.githubusercontent.com/11216561/32531010-660e6d5c-c3f6-11e7-9b33-67a3b15cb4b9.png)




Time to generate last 10 frames





![image](https://user-images.githubusercontent.com/11216561/32531750-908d6926-c3fa-11e7-9f87-7fe918e522e6.png)






