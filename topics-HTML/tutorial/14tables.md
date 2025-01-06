# Tables

[go back to Tutorial](00tutorial.md)

- [Beginning Tables](#beginning-tables)
- [Borders](#borders)
- [Sizes](#sizes)
- [Headers](#headers)
- [Padding and Spacing](#padding-and-spacing)
- [Colspan and Rowspan](#colspan-and-rowspan)
- [Styling](#styling)
- [Colgroup](#colgroup)

## Beginning Tables

### Define an HTML Table

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

## Borders

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

## Sizes

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

## Headers

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

## Padding and Spacing

In tables you can adjust the padding inside cells and the spaces between the cells.

### Cell Padding

It´s the space between the cell edges and the cell content.

The default is 0.

Use the CSS `padding` property:

```CSS
th, td {
    padding: 15px;
}
```

You can also use `padding-top`, `padding-bottom`, `padding-left` and `padding-right`:

```CSS
th, td {
    padding-top: 10px;
    padding-bottom: 20px;
    padding-left: 30px;
    padding-right: 40px;
}
```

### Cell Spacing

That´s the space between each cell.

The default is 2.

Use the CSS `border-spacing` property to change the spacing:

```CSS
table {
    border-spacing: 30px;
}
```

## Colspan and Rowspan

As seen before tables can have cells that span over multiple columns and/or rows.

### Colspan

Use `colspan` to span a cell over multiple columns:

```HTML
<table>
    <tr>
        <th colspan="2">Name</th>
        <th>Age</th>
    </tr>
    <tr>
        <td>Jill</td>
        <td>Smith</td>
        <td>43</td>
    </tr>
    <tr>
        <td>Eve</td>
        <td>Jackson</td>
        <td>57</td>
    </tr>
</table>
```

### Rowspan

Use `rowspan` to span a cell over multiple rows:

```HTML
<table>
    <tr>
        <th>Name</th>
        <td>Jill</td>
    </tr>
    <tr>
        <th rowspan="2">Phone</th>
        <td>555-1234</td>
    </tr>
    <tr>
        <td>555-8745</td>
    </tr>
</table>
```

## Styling

Use CSS to style tables.

### Horizontal Zebra Stripes

Add a background to every second row, to get a zebra stripes effect.

To do this, use the `:n-thchild(even)` selector:

```CSS
tr:nth-child(even) {
    background-color: #D6EEEE;
}
```

### Vertical Zebra Stripes

Add a background to every second column, to get a zebra stripes effect.

To do this, use the `:n-thchild(even)` selector:

```CSS
td:nth-child(even), th:nth-child(even) {
    background-color: #D6EEEE;
}
```

### Combine Vertical and Horizontal Zebra Stripes

Combine both stripe variants and use `rgba()` [color](/topics-HTML/tutorial/08colors.md/#rgb-and-rgba-colors) to specify the transparency of the color:

```CSS
tr:nth-child(even) {
    background-color: rgba(150, 212, 212, 0.4);
}

th:nth-child(even),td:nth-child(even) {
    background-color: rgba(150, 212, 212, 0.4);
}
```

### Horizontal Dividers

Specifying only borders on the bottom of each row will get you a table with horizontal dividers.

Add the `border-bottom` property to all `tr` elements:

```CSS
tr {
    border-bottom: 1px solid #dddddd;
}
```

### Hoverable Table

Use `:hover` selector for any table element to highlight the part.

Example:
```CSS
tr:hover {
    background-color: #8b8b8b;
}
```

## Colgroup

Colgroup is there for styling the first columns of a table, using `<colgroup>`, `<col>` and `span` as a style attribute for `<col>`.

Example:

```HTML
<table>
  <colgroup>
    <col span="2" style="background-color: #D6EEEE">
  </colgroup>
  <tr>
    <th>MON</th>
    <th>TUE</th>
    <th>WED</th>
    <th>THU</th>
... 
```

### CSS Properties

`width`, `visibility`, `background` and `border` properties can be used with colgroups, all other will have no effect on the table.

### Multiple Col Elements

```HTML
<colgroup>
    <col span="2" style="background-color: #D6EEEE">
    <col span="3" style="background-color: pink">
</colgroup>
```

### Empty Colgroups

```HTML
<colgroup>
    <col span="2">
    <col span="3" style="background-color: pink">
</colgroup>
```

### Hide Columns

```HTML
<colgroup>
    <col span="2">
    <col span="3" style="visibility: collapse">
</colgroup>
```

[go back to Tutorial](00tutorial.md)
