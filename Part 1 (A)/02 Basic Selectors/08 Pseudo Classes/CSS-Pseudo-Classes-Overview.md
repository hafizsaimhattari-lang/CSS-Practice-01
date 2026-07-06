# CSS Pseudo Classes - Mukammal Overview

## Pseudo Class Kya Hai?
Pseudo Class ek CSS selector hai jo kisi element ki **khaas halat (state)** mein style apply karta hai — maslan jab mouse us par ho, ya jab use click kiya ja raha ho.

```css
selector:pseudo-class {
    property: value;
}
```

Colon (`:`) lagane ke baad pseudo class ka naam aata hai.

---

## Folder Structure

```
08 Pseudo Classes/
|-- 01 hover Pseudo Class/     :hover — mouse upar aane par
|-- 02 Active Pseudo Class/    :active — click hone ke waqt
```

---

## Common Pseudo Classes

| Pseudo Class | Kab Apply Hoti Hai |
|-------------|-------------------|
| `:hover` | Jab mouse element par aata hai |
| `:active` | Jab element click ho raha ho |
| `:focus` | Jab input mein cursor ho |
| `:visited` | Jab link already visit ki gayi ho |
| `:first-child` | Parent ka pehla bacha |
| `:last-child` | Parent ka aakhri bacha |
| `:nth-child(n)` | nth numbered bacha |

---

## Practical Use

```css
/* Button par hover */
button:hover { background-color: darkblue; }

/* Click ke waqt */
button:active { transform: scale(0.95); }

/* Input mein focus */
input:focus { border: 2px solid blue; outline: none; }

/* Link visited */
a:visited { color: purple; }
```

---

## Yaad Rakho
- Pseudo class element ki **state** target karti hai
- Real element nahi badalta — sirf styling temporarily lagti hai
- `:hover` aur `:active` sabse zyada use hote hain
