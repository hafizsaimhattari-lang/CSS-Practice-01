# 🎯 02 Class Selector

## 📚 Is Folder Ka Maqsad
Yeh folder **Class Selector** ki practice ke liye hai.

---

## 📖 Class Selector Kya Hai?
Class selector un elements ko select karta hai jinka `class=""` attribute ek specific naam ka ho. CSS mein class selector `.` (dot) se likha jata hai.

```html
<!-- HTML -->
<h1 class="title">Main Heading</h1>
<p class="intro">Yeh paragraph hai.</p>
```

```css
/* CSS */
.title {
    color: darkblue;
    font-size: 36px;
}
.intro {
    color: gray;
    font-size: 18px;
}
```

---

## 📌 Yaad Rakho
- Ek hi class **kai elements** par lagayi ja sakti hai.
- Ek element mein **kai classes** bhi ho sakti hain: `class="btn primary large"`.
- Class selector ID selector se zyada use hota hai.

### Multi-class Example:
```html
<button class="btn primary">Click Me</button>
```
```css
.btn { padding: 10px 20px; border-radius: 5px; }
.primary { background-color: blue; color: white; }
```

---

## 📁 Files
| Folder                       | Description                                |
|------------------------------|--------------------------------------------|
| `01 Class Selector Practice` | Pehli practice (External CSS ke sath)      |
| `02 Class Selector Practice` | Doosri practice (Internal CSS ke sath)     |

---

## 📝 Summary
Class selector CSS ka sabse zyada use hone wala selector hai. Isko perfect karo!
