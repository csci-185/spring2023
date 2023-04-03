---
layout: assignment-two-column
title: Make some algorithmic art
type: tutorial
abbreviation: Tutorial 9
draft: 1
points: 6
num: 9
due_date: 2023-04-07
---

<style>
    .cars {
        min-width: 450px;
        border-top: solid 1px #666;
        border-left: solid 1px #666;
        border-right: solid 1px #666;
        border-radius: 4px;
        width: 70%;
    } 

    .grid {
        display: grid;
        grid-template-columns: 1fr 1fr;
        column-gap: 10px;
        row-gap: 10px;
    }
    .grid img {
        width: 100%;
    }

    .span2 {
        grid-column: 1 / span 2;
    }
</style>

<a class="nu-button" href="/spring2023/course-files/tutorials/tutorial09.zip" target="_blank">
    Tutorial 09 Starter Files <i class="fas fa-download"></i>
</a> 

The goal of this tutorial is to get you more comfortable working with loops and conditional statements.

{: .blockquote-no-margin}
> **LEARNING OBJECTIVES:** 
> 1. Practice working with loops
> 1. Practice working with if statements
> 1. Practice working with JavaScript's built-in Math.random() module

## Part 1: Loop Art

<div class="grid">
    <img class="span2" src="/spring2023/assets/images/tutorials/tutorial09/bubbles.png" /> 
    <img class="span2" src="/spring2023/assets/images/tutorials/tutorial09/stars.png" /> 
    <img src="/spring2023/assets/images/tutorials/tutorial09/lines.png" /> 
    <img src="/spring2023/assets/images/tutorials/tutorial09/crosses.png" /> 
    <img src="/spring2023/assets/images/tutorials/tutorial09/color-shapes.png" /> 
    <img src="/spring2023/assets/images/tutorials/tutorial09/lines-rotating.gif" /> 
    <img src="/spring2023/assets/images/tutorials/tutorial09/squares-rotating.gif" /> 
    <img src="/spring2023/assets/images/tutorials/tutorial09/bubbles.gif" /> 
</div>

> ### Your task (8 pts)
> In `landscapes/sketch.js`, replace the code on lines 18-22 (which is repetitive) with a loop (any kind of loop you want) that makes 1,000 stars (or bubbles -- up to you) that fill the entire canvas. 

#### Hints:

* Use a loop
* Use JavaScript's built-in `Math.random()` function to give each star (or bubble) a random (x, y) position (given the dimensions of the screen) and a random width (so that it renders stars / bubbles of different sizes).
    * Hint: There is some sample code on lines 7-13 that demonstrates how to use the `Math.random()` function. Once you get the hang of it, you can delete those lines...they're just for your reference. 

> ### Optional enhancements (extra credit)
> 1. **[1pt]** Draw a constellation (Orion's Belt, Big Dipper, etc.)
> 1. **[2pts]** Make your stars twinkle
>     * Hint: You will need to implement the `draw()` function and periodically show and hide select stars. 
> 1. **[2pts]** Animate your bubbles
>     * Hint: You will need to implement the `draw()` function so that it moves each bubble. Consider storing your bubble positions in an array so that you can update each of them everytime the `draw()` function is invoked by the `p5.js` animation loop.

## Part 2: Animation

<img class="cars" src="/spring2023/assets/images/tutorials/tutorial09/cars.gif" /> 

### Introduction
Open the `cars/sketch.js` file and examine the starter code. Some things to note:
* I have created a `drawCar()` function for you, which draws a car of any position, size, and color, depending on the values passed into the function as arguments. 
* I have also created an object called `c1` that is called a "state object." It keeps track of the data values for the car. You can create additional state objects to keep track of additional cars.
* `p5.js` requires us to define a `setup()` function to define the canvas we'll be using for our animation.
* `p5.js` also allows us to define an optional `draw()` function, which will be invoked in p5's built-in animation loop. Everything inside of `draw()` will be called over and over again as part of the animation loop.
* Within the `draw()` loop, I have already started animating the pink car. Your job will involve enhancing this code so that it looks like the one in the animation above.

> ### Your tasks (8 pts)
> * Currently, the pink car moves very slowly. Make it move at a reasonable pace by modifying the data in the `c1` object at the top of the page.
> * If the pink car gets past the end of the screen, it should seamlessly be moved to the beginning of the screen, so that it looks like it's wrapping around.
> * Next, add a second car to your animation, which should move in the opposite direction, and also loop back around when it gets to the end of the screen (see the animated gif). To do this:
>    * Copy the `c1` object, paste it below the first one. Rename the copied object to `c2.` This new `c2` state object will help you animate a second car. 
>    * Within the `draw()` function, add another `drawCar()` function call, but using the c2 object to position the car.
>    * Note: the cars don't have to be the same size or go the same speed.


> ### Optional enhancements (extra credit)
> The more you practice, the better you'll get!
> 
> 1. **[1pt]** Add a third car with a different position, size, and color (and make sure it also wraps around when it gets to the end).
> 1. **[2pts]** Create a `drawTruck()` function that draws a truck. Then add the truck to your animation (in addition to the 2 cars and make sure it also wraps around when it gets to the end).
> 1. **[1pt]** Make the cars accelerate over time (start off slow and gradually move faster).
> 1. **[2pt]** Add your creature to your animation:
>     * Inside `helpers.py`:
>     * Add your `drawCreature` function definition (adapt from Homework 3). 
>     * In `cars/sketch.js`: animate your creature
> 1. **[3pt]** Add one of your classmate's creatures to your animation, and complete the steps from #2 directly above. 


## What to Submit
**Please Read Carefully:** To submit Homework 4, please paste the following links into the Moodle under the Homework 4 submission section:

1. A link to your **homepage** on GitHub pages, which should link to:
    * Your landscape page (8pts)
    * Your animation page (8pts)
2. A link to your GitHub **code repository** (where your code files are stored).
3. If you did any extra credit, please describe what you did, so that I can make sure I give you the appropriate points.    
    * You may earn up to 4pts extra credit.

See <a href="https://vanwars.github.io/csci185-coursework/" target="_blank">Sarah's homepage</a> for an example.
