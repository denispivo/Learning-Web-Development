# Tutorial

## All upcoming tags are tested in the test.html file

## Elements

- `<html>` -> Defines the root of an HTML document
- `<body>` -> Defines the document's body
- `<h1>` to `<h6>` -> Defines HTML headings

## Attributes

- All HTML elements can have **attributes**
- The `href` attribute of `<a>` specifies the URL of the page the link goes to
- The `src` attribute of `<img>` specifies the path to the image to be displayed
- The `width` and height attributes of `<img>` provide size information for images
- The `alt` attribute of `<img>` provides an alternate text for an image
- The `style` attribute is used to add styles to an element, such as color, font, size, and more
- The `lang` attribute of the `<html>` tag declares the language of the Web page
- The `title` attribute defines some extra information about an element

## Paragraphs

- `<p>` -> Defines a paragraph
- `<hr>` -> Defines a thematic change in the content
- `<br>` -> Inserts a single line break
- `<pre>` -> Denies a pre-formatted text

## Styles

- Use the `style` attribute for styling HTML elements
- Use `background-color` for background color
- Use `color` for text colors
- Use `font-family` for text fonts
- Use `font-size` for text sizes
- Use `text-align` for text alignment

## Formatting

|element|description|
|---|---|
|`<b>`|-> Defines bold text <br>-> without any extra importance|
|`<strong>`|-> Defines important text <br>-> content is typically in bold|
|`<i>`|-> Defines a part of text in an alternate voice or mood <br>-> content inside is typically displayed in italic <br>=> Tip: The `<i>` tag is often used to indicate a technical term, a phrase from another language, a thought, a ship name, etc.|
|`<em>`|- `<em>` -> Defines emphasized text <br>-> content inside is typically displayed in italic <br>=> Tip: A screen reader will pronounce the words in `<em>` with an emphasis, using verbal stress.|
|   |   |
|   |   |
|   |   |
|   |   |
|   |   |
|   |   |

- `<em>` -> Defines emphasized text <br>-> content inside is typically displayed in italic <br>=> Tip: A screen reader will pronounce the words in `<em>` with an emphasis, using verbal stress.
- `<small>` -> Defines smaller text
- `<mark>` -> Defines marked/highlighted text
- `<del>` -> Defines text, that has been deleted from a document
    <br>-> browsers will usually strike a line through deleted text
- `<ins>` -> Defines text, that has been inserted into a document
    <br>-> browsers will usually underline inserted text
- `<sub>` -> Defines subscripted text
    <br>-> appears half a character below the normal line and is sometimes rendered in a smaller font
    <br>=> Subscript text can be used for chemical formulas, like H<sub>2</sub>O
- `<sup>` -> Defines superscripted text
    <br>-> appears half a character above the normal line and is sometimes rendered in a smaller font
    <br>=> Superscript text can be used for footnotes, like WWW<sup>[1]</sup>

## Quotation and Citation

- `<blockquote>` -> element defines a section that is quoted from another source
- `<q>` -> tag defines a short quotation
- `<abbr>` -> tag defines an abbreviation or an acronym
    <br>-> Marking abbreviations can give useful information to browsers, translation systems and search-engines
    <br>=> Tip: Use the global title attribute to show the description for the abbreviation/acronym when you mouse over the element.
- `<address>` -> tag defines the contact information for the author/owner of a document or an article
    <br> -> The contact information can be an email address, URL, physical address, phone number, social media handle, etc
    <br> -> usually renders in italic, and browsers will always add a line break before and after the `<address>` element
- `<cite>` -> tag defines the title of a creative work
- `<bdo>` -> Bi-Directional Override
    -> this tag is used to override the current text direction