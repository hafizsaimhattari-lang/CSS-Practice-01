# CSS Background Color Property

## `background-color` kya hoti hai?

`background-color` CSS property kisi element ka background color change karti hai.

Simple line:

`background-color` element ke peeche ka color change karti hai.

## Basic syntax

```css
selector {
  background-color: value;
}
```

Example:

```css
body {
  background-color: black;
}
```

Iska matlab:

Page ka background black ho jayega.

## Files

```text
01 Background-color.html
01 Background-color.css
CSS-Background-Color-Notes.md
```

## Practice example

HTML:

```html
<div>
  <h1>Background-color Test</h1>
  <p>Paragraph text</p>
</div>
```

CSS:

```css
body {
  background-color: rgb(0, 74, 74);
}

div {
  background-color: black;
}

p {
  background-color: maroon;
}

h1 {
  background-color: blue;
}
```

## Is practice me kya ho raha hai?

Page me multiple elements ke background colors different hain:

- `body` ka background dark teal hai
- `div` ka background black hai
- `h1` ka background blue hai
- `p` ka background maroon hai

Is se clear hota hai ke har element ka apna background color ho sakta hai.

## `color` aur `background-color` ka relation

Agar background dark ho to text light rakhna chahiye.

Example:

```css
p {
  background-color: black;
  color: white;
}
```

Is se text readable rehta hai.

## Common mistakes

- `background color` space ke sath likhna; correct property `background-color` hai.
- Text aur background same color rakh dena.
- Parent aur child background ka farq confuse karna.
- CSS file ka link galat dena.

## Short summary

`background-color` kisi element ka background color change karti hai.

Readable design ke liye text color aur background color ka contrast clear hona chahiye.
