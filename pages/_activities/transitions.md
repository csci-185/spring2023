---
layout: module
title: "Activity: Transitions"
type: activity
draft: 0
---

Please download the exercise files (below).

<a href="/spring2023/course-files/activities/transitions.zip" class="nu-button">Download Activity Files <i class="fas fa-download"></i></a>

## 1. Uncomment the relevant CSS style blocks
Inside of the `your-task` downloads folder, open `02-transitions`, and take a look at the HTML and CSS files to get oriented with them. Then, before making any changes to the code, preview the `index.html` page in your web browser.

After previewing your webpage, **uncomment** the following lines inside your `styles.css` style block:

```css
/*
#section1 {
    background: #0c7474;
    color: white;
    transition: all 0.3s ease-out;
}

#section1:hover {
    background: purple;
    width: 220px;
    height: 220px;
}
*/
```

When you're done, preview the page, noting what changed. When you hover over the first section, you the section should grow and change color (horray)! 

## 2. Create two more transition effects
Your job is to experiment with the other two section tags (`#section2` and `#section3`) by making some interesting interactions, using transitions. Some tips:

1. To make a <a href="https://www.w3schools.com/css/css3_transitions.asp" target="_blank">transition</a>, you define a transition inside of a style block (e.g., `#section1`) as follows: `transition: <property> <duration> <timing-function> <delay>;` Examples:
    * transition: all 0.3s ease-out;
    * transition: background 1s ease-in;
    * transition: all 3s linear;
    * transition: all 0.3s ease;
    {:.compact}
2. Some properties that you may want to change:
    * border-radius
    * margin
    * padding
    * width
    * height
    * border-width
    * background-color
    * rotation
    * opacity
    * <a href="https://www.w3schools.com/css/css3_2dtransforms.asp" target="_blank">transform</a>. Examples<br>transform: skewX(20deg);<br>transform: rotate(-10deg);
    {:.compact}

Feel free to look at `sample-files/02-pseudo-classes` and `sample-files/03-transitions` to get ideas.