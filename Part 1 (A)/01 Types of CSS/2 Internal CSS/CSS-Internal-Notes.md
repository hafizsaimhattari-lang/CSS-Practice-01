# 🎨 2 Internal CSS

## 📚 Is Folder Ka Maqsad
Yeh folder **Internal CSS** (Embedded CSS) ki practice ke liye hai.

---

## 📖 Internal CSS Kya Hai?
Internal CSS mein HTML file ke `<head>` section mein `<style>` tag banaya jata hai aur sari CSS us ke andar likhi jati hai.

```html
<head>
    <style>
        h1 {
            color: green;
            text-align: center;
        }
        p {
            color: purple;
            font-size: 20px;
        }
    </style>
</head>
```

---

## ✅ Fayde
- Inline se behtar — ek jagah se sab elements style hote hain.
- Chote single-page projects ke liye theek hai.

## ❌ Nuqsanat
- Sirf usi ek HTML file pe kaam karti hai.
- Ek se zyada pages hoon to har mein alag CSS likhni padti hai.

---

## 📁 Files
| File                      | Description                          |
|---------------------------|--------------------------------------|
| `01 internal CSS.html`    | Internal CSS ki practice             |

---

## 📝 Summary
Internal CSS inline se achi hai magar External CSS se buri. Medium complexity ke liye use karo.
