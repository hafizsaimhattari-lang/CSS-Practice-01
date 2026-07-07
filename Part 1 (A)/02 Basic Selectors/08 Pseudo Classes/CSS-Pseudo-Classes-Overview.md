# CSS Pseudo Classes - Mukammal Overview

## Pseudo Class Kya Hai?

Pseudo class CSS selector ka special part hota hai jo kisi element ki khaas state ya condition par style apply karta hai.

Simple alfaaz me:

Jab user kisi element ke sath interact karta hai, ya element kisi special halat me hota hai, to pseudo class us state ko target karti hai.

Basic syntax:

```css
selector:pseudo-class {
  property: value;
}
```

Example:

```css
button:hover {
  background-color: yellow;
}
```

Iska matlab:

Jab mouse button ke upar aayega, button ka background yellow ho jayega.

## Folder Structure

```text
08 Pseudo Classes/
|-- 01 hover Pseudo Class/     :hover  - mouse element ke upar ho
|-- 02 Active Pseudo Class/    :active - element press/click ho raha ho
|-- 03 Focus Pseudo Class/     :focus  - element selected/focused ho
```

## Is Folder Me Covered Pseudo Classes

| Pseudo Class | Kab Apply Hoti Hai? | Example |
| --- | --- | --- |
| `:hover` | Jab mouse element ke upar ho | Button par mouse le jana |
| `:active` | Jab element press ho raha ho | Button click hold karna |
| `:focus` | Jab element selected/focused ho | Input field par click ya Tab |

## Common Pseudo Classes

| Pseudo Class | Matlab |
| --- | --- |
| `:hover` | Mouse element ke upar ho |
| `:active` | Element click/press ho raha ho |
| `:focus` | Element selected ya focused ho |
| `:focus-visible` | Browser keyboard focus visibly show kare |
| `:visited` | Link pehle visit ho chuki ho |
| `:checked` | Checkbox ya radio selected ho |
| `:disabled` | Form control disabled ho |
| `:first-child` | Parent ka pehla child |
| `:last-child` | Parent ka last child |
| `:nth-child(n)` | Parent ka nth child |

## `:hover` Example

```css
button:hover {
  background-color: black;
  color: white;
}
```

Yahan jab mouse button ke upar aayega, button ka background black aur text white ho jayega.

## `:active` Example

```css
button:active {
  background-color: blue;
  color: white;
}
```

Yahan jab button press ho raha hoga, active style apply hogi.

## `:focus` Example

```css
input:focus {
  border: 3px solid red;
  background-color: lightgray;
}
```

Yahan input field click ya keyboard Tab se focus me aaye to style change hogi.

## User Interaction Pseudo Classes

Ye pseudo classes user ke action ke mutabiq kaam karti hain:

- `:hover` mouse movement ke sath
- `:active` click press ke sath
- `:focus` selected element ke sath

## Form State Pseudo Classes

Form controls ke sath bhi pseudo classes use hoti hain:

```css
input:checked {
  outline: 2px solid green;
}

input:disabled {
  opacity: 0.5;
}
```

## Structure Pseudo Classes

Kuch pseudo classes element ki position ko target karti hain:

```css
li:first-child {
  color: red;
}

li:last-child {
  color: blue;
}

li:nth-child(2) {
  color: green;
}
```

## Pseudo Class Aur Pseudo Element Me Farq

Pseudo class single colon `:` use karti hai.

Example:

```css
a:hover {
  color: red;
}
```

Pseudo element double colon `::` use karta hai.

Example:

```css
p::first-line {
  color: blue;
}
```

Short farq:

- Pseudo class element ki state target karti hai
- Pseudo element element ka specific part target karta hai

## Accessibility Important Point

Sirf `:hover` par important information depend nahi karni chahiye.

Reason:

Mobile users aur keyboard users hover use nahi karte.

Focus style ko visible rakhna bohat zaroori hai.

Example:

```css
button:focus {
  outline: 3px solid yellow;
}
```

## Common Mistakes

### Mistake 1: Space laga dena

Galat:

```css
.button :hover {
  color: red;
}
```

Theek:

```css
.button:hover {
  color: red;
}
```

### Mistake 2: Double colon use karna

Galat:

```css
button::hover {
  color: red;
}
```

Theek:

```css
button:hover {
  color: red;
}
```

### Mistake 3: `:active` ko permanent state samajhna

`:active` sirf press/click ke waqt hoti hai.

Permanent selected state ke liye usually class ya JavaScript use hota hai.

## Short Summary

Pseudo classes element ki state ko target karti hain.

Part 1 me hum ne basic interaction states cover ki hain:

- `:hover`
- `:active`
- `:focus`

Ye teeno user interaction samajhne ke liye bohat important hain.
