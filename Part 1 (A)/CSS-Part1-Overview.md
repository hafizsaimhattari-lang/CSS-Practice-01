# 🎨 CSS - Part 1 (A) Mukammal Jaiza

## 📚 Yeh Part Kyun Seekha?
CSS (Cascading Style Sheets) woh tool hai jis se hum apne HTML pages ko khubsoorat banate hain. Bina CSS ke webpage sirf sadda kala-safed text hota hai. Is Part mein CSS ki bunyad rakhi gayi hai.

---

## 🗂️ Folder Structure

```
Part 1 (A)/
├── 00 CSS Basic intro/         → CSS kya hoti hai, syntax kya hai
├── 01 Types of CSS/            → Inline, Internal, External CSS ka farq
├── 02 Basic Selectors/         → Selectors, combinators aur pseudo-classes
└── CSS-Part1-Overview.md       → Yeh file
```

---

## 🎯 Kya Kya Seekha?

### 📁 00 CSS Basic Intro
- CSS kya hoti hai (HTML + CSS + JS ka kirdar)
- Selector, Property aur Value ka concept
- Basic CSS syntax

### 📁 01 Types of CSS
| Qism | Tareeqa | Use |
|------|---------|-----|
| Inline CSS | `style=""` seedha tag mein | Testing sirf |
| Internal CSS | `<style>` head mein | Chote pages |
| External CSS | Alag `.css` file + `<link>` | Professional ✅ |

### 📁 02 Basic Selectors
| Selector | Symbol | Kaam |
|----------|--------|------|
| Element | `p { }` | Tag naam se select |
| Class | `.className` | Class se select (kai elements) |
| ID | `#idName` | ID se select (ek element) |
| Universal | `*` | Sab kuch select |
| Grouping | `h1, p, div` | Kai selectors ek sath |
| Descendant | `div p` | Andar wala element |
| Child combinator | `>` | Direct child |
| Sibling combinators | `+` / `~` | Foran agla ya baad ke siblings |
| Pseudo class | `:hover`, `:active` | Element ki state |

---

## 💡 Zaroori Yaad Rakhne Wali Batein
- Hamesha **External CSS** use karo professional kaam mein
- **Class** selector sabse zyada use hota hai
- **ID** unique hoti hai — ek page pe ek hi baar
- `*` reset ke liye use karo
- Combinator do selectors ka HTML relationship batata hai
- Pseudo class state ko target karti hai; naya HTML element nahi banati

---

## Basic CSS Rule Ko Parhna

```css
.card > p:hover {
    color: blue;
}
```

- `.card` class wala parent
- `>` direct child relation
- `p` target element
- `:hover` mouse wali state
- `color` property aur `blue` uski value

---

## Agla Practical Qadam

Ab selectors ko layout aur visual properties ke sath practice karein: box model, colors, typography, display, Flexbox aur Grid. Har example mein browser DevTools se dekhein ke kaunsa rule apply ya override ho raha hai.

---

**Status:** ✅ Part 1 Complete | Agla Qadam: Part 2 CSS Properties
