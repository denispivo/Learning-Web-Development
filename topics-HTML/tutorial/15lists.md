# Lists

[go back to Tutorial](00tutorial.md)

- [Beginning Lists](#beginning-lists)
- [Unordered Lists](#unordered-lists)
- [Ordered Lists](#ordered-lists)
- [Other Lists](#other-lists)

## Beginning Lists

Lists are there to group a set of related items.

Example:

| Unordered List                          | Ordered List                                |
| --------------------------------------- | ------------------------------------------- |
| - Item <br>- Item <br>- Item <br>- Item | 1. Item <br>2. Item <br>3. Item <br>4. Item |

## Unordered Lists

Unordered lists start with the `<ul>` tag and each list item start with the `<li>` tag.

By default the items will get be marked with bullets (small black circle).

Example:

```HTML
<ul>
    <li>Coffee</li>
    <li>Tea</li>
    <li>Milk</li>
</ul>
```

To define the style of the list marker use the `list-style-type` property.

Values:

| Value  | Description                                     |
| ------ | ----------------------------------------------- |
| disc   | Sets the list item marker to a bullet (default) |
| circle | Sets the list item marker to a circle           |
| square | Sets the list item marker to a square           |
| none   | The list items will not be marked               |

Lists can also be nested:

```HTML
<ul>
    <li>Coffee</li>
    <li>Tea
        <ul>
            <li>Black tea</li>
            <li>Green tea</li>
        </ul>
    </li>
    <li>Milk</li>
</ul>
```

### Horizontal List with CSS

Horizontal lists are for example used to create a navigation menu:

```HTML
 <!DOCTYPE html>
<html>
<head>
<style>
ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: #333333;
}

li {
    float: left;
}

li a {
    display: block;
    color: white;
    text-align: center;
    padding: 16px;
    text-decoration: none;
}

li a:hover {
    background-color: #111111;
}
</style>
</head>
<body>

<ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#news">News</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#about">About</a></li>
</ul>

</body>
</html>
```

## Ordered Lists

Ordered lists start with the `<ol>` tag and each list item start with the `<li>` tag.

By default the items will be marked with numbers.

Example:

```HTML
<ol>
    <li>Coffee</li>
    <li>Tea</li>
    <li>Milk</li>
</ol>
```

### Type Attribute

Types:

| Type     | Description                                                  |
| -------- | ------------------------------------------------------------ |
| type="1" | The list items will be numbered with numbers (default)       |
| type="A" | The list items will be numbered with uppercase letters       |
| type="a" | The list items will be numbered with lowercase letters       |
| type="I" | The list items will be numbered with uppercase roman numbers |
| type="i" | The list items will be numbered with lowercase roman numbers |

By default the count of a list starts at 1.

You can change the start count with the `start` attribute:

```HTML
<ol start="50">
    <li>Coffee</li>
    <li>Tea</li>
    <li>Milk</li>
</ol>
```

=> This list will start counting from 50 upwards.

### Nested List

Lists can be nested:

```HTML
<ol>
    <li>Coffee</li>
    <li>Tea
        <ol>
            <li>Black tea</li>
            <li>Green tea</li>
        </ol>
    </li>
    <li>Milk</li>
</ol> 
```

## Description Lists

A list of items with descriptions.

The <dl> tag defines the description list, the <dt> tag defines the term (name), and the <dd> tag describes each term.

Example:

```HTML
<dl>
    <dt>Coffee</dt>
    <dd>- black hot drink</dd>
    <dt>Milk</dt>
    <dd>- white cold drink</dd>
</dl>
```

[go back to Tutorial](00tutorial.md)
