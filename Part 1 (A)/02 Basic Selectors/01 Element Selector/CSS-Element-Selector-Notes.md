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
- HTML ke standard tag names lowercase likhna best practice hai

---

## Multiple Element Selectors

```css
h1 { font-size: 32px; }
h2 { font-size: 24px; }
p  { line-height: 1.6; }
```

Har rule apne matching tag ko target karta hai. Agar same declarations chahiye hon to grouping use karein:

```css
h1, h2, p { font-family: Arial, sans-serif; }
```

---

## Specificity

Element selector ki specificity class aur ID se kam hoti hai.

```css
p { color: blue; }
.warning { color: red; }
```

`<p class="warning">` par class rule jeetega aur text red hoga.

---

## Kab Avoid Karein?
Jab sirf kuch khaas elements style karne hon:
```css
/* Bura - sare p red ho jayenge */
p { color: red; }

/* Behtar - sirf error class wale */
.error { color: red; }
```

---

## Common Mistakes Aur Summary

- `p.` ya `#p` element selector nahi hain.
- Broad element rule component ke har matching tag par asar kar sakta hai.
- Element selector basic/default styling ke liye acha hai; specific variants ke liye class use karein.
