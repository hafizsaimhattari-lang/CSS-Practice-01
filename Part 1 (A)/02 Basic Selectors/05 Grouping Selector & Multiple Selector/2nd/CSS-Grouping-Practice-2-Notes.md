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

Is practice me selector list clean rakhi gayi hai:

```css
p, h1, h2
```

Har selector ek baar likha gaya hai. Agar selector duplicate ho bhi jaye to result usually same rehta hai, lekin proper code me repeated selector avoid karna behtar hota hai.

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

## Common Mistakes

- Comma bhool jana: `h1 p` ka matlab grouping nahi, descendant selector hota hai.
- Same selector ko baar baar likhna.
- Grouping me unrelated selectors ko ek sath rakh dena.

## Best Practice

Agar multiple elements ko same CSS deni ho, to grouping selector use karo.

Lekin agar kisi element ki styling different hai, to us ke liye separate rule likhna zyada readable hota hai.
