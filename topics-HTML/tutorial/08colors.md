# Colors

[go back to Tutorial](00tutorial.md)

- [Color Names](#color-names)
- [Background Color](#background-color)
- [Text Color](#text-color)
- [Border Color](#border-color)
- [Color Values](#color-values)
- [RGB and RGBA Colors](#rgb-and-rgba-colors)
- [HEX Colors](#hex-colors)
- [HSL and HSLA Colors](#hsl-and-hsla-colors)

Colors are predefindes with color names, RGB, HEX, HSL, RGBA or HSLA values.

## Color Names

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

## Background Color

You can set the background color for HTML elements with `style="background-color:___"`
Example: `<h1 style="background-color:DodgerBlue;">Hello World</h1>`

## Text Color

You can set the Text color with `style="color:___"`
Example: `<h1 style="color:Tomato;">Hello World</h1>`

## Border Color

You can set the color of borders with `style="border:__ __ __"`
Example: `<h1 style="border:2px solid Tomato;">Hello World</h1>`

## Color Values

In HTML colors can also be specified using RGB, HEX, HSL, RGBA and HSLA values.

| Value Type | Example                                            | HTML Example                                                     |
| ---------- | -------------------------------------------------- | ---------------------------------------------------------------- |
| RGB        | `rbg(255, 99 ,71)`                                 | `<h1 style="background-color:rgb(255, 99, 71);">...</h1>`        |
| HEX        | `#ff6347`                                          | `<h1 style="background-color:#ff6347;">...</h1>`                 |
| HSL        | `hsl(9, 100%, 64%)`                                | `<h1 style="background-color:hsl(9, 100%, 64%);">...</h1>`       |
| RGBA       | `rgba(255, 99 , 71, 0.5)` <br> -> 50% transparency | `<h1 style="background-color:rgba(255, 99, 71, 0.5);">...</h1>`  |
| HSLA       | `hsla(9, 100%, 64%, 0.5)` <br> -> 50% transparency | `<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">...</h1>` |

## RGB and RGBA Colors

RGB = (RED, GREEN, BLUE)

- every value can be between 0 and 255

RGBA = (RED, GREEN, BLUE, {alpha channel})

- the same as RGB, but with an extra alpha value

## HEX Colors

HEX = #rrggbb (#red green blue)

- every hexadecimal value can be between 0 and 15, with {0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F}

## HSL and HSLA Colors

HSL = (hue, saturation, lightness)

- hue is a degree on the color wheel, from 0 to 360 (0 = red; 120 = green; 240 = blue;)
- saturation is a percentage value (0% = shades of gray; 100% = full color;)
- lightness is also a percentage value (0% = black; 100% = white;)

HSLA = (hue, saturation, lightness, alpha)

- the same as HSL, but with an extra alpha value

[go back to Tutorial](00tutorial.md)
