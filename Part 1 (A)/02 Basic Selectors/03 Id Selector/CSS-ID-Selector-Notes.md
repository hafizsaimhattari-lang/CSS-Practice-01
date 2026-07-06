# CSS ID Selector - Mukammal Notes

## ID Selector Kya Hai?
`id=""` attribute wale ek specific element ko target karta hai. CSS mein hash (`#`) se likha jata hai.

```css
#idNaam {
    property: value;
}
```

---

## Hamari Practice File: `01 id Selector.html`

### HTML:
```html
<!-- Unique ID: "special-box" -->
<h1 id="special-box">Hafiz Saim - The Elite Coder</h1>

<!-- Koi ID nahi - style nahi milegi -->
<p>Yeh aam text hai, iska design simple hi rahega.</p>
```

### CSS (`01 Id Selector.css`):
```css
#special-box {
    /* ID selector # se shuru hota hai */
}
```

---

## ID Ki Sabse Zaroori Baat - UNIQUENESS

```html
<!-- GALAT - ek ID do jagah -->
<h1 id="title">Heading 1</h1>
<h2 id="title">Heading 2</h2>

<!-- SAHIH - alag alag IDs -->
<h1 id="main-title">Heading 1</h1>
<h2 id="sub-title">Heading 2</h2>
```

---

## ID vs Class

| Feature | Class (.) | ID (#) |
|---------|-----------|--------|
| Ek page par | Kai elements | Sirf ek element |
| CSS Power | Medium | Zyada |
| Styling ke liye | Preferred | Avoid |
| JS ke liye | querySelectorAll | getElementById |

---

## Professional Advice
- Styling ke liye: Class use karo
- JavaScript targets ke liye: ID use karo
