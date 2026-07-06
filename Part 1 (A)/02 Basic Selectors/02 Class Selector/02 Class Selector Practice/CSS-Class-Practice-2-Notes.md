# Class Selector - Practice 2

Is practice mein Internal CSS ke sath ek class ko kai headings par reuse kiya gaya hai.

## Files

| File | Kaam |
|------|------|
| `02 Class Selector (Internal CSS).html` | Internal CSS ke sath class practice |

---

## HTML Mein Classes

```html
<h1 class="small-heading">This is 1st Heading 1</h1>
<h2 class="small-heading">This is 2nd Heading 2</h2>
<h3 class="small-heading">This is 3rd Heading 3</h3>

<hr class="Horizontal-Line">

<h4 class="large-heading">This is 4th Heading 4</h4>
<h5 class="large-heading">This is 5th Heading 5</h5>
<h6 class="large-heading">This is 6th Heading 6</h6>
```

- `.small-heading` teen alag heading tags par reuse hui.
- `.large-heading` bhi teen headings par reuse hui.
- `.Horizontal-Line` sirf `<hr>` ko style karti hai.

---

## Internal CSS

```css
.small-heading {
    color: white;
    font-size: small;
    background-color: blue;
    padding: 10px;
    border-radius: 5px;
    text-align: center;
}

.large-heading {
    color: white;
    font-size: larger;
    background-color: red;
    padding: 10px;
    border-radius: 5px;
    text-align: center;
}
```

CSS `<head>` ke `<style>` tag mein likhi hai, lekin class selector ka syntax external CSS jaisa hi rehta hai.

---

## Seekha Kya?

- Class selector dot (`.`) se shuru hota hai.
- Ek class mukhtalif HTML tags par lag sakti hai.
- Class ka naam case-sensitive hota hai: `Horizontal-Line` aur `horizontal-line` alag names hain.
- Internal ya External CSS se selector ka behavior nahi badalta; sirf CSS likhne ki jagah badalti hai.
