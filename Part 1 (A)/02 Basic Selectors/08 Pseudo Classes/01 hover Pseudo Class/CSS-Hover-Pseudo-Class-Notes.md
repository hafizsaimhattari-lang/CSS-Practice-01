# CSS :hover Pseudo Class - Mukammal Notes

## :hover Kya Hai?
`:hover` pseudo class tab apply hoti hai jab **mouse cursor element par aata hai**. Yeh interactive effects banane ka sabse common tareeqa hai.

```css
selector:hover {
    property: value;
}
```

---

## Hamari Practice File: `01 hover Pseudo Class.html` + `01 hover-Pseudo-Class.css`

### HTML Structure:
```html
<!-- Form section -->
<div class="form-div">
    <form class="Form" action="#">
        <label for="Full-Name">Full Name : </label>
        <input type="text" id="Full-Name" placeholder="Enter Your Name">
        <button type="Submit" id="Submit-Button-01" class="Submit-Form-Button">Submit</button>
    </form>
</div>

<!-- Paragraph -->
<p class="first-para">Lorem ipsum dolor sit amet...</p>

<!-- Anchor Links -->
<h1>Anchor Links</h1>
<div class="anchor-links">
    <ul>
        <li><a href="https://www.google.com" target="_blank">Saim</a></li>
        <li><a href="https://www.google.com" target="_blank">Kashif</a></li>
        <li><a href="https://www.google.com" target="_blank">Imran</a></li>
        <li><a href="https://www.google.com" target="_blank">Abdul</a></li>
        <li><a href="https://www.google.com" target="_blank">Talha</a></li>
    </ul>
</div>
```

### CSS - Poori File:
```css
body {
    background-color: blue;
}

/* Universal selector - sab text white */
* {
    color: white;
}

.form-div {
    text-align: center;
}

/* ID selector + :hover — Submit button par mouse aane par */
#Submit-Button-01:hover {
    background-color: black;
    color: white;
    border: 2px solid white;
}

/* Normal state mein button */
.Submit-Form-Button {
    color: black;
}

/* Form ke input par hover */
.Form input:hover {
    background-color: black;
    color: white;
}

/* Normal state mein input */
.Form input {
    color: black;
}

/* Next Sibling Combinator + color - paragraph */
br + p {
    color: yellow;
    text-align: center;
}

/* Anchor links par hover */
.anchor-links ul li a:hover {
    color: chartreuse;
    text-decoration: underline;
}

/* h1 par hover (next sibling se) */
.first-para + h1:hover {
    color: white;
}

/* h1 normal state */
.first-para + h1 {
    color: yellow;
}

/* Paragraph par hover */
.first-para:hover {
    color: white;
}

/* Paragraph normal state */
.first-para {
    color: yellow;
}
```

---

## Is Practice Mein Use Hone Wali Properties

| CSS Rule | Kaam |
|----------|------|
| `#Submit-Button-01:hover` | ID + hover — button black ho jata hai |
| `.Form input:hover` | Class + descendant + hover — input dark |
| `.anchor-links ul li a:hover` | Deep descendant + hover — links chartreuse |
| `.first-para:hover` | Class + hover — paragraph white |
| `.first-para + h1:hover` | Next sibling + hover — heading white |

---

## Seekha Kya?

1. `:hover` kisi bhi selector ke sath lagta hai — element, class, ID, descendant, sibling
2. Normal state aur hover state dono alag likhte hain
3. Hover + multiple selectors combine kar sakte hain

```css
/* Combination examples from practice */
#id:hover { }               /* ID + hover */
.class:hover { }            /* Class + hover */
.parent input:hover { }     /* Descendant + hover */
.class + h1:hover { }       /* Sibling + hover */
```
