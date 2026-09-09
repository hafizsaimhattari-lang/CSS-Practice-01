# CSS Vertical Align Property

## `vertical-align` kya hoti hai?

`vertical-align` CSS property inline content aur table cells ki vertical position control karti hai.

Simple alfaaz me:

Ye property image, span, checkbox, radio button, ya table cell ko text line ke mutabiq upar, middle, neeche, baseline, subscript, ya superscript position par align karne ke liye use hoti hai.

## Important baat

`vertical-align` normal block elements par expected tarah se kaam nahi karti.

Ye zyada useful hoti hai:

- inline elements
- inline-block elements
- images
- form controls
- table cells

## Basic syntax

```css
selector {
  vertical-align: value;
}
```

Example:

```css
img {
  vertical-align: middle;
}
```

Iska matlab:

Image surrounding text ke sath middle me align hogi.

## Practice files

```text
01 Vertical-Align.html
01 Vertical-Align.css
02 Major Practice.html
02 Major Practice.css
CSS-Vertical-Align-Notes.md
```

## Common values

| Value | Kaam |
| --- | --- |
| `baseline` | Default baseline par align |
| `top` | Line/table cell ke top par align |
| `middle` | Middle par align |
| `bottom` | Bottom par align |
| `text-top` | Text ke top ke according align |
| `text-bottom` | Text ke bottom ke according align |
| `sub` | Subscript jaisa neeche |
| `super` | Superscript jaisa upar |
| `10px` | Baseline se 10px upar |
| `-10px` | Baseline se 10px neeche |
| `20%` | Percentage ke mutabiq adjust |

## Table cells example

```css
.td-02 {
  vertical-align: middle;
}

.td-2 {
  vertical-align: bottom;
}
```

Table cells me `vertical-align` bohat clearly kaam karti hai.

## Image with text example

```css
img {
  vertical-align: middle;
}
```

Ye image ko text ke sath behtar line me align karta hai.

## Checkbox aur radio example

```css
input {
  vertical-align: middle;
}
```

Forms me checkbox/radio aur label ko same line me clean dikhane ke liye useful hai.

## Major practice ka purpose

`02 Major Practice.html` aur `02 Major Practice.css` me text alignment aur vertical alignment ko ek combined practice page me use kiya gaya hai.

Is major practice me:

- `text-align` values repeat hoti hain
- `text-align-last` values repeat hoti hain
- `vertical-align` values image icons ke sath compare hoti hain

## `vertical-align` aur `text-align` me farq

| Property | Kaam |
| --- | --- |
| `text-align` | Text ko horizontally left/right/center karta hai |
| `vertical-align` | Inline/table content ko vertically align karta hai |

## Common mistakes

- `vertical-align` ko normal `div` block par use karna aur result expect karna.
- Is property ko Flexbox vertical centering samajhna.
- `middle` aur `center` confuse karna; `vertical-align` me `center` value nahi hoti.
- Image aur text ke alignment issue me property target galat element par lagana.

## Short summary

`vertical-align` inline content aur table cells ki vertical position adjust karne ke liye use hoti hai.

Most common practical use:

- image + text alignment
- checkbox/radio + label alignment
- table cell content alignment
