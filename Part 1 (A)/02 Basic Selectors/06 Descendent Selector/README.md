# 🎯 06 Descendant Selector

## 📚 Is Folder Ka Maqsad
Yeh folder **Descendant Selector** ki practice ke liye hai.

---

## 📖 Descendant Selector Kya Hai?
Descendant selector kisi parent element ke **andar** wale specific child elements ko target karta hai. Iske liye dono selectors ke beech **space** rakha jata hai.

```css
/* Syntax */
parent child {
    property: value;
}
```

### Example:
```html
<div>
    <p>Yeh div ke andar hai.</p>
</div>
<p>Yeh div ke bahar hai.</p>
```

```css
div p {
    color: red;   /* Sirf div ke ANDAR wala p red hoga */
}
```

---

## 🔑 Key Points
- Space ka matlab hai "andar ka element" (descendant).
- Direct child ya deep-nested dono par kaam karta hai.
- Zyada specific styling ke liye bahut useful hai.

### Deep Nesting bhi kaam karta hai:
```css
.card .content p {
    font-size: 14px;
}
```

---

## 📁 Files
| Folder      | File                          | Description                   |
|-------------|-------------------------------|-------------------------------|
| `01 First`  | `01 Descendent Selector.html` | Pehli practice                |
| `01 First`  | `01 Descendent Selector.css`  | Uski CSS                      |
| `02 Second` | `02 Descendent Selector.html` | Doosri practice               |
| `02 Second` | `02 Descendent Selector.css`  | Uski CSS                      |

---

## 📝 Summary
Descendant selector real-world projects mein bahut zyada use hota hai — components ki nested styling ke liye.
