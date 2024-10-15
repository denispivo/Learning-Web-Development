# Favicon

[go back to Tutorial](00tutorial.md)

A favicon is a small picture to the left of the page title in the browser tab.

Any image can be used. Create your own favicon on sites like this: [https://www.favicon.cc/](https://www.favicon.cc/).

## How To Add a Favicon in HTML

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

## Favicon File Format Support

| Browser | ICO | PNG | GIF | JPEG | SVG |
| ------- | --- | --- | --- | ---- | --- |
| Edge    | Yes | Yes | Yes | Yes  | Yes |
| Chrome  | Yes | Yes | Yes | Yes  | Yes |
| Firefox | Yes | Yes | Yes | Yes  | Yes |
| Opera   | Yes | Yes | Yes | Yes  | Yes |
| Safari  | Yes | Yes | Yes | Yes  | Yes |

[go back to Tutorial](00tutorial.md)
