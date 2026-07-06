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
- Shared styles cache/reuse nahi hote jaise external file mein hote hain

---

## 💡 Kab Use Karein?
Sirf tab jab:
- Testing ya demo banana ho
- Ek hi page ka project ho
- Page-specific critical ya generated styling ho

---

## Placement Aur Scope

```html
<head>
    <style>
        .notice { color: red; }
    </style>
</head>
```

`<style>` aam tor par `<head>` mein rakha jata hai. Is block ke selectors poore current document ko target kar sakte hain, sirf neeche wale element ko nahi.

## Internal Aur External Dono Sath

```html
<link rel="stylesheet" href="style.css">
<style>
    p { color: green; }
</style>
```

Agar importance aur specificity same ho to baad mein aane wala rule jeetta hai. Is example mein internal rule link ke baad hai, is liye same `p` property par internal value jeet sakti hai.

---

## Common Mistakes

- `<style>` ko galti se `<body>` ke content mein rakhna.
- CSS declarations ko HTML attributes ki tarah likhna.
- Closing `</style>` tag bhoolna.
- Har page mein same internal CSS copy karna; shared CSS ke liye external file behtar hai.

---

## Summary

Internal CSS current HTML document ke `<style>` block mein hoti hai. Single-page demo ya page-specific rules ke liye useful hai, lekin multi-page reuse ke liye External CSS zyada maintainable hoti hai.
