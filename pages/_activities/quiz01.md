---
layout: two-column
title: Quiz 1
type: tutorial
draft: 0
points: 6
num: 4
due_date: 2023-02-10
---

<style>
    img {
        max-width: 70%;
    }
</style>

Please download the starter files and complete the tasks described below. Read the instructions that are outlined under each task very carefully. Complete as many tasks as you can by the end of the quiz. Just do your best.

## Part 1. HTML Tasks (index.html)

### 1. Stylesheet Link
1. Open `index.html`
2. Add a stylesheet link to `styles.css`, which is located in the `assets` folder.

If you did it correctly, the background of your web page should turn dark blue.

### 2. Header Section
1. Add three semantic tags inside the body tag:
    * a `header` tag
    * a `main` tag
    * a `footer` tag
1. Inside the `header` tag, add an `img` tag that links to the `taco-temple-logo.webp` file (in the `images` folder).

### 3. Navigation Section
1. Next to the `img` tag (but still inside the `header` tag), add a `nav` tag.
1. Inside the `nav` tag, add 3 hyperlinks:
    * One called **Menu** that links to `menu.html`
    * One called **Contact** that links to `contact.html` 
    * One called **Hours & Location** that links to `location-hours.html` 

<img src="/spring2023/assets/images/quizzes/quiz01/ss01.png" />

### 4. Main Section
1. Give the `main` task a class called "landing.
1. Inside the `main` tag, add two tags:
1. An `img` tag that links to the `landing-image.webp` file (in the images folder).
2. A `section` tag. Inside the section tag, add two tags:
    * An `h1` that says: "Call 828-255-8098 for take-out or click below to order online!"
    * A hyperlink that links to the Taco Temple order online page here: <a href="https://www.mamacitastacotemple.com/s/order" target="_blank">https://www.mamacitastacotemple.com/s/order</a>

<img src="/spring2023/assets/images/quizzes/quiz01/ss02.png" />

### 5. Footer
Within the `footer` tag, create a paragraph tag that says “Copyright 2023, Taco Temple.”

## Part 2. HTML Tasks (other files)

### 1. Stylesheet Link
1. Open `menu.html`
2. Add a  stylesheet link to `styles.css`, which is located in the `assets` folder.

### 2. Header Section
1. Copy the entire `header` tag (and everything inside of it) from `index.html` and paste it into `menu.html` **above** the `main` tag.
2. Adjust the file paths for the relative links so that the relative paths don't break (now that you're editing a file in the `site-pages` folder).

### 3. Footer Section
1. Copy the entire `header` tag  (and everything inside of it) from `index.html` and paste it into `menu.html` **below** the `main` tag.

### 4. Repeat with contact.html & location-hours.html
Repeat steps 1-3 above with `contact.html` & `location-hours.html`. 

## Part 3: Styling tasks

### 1. Style the image inside the header tag
Create a ruleset for **"img" elements inside of "header" elements**. The rule should set the width to `180px` and the right margin to `100px`.

### 2. Style the header tag
Create a rulset for **"header" elements** that applies the following styles:

```css
padding: 25px 13vw;
display: flex;
align-items: center;
```

### 3. Style the main tag with a class of "landing"
Create a ruleset for **elements with a class of "landing"** that applies the following styles:

```css
background: white;
padding: 50px 15vw 200px 15vw;
display: grid;
grid-template-columns: 60% 40%;
align-items: center;
justify-content: center;
```

Target **"img" elements inside of main elements** and give them a width of `100%`.

### 4. h1 styling
Apply the following style rules to **"h1" elements inside of elements with a class of "landing"**:

```css
color: black;
line-height: 1.2em;
font-size: 1.7em;
font-family: Malamondo-Alt;
```

### 5. link styling
Apply the following style rules to **"a" elements inside of elements with a class of "landing"**:

```css
 text-align: center;
background-color: #013672;
color: white;
border: solid 2px white;
padding: 10px 20px;
font-weight: 300;
margin: auto;
display: block;
width: 100px;
border-radius: 4px;
text-decoration: none;
```

### 6. Body Copy
Add the following rules to the existing `body` ruleset in your CSS file:

```css
font-family: 'Work Sans', sans-serif;
font-size: 1.1em;
font-weight: 400;
line-height: 1.5em;
```

