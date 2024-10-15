# Styles - CSS

[go back to Tutorial](00tutorial.md)

CSS = Cascading Style Sheets

CSS is used to format the layout of multiple web pages all at once.

## Using CSS

CSS can be added to HTML documents in 3 ways:

| Type     | Attribute | Description                                      |
| -------- | --------- | ------------------------------------------------ |
| Inline   | `style`   | Using thins inside HTML elements                 |
| Internal | `<style>` | Using this element in the `<head>` section       |
| External | `<link>`  | Using this element to link to external CSS files |

=> The most common way to use CSS is by writing the styles in an external CSS files.

## Inline CSS

Example:

```HTML
<h1 style="color:blue;">A Blue Heading</h1>

<p style="color:red;">A red paragraph.</p>
```

## Internal CSS

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

## External CSS

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

## CSS Colors, Fonts and Sizes

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

## CSS Border, Padding, Margin

| Property  | Description                                               | HTML Example                                                                                 |
| --------- | --------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `border`  | Defines a border around HTMl elements                     | <code>p { <br> &nbsp; border: 2px solid powderblue; <br> }</code>                            |
| `padding` | Defines a padding (space) between the text and the border | <code>p { <br> &nbsp; border: 2px solid powderblue; <br> &nbsp; padding: 30px; <br> }</code> |
| `margin`  | Defines a margin (space) outside the border               | <code>p { <br> &nbsp; border: 2px solid powderblue; <br> &nbsp; margin: 50px; <br> }</code>  |

## Link to External CSS

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

[go back to Tutorial](00tutorial.md)
