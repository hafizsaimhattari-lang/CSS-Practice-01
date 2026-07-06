# Grouping Selector - Practice 2

Is practice mein kai element selectors ko ek rule mein group karke repeated declarations bachai gayi hain.

## Files

| File | Kaam |
|------|------|
| `02 Grouping Selector.html` | `h1`, `h2` aur multiple `p` elements |
| `02 Grouping Selector.css` | Universal aur grouping selectors |

---

## HTML Structure

```html
<h1>Grouping Selector Example</h1>
<h2>Multiple selectors share the same styles</h2>
<p>First paragraph...</p>
<p>Second paragraph...</p>
```

## Practice CSS

```css
* {
    text-align: center;
    color: white;
}

p, h1, h2 {
    border: 2px solid red;
    border-radius: 10px;
    padding: 10px;
}

body {
    background-color: black;
}
```

`p`, `h1` aur `h2` sab ko red border, rounded corners aur padding milti hai. Universal selector sab elements ka text center aur white karta hai.

> Original practice rule mein `p` do baar likha hua hai. Duplicate selector result nahi badalta, lekin clean code mein har selector ek baar likhna behtar hai.

---

## Grouping Aur Descendant Mein Farq

```css
h1, p { } /* h1 aur p dono select */
h1 p  { } /* sirf h1 ke andar wala p select */
```

---

## Seekha Kya?

- Comma ka matlab **aur / and** hai.
- Group ke har selector par poora declaration block apply hota hai.
- Duplicate selector ki zaroorat nahi hoti.
- Grouping code ko short aur maintainable banati hai.
