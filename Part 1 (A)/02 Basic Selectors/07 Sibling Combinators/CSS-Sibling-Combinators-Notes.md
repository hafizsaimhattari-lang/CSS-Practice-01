# 🎯 07 Sibling Combinators

## 📚 Is Folder Ka Maqsad
Yeh folder **Sibling Combinators** ki practice ke liye hai — yeh selectors ek dusre ke "bhai-bhan" (sibling) elements ko target karte hain.

---

## 📖 Sibling Kya Hote Hain?
Jab do ya zyada elements ek hi parent ke andar hon, to unhe sibling kehte hain.

```html
<div>
    <h1>Heading</h1>   <!-- Sibling -->
    <p>Para 1</p>      <!-- Sibling -->
    <p>Para 2</p>      <!-- Sibling -->
    <span>Text</span>  <!-- Sibling -->
</div>
```

---

## 📁 Folder Structure

```
07 Sibling Combinators/
├── 01 Descendant combinator (space)/   (Space " " — nested element)
├── 02 Child combinator/                (Arrow ">" — direct child sirf)
├── 03 Next sibling combinator (+)/    (Plus "+" — agla ek sibling)
├── 04 Subsequent-sibling combinator(~)/ (Tilde "~" — baad ke sare siblings)
└── README.md                           (Yeh file)
```

---

## 🔑 Teeno Combinators Ka Farq

### 1. Descendant (Space ` `)
```css
div p { color: red; }   /* div ke andar ke SARE p — direct ya nested */
```

### 2. Child (`>`)
```css
div > p { color: blue; }   /* div ke SEEDHE BACHY p sirf */
```

### 3. Next Sibling (`+`)
```css
h1 + p { color: green; }   /* h1 ke TURANT baad wala sirf ek p */
```

### 4. Subsequent Siblings (`~`)
```css
h1 ~ p { color: orange; }   /* h1 ke baad ke SARE p siblings */
```

---

## 📌 Jaldi Yaad Karne Ka Tareeqa
| Symbol | Naam               | Matlab                     |
|--------|--------------------|----------------------------|
| ` `    | Descendant         | Andar ka koi bhi           |
| `>`    | Child              | Seedha bacha sirf          |
| `+`    | Adjacent Sibling   | Agla ek bhai-bhan          |
| `~`    | General Sibling    | Baad ke sare bhai-bhan     |

---

## 📝 Summary
Sibling combinators advanced CSS mein bahut kaam aate hain. Layouts aur list styling mein yeh frequently use hote hain.
