# Images

[go back to Tutorial](00tutorial.md)

## Beginning Images

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

[go back to Tutorial](00tutorial.md)
