# Links

[go back to Tutorial](00tutorial.md)

- [Beginning Links](#beginning-links)
- [Link Colors](#link-colors)
- [Create Bookmarks](#create-bookmarks)

## Beginning Links

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

## Link Colors

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

## Create Bookmarks

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

[go back to Tutorial](00tutorial.md)
