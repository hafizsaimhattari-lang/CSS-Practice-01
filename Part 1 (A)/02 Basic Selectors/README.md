# 🎯 02 Basic Selectors

## 📚 Is Folder Ka Maqsad
Yeh folder **CSS Basic Selectors** ki practice ke liye hai. CSS mein kisi bhi element ko style karne se pehle use **select** karna padta hai — yahi kaam Selectors karte hain.

---

## 📁 Folder Structure

```
02 Basic Selectors/
├── 01 Element Selector/              (Tag naam se select karo)
├── 02 Class Selector/               (Class naam se select karo)
├── 03 Id Selector/                  (ID se select karo - unique element)
├── 04 Univercal Selector/           (Sab elements ek sath)
├── 05 Grouping Selector & Multiple/ (Kai selectors ek sath)
├── 06 Descendent Selector/          (Nested elements ko target karo)
├── 07 Sibling Combinators/          (Bhai-bhai elements ko select karo)
└── README.md                        (Yeh file)
```

---

## 🎯 Har Selector Ka Mukhtar Idea

### 1️⃣ Element Selector
```css
p { color: red; }    /* Sare <p> tags red ho jayenge */
h1 { font-size: 40px; }
```

### 2️⃣ Class Selector (`.`)
```css
.btn { background-color: blue; }   /* class="btn" wale elements */
```

### 3️⃣ ID Selector (`#`)
```css
#main-heading { color: green; }   /* id="main-heading" wala element */
```
> ⚠️ ID unique hoti hai — ek page par ek element ka hi ID hona chahiye.

### 4️⃣ Universal Selector (`*`)
```css
* { margin: 0; padding: 0; }   /* Sab elements */
```

### 5️⃣ Grouping Selector
```css
h1, h2, h3, p { font-family: Arial; }
```

### 6️⃣ Descendant Selector (Space)
```css
div p { color: purple; }   /* Sirf div ke andar wale <p> */
```

### 7️⃣ Sibling Combinators
```css
h1 + p { color: orange; }  /* h1 ke turant baad wala p (+) */
h1 ~ p { color: gray; }    /* h1 ke baad ke sare p (~) */
```

---

## 📝 Summary
Selectors CSS ki jaan hain. Agar selector theek se nahi aaya toh styling fail ho jati hai. Inhe achi tarah practice karo.
