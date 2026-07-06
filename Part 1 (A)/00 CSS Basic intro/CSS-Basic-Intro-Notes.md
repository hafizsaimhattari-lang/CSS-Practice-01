# 🎨 CSS Basic Introduction - Mukammal Notes

## 📚 CSS Kya Hoti Hai?
**CSS (Cascading Style Sheets)** ek styling language hai jo HTML web pages ko design karti hai. Yeh HTML elements ka rang, size, position, font aur layout control karti hai.

### HTML + CSS + JS ka kirdar:
```
HTML  → Structure   → Makan ki deewaren aur chhat
CSS   → Design      → Rang, rangai, sajaawat
JS    → Behaviour   → Doors, switches, bijli
```

---

## 🔑 CSS Ki Basic Syntax

```css
selector {
    property: value;
    property: value;
}
```

### Har hissa kya karta hai:
| Hissa | Matlab | Misal |
|-------|--------|-------|
| **Selector** | Konsa element target karna hai | `h1`, `.box`, `#title` |
| **Property** | Kya badalna hai | `color`, `font-size`, `background` |
| **Value** | Kya value deni hai | `red`, `20px`, `#222` |

---

## 📝 Pehla CSS Example

```css
h1 {
    color: blue;
    font-size: 32px;
    text-align: center;
}
```
Yeh CSS code page ke sare `<h1>` tags ko neele rang ka, 32px bada, aur center mein kar dega.

---

## 🌊 "Cascading" Ka Matlab

CSS mein "C" ka matlab **Cascading** hai — yani agar kisi element ko kai jagah se style mile, toh ek khas tarteeq ke mutabiq ek jeete ga:
1. `!important` (sabse powerful)
2. Inline CSS
3. ID selector
4. Class selector
5. Element selector
6. Browser default (sabse kamzor)

---

## 💡 Notes
- CSS comments `/* yahan likho */` se likhte hain
- Har property ke aakhir mein `;` (semicolon) zaroori hai
- CSS **case-insensitive** hai lekin lowercase likhna best practice hai
