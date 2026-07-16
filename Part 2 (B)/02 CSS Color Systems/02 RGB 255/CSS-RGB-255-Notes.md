# CSS RGB 255 Colors

## RGB kya hota hai?

RGB ka matlab hai:

```text
Red Green Blue
```

CSS me RGB color likhne ke liye `rgb()` function use hota hai.

## Basic syntax

```css
selector {
  color: rgb(red, green, blue);
}
```

Har value `0` se `255` ke darmiyan hoti hai.

## Examples

```css
p {
  color: rgb(255, 255, 255);
}
```

Ye white color hai.

```css
p {
  color: rgb(0, 0, 0);
}
```

Ye black color hai.

## Practice files

```text
01 RGB 255.html
01 RGB-255.css
CSS-RGB-255-Notes.md
```

## Is practice me kya ho raha hai?

Is practice me page ke different parts ko RGB values se color diya gaya hai:

- `body` ka background `rgb(2, 67, 67)`
- `main` ka background `rgb(72, 6, 134)`
- headings ka background `rgb(60, 2, 2)`
- text ka color `rgb(255, 255, 255)`
- paragraph hover color `rgb(0, 251, 255)`

## RGB value ka idea

```text
rgb(255, 0, 0)     red
rgb(0, 255, 0)     green
rgb(0, 0, 255)     blue
rgb(255, 255, 255) white
rgb(0, 0, 0)       black
```

## Common mistakes

- RGB values ko 255 se zyada likhna.
- Commas miss karna.
- `rgb` ke brackets miss karna.
- Dark background par dark text rakhna.

## Short summary

RGB exact color control deta hai.

Har color red, green, aur blue values ke mix se banta hai.
