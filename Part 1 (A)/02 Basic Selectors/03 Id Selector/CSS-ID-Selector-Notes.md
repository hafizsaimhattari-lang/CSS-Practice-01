# 🎯 03 ID Selector

## 📚 Is Folder Ka Maqsad
Yeh folder **ID Selector** ki practice ke liye hai.

---

## 📖 ID Selector Kya Hai?
ID selector ek specific element ko select karta hai jis par `id=""` attribute diya hua ho. CSS mein ID selector `#` (hash) se likha jata hai.

```html
<!-- HTML -->
<h1 id="main-title">Mera Main Title</h1>
<p id="intro-text">Yeh mera intro paragraph hai.</p>
```

```css
/* CSS */
#main-title {
    color: crimson;
    font-size: 40px;
    text-decoration: underline;
}
#intro-text {
    color: navy;
    font-size: 20px;
}
```

---

## ⚠️ Zaroori Baat — ID Ki Khasiyat
- **ID unique hoti hai** — ek page par ek element ka hi woh ID hona chahiye.
- ID class se zyada **specific** (powerful) hoti hai.

### ID vs Class ka Farq:
| Feature         | Class (`.`)       | ID (`#`)          |
|-----------------|-------------------|-------------------|
| Use             | Kai elements par  | Sirf ek element   |
| CSS             | `.className`      | `#idName`         |
| Power/Specificity | Kam              | Zyada             |

---

## 📁 Files
| File                  | Description                     |
|-----------------------|---------------------------------|
| `01 id Selector.html` | ID selector ka HTML practice    |
| `01 Id Selector.css`  | Uski linked CSS file            |

---

## 📝 Summary
ID selector unique identification ke liye hoti hai. Prefer classes over IDs for styling.
