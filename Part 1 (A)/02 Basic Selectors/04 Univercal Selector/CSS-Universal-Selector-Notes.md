# 🎯 04 Universal Selector

## 📚 Is Folder Ka Maqsad
Yeh folder **Universal Selector** ki practice ke liye hai.

---

## 📖 Universal Selector Kya Hai?
Universal selector page ke **har ek element** ko ek sath select karta hai. Iske liye `*` (asterisk/star) use hota hai.

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

---

## 🔥 Sabse Common Use Case — CSS Reset
Browser apne default margin aur padding add karta hai. Universal selector se unhe zero kar diya jata hai:

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```
> Yeh almost **har professional CSS file** ke sabse upar likha jata hai!

---

## ⚠️ Savdhaani
- Universal selector bahut powerful hai — galat use karne se poora design bigad sakta hai.
- Mostly sirf CSS reset ke liye use karo.

---

## 📁 Files
| File                          | Description                     |
|-------------------------------|---------------------------------|
| `01 Univercal Selector.html`  | Universal selector ka HTML      |
| `01 Univercal Selector.css`   | Universal selector ka CSS       |

---

## 📝 Summary
`*` selector jadugarni hai magar savdhaani se use karo. CSS reset ke liye yeh ek standard practice hai.
