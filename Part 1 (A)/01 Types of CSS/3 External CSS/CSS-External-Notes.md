# CSS External CSS - Mukammal Notes (Professional Tareeqa)

## External CSS Kya Hai?
Ek bilkul alag `.css` file mein saari CSS likhi jati hai. HTML file mein `<link>` tag se connect kiya jata hai. Yeh CSS ka sabse professional tareeqa hai.

---

## Hamari Practice Files

### HTML: `01 External CSS.html`
```html
<head>
    <link rel="stylesheet" href="02 style.css">
</head>
<body>
    <h1>Yeh External CSS Hai! (Professional Way)</h1>
    <p>HTML bilkul saaf hai, aur saara design doosri file se aa raha hai!</p>
</body>
```

### CSS: `02 style.css`
```css
/* Yeh alag CSS file hai */
body {
    background-color: #222222;  /* Dark Theme */
}

h1 {
    color: white;
    text-align: center;
    border: 2px solid white;
    padding: 10px;
}

p {
    color: white;
    text-align: center;
    font-size: 24px;
}
```

### Use Hone Wali Properties:
| Property | Value | Kaam |
|----------|-------|------|
| `background-color` | `#222222` | Body ka dark background |
| `color` | `white` | Text safeed |
| `text-align` | `center` | Text center mein |
| `border` | `2px solid white` | H1 ke gird border |
| `padding` | `10px` | Andar se jagah |
| `font-size` | `24px` | Paragraph ka size |

---

## `<link>` Tag Ke Attributes
```html
<link rel="stylesheet" href="02 style.css">
```
| Attribute | Matlab |
|-----------|--------|
| `rel="stylesheet"` | Batata hai ke yeh CSS file hai |
| `href="..."` | CSS file ka raasta (path) |

---

## Fayde
- Ek CSS file - kai sari HTML files par apply
- HTML aur CSS alag, saaf aur reusable
- Professional aur real-world standard
- Browser caching se performance behtar

## Nuqsan
- Ek extra file manage karni padti hai (koi bari baat nahi)
