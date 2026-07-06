# CSS Element Selector - Mukammal Notes

## Element Selector Kya Hai?
HTML ke tag ke naam se seedha element ko target karta hai. CSS ka sabse simple aur seedha selector.

```css
tagNaam {
    property: value;
}
```

---

## Hamari Practice File: `01 Element Selector.html`

```css
/* body tag ko target kiya */
body {
    background-color: black;
}

/* h1 tag ko directly select kiya */
h1 {
    color: white;
}
```

```html
<body>
    <h1>This is my First paragraph</h1>
</body>
```

**Natija:** Poora page kala, heading safeed.

### Properties:
| Property | Value | Element | Kaam |
|----------|-------|---------|------|
| `background-color` | `black` | `body` | Page ka background kala |
| `color` | `white` | `h1` | Heading safeed |

---

## Element Selector Ke Rules
- Koi `.` ya `#` nahi — sirf tag ka naam
- Page ke SARE matching tags par apply hota hai
- `p { color: red }` se page ke har `<p>` red hoga

---

## Kab Avoid Karein?
Jab sirf kuch khaas elements style karne hon:
```css
/* Bura - sare p red ho jayenge */
p { color: red; }

/* Behtar - sirf error class wale */
.error { color: red; }
```
