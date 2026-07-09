# CSS - Part 1 (A) Mukammal Jaiza

## Yeh Part Kyun Seekha?

CSS ka full form Cascading Style Sheets hai.

CSS se hum HTML page ko style dete hain.

HTML structure banata hai, CSS us structure ko design deti hai.

Is Part me CSS ki bunyad rakhi gayi hai:

- CSS basic syntax
- CSS likhne ke tareeqay
- Basic selectors
- Combinators
- Pseudo classes
- Basic practice

## Folder Structure

```text
Part 1 (A)/
|-- 00 CSS Basic intro/
|-- 01 Types of CSS/
|-- 02 Basic Selectors/
|-- 03 Basic Practice/
|-- CSS-Part1-Overview.md
```

## 00 CSS Basic Intro

Is folder me CSS ka basic concept samjhaya gaya hai.

Important points:

- CSS kya hoti hai
- CSS ka kaam kya hai
- Selector, property, aur value kya hotay hain
- Basic CSS rule ka structure

Example:

```css
h1 {
  color: red;
}
```

Yahan:

- `h1` selector hai
- `color` property hai
- `red` value hai

## 01 Types of CSS

CSS likhne ke 3 basic tareeqay:

| Type | CSS kahan likhte hain? | Use |
| --- | --- | --- |
| Inline CSS | HTML tag ke `style` attribute me | Quick testing |
| Internal CSS | HTML file ke `<style>` tag me | Small pages |
| External CSS | Alag `.css` file me | Professional work |

Best practice:

External CSS zyada clean aur maintainable hoti hai.

## 02 Basic Selectors

Selectors se hum HTML elements ko target karte hain.

Part 1 me ye selectors cover hue:

| Selector | Example | Kaam |
| --- | --- | --- |
| Element selector | `p` | Tag name se select |
| Class selector | `.box` | Class name se select |
| ID selector | `#main` | Unique ID se select |
| Universal selector | `*` | Sab elements select |
| Grouping selector | `h1, p` | Multiple selectors ek sath |
| Descendant selector | `div p` | Parent ke andar element |
| Child combinator | `section > p` | Direct child |
| Next sibling | `h1 + p` | Foran agla sibling |
| Subsequent sibling | `h1 ~ p` | Baad ke matching siblings |
| Pseudo class | `button:hover` | Element ki state |

## 03 Basic Practice

Is folder me Part 1 ke concepts ko combined practice ke form me repeat kiya gaya hai.

Practice 01 me:

- Element selector
- Class selector
- ID selector
- Grouping selector
- Hover
- Selection styling
- External CSS link

use kiye gaye hain.

## Basic CSS Rule Ko Kaise Parhein?

```css
.card > p:hover {
  color: blue;
}
```

Is rule ko yun parhein:

- `.card` class wala parent
- `>` direct child relation
- `p` paragraph element
- `:hover` mouse wali state
- `color` CSS property
- `blue` property value

## Zaroori Yaad Rakhne Wali Batein

- External CSS professional projects me best hoti hai.
- Class selector reusable hota hai.
- ID selector unique hota hai.
- Universal selector sab elements ko target karta hai.
- Combinators HTML relationship ko target karte hain.
- Pseudo classes element ki state ko target karti hain.
- CSS me semicolon aur braces ka khayal rakhna zaroori hai.

## Part 1 Ka Result

Part 1 ke baad student ko CSS basics clear hone chahiye:

- CSS file link karna
- Selectors likhna
- Basic styling apply karna
- Hover/focus/active states samajhna
- Parent-child aur sibling relations samajhna

## Agla Qadam

Part 1 ke baad Part 2 me CSS properties ko detail me practice kiya jayega.

Examples:

- Color
- Background color
- Font properties
- Text properties
- Box model
- Border
- Margin
- Padding

## Status

Part 1 complete hai, aur ab Basic Practice folder se revision bhi start ho gayi hai.
