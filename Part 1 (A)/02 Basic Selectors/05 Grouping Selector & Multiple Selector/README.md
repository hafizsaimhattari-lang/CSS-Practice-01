# 🎯 05 Grouping Selector & Multiple Selector

## 📚 Is Folder Ka Maqsad
Yeh folder **Grouping Selector** ki practice ke liye hai.

---

## 📖 Grouping Selector Kya Hai?
Jab kai elements par ek jaisi CSS lagani ho, to unhe ek sath group karke style kar sakte hain. Elements ke beech comma (`,`) dala jata hai.

### Grouping ke bina (Repetition):
```css
h1 { color: blue; font-family: Arial; }
h2 { color: blue; font-family: Arial; }
h3 { color: blue; font-family: Arial; }
p  { color: blue; font-family: Arial; }
```

### Grouping ke sath (Clean Code):
```css
h1, h2, h3, p {
    color: blue;
    font-family: Arial;
}
```

---

## 📌 Multiple Selectors
Aap class, id, aur element selectors sab ko group kar sakte ho:
```css
h1, .intro, #hero {
    font-size: 24px;
    margin-bottom: 10px;
}
```

---

## 📁 Files
| Folder  | Description                                      |
|---------|--------------------------------------------------|
| `1st`   | Pehli practice — basic grouping                  |
| `2nd`   | Doosri practice — mixed selectors grouping        |

---

## 📝 Summary
Grouping selector code duplication rokta hai. Yeh clean aur DRY (Don't Repeat Yourself) code likhne ka tareeqa hai.
