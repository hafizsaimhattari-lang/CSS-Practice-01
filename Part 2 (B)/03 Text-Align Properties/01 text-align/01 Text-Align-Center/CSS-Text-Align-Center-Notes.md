# CSS Text Align Center

## `text-align: center;` kya karta hai?

`text-align: center;` kisi element ke andar text ko center me align karta hai.

Example:

```css
h1 {
  text-align: center;
}
```

Iska matlab:

`h1` ka text center me show hoga.

## Practice files

```text
01 text-align-center.html
01 text-align-center.css
CSS-Text-Align-Center-Notes.md
```

## Is practice me kya ho raha hai?

HTML me 5 headings hain:

```html
<h1 class="text-align-class" id="heading-01">Text Align Center 1</h1>
```

CSS me har heading ko ID selector se center align kiya gaya hai:

```css
#heading-01 {
  text-align: center;
}
```

## Class ka role

`.text-align-class` common styling deti hai:

```css
.text-align-class {
  color: white;
  background-color: black;
  border-radius: 10px;
  padding: 10px;
}
```

## Hover practice

```css
.text-align-class:hover {
  color: yellow;
}
```

Mouse heading par lane se text yellow ho jata hai.

## Common mistakes

- `text-align` ko `text align` likhna.
- `center` ki spelling galat likhna.
- Sirf element ko center samajhna; `text-align` text ko center karta hai, pura block element ko nahi.

## Short summary

`text-align: center;` text ko horizontally center karne ke liye use hota hai.

Ye headings, paragraphs, buttons ke text, aur containers ke inline content ke liye useful hai.
