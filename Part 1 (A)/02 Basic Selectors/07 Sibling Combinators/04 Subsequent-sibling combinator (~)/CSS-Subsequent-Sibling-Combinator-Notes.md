# Subsequent Sibling Combinator (`~`) - Mukammal Notes

## Kya Hai?
Subsequent Sibling Combinator (`~`) pehle selector ke baad aane wale tamam matching siblings ko target karta hai. Dono taraf ke elements ka parent same hona zaroori hai.

```css
h1 ~ p { color: orange; }
/* h1 ke baad aane wale tamam p siblings */
```

---

## Zaroori Rules

- Dono elements ka parent same hona chahiye.
- Sirf pehle element ke **baad** aane wale siblings select hote hain; pehle wale nahi.
- Beech mein doosre elements aa sakte hain.
- Right side par diya gaya selector match hona zaroori hai.

```html
<section>
    <p>Yeh select nahi hoga: h1 se pehle hai.</p>
    <h1>Heading</h1>
    <span>Beech mein span ho sakta hai.</span>
    <p>Yeh select hoga.</p>
    <p>Yeh bhi select hoga.</p>
</section>
```

---

## Hamari Practice Files

- `01 Subsequent-Sibling-Combinator.html` mein woh elements hain jin par selector test kiya gaya hai.
- `01 Subsequent-Sibling-Combinator.css` mein `~` ko element, class aur nested selectors ke sath use kiya gaya hai.

### Practice CSS Ki Samajh

```css
header ~ h1 {
    color: yellow;
}
```

`body` ke andar `header` ke baad aane wale tamam `h1` siblings yellow honge.

```css
h1 ~ .div-para > p {
    color: white;
    text-align: center;
    text-decoration: underline;
}
```

Yeh pehle `h1` ke baad aane wale `.div-para` siblings ke direct-child `p` elements ko style karta hai. Is selector mein `~` aur `>` dono combinators use hue hain.

```css
br ~ div ol li {
    color: chartreuse;
    text-decoration: underline;
}
```

Yeh `br` ke baad wale `div` sibling ke andar maujood ordered list ke `li` elements ko select karta hai.

---

## Next Sibling (`+`) Se Farq

```css
h1 + p { }  /* Sirf agla ek p */
h1 ~ p { }  /* Baad ke tamam matching p siblings */
```

### Example

```html
<h1>Heading</h1>
<p>Para 1</p> <!-- + aur ~ dono select karenge -->
<p>Para 2</p> <!-- sirf ~ select karega -->
<p>Para 3</p> <!-- sirf ~ select karega -->
```

---

## Real-World Use

```css
/* Checked input ke baad ke tamam matching labels */
input:checked ~ label { text-decoration: line-through; }

/* H2 ke baad ke tamam paragraph siblings */
h2 ~ p { color: #555; font-size: 16px; }
```

---

## Summary

`A ~ B` ka matlab hai: `A` ke baad aane wale tamam matching `B` siblings select karo. `A` aur `B` ka same parent hona chahiye, lekin unka bilkul sath hona zaroori nahi.
