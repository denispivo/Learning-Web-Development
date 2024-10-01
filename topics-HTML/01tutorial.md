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
- []()
- []()
- []()
- []()
- []()

## Elements

|Element|Description|
|---|---|
|`<html>`|Defines the root of an HTML document|
|`<body>`|Defines the document's body|
|`<h1>` to `<h6>`|Defines HTML headings|

## Attributes

All HTML elements can have **attributes**

|Element|Attribute|Description|
|---|---|---|
|`<a>`|`href`|Specifies the URL of the page the link goes to|
|`<img>`|`src`|Specifies the path to the image to be displayed|
|`<img>`|`width` and `height`|Provide size information for images|
|`<img>`|`alt`|Provides an alternate text for an image|
|`<html>`|`lang`|Tag declares the language of the Web page|
||`style`|Attribute is used to add styles to an element, such as color, font, size, and more|
||`title`|Attribute defines some extra information about an element|

## Paragraphs

|Element|Description|
|---|---|
|`<p>`|Defines a paragraph|
|`<hr>`|Defines a thematic change in the content|
|`<br>`|Inserts a single line break|
|`<pre>`|Denies a pre-formatted text|

## Styles

|Element|Description|
|---|---|
|`style`|Used for styling HTML elements|
|`background-color`|Used for background color|
|`color`|Used for text color|
|`font-family`|Used for text fonts|
|`font-size`|Used for text sizes|
|`text-align`|Used for text alignment (top/bottom/left/right/center)|

## Formatting

|Element|Description|
|---|---|
|`<b>`|- Defines bold text <br>- without any extra importance|
|`<strong>`|- Defines important text <br>- content is typically in bold|
|`<i>`|- Defines a part of text in an alternate voice or mood <br>- content inside is typically displayed in italic <br>=> Tip: The `<i>` tag is often used to indicate a technical term, a phrase from another language, a thought, a ship name, etc.|
|`<em>`|- Defines emphasized text <br>- content inside is typically displayed in italic <br>=> Tip: A screen reader will pronounce the words in `<em>` with an emphasis, using verbal stress.|
|`<small>`|- Defines smaller text|
|`<mark>`|- Defines marked/highlighted text|
|`<del>`|- Defines text, that has been deleted from a document <br>- browsers will usually strike a line through deleted text|
|`<ins>`|- Defines text, that has been inserted into a document <br>- browsers will usually underline inserted text|
|`<sub>`|- Defines subscripted text <br>- appears half a character below the normal line and is sometimes rendered in a smaller font <br>=> Subscript text can be used for chemical formulas, like H<sub>2</sub>O|
|`<sup>`|- Defines superscripted text <br>- appears half a character above the normal line and is sometimes rendered in a smaller font <br>=> Superscript text can be used for footnotes, like WWW<sup>[1]</sup>|

## Quotation and Citation

|Element|Description|
|---|---|
|`<blockquote>`|- element defines a section that is quoted from another source|
|`<q>`|- tag defines a short quotation|
|`<abbr>`|- tag defines an abbreviation or an acronym <br>- Marking abbreviations can give useful information to browsers, translation systems and search-engines <br>=> Tip: Use the global title attribute to show the description for the abbreviation/acronym when you mouse over the element.|
|`<address>`|- tag defines the contact information for the author/owner of a document or an article <br> - The contact information can be an email address, URL, physical address, phone number, social media handle, etc <br> -> usually renders in italic, and browsers will always add a line break before and after the `<address>` element|
|`<cite>`|- tag defines the title of a creative work|
|`<bdo>`|- Bi-Directional Override <br>- this tag is used to override the current text direction|

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

|Value Type|Example|HTML Example|
|---|---|---|
|RGB|`rbg(255, 99 ,71)`|`<h1 style="background-color:rgb(255, 99, 71);">...</h1>`|
|HEX|`#ff6347`|`<h1 style="background-color:#ff6347;">...</h1>`|
|HSL|`hsl(9, 100%, 64%)`|`<h1 style="background-color:hsl(9, 100%, 64%);">...</h1>`|
|RGBA|`rgba(255, 99 , 71, 0.5)` <br> -> 50% transparency|`<h1 style="background-color:rgba(255, 99, 71, 0.5);">...</h1>`|
|HSLA|`hsla(9, 100%, 64%, 0.5)` <br> -> 50% transparency|`<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">...</h1>`|

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

|Type|Attribute|Description|
|---|---|---|
|Inline|`style`|Using thins inside HTML elements|
|Internal|`<style>`|Using this element in the `<head>` section|
|External|`<link>`|Using this element to link to external CSS files|

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

|Element|Description|
|---|---|
|`color`|Defines the text color|
|`font-family`|Defines the font|
|`font-size`|Defines the text size|

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

|Property|Description|HTML Example|
|---|---|---|
|`border`|Defines a border around HTMl elements|<code>p { <br> &nbsp; border: 2px solid powderblue; <br> }</code>|
|`padding`|Defines a padding (space) between the text and the border|<code>p { <br> &nbsp; border: 2px solid powderblue; <br> &nbsp; padding: 30px; <br> }</code>|
|`margin`|Defines a margin (space) outside the border|<code>p { <br> &nbsp; border: 2px solid powderblue; <br> &nbsp; margin: 50px; <br> }</code>|

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

|Value|Definition|
|---|---|
|`_self`|Default, opens in the same window/tab.|
|`_blank`|Opens in a new window/tab.|
|`_parent`|Opens in the parent frame. Does what is defined in the parent frame.|
|`_top`|Opens in the full body of window. Does what is defined in the top frame.|

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

[go back to REDME.md](/README.md)
