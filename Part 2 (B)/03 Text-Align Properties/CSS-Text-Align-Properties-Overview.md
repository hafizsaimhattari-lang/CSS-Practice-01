# CSS Text Align Properties Overview

## Text align properties kya hoti hain?

Text align properties text aur inline content ki alignment control karti hain.

Is section me horizontal text alignment ke sath vertical inline/table alignment bhi practice ho rahi hai.

## Is folder me topics

```text
03 Text-Align Properties/
|-- 01 text-align/
|-- 02 Text-Align-Last Property/
|-- 03 Vertical-Align Property/
```

## `text-align` property

`text-align` property text ko left, right, center, start, end, ya justify align karne ke liye use hoti hai.

Example:

```css
h1 {
  text-align: center;
}
```

Iska matlab:

`h1` ka text center me show hoga.

## Common `text-align` values

| Value | Kaam |
| --- | --- |
| `left` | Text left side par |
| `right` | Text right side par |
| `center` | Text center me |
| `justify` | Text dono sides se align |
| `start` | Language direction ke start par |
| `end` | Language direction ke end par |

## `text-align-last` property

`text-align-last` paragraph ki last line ko align karne ke liye use hoti hai.

Example:

```css
p {
  text-align: justify;
  text-align-last: center;
}
```

Yahan paragraph justify hoga, lekin last line center align hogi.

## `vertical-align` property

`vertical-align` inline elements aur table cells ko vertically align karne ke liye use hoti hai.

Example:

```css
img {
  vertical-align: middle;
}
```

Important:

`vertical-align` normal block elements ko vertically center karne ke liye nahi hoti.

## Short summary

Text alignment readable layout banane ke liye important hoti hai.

Is section me `text-align`, `text-align-last`, aur `vertical-align` ki practice included hai.
