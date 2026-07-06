# 🎨 Internal CSS (Embedded CSS) - Mukammal Notes

## 📚 Internal CSS Kya Hai?
Internal CSS (ise Embedded CSS bhi kehte hain) mein HTML file ke `<head>` section ke andar `<style>` tag banaya jata hai. Saari CSS wahan likhi jati hai.

---

## ✍️ Hamari Practice File: `01 internal CSS.html`

```html
<head>
    <meta charset="UTF-8">
    <title>Internal CSS Test</title>

    <!-- CSS yahan head ke andar style tag mein likhi hai! -->
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
<body>
    <h1>Yeh Internal CSS Hai!</h1>
    <p>HTML aur CSS ek hi file mein hain, lekin code thora saaf hai!</p>
</body>
```

### Is file mein use hone wali properties:
| Property | Value | Element | Kaam |
|----------|-------|---------|------|
| `color` | `green` | `h1` | Heading green |
| `text-align` | `center` | `h1` | Center mein |
| `background-color` | `lightgray` | `h1` | Gray background |
| `color` | `purple` | `p` | Paragraph purple |
| `font-size` | `20px` | `p` | Font bada karna |

---

## Inline se Farq

```
Inline  → <h1 style="color:green">  (CSS tag ke andar)
Internal → <style> h1 { color:green } </style>  (CSS head mein)
```

Internal mein ek jagah se poore page ke elements style hote hain — yeh inline se kaafi behtar hai.

## ✅ Internal CSS Ke Fayde
- Inline se behtar — ek jagah se sab elements style hote hain
- Chote single-page projects ke liye theek hai
- Alag file ki zaroorat nahi

## ❌ Internal CSS Ke Nuqsanat
- Sirf usi ek HTML file pe kaam karti hai
- 10 pages hoon toh 10 files mein alag likhni padti hai
- HTML file bhari ho jati hai
- Professional use ke liye nahi

---

## 💡 Kab Use Karein?
Sirf tab jab:
- Testing ya demo banana ho
- Ek hi page ka project ho
- External CSS possible na ho (rare case)
