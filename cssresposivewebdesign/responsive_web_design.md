# Responsive Web Design - Introduction

## What is Responsive Web Design?

Responsive web design makes your web page look good on all devices.

Responsive web desing uses only HTML and CSS.

Responsive web design is not a program or a JavaScript.

## Designing for the best experience for all users

Web pages can be viewed using many different devices: desktops, tablets, and phones. Your web page should look good, and be easy to use, regardless of the device.

Web pages should not leave out infromation to fit smaller devices, but rather adapt its content to fit any device:

![Destop layout](rwd_desktop.png)

![Tablet layout](rwd_tablet.png)

![Phone layout](rwd_phone.png)

It is called responsive web design when you use CSS and HTML to resize, hide, shrink, enlarge, or move the content to make it look good on any screen.


# Responsive Web Design - The Viewport

## What is the Viewport?

The viewport is the user's visible area of a web page.

The viewport varies with the device, and will be smaller on a mobile phone than on a computer screen.

Before tablets and mobile phones, web pages were designed only for computer screens, and it was common for web pages to have a static design and a fixed size.

Then, when we started surfing the internet using tablets and mobile phones, fixed size web pages were too large to fit the viewport. To fix this, browsers on those devices scaled down the entire web page to fit the screen.

This was not perfect!! But a quick fix.

## Setting the viewport

HTML5 introduced a method to let web designers take control over the viewport, through the ```<meta>``` tag.

You should include the following ```<meta>``` viewport element in the ```<head>``` section of al lyour web pages:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

This gives the browser instruction on how to control the pages, dimensions and scaling. The ```width=device-width``` part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).

The ```initial-scale=1.0``` part sets the intial zoom level when the page is first loaded by the browser.

Here is an example of a web page without the viewport meta tag, and the same web page with the viewport meta tag:

![Without the viewport tag](img_viewport1.png)

**Without the viewport tag**

![With the viewport tag](img_viewport2.png)

**With the viewport tag**

Tip: If you are browsing this page with a phone or a tablet, you can click on the two links above to see the difference.

## Size content to the viewport

Users are used to scroll websites vertically on both desktop and mobile devices - but not horizontally!

So, if the user is forced to scroll horizontally, or zoom out, to see the whole web page it results in a poor user experience.

Some additional rules to follow:

1. Do NOT use large fixed-width elements - For example, if an image has a width wider than the viewport, it causes the viewport to scroll horizontally. Remember to adjust this content to fit within the width of the viewport.

2. Do NOT let the content rely on a particular width to render well - Since screen dimensions and width in CSS pixels vary widely between devices, content should not rely on a particular viewport width to render well.

3. Use CSS media queries to apply different styling for small and large screens - Setting large absolute CSS widths for page elements will cause the elements to be too wide for smaller devices. Instead, consider using relative width values, such as width: 100%. Also, be careful of using large absolute positioning values. It may cause the element to fall outside the viewport on small devices.