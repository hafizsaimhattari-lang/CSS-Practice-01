# CSS Basic Practice 1

## Practice ka maqsad

Is practice ka maqsad Part 1 ke basic CSS concepts ko ek hi file pair me repeat karna hai.

Is example me ye cheezen practice ho rahi hain:

- Element selector
- ID selector
- Class selector
- Grouping selector
- Hover pseudo class
- `::selection` pseudo element
- External CSS linking

## Files

```text
01.html
01.css
```

## HTML file ka kaam

`01.html` me different HTML elements rakhe gaye hain:

- `h1`
- `div`
- `ul`
- `li`
- `p`
- `h2`
- `h3`
- `h4`
- `h5`

In elements par CSS selectors apply kiye gaye hain.

## CSS file ka kaam

`01.css` me different selectors use kiye gaye hain.

Example:

```css
h1 {
  background-color: black;
  color: white;
}
```

Yahan `h1` element selector hai.

## ID selector example

```css
#div-lists {
  background-color: darkred;
  color: white;
}
```

`#div-lists` sirf us element ko target karta hai jiski ID `div-lists` hai.

## Class selector example

```css
.hello-hi-para {
  font-size: larger;
}
```

`.hello-hi-para` class selector hai.

Class selector reusable hota hai.

## Grouping selector example

```css
h4,
h5 {
  background-color: yellow;
  padding: 5px;
}
```

Yahan `h4` aur `h5` dono ko same style mil rahi hai.

## Hover example

```css
#hal-chal-2:hover {
  color: red;
}
```

Jab user first `h3` par mouse le kar jayega, uska color red ho jayega.

## Selection example

```css
h1::selection {
  background-color: white;
  color: black;
}
```

Jab user `h1` ka text select karega, selected text ka background white aur color black ho jayega.

## Browser me result

Page open karne par:

- Main heading black background aur white text me show hoti hai.
- List box dark red background ke sath show hota hai.
- List box hover par black ho jata hai.
- Paragraphs aur headings different colors me show hotay hain.
- Text select karne par `::selection` styles apply hoti hain.

## Common mistakes

- CSS file ka link galat dena.
- ID selector me `#` bhool jana.
- Class selector me `.` bhool jana.
- Semicolon `;` miss kar dena.
- Hover test karte waqt mouse element par na le jana.

## Short summary

Ye practice Part 1 ke basic selectors aur pseudo concepts ka combined revision hai.

Is file ko baar baar edit karke colors, padding, hover, aur selection styles practice karo.
