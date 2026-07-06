# Descendant Selector - Practice 1

Is practice mein `div` ke andar maujood headings aur paragraphs ko element-based descendant selectors se target kiya gaya hai.

## Files

| File | Kaam |
|------|------|
| `01 Descendent Selector.html` | HTML structure |
| `01 Descendent Selector.css` | `parent child { }` CSS |

---

## HTML Ka Basic Pattern

```html
<div>
    <h1>Descendent Selector Test 01</h1>
</div>

<div>
    <p>Paragraph inside div...</p>
</div>
```

## Practice CSS

```css
div p {
    color: red;
    font-size: 20px;
    font-weight: bold;
    text-align: center;
}

div h1 {
    color: blue;
    font-size: 30px;
    font-weight: bold;
    text-align: center;
}
```

`div p` ka matlab page ke tamam paragraphs nahi, balki sirf woh `p` hain jo kisi `div` ke andar hain. Isi tarah `div h1` sirf `div` ke andar headings select karta hai.

---

## Grouping Ke Sath

```css
div p, div h1 {
    border: 2px solid black;
    padding: 10px;
}
```

Yahan do complete descendant selectors comma se group hue hain.

---

## Seekha Kya?

- Selectors ke darmiyan space ka matlab **andar** hai.
- Descendant direct child bhi ho sakta hai aur deeply nested bhi.
- Class ke sath `.vip-box p` aur ID ke sath `#vip-box p` likh sakte hain.
- Bahar ka matching element select nahi hota.
