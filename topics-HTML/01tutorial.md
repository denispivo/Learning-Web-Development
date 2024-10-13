# Tutorial

[go back to REDME.md](/README.md)

All upcoming topics are tested in the test.html file

- [Elements](#elements)
- [Attributes](#attributes)
- [Paragraphs](#paragraphs)
- [Styles](#styles)
- [Formatting](#formatting)
- [Quotation and Citation](#quotation-and-citation)
- [Comments](#comments)
- [Colors](#colors)
- [Styles - CSS](#html-styles---css)
- [Links](#links)
- [Images](#images)
- [Image Maps](#image-maps)
- [Background Images](#background-images)
- [Picture Element](#picture-element)
- [Favicon](#favicon)
- [Page Title](#page-title)
- [Tables](#tables)
- [Table Borders](#table-borders)
- [Table Sizes](#table-sizes)
- [Table Headers](#table-headers)
- []()
- []()

## Elements

| Element          | Description                          |
| ---------------- | ------------------------------------ |
| `<html>`         | Defines the root of an HTML document |
| `<body>`         | Defines the document's body          |
| `<h1>` to `<h6>` | Defines HTML headings                |

## Attributes

All HTML elements can have **attributes**

| Element  | Attribute            | Description                                                                        |
| -------- | -------------------- | ---------------------------------------------------------------------------------- |
| `<a>`    | `href`               | Specifies the URL of the page the link goes to                                     |
| `<img>`  | `src`                | Specifies the path to the image to be displayed                                    |
| `<img>`  | `width` and `height` | Provide size information for images                                                |
| `<img>`  | `alt`                | Provides an alternate text for an image                                            |
| `<html>` | `lang`               | Tag declares the language of the Web page                                          |
|          | `style`              | Attribute is used to add styles to an element, such as color, font, size, and more |
|          | `title`              | Attribute defines some extra information about an element                          |

## Paragraphs

| Element | Description                              |
| ------- | ---------------------------------------- |
| `<p>`   | Defines a paragraph                      |
| `<hr>`  | Defines a thematic change in the content |
| `<br>`  | Inserts a single line break              |
| `<pre>` | Denies a pre-formatted text              |

## Styles

| Element            | Description                                            |
| ------------------ | ------------------------------------------------------ |
| `style`            | Used for styling HTML elements                         |
| `background-color` | Used for background color                              |
| `color`            | Used for text color                                    |
| `font-family`      | Used for text fonts                                    |
| `font-size`        | Used for text sizes                                    |
| `text-align`       | Used for text alignment (top/bottom/left/right/center) |

## Formatting

| Element    | Description                                                                                                                                                                                                                                     |
| ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `<b>`      | - Defines bold text <br>- without any extra importance                                                                                                                                                                                          |
| `<strong>` | - Defines important text <br>- content is typically in bold                                                                                                                                                                                     |
| `<i>`      | - Defines a part of text in an alternate voice or mood <br>- content inside is typically displayed in italic <br>=> Tip: The `<i>` tag is often used to indicate a technical term, a phrase from another language, a thought, a ship name, etc. |
| `<em>`     | - Defines emphasized text <br>- content inside is typically displayed in italic <br>=> Tip: A screen reader will pronounce the words in `<em>` with an emphasis, using verbal stress.                                                           |
| `<small>`  | - Defines smaller text                                                                                                                                                                                                                          |
| `<mark>`   | - Defines marked/highlighted text                                                                                                                                                                                                               |
| `<del>`    | - Defines text, that has been deleted from a document <br>- browsers will usually strike a line through deleted text                                                                                                                            |
| `<ins>`    | - Defines text, that has been inserted into a document <br>- browsers will usually underline inserted text                                                                                                                                      |
| `<sub>`    | - Defines subscripted text <br>- appears half a character below the normal line and is sometimes rendered in a smaller font <br>=> Subscript text can be used for chemical formulas, like H<sub>2</sub>O                                        |
| `<sup>`    | - Defines superscripted text <br>- appears half a character above the normal line and is sometimes rendered in a smaller font <br>=> Superscript text can be used for footnotes, like WWW<sup>[1]</sup>                                         |

## Quotation and Citation

| Element        | Description                                                                                                                                                                                                                                                                                                                        |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `<blockquote>` | - element defines a section that is quoted from another source                                                                                                                                                                                                                                                                     |
| `<q>`          | - tag defines a short quotation                                                                                                                                                                                                                                                                                                    |
| `<abbr>`       | - tag defines an abbreviation or an acronym <br>- Marking abbreviations can give useful information to browsers, translation systems and search-engines <br>=> Tip: Use the global title attribute to show the description for the abbreviation/acronym when you mouse over the element.                                           |
| `<address>`    | - tag defines the contact information for the author/owner of a document or an article <br> - The contact information can be an email address, URL, physical address, phone number, social media handle, etc <br> -> usually renders in italic, and browsers will always add a line break before and after the `<address>` element |
| `<cite>`       | - tag defines the title of a creative work                                                                                                                                                                                                                                                                                         |
| `<bdo>`        | - Bi-Directional Override <br>- this tag is used to override the current text direction                                                                                                                                                                                                                                            |

## Comments

Comments exist to give more information to the written code. Use it to describe your code, so that you and your team can easily understand later what the code does.

This is ho to write a comment in HTML:

```HTML code
<!-- This is a comment -->

<p>This is a paragraph.</p>
```

Use comments to hide content to test the code when an bug occurs:

```HTML code
<p>This is a paragraph.</p>

<!-- <p>This is another paragraph </p> -->

<p>This is a paragraph too.</p>
```

## Colors

Colors are predefindes with color names, RGB, HEX, HSL, RGBA or HSLA values.

### Color names

Examples:

- Tomato
- Orange
- DodgerBlue
- MediumSeaGreen
- Gray
- SlateBlue
- Violet
- LightGray

HTML supports [140 standard color names](https://www.w3schools.com/colors/colors_names.asp).

### Background Color

You can set the background color for HTML elements with `style="background-color:___"`
Example: `<h1 style="background-color:DodgerBlue;">Hello World</h1>`

### Text Color

You can set the Text color with `style="color:___"`
Example: `<h1 style="color:Tomato;">Hello World</h1>`

### Border Color

You can set the color of borders with `style="border:__ __ __"`
Example: `<h1 style="border:2px solid Tomato;">Hello World</h1>`

### Color Values

In HTML colors can also be specified using RGB, HEX, HSL, RGBA and HSLA values.

| Value Type | Example                                            | HTML Example                                                     |
| ---------- | -------------------------------------------------- | ---------------------------------------------------------------- |
| RGB        | `rbg(255, 99 ,71)`                                 | `<h1 style="background-color:rgb(255, 99, 71);">...</h1>`        |
| HEX        | `#ff6347`                                          | `<h1 style="background-color:#ff6347;">...</h1>`                 |
| HSL        | `hsl(9, 100%, 64%)`                                | `<h1 style="background-color:hsl(9, 100%, 64%);">...</h1>`       |
| RGBA       | `rgba(255, 99 , 71, 0.5)` <br> -> 50% transparency | `<h1 style="background-color:rgba(255, 99, 71, 0.5);">...</h1>`  |
| HSLA       | `hsla(9, 100%, 64%, 0.5)` <br> -> 50% transparency | `<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">...</h1>` |

### RGB and RGBA Colors

RGB = (RED, GREEN, BLUE)

- every value can be between 0 and 255

RGBA = (RED, GREEN, BLUE, {alpha channel})

- the same as RGB, but with an extra alpha value

### HEX Colors

HEX = #rrggbb (#red green blue)

- every hexadecimal value can be between 0 and 15, with {0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F}

### HSL and HSLA Colors

HSL = (hue, saturation, lightness)

- hue is a degree on the color wheel, from 0 to 360 (0 = red; 120 = green; 240 = blue;)
- saturation is a percentage value (0% = shades of gray; 100% = full color;)
- lightness is also a percentage value (0% = black; 100% = white;)

HSLA = (hue, saturation, lightness, alpha)

- the same as HSL, but with an extra alpha value

## Styles - CSS

CSS = Cascading Style Sheets

CSS is used to format the layout of multiple web pages all at once.

### Using CSS

CSS can be added to HTML documents in 3 ways:

| Type     | Attribute | Description                                      |
| -------- | --------- | ------------------------------------------------ |
| Inline   | `style`   | Using thins inside HTML elements                 |
| Internal | `<style>` | Using this element in the `<head>` section       |
| External | `<link>`  | Using this element to link to external CSS files |

=> The most common way to use CSS is by writing the styles in an external CSS files.

### Inline CSS

Example:

```HTML
<h1 style="color:blue;">A Blue Heading</h1>

<p style="color:red;">A red paragraph.</p>
```

### Internal CSS

Example:

```HTML
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {background-color: powderblue;}
            h1   {color: blue;}
            p    {color: red;}
        </style>
    </head>
    <body>

        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>

    </body>
</html>
```

### External CSS

Example:

```HTML
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="styles.css">
    </head>
    <body>

        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>

    </body>
</html>
```

"styles.css":

```CSS
body {
    background-color: powderblue;
}
h1 {
    color: blue;
}
p {
    color: red;
}
```

### CSS Colors, Fonts and Sizes

| Element       | Description            |
| ------------- | ---------------------- |
| `color`       | Defines the text color |
| `font-family` | Defines the font       |
| `font-size`   | Defines the text size  |

Example:

```HTML
 <!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {
                color: blue;
                font-family: verdana;
                font-size: 300%;
            }
            p {
                color: red;
                font-family: courier;
                font-size: 160%;
            }
        </style>
    </head>
    <body>

        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>

    </body>
</html>
```

### CSS Border, Padding, Margin

| Property  | Description                                               | HTML Example                                                                                 |
| --------- | --------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `border`  | Defines a border around HTMl elements                     | <code>p { <br> &nbsp; border: 2px solid powderblue; <br> }</code>                            |
| `padding` | Defines a padding (space) between the text and the border | <code>p { <br> &nbsp; border: 2px solid powderblue; <br> &nbsp; padding: 30px; <br> }</code> |
| `margin`  | Defines a margin (space) outside the border               | <code>p { <br> &nbsp; border: 2px solid powderblue; <br> &nbsp; margin: 50px; <br> }</code>  |

### Link to External CSS

External CSS can be referenced with a full URL or with a path relative to the current web page.

Example with full URL:

```HTML
<link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">
```

Example with a style sheet located in the html folder on the current web site:

```HTML
<link rel="stylesheet" href="/html/styles.css">
```

Example with a style sheet located in the same folder as the page:

```HTML
<link rel="stylesheet" href="styles.css">
```

## Links

HTML links are hyperlinks. Click a link and get to another document (HTML, IMG, PNG, ...).

Links don´t need to be text, they can be every other element.

### Syntax

`<a>` defines a hyperlink.

Syntax:

```HTML
<a href="url">link text</a>
```

The most important part is the `href` attribute, it defines the destination of the hyperlink.

"link text" is shown to the user and can be clicked to send the user to the specified URL.

Example:

```HTML
<a href="https://www.w3schools.com/">Visit W3Schools.com!</a>
```

By default, links are...

    ... underlined and blue, when not visited.
    ... underlined and purple, when visited.
    ... underlined and red, when active. That means, when the user clicks on the link, it gets red while pressed.

=> Links can be styled with CSS.

### The target Attribute

By default the link will open in the current browser window.

The `target` attribute specifies where to open the linked document.

Values you can set of `target`:

| Value     | Definition                                                               |
| --------- | ------------------------------------------------------------------------ |
| `_self`   | Default, opens in the same window/tab.                                   |
| `_blank`  | Opens in a new window/tab.                                               |
| `_parent` | Opens in the parent frame. Does what is defined in the parent frame.     |
| `_top`    | Opens in the full body of window. Does what is defined in the top frame. |

=> Go read Iframe to know how frames work. (not done yet)

Example:

```HTML
<a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>
```

### Absolute URLs vs. Relative URLs

An absolute URL is the full address of a webpage.

Example:

```HTML
<h2>Absolute URLs</h2>
<p><a href="https://www.w3.org/">W3C</a></p>
<p><a href="https://www.google.com/">Google</a></p>
```

A relative URL is a local link to the page on the same website. (without the "https://www." part)

Example:

```HTML
<h2>Relative URLs</h2>
<p><a href="html_images.asp">HTML Images</a></p>
<p><a href="/css/default.asp">CSS Tutorial</a></p>
```

### Links - Use an Image as a Link

Just put an image tag (`<img>`) inside the link tag (`<a>`).

Example:

```HTML
<a href="default.asp">
<img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a>
```

### Link to an Email Address

Use `mailto:` inside the `href`.

Example:

```HTML
<a href="mailto:someone@example.com">Send email</a>
```

### Button as a Link

To use a button, you need to add some JavaScript code, to specify what the button will do, at certain events.

Example:

```HTML
<button onclick="document.location='default.asp'">HTML Tutorial</button>
```

### Link Titles

Titles can also be used with links, as in this [definition](#attributes) of the attribute title.

Example:

```HTML
<a href="https://www.w3schools.com/html/" title="Go to W3Schools HTML section">Visit our HTML Tutorial</a>
```

### Link Colors

As said before:

By default, links are...

    ... underlined and blue, when not visited.
    ... underlined and purple, when visited.
    ... underlined and red, when active. That means, when the user clicks on the link, it gets red while pressed.

Use CSS to change those colors:

```HTML
<style>
a:link {
  color: green;
  background-color: transparent;
  text-decoration: none;
}

a:visited {
  color: pink;
  background-color: transparent;
  text-decoration: none;
}

a:hover {
  color: red;
  background-color: transparent;
  text-decoration: underline;
}

a:active {
  color: yellow;
  background-color: transparent;
  text-decoration: underline;
}
</style>
```

### Buttons

As said before, the functionality of a button comes with JavaScript. To style the button you need CSS.

Example:

```HTML
<style>
a:link, a:visited {
  background-color: #f44336;
  color: white;
  padding: 15px 25px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
}

a:hover, a:active {
  background-color: red;
}
</style>
```

### Create Bookmarks

Bookmarks are used if the website is long and to see the topics at the top, to instantly go to the topic written on the website. (commonly used on wikipedia)

Use `id` attribute to create the bookmark:

```HTML
<h2 id="C4">Chapter 4</h2>
```

Add `id` of the bookmark to the link, to jump to the bookmark:

```HTML
<a href="#C4">Jump to Chapter 4</a>
```

You can also jump to a bookmark on another page:

```HTML
<a href="html_demo.html#C4">Jump to Chapter 4</a>
```

## Images

The HMTL `<img>` tag is used to link images to websites, they are technically not inserted.

This tag is empty and only holds attributes.

The two required attributes are:

- `src` -> path to the image
- `alt` -> alternate text for the image

Syntax:

```HTML
<img src="url" alt="alternatetext">
```

### `src` Attribute

This tag specifies the path (URL) to the image.

Example:

```HTML
<img src="img_chania.jpg" alt="Flowers in Chania">
```

### `alt` Attribute

Alternate provides text for an image, if the image can´t be shown for some reason.

The value of `alt` should describe the image:

Example:

```HTML
<img src="img_chania.jpg" alt="Flowers in Chania">
```

If a browser cannot find an image, it will display the value of the alt attribute:

```HTML
<img src="wrongname.gif" alt="Flowers in Chania">
```

### Image Size - Width and Height

Use CSS or the `style` attribute to specify the width and height of an image.

```HTML
<img src="img_girl.jpg" alt="Girl in a jacket" style="width:500px;height:600px;">
```

There is also an option to use `width` and `height` as attributes (values are always in pixels):

```HTML
<img src="img_girl.jpg" alt="Girl in a jacket" width=500 height=600>
```

### Images in Another Folder

If the images are in another folder, you need to specify the path in the `src` attribute:

```HTML
<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
```

### Images on Another Server/Website

If the images are on another server, you need to specify the full URL in the `src` attribute:

```HTML
<img src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com">
```

### Animated Images

HTML allowes GIFs:

```HTML
<img src="programming.gif" alt="Computer Man" style="width:48px;height:48px;">
```

### Image as a Link

Just put the `<img>` tag inside the `<a>` tag:

```HTML
<a href="default.asp">
    <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a>
```

### Image Floating

As for text you can use the CSS `float` property to let the image float at the light or left:

```HTML
<p><img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">
The image will float to the right of the text.</p>

<p><img src="smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">
The image will float to the left of the text.</p>
```

### Common Image Formats

Most common image file types (supported in all browsers (Chrome, Edge, Firefox, Safari, Opera)):

| Abbreviation | File Format                           | File Extension                   |
| ------------ | ------------------------------------- | -------------------------------- |
| APNG         | Animated Portable Network Graphics    | .apng                            |
| GIF          | Graphics Interchange Format           | .gif                             |
| ICO          | Microsoft Icon                        | .ico, .cur                       |
| JPEG         | Joint Photographic Expert Group Image | .jpg, .jpeg, .jfif, .pjpeg, .pjp |
| PNG          | Portable Network Graphics             | .png                             |
| SVG          | Scalable Vector Graphics              | .svg                             |

### HTML Image Tags

| Tag         | Description                                      |
| ----------- | ------------------------------------------------ |
| `<img>`     | Defines an image                                 |
| `<map>`     | Defines an image map                             |
| `<area>`    | Defines a clickable area inside an image map     |
| `<picture>` | Defines a container for multiple image resources |

## Image Maps

The `<map>` tag defines an image map, that´s an image with clickable areas. The areas are defined with one or more `<area>` tags.

Example:

```HTML
<img src="workplace.jpg" alt="Workplace" usemap="#workmap">

<map name="workmap">
    <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">
    <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">
    <area shape="circle" coords="337,300,44" alt="Coffee" href="coffee.htm">
</map>
```

### Why using Image Maps?

The idea is that you can perform different actions when pressing on different parts of the image.

Creating the image map you need an image and HTML code that describes the clickable areas.

### The Image

The image is inserted with the `<img>` tag, the only differents is that it needs `usemap` as an attribute, to link the map and the image together:

```HTML
<img src="workplace.jpg" alt="Workplace" usemap="#workmap">
```

The `usemap` value starts with a `#` followed by the name of the `<map>`.

### Create Image Map

After creating the image with the `usemap` attribute, add a `<map>` element.

It´s used to create an image map and also link the map to the image, using the `name` attribute:

```HTML
<map name="workmap">
```

The `name` attribute must habe the same name as the `usemap` attribute from the `<img>`.

### The Areas

Create/define an clickable area, using an `<area>` element.

You need a shape and define the coordinates of the shape on the image.

Different shapes:

| shape   | description                  |
| ------- | ---------------------------- |
| rect    | defines a rectangular region |
| circle  | defines a circular region    |
| poly    | defines a polygonal region   |
| default | defines the entire region    |

### Shape="rect"

The coordinates come in two pairs, one pair consists of values for the x-axis and y-axis.

For the first corner we have `34,44`, it´s located 34 pixels from the left margin and 44 pixels from the top margin:

![workplace_top_left](/images/workplace_top_left.PNG)

For the second corner we have `270,350`, it´s located 250 pixels from the left margin and 350 pixels from the top margin:

![workplace_bottom_right](/images/workplace_bottom_right.PNG)

Now we have enough data to create a clickable rectangular area:

```HTML
<area shape="rect" coords="34, 44, 270, 350" href="computer.html">
```

That´s the created clickable area, when clicking the user gets to the page "computer.html":

![workplace_rect](/images/workplace_rect.PNG)

### Shape="circle"

The coordinates consist of the center of the circle and the radius.

For the center we have `337,300`, it´s located 337 pixels from the left margin and 300 pixels from the top margin:

![workplace_circle_center](/images/workplace_circle_center.PNG)

For the radius we have `44`:

![workplace_circle_radius](/images/workplace_circle_radius.PNG)

Now we have enough data to create a clickable rectangular area:

```HTML
<area shape="circle" coords="337, 300, 44" href="coffee.htm">
```

That´s the created clickable area, when clicking the user gets to the page "coffee.html":

![workplace_circle](/images/workplace_circle.PNG)

### Shape="poly"

Just like for `shape="rect"` the coordinates come in pairs, but with a lot more pairs, from which you can create any shape you like.

Example a croissant shape:

![croissant](/images/frenchfood.jpg)

Find all the coordinates you like to have in the shape:

![croissant_poly](/images/frenchfood_poly.jpg)

Example:

```HTML
<area shape="poly" coords="140,121,181,116,204,160,204,222,191,270,140,329,85,355,58,352,37,322,40,259,103,161,128,147" href="croissant.htm">
```

That´s the created clickable area:

![croissant_area](/images/frenchfood_area.jpg)

### Image Map and JavaScript

A clickable are can trigger a JavaScript function.

Add a `onclick` event in the `<area>` element to execute a JavaScript function:

```HTML
<map name="workmap">
    <area shape="circle" coords="337,300,44" href="coffee.html" onclick="myFunction()">
</map>

<script>
function myFunction() {
    alert("You clicked the coffee cup!");
}
</script>
```

## Background Images

A background image can be specified for almost any HTML element.

### Background Image on a HTML element

Use the `style` attribute and the CSS `background-image` property to add a background image:

```HTML
<p style="background-image: url('img_girl.jpg');">
```

### Background Image on a Page

To get a full background on the whole page, add the property to the `<body>` element:

```HTML
<style>
    body {
        background-image: url('img_girl.jpg');
    }
</style>
```

### Background Repeat

While the image is smaller then the background, the image repeats itself vertically and horizontally, until the whole background is full.

Example:

```HTML
<style>
    body {
        background-image: url('img_girl.jpg');
    }
</style>
```

To avoid the image to repeat in the background, use the `background-repeat` property with `no-repeat`:

```HTML
<style>
    body {
        background-image: url('img_girl.jpg');
        background-repeat: no-repeat;
    }
</style>
```

### Background Cover

Use the `background-size` property with `cover`, to cover the entire background of the element.

To make sure that the entire element is always covered, set the `background-attachment` property to `fixed`.

Like this the image won´t stretch and cover the entire element:

```HTML
<style>
    body {
        background-image: url('img_girl.jpg');
        background-repeat: no-repeat;
        background-attachment: fixed;
        background-size: cover;
    }
</style>
```

### Background Stretch

Use the `background-size` property with `100% 100%` to stretch the image to fit the entire element:

```HTML
<style>
    body {
        background-image: url('img_girl.jpg');
        background-repeat: no-repeat;
        background-attachment: fixed;
        background-size: 100% 100%;
    }
</style>
```

## Picture Element

The `<picture>` element allows you to display different pictures for different devices or screen sizes.

The `<picture>` element has one or more `<source>` elements, each reffers to different images through the `srcset` attribute and has a `media` attribute that defines when which image will show up.

Example:

```HTML
<picture>
    <source media="(min-width: 650px)" srcset="img_food.jpg">
    <source media="(min-width: 465px)" srcset="img_car.jpg">
    <img src="img_girl.jpg">
</picture>
```

### When to use the Picture Element

There are two main purposes for the `<picture>` element:

#### 1. Bandwidth

If you have a small screen or device, it is not necessary to load a large image file. The browser will use the first `<source>` element with matching attribute values, and ignore any of the following elements.

#### 2. Format Support

Some browsers or devices may not support all image formats. By using the `<picture>` element, you can add images of all formats, and the browser will use the first format it recognizes, and ignore any of the following elements.

Example:

```HTML
<picture>
    <source srcset="img_avatar.png">
    <source srcset="img_girl.jpg">
    <img src="img_beatles.gif" alt="Beatles" style="width:auto;">
</picture>
```

## Favicon

A favicon is a small picture to the left of the page title in the browser tab.

Any image can be used. Create your own favicon on sites like this: [https://www.favicon.cc/](https://www.favicon.cc/).

### How To Add a Favicon in HTML

Safe the image you like, like other images, the common name for a favicon file is "favicon.ico".

Next, add a `<link>` element to your "index.html" file, after the `<title>` element, like this:

```HTML
<!DOCTYPE html>
<html>
<head>
    <title>My Page Title</title>
    <link rel="icon" type="image/x-icon" href="/images/favicon.ico">
</head>
<body>

<h1>This is a Heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

### Favicon File Format Support

| Browser | ICO | PNG | GIF | JPEG | SVG |
| ------- | --- | --- | --- | ---- | --- |
| Edge    | Yes | Yes | Yes | Yes  | Yes |
| Chrome  | Yes | Yes | Yes | Yes  | Yes |
| Firefox | Yes | Yes | Yes | Yes  | Yes |
| Opera   | Yes | Yes | Yes | Yes  | Yes |
| Safari  | Yes | Yes | Yes | Yes  | Yes |

## Page Title

Every web page should have a page title to describe the content and the meaning of the page.

The title is seen in the browser tab.

The `<title>` element adds a title to your page:

```HTML
<!DOCTYPE html>
<html>
<head>
    <title>Testing HTML and CSS</title>
</head>
<body>

<h1>This is a Heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

The `<title>` element:

- defines a title in the browser toolbar
- provides a title for the page when it is added to favorites
- **most importantly** displays a title for the page in search engine-results

So the most important part is to make the title as accurate and meaningful, for search engine optimization (SEO).

## Tables

### Dafine an HTML Table

A table consists of table cells inside rows and columns:

```HTML
<table>
    <tr>
        <th>Company</th>
        <th>Contact</th>
        <th>Country</th>
    </tr>
    <tr>
        <td>Alfreds Futterkiste</td>
        <td>Maria Anders</td>
        <td>Germany</td>
    </tr>
    <tr>
        <td>Centro comercial Moctezuma</td>
        <td>Francisco Chang</td>
        <td>Mexico</td>
    </tr>
</table>
```

### Cells

Each table cell is defined by a `<td>` and a `</td>` tag, everything between them is the content of the cell.

=> `td` = table data

### Rows

Each table row starts with a `<tr>` and ends with a `</tr>` tag.

A table can have as many table rows as possible, but the number of cells should be the same in each row.

=> `tr` = table row

### Headers

Sometimes you need your cells to be header cells, those are headers for the columns. Just use the `<th>` tag instead of the `<td>` tag.

=> `th` = table header

### Tags

| Tag          | Definition                                                                |
| ------------ | ------------------------------------------------------------------------- |
| `<table>`    | Defines a table                                                           |
| `<th>`       | Defines a header cell in a table                                          |
| `<tr>`       | Defines a row in a table                                                  |
| `<td>`       | Defines a cell in a table                                                 |
| `<caption>`  | Defines a table caption                                                   |
| `<colgroup>` | Specifies a group of one or more columns in a table for formatting        |
| `<col>`      | Specifies column properties for each column within a `<colgroup>` element |
| `<thead>`    | Groups the header content in a table                                      |
| `<tbody>`    | Groups the body content in a table                                        |
| `<tfoot>`    | Groups the footer content in a table                                      |

## Table Borders

Tables can have different styles and shapes.

### How To Add a Border

Use the Css `border` property on `table`, `th` and `td` elements:

```CSS
table, th, td {
    border: 1px solid black;
}
```

### Collapsed Table Borders

To avoid double borders, set the CSS `border-collapse` property to `collapse`:

```CSS
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}
```

### Style Table Borders

Create an impression of an invisible border, give the cells a background and set the border color to the document color:

```CSS
table, th, td {
    border: 1px solid white;
    border-collapse: collapse;
}
th, td {
    background-color: #96D4D4;
}
```

### Round Table Borders

Use the `border-radius` property to get rounded borders:

```CSS
table, th, td {
    border: 1px solid black;
    border-radius: 10px;
}
```

=> leave out the `table` of the CSS selector, to only have the rounded cells:

```CSS
th, td {
    border: 1px solid black;
    border-radius: 10px;
}
```

### Dotted Table Borders

Set the appearence of the border with the `border-style` property:

```CSS
th, td {
    border-style: dotted;
}
```

Allowed values:

| Value    | Example                                                                                                                          |
| -------- | -------------------------------------------------------------------------------------------------------------------------------- |
| `dotted` | <div style="text-align:center;"><span style="xborder:2px solid black;border-style:dotted;">&nbsp;&nbsp;&nbsp;&nbsp;</span></div> |
| `dashed` | <div style="text-align:center;"><span style="xborder:2px solid black;border-style:dashed">&nbsp;&nbsp;&nbsp;&nbsp;</span></div>  |
| `solid`  | <div style="text-align:center;"><span style="xborder:2px solid black;border-style:solid">&nbsp;&nbsp;&nbsp;&nbsp;</span></div>   |
| `double` | <div style="text-align:center;"><span style="xborder:2px solid black;border-style:double">&nbsp;&nbsp;&nbsp;&nbsp;</span></div>  |
| `groove` | <div style="text-align:center;"><span style="xborder:2px solid black;border-style:groove">&nbsp;&nbsp;&nbsp;&nbsp;</span></div>  |
| `ridge`  | <div style="text-align:center;"><span style="xborder:2px solid black;border-style:ridge">&nbsp;&nbsp;&nbsp;&nbsp;</span></div>   |
| `inset`  | <div style="text-align:center;"><span style="xborder:2px solid black;border-style:inset">&nbsp;&nbsp;&nbsp;&nbsp;</span></div>   |
| `outset` | <div style="text-align:center;"><span style="xborder:2px solid black;border-style:outset">&nbsp;&nbsp;&nbsp;&nbsp;</span></div>  |
| `none`   | <div style="text-align:center;"><span style="xborder:2px solid black;border-style:none">&nbsp;&nbsp;&nbsp;&nbsp;</span></div>    |
| `hidden` | <div style="text-align:center;"><span style="xborder:2px solid black;border-style:hidden">&nbsp;&nbsp;&nbsp;&nbsp;</span></div>  |

### Border Color

Use the `border-color` property to set the color of the border:

```CSS
th, td {
    border-color: #96D4D4;
}
```

## Table Sizes

The entire table, each column and row can have different sizes.

Using the `style` attribute, with the `height` and `width` properties.

### Table Width and Height

For the whole table width, use `style` to the `<table>` element:

```HTML
<table style="width:100% height:200px">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th>
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
</table> 
```

### Table Column Width

Use `style` to an `<th>` or `<td>` element:

```HTML
<table style="width:100% height:200px">
    <tr>
        <th style="width:20%">Firstname</th>
        <th>Lastname</th>
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
</table> 
```

### Table Row Height

Use `style` to an `<tr>` element:

```HTML
<table style="width:100% height:200px">
    <tr>
        <th>Firstname</th>
        <th>Lastname</th>
        <th>Age</th>
    </tr>
    <tr style="height:200px">
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
</table> 
```

## Table Headers

Tables can have headers for each column, row or multiple columns/rows.

As said before, table headers are defined with `<th>`.

### Horizontal Table Headers

Define all elements of the first row as a `<th>` element:

```HTML
<table>
    <tr>
        <th>Firstname</th>
        <th>Lastname</th>
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
</table> 
```

### Vertical Table Headers

Define the first element of each table row as a `<th>` element:

```HTML
<table>
    <tr>
        <th>Firstname</th>
        <td>Jill</td>
        <td>Eve</td>
    </tr>
    <tr>
        <th>Lastname</th>
        <td>Smith</td>
        <td>Jackson</td>
    </tr>
    <tr>
        <th>Age</th>
        <td>94</td>
        <td>50</td>
    </tr>
</table> 
```

### Align Table Headers

By default the headers are bold and centered.

To align the table headers use the CSS `text-align` property.

For Example to align the header to the left:

```CSS
th {
    text-align: left;
}
```

### Header for Multiple Columns/Rows

Use the `colspan` attribute, for columns and the `rowspan` attribute, for rows, on the `<th>` element:

`colspan`:

```HTML
<table>
    <tr>
        <th colspan="2">Name</th>
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>50</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>94</td>
    </tr>
</table> 
```

`rowspan`:

```HTML
<table>
    <tr>
        <th rowspan="2">Name</th>
        <td>Jill</td>
        <td>Eve</td>
    </tr>
    <tr>
        <td>Smith</td>
        <td>Jackson</td>
    </tr>
    <tr>
        <th>Age</th>
        <td>94</td>
        <td>50</td>
    </tr>
</table> 
```

### Caption

Add a caption, as a heading for a table, by using the `<caption>` tag:

```HTML
<table style="width:100%">
    <caption>Monthly savings</caption>
    <tr>
        <th>Month</th>
        <th>Savings</th>
    </tr>
    <tr>
        <td>January</td>
        <td>$100</td>
    </tr>
        <tr>
        <td>February</td>
        <td>$50</td>
    </tr>
</table> 
```

## Table Padding and Spacing

[go back to REDME.md](/README.md)
