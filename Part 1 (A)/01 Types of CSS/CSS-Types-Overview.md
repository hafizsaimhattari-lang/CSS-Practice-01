# 🎨 CSS ke Teen Qisam - Mukammal Overview

## 📚 Parichay
CSS likhne ke teen tareeqay hain. Har tareeqay ke apne fawaid aur nuqsanat hain. Yeh folder inhe alag alag practice karta hai.

---

## 🗂️ Folder Structure

```
01 Types of CSS/
├── 1 inline CSS/       → Inline CSS practice
├── 2 Internal CSS/     → Internal/Embedded CSS
├── 3 External CSS/     → External CSS (Professional ✅)
└── CSS-Types-Overview.md
```

---

## ⚖️ Teeno Ka Muqabla

| Feature | Inline CSS | Internal CSS | External CSS |
|---------|-----------|--------------|--------------|
| Jagah | HTML tag ke andar | `<head>` mein `<style>` | Alag `.css` file |
| Scope | Sirf ek tag | Sirf ek HTML file | Kai HTML files |
| Maintainability | ❌ Mushkil | ⚠️ Theek | ✅ Asaan |
| Professional | ❌ Nahi | ⚠️ Chote projects | ✅ Haan |
| Code Cleanliness | ❌ Ganda | ⚠️ Medium | ✅ Saaf |

---

## 1️⃣ Inline CSS (Practice file: `01 Inline CSS.html`)

```html
<h1 style="color: blue; text-align: center; background-color: yellow;">
    Yeh Inline CSS Hai!
</h1>
<p style="color: green; font-weight: bold;">
    Isme har line ko alag se design dena parta hai!
</p>
```
❌ **Avoid karo** — har element ko alag likhna padta hai.

---

## 2️⃣ Internal CSS (Practice file: `01 internal CSS.html`)

```html
<head>
    <style>
        h1 {
            color: green;
            text-align: center;
            background-color: lightgray;
        }
        p {
            color: purple;
            font-size: 20px;
        }
    </style>
</head>
```
⚠️ **Chote projects ke liye theek** — sirf ek file mein kaam karta hai.

---

## 3️⃣ External CSS ✅ (Practice file: `01 External CSS.html` + `02 style.css`)

**HTML:**
```html
<head>
    <link rel="stylesheet" href="02 style.css">
</head>
```

**CSS file (`02 style.css`):**
```css
body { background-color: #222222; }

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
✅ **Yahi tareeqa use karo** — HTML aur CSS bilkul alag, saaf aur reusable.

---

## 📝 Akhiri Baat
Real-world mein hamesha **External CSS** use karo. Inline aur Internal sirf debugging ya quick testing ke liye.
