# 🎨 01 Types of CSS

## 📚 Is Folder Ka Maqsad
Yeh folder **CSS ke teen qisam** ki practice ke liye hai. Har qism ek alag file mein demonstrate ki gayi hai.

---

## 📁 Folder Structure

```
01 Types of CSS/
├── 1 inline CSS/       (Inline CSS practice)
├── 2 Internal CSS/     (Internal/Embedded CSS practice)
├── 3 External CSS/     (External CSS practice - professional tareeqa)
└── README.md           (Yeh file)
```

---

## 🎯 Teeno Qisam Ka Farq

### 1️⃣ Inline CSS
```html
<h1 style="color: blue;">Hello</h1>
```
- CSS seedha HTML tag ke `style=""` attribute mein likhi jati hai.
- Har ek tag ko alag se style dena parta hai.
- **Nuqsan:** Boht mushkil maintain karna. ❌ Professional use mein avoid karo.

---

### 2️⃣ Internal CSS (Embedded)
```html
<head>
    <style>
        h1 { color: green; }
    </style>
</head>
```
- CSS `<head>` tag ke andar `<style>` block mein likhi jati hai.
- Sirf isi ek HTML file par apply hoti hai.
- **Nuqsan:** Har file ke liye alag CSS likhni padti hai. ⚠️

---

### 3️⃣ External CSS ✅ (Professional Tareeqa)
```html
<link rel="stylesheet" href="style.css">
```
- CSS ka kaam ek alag `.css` file mein hota hai.
- Ek CSS file kai HTML files par apply ho sakti hai.
- **Fayda:** Code saaf, manageable, aur reusable hota hai. ✅

---

## 📝 Summary
Teeno tareeqay seekhna zaroori hai lekin real projects mein hamesha **External CSS** use karo.
