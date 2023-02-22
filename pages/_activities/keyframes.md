---
layout: module
title: "Activity: Keyframes"
type: activity
draft: 0
---

Please download the exercise files (below).

<a href="/spring2023/course-files/activities/keyframes.zip" class="nu-button">Download Activity Files <i class="fas fa-download"></i></a>


## 1. Uncomment the relevant CSS style blocks
Inside of the `your-task` downloads folder, open `03-keyframes`, and take a look at the HTML and CSS files to get oriented with them. Then, before making any changes to the code, preview the index.html page in your web browser. You should see one cloud moving from left to right.

After previewing your webpage, **uncomment** the following two blocks of code lines inside your `styles.css`:

Inside of #cloud2:
```css
/*  animation-timing-function: linear;
    animation-iteration-count: infinite; 
    animation-name: moveCloudLeft;
    animation-delay: 3s;
    animation-duration: 5s; 
*/
```

Keyframe the bottom:
```css
/* @keyframes moveCloudLeft {
    from { 
        left: calc(100vw + 100px); 
    }
    to { 
        left: -100px; 
    }
} */
```

When you’re done, preview the page, noting what changed. You should now see a second cloud moving from right to left.

## 2. Play around with the existing animation

1. Try experimenting with the `animation-delay`, `animation-duration`, and `animation-timing-function` (ease-in, ease-out, ease, etc.) to change the speed and timing of the animation.
2. See if you can make `#cloud2` change to a darker gray and get larger as it moves across the screen.
    * Hint: Add some additional style rules to the `to {}` block of the `moveCloudLeft` keyframe.

## 3. Create a sunrise
See if you can make the circle on the bottom rise to the top (like a sunrise). To do this, you will have to define a new keyframe at the bottom of your stylesheet, and apply the keyframe to the `#sun` selector.