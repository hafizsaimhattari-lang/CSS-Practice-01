# Vertical Align Major Practice

## Is practice ka maqsad

`02 Major Practice.html` ek combined revision page hai.

Is file me 3 related CSS alignment topics ek sath practice hotay hain:

- `text-align`
- `text-align-last`
- `vertical-align`

## Practice files

```text
02 Major Practice.html
02 Major Practice.css
CSS-Vertical-Align-Major-Practice-Notes.md
```

## HTML structure

Page me 3 main sections hain:

1. Text Align Practice
2. Text Align Last Practice
3. Vertical Align Practice

## Text align section

Is section me paragraph text ko different directions me align kiya gaya hai.

Example:

```css
.left-para {
  text-align: left;
}

.center-para {
  text-align: center;
}
```

## Text align last section

Is section me paragraph ki last line ko control kiya gaya hai.

Example:

```css
.text-align-last-center-para {
  text-align-last: center;
}
```

Ye property especially long paragraphs me useful hoti hai.

## Vertical align section

Is section me text ke sath small images/icons use kiye gaye hain.

Har image ko different `vertical-align` value di gayi hai.

Example:

```css
.middle {
  vertical-align: middle;
}

.super {
  vertical-align: super;
}
```

## Important learning

`vertical-align` text ke andar images/icons ko line ke mutabiq adjust karta hai.

Ye normal block element ko page ke center me vertically align karne ke liye use nahi hota.

## Common mistakes

- `vertical-align: center;` likhna. Correct value `middle` hoti hai.
- `vertical-align` ko block `div` par laga kar vertical center expect karna.
- `text-align` aur `vertical-align` ko same samajhna.

## Short summary

Ye major practice alignment properties ka combined revision hai.

Is file ko browser me open karke har section ka result compare karo.
