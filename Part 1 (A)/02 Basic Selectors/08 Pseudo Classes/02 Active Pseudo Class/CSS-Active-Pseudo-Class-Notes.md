# CSS :active Pseudo Class - Mukammal Notes

## :active Kya Hai?
`:active` pseudo class tab apply hoti hai jab **element ko click kiya ja raha ho** (mouse button neeche dabaya hua ho). Jaise hi click chhorte hain, style hatt jati hai.

```css
selector:active {
    property: value;
}
```

---

## Hamari Practice File: `01 Active Pseudo Class.html` + `01 Active-Pseudo-Class.css`

### HTML Structure:
```html
<div class="form-div">
    <form class="Form" action="#">
        <label for="Full-Name">Full Name : </label>
        <input type="text" id="Full-Name" placeholder="Enter Your Name">
        <button type="Submit" id="Submit-Button-01" class="Submit-Form-Button">Submit</button>
    </form>
</div>
```

### CSS - Poori File:
```css
body {
    background-color: black;
}

label {
    color: white;
}

/* Input par mouse aane par (hover) */
input:hover {
    background-color: yellow;
    color: black;
}

/* Input click hone ke waqt (active) */
input:active {
    border: 3px solid white;
    background-color: blue;
    color: white;
}

/* Button click hone ke waqt (active) */
button:active {
    background-color: blue;
    color: white;
    border: 3px solid white;
    border-radius: 5px;
}
```

---

## Is Practice Mein Use Hone Wali Properties

| CSS Rule | Kaam |
|----------|------|
| `input:hover` | Mouse aane par — yellow background |
| `input:active` | Click ke waqt — blue background, white border |
| `button:active` | Button dabane par — blue, white border, gol corners |

---

## :hover aur :active Ka Farq

| State | Kab | Duration |
|-------|-----|----------|
| `:hover` | Mouse upar aata hai | Jab tak mouse ruke |
| `:active` | Mouse click ho | Sirf click ke waqt |

```css
/* Pehle hover, phir click ke waqt active */
button:hover  { background-color: darkblue; }
button:active { background-color: black; transform: scale(0.95); }
```

---

## Real-World Use

```css
/* Professional button states */
.btn {
    background-color: blue;
    color: white;
    padding: 10px 20px;
}

.btn:hover {
    background-color: darkblue;  /* Mouse aane par */
}

.btn:active {
    background-color: black;     /* Click hone par */
    transform: scale(0.97);      /* Thoda chota hona — press effect */
}
```

---

## Seekha Kya?
- `:active` click ka momentary (sirf click ke waqt) style deta hai
- `:hover` + `:active` combine karna button ko interactive feel deta hai
- `border-radius` ke sath active state aur achi lagti hai

---

## `:active` Aur Selected State Mein Farq

`:active` aam tor par pointer/button press ke duration tak rehti hai. Menu ka permanently selected item dikhane ke liye class ya relevant state use karein:

```html
<a class="current-page" href="/about">About</a>
```

```css
.current-page { font-weight: bold; }
```

Checkbox ki persistent state ke liye `:checked` hoti hai, `:active` nahi.

---

## Keyboard Aur Focus

Button activate karne ke baad keyboard focus reh sakta hai. Is liye active ke sath focus style bhi rakhein:

```css
button:focus-visible {
    outline: 3px solid orange;
    outline-offset: 2px;
}
```

---

## Common Mistakes Aur Summary

- `:active` ko click ke baad permanently apply samajhna.
- Press effect mein itna transform karna ke layout ya readability disturb ho.
- Focus outline remove karke keyboard users ko current position se mehroom karna.
- `:active` instant feedback deta hai; persistent application state ke liye class/attribute zyada munasib hai.
