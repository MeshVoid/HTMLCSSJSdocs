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

| Selector   |  	Example  |  	Example description  |
| ------------- | ------------- | ------------- |
| #id           | #firstname    | Selects the element with id="firstname" |
| .class        | .intro | Selects all elements with class="intro"|
| *       |  	*| Selects all elements|
| element      |  	p | Selects all <p> elements|
| element,element,..        | div, p | Selects all <div> elements and all <p> elements|


# How To Add CSS

When a browser reads a style sheet, it will format the HTML document according to the information in the style sheet.

## Three ways to insert CSS

There are three ways of inserting a style sheet:

- External CSS
- Internal CSS
- Inline CSS

## External CSS

With an external style sheet, you can change the look of an entire website by changing just on file!

Each HTML page must include a reference to the external style sheet file inside the ```<link>``` element, inside the head section.

### Example

External styles are defined within the ```<link>``` element, inside he ```<head>``` section of an HTML page:

```html
<!DOCTYPE html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

An external style sheet can be written in any text editor, and must be saved with a .css extension.

The external .css file should not contain any HTML tags.

Here is how the "mystyle.css" file looks:

### "mystyle.css"

```css
body {
    background-color:lightblue;
}

h1 {
    color: navy;
    margin-left: 20px;
}
```
## Internal CSS

An internal style sheet may be used if one single HTML page has a unique style.

The internal style is defined insdie the ```<style>``` element, inside the head section.

### Example

Internals styles are defined within the ```<style>``` element, inside the ```<head>``` section of an HTML page:

```html
<html>
    <head>
        <style>
            body {
                background-color: linen;
            }

            h1 {
                color: maroon;
                margin-left: 40px;
            }
        </style>
    </head>
    <body>
        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>
    </body>
</html>
```

## Inline CSS

An inline style may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

### Example

Inline styles are defined within the "style" attribute of the relevant element:

```html
<!DOCTYPE html>
<html>
    <body>
        <h1 style="color:blue; text-aling:center;">This is a heading</h1>
        <p style="color:red;">This is a paragraph.</p>
    </body>
</html>
```

**Tip:** An inline style loses many of the advantages of a style sheet (by mixing content with presentation). Use this method sparingly.


## Multiple Style Sheets

If some properties have been defined for the same selector (element) in different style sheets, the value from the last read style sheet will be used.

Assume that an external style sheet has the following style for the ```<h1>``` element:

```css
h1 {
    color:navy;
}
```
Then, assume that an internal style sheet also has the following style for the ```<h1>``` element:

```css
h1 {
    color: orange;
}
```

### Example

If the internal style is defined **after** the link to the external style sheet, the ```<h1>``` elements will be "orange":

```html
<head>
    <link rel="stylesheet" type="text/css" href="mystyle.css">
    <style>
        h1 {
            color: orange;
        }
    </style>
</head>
```

### Example

However, if the internal style is defined before the link to the external style sheet, the ```<h1>``` elements wil be "navy":

```css
<head>
<style>
    h1 {
        color: orange;
    }
</style>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```

## Cascading Order

What style will be used when there is more one style specified for an HTML element?

All the styles in a page will "cascade" into a new "virtual" style sheet by the following rules, where number one has the highest priority:

1. Inline style (inside an HTML element)
2. External and internal style sheets (in the head section)
3. Browser default

So, an inline style has the highest priority, and will override external and internal styles and browser defaults.

**Video tutorial:**

[![Videotutorial](https://img.youtube.com/vi/VSwaoQ3TFkQ/maxresdefault.jpg)](https://youtu.be/VSwaoQ3TFkQ)

# CSS Comments

CSS comments are not displayed in the browser, but the ycan help document you source doe.

## CSS Comments

Comments are used to explain the code, and may help when you edit the source code at a later date.

Comments are ignored by browsers.

A CSS comment is placed inside the ```<style>``` element, and starts with ```/*``` and ends with ```*/```:

### Example

```css
/* This is a single-line comment */
p {
    color:red;
}
```

You can add comments wherever you want in the code:

### Example

```css
p {
    color:red; /* Set text color to red*/
}
```

Even in the middle of a code line:

```css
p {
    color: /*red*/blue;
}
```

Comments can also span multiple lines:

### Example

```css
/* This is a
multi-line
comment */

p {
    color: red;
}
```


## HTML and CSS Comments

From the HTML tutorial, you learned that you can add comments to your HTML source by using ```<!--...-->``` syntax.

In the following example, we use a combination of HTML and CSS comments:

### Example

```html
<!DOCTYPE html>
<html>
<head>
<style>
    p {
        color: red; /* Set text color to red */
    }
</style>
</head>
<body>

<h2>My Heading</h2>

<!-- These paragraphs will be red -->

<p>Hello World!</p>
<p>This paragraph is styled with CSS.</p>
<p>HTML and CSS comments are not shown in the output.</p>

</body>
</html>
```

**Video tutorial:**

[![Videotutorial](https://img.youtube.com/vi/uVtEJD3vBEs/maxresdefault.jpg)](https://youtu.be/uVtEJD3vBEs)


# CSS Colors

Colors are specified using predefined color names, or RGB, HEX, HSL, RGBA, HSLA values.

## CSS Color Names

In CSS, a color can be specified by using a predefined color name:

Tomato
Orange
DodgerBlue
MediumSeaGreen
Gray
SlateBlue
Violet
LightGray

CSS/HTML support 140 standard color names.

## CSS Background Color

You can set the backgroun color for HTML elements.

```html
<h1 style="background-color:DodgerBlue;">Hello World</h1>
<p style="background-color:Tomato;">Lorem ipsum...</p> 
```

## CSS Text Color

You can set the color of text:

```html
<h1 style="color:Tomato;">Hello World</h1>
<p style="color:DodgerBlue;">Lorem ipsum...</p>
<p style="color:MediumSeaGreen;">Ut wisi enim...</p> 
```

## CSS Border Color

You can set the color of borders:


```html
<h1 style="border:2px solid Tomato;">Hello World</h1>
<h1 style="border:2px solid DodgerBlue;">Hello World</h1>
<h1 style="border:2px solid Violet;">Hello World</h1> 
```

## CSS Color Values

In CSS, colors can also be specified using RGB values, HEX values, HSL values, RGBA values, and HSLA values:

Same as color name "Tomato":

- rgb(255, 99, 71)
- #ff6347
- hsl(9, 100%, 64%)

Same as color name "Tomato", but 50% transparent:

- rgba(255, 99, 71, 0.5)
- hsla(9, 100%, 64%, 0.5)

### Example

```html
<h1 style="background-color:rgb(255, 99, 71);">...</h1>
<h1 style="background-color:#ff6347;">...</h1>
<h1 style="background-color:hsl(9, 100%, 64%);">...</h1>

<h1 style="background-color:rgba(255, 99, 71, 0.5);">...</h1>
<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">...</h1> 
```
























































