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
| `:focus-visible` | Jab browser visible keyboard focus dikhana munasib samjhe |
| `:visited` | Jab link already visit ki gayi ho |
| `:checked` | Checked checkbox/radio |
| `:disabled` | Disabled form control |
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

## State Aur Structure Pseudo Classes

| Qisam | Examples | Matlab |
|-------|----------|--------|
| User interaction | `:hover`, `:active`, `:focus` | User ki current action/state |
| Form state | `:checked`, `:disabled`, `:valid` | Control ki halat |
| Link state | `:link`, `:visited` | Link history/state |
| Structure | `:first-child`, `:last-child`, `:nth-child()` | DOM mein position |

Pseudo class colon (`:`) use karti hai. Pseudo-element, jaise `::before`, double colon use karta aur element ka ek virtual part target karta hai.

---

## Selectors Ke Sath Combine Karna

```css
.menu a:hover { color: orange; }
input:focus { outline: 2px solid blue; }
li:first-child { font-weight: bold; }
button.primary:active { transform: scale(0.98); }
```

Ek selector par multiple pseudo-classes bhi ho sakti hain:

```css
button:hover:enabled { background-color: navy; }
```

---

## Accessibility

- Sirf `:hover` par zaroori information depend na karein; touch aur keyboard users hover nahi kar sakte.
- Focus indicator ko bina replacement ke remove na karein.
- Color change ke sath border, underline ya doosra visible cue dena useful hota hai.
- Interactive behavior ke liye semantic `<button>` aur `<a>` elements prefer karein.

---

## Common Mistakes

- `.button :hover` mein space dena descendant ki hover state dhoondta hai; `.button:hover` khud button ko target karta hai.
- `::hover` galat hai; hover pseudo-class single colon leti hai.
- `:active` ko permanent selected state samajhna; yeh aam tor par press ke waqt hoti hai.

---

## Yaad Rakho
- Pseudo class element ki **state** target karti hai
- Real element nahi badalta — sirf styling temporarily lagti hai
- `:hover` aur `:active` sabse zyada use hote hain
- Pseudo-class selector ki specificity class jaisi category mein count hoti hai
