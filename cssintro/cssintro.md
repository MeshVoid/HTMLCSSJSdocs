# CSS Tutorial

## Learn CSS

CSS is the language we use to style an HTML document.
CSS describes how HTML elements should be displayed.
This tutorial will teach you CSS from basic to advanced.

## Examples in each chapter

### CSS Example

```css
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
```

FREE CSS TEMPLATES CAN BE FOUND HERE:
https://www.w3schools.com/css/css_rwd_templates.asp

# CSS Introduction

CSS is the language we use to style a web page.

## What is CSS?

- CSS stands for Cascading Style Sheets
- CSS describes how HTML elements are to be displayed on screen, paper, or in other media
- External stylesheets are stored in CSS files

## Why Use CSS?

CSS is used to define styles for your web pages, including the design, layout and variation in display for different devices and screen sizes.

```css
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
```

## CSS Solved a Big Problem

HTML was NEVER intended to contain tags for formatting a web page!

HTML was created to describe the content of a web page, like:

```html
<h1>This is a heading</h1>
<p>This is a paragraph.</p>
```

When tags line <font>, and color attributes were added to the HTML 3.2 specification, it started a nightmare for web developers. Development of large websites, where fonts and color information were added to every single page, became a long and expensive process.

To solve this problem, the World Wide Web Consortium (W3C) created CSS.

CSS removed the style formatting from the HTML page!

## CSS Saves a lot of work!

The style definitions are normally saved in external .css files.

With an external stylesheet file, you can change the look of an entire website by changing just one file!

Video tutorial:


[![Videotutorial](https://img.youtube.com/vi/AGDDdsiZ0Ko/maxresdefault.jpg)](https://youtu.be/AGDDdsiZ0Ko)

# CSS Syntax

A CSS rule consists of a selector and a declaration block.

![css example scheme](img_selector.gif)

The selector points to the HTML element you want to style.

The declaration block contains one or more declarations separated by semicolons.

Each declaration includes a CSS property name and a value, separated by a colon.

Multiple CSS declarations are separated with semicolons, and declaration blocks are surrounded by curly braces.

## Example

In this example all ```<p>``` elements will be center-aligned, with a red text color:

```css
p {
    color: red;
    text-align: center;
}
```

### Example explainded
```p``` is a selector in CSS (it points to the HTML element you want to style: ```<p>```).
```color``` is a property, and ```red``` is the property value
```text-align``` is a property, and ```center``` is the property value

Video tutorial:

[![Videotutorial](https://img.youtube.com/vi/G8r00ZNopTE/maxresdefault.jpg)](https://youtu.be/G8r00ZNopTE)

# CSS Selectors

A CSS selector selects the HTML element you want to style.

## CSS Selectors

CSS selectors are used to "find" (or select) the HTML elements you want to style.

We can divide CSS selectors into five categories:

- Simple selectors (select elements based on name, id, class)
- Combinator selectors (select elements based on a specific relationship between them)
- Pseudo-class selectors (select elements based on a certain state)
- Pseudo-elements selectors (select and style a part of an element)
- Attribute selectors (select elements based on an attribute or attribute value)

This page will explain the most basic CSS selectors.

## The CSS element selector

The element selector selects HTML elements based on the element name.

### Example

Here, all ```<p>``` elements on the page will be center-aligned, with a red text color:

```css
p {
    text-align: center;
    color: red;
}
```

## The CSS id Selector

The id selector uses the id attribute of an HTML element to select a specific element.

The id of an element is unique within a page, so the id selector is used to select one unique element!

To select an element with a specific id, write a hash (#) character, followed by the id of the element.

### Example

The CSS rule below will be applied to the HTML element with id="para1":

```css
#para1 {
    text-align: center;
    color: red;
}
```

**Note:** And id name cannot start with a number!

## The CSS class selector

The class selector selects HTML elements with a specific class attribute.

To select elements with a specific class, write a period (.) character, followed by the class name.


### Example

In this example all HTML elements with class="center" will be red and center-aligned:

```css
    text-align: center;
    color: red;
```
You can also specify that only specific HTML elements should be affected by a class.

### Example

In this example only ```<p>``` elements with class="center" will be red and center-aligned:

```css
p.center {
    text-align: center;
    color: red;
}
```
HTML elements can also refer to more than one class.

### Example

In this example the ```<p>``` element will be styled according to class="center" and to class="large":
```html
<p class="center large">This paragraph refers to two classes.</p>
```

**Note:** A class name cannot start with a number!

## The CSS universal selector

The universal selector (*) selects all HTML elements on the page.

### Example

```css
* {
    text-align: center;
    color: blue;
}
```

## The CSS Grouping selector

The grouping selector selects all the HTML elements with the same style definitions.

Look at the following CSS code (the h1, h2, and p elements have the same style definitions):

```css
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

It will be better to group the selectors, to minimize the code.

To group selectors, separate each selector with a comma.

### Example 

In this example we have grouped the selectors from the code above:

```css
h1, h2, p {
    text-align: center;
    color: red;
}
```

### ALL CSS simple selectors

| Column 1      | Column 2      |   Column 3   |
| ------------- | ------------- | ------------- |
| Cell 1, Row 1 | Cell 2, Row 1 |  |
| Cell 1, Row 2 | Cell 1, Row 2 | |