# CSS Class Selector - Mukammal Notes

## Class Selector Kya Hai?
`class=""` attribute wale elements ko target karta hai. CSS mein dot (`.`) se likha jata hai. CSS ka sabse zyada use hone wala selector.

```css
.className {
    property: value;
}
```

---

## Hamari Practice File 1: `01 Class Selector Practice/`

### HTML:
```html
<h2 class="heading-highlight">Primary Heading</h2>
<p class="paragraph-highlight">This paragraph shares the exact same design.</p>
<p class="paragraph-highlight">This is another paragraph styled simultaneously.</p>
```

### CSS (`01 Class Selector.css`):
```css
body { background-color: black; }

.heading-highlight {
    color: white;
    background-color: red;
    padding: 10px;
    border-radius: 5px;
    text-align: center;
}

.paragraph-highlight {
    color: white;
    background-color: red;
    padding: 10px;
    border-radius: 5px;
    text-align: center;
}
```

**Natija:** Dono paragraphs aur heading ek jaisi red styling milti hai.

### Properties:
| Property | Value | Kaam |
|----------|-------|------|
| `background-color` | `red` | Background rang |
| `color` | `white` | Text ka rang |
| `padding` | `10px` | Andar jagah |
| `border-radius` | `5px` | Corners gol |
| `text-align` | `center` | Center mein |

---

## Class Ke Zaroori Rules

### Ek class -> Kai elements
```html
<h1 class="highlight">Heading</h1>
<p class="highlight">Para</p>
<span class="highlight">Span</span>
```

### Ek element -> Kai classes
```html
<button class="btn primary large">Click</button>
```

---

## Class vs ID

| Feature | Class (.) | ID (#) |
|---------|-----------|--------|
| Ek page par | Kai elements | Sirf ek element |
| CSS mein | `.className` | `#idName` |
| Preferred | Styling ke liye | Uniqueness ke liye |
