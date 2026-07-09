# CSS Color Property

## `color` property kya hoti hai?

CSS me `color` property text ka color change karti hai.

Simple line:

`color` text ka rang change karti hai.

## Basic syntax

```css
selector {
  color: value;
}
```

Example:

```css
h1 {
  color: red;
}
```

Iska matlab:

`h1` ka text red ho jayega.

## Files

```text
01 Color.html
01 Color.css
02 color practice.html
CSS-Color-Property-Notes.md
```

## External CSS example

HTML:

```html
<h1>Color Property Test</h1>
<p>This is a simple paragraph.</p>
```

CSS:

```css
h1 {
  color: white;
}

p {
  color: white;
}
```

Yahan heading aur paragraph dono ka text white hai.

## Internal CSS practice

`02 color practice.html` me internal CSS use ki gayi hai.

Is file me:

- `h1` white color ka hai
- `h2` yellow color ka hai
- normal `p` lightgreen color ka hai
- `.red-text` red color ka hai
- `.blue-text` blue color ka hai
- `#orange-text` orange color ka hai

## Color values ke types

CSS me color value different tareeqon se likh sakte hain.

### Named color

```css
p {
  color: red;
}
```

### RGB color

```css
p {
  color: rgb(255, 0, 0);
}
```

### HEX color

```css
p {
  color: #ff0000;
}
```

## `color` aur `background-color` me farq

```css
p {
  color: white;
  background-color: black;
}
```

Yahan:

- `color` text ko white banati hai
- `background-color` background ko black banati hai

## Common mistakes

- `colour` likhna; CSS me correct spelling `color` hai.
- Semicolon `;` miss karna.
- Text aur background dono same color rakh dena.
- CSS file link karna bhool jana.

## Short summary

`color` property text color change karne ke liye use hoti hai.

Ye CSS ki sabse basic aur important properties me se ek hai.
