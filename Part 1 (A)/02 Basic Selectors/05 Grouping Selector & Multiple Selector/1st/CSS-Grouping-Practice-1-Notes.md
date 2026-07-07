# Grouping Selector - Practice 1

Is practice mein class selectors aur element selectors ko comma (`,`) se group karke same declarations di gayi hain.

## Files

| File | Kaam |
|------|------|
| `01 Grouping Selector.html` | Headings aur paragraphs ki structure |
| `01 Grouping Selector.css` | Class aur element grouping ki practice |

---

## HTML Structure

```html
<h1 class="headings">Grouping Selector Practice</h1>
<p class="paragraph">This is a paragraph.</p>
<p class="paragraph">This is another paragraph.</p>
<h2 class="headings">This is a heading 2</h2>
<h3 class="headings">This is a heading 3</h3>
```

---

## Class Selectors Ki Grouping

```css
.headings, .paragraph {
    text-align: center;
    border: 2px solid yellow;
    border-radius: 10px;
    padding: 10px;
}
```

`.headings` aur `.paragraph` dono ko ek hi declaration block milta hai.

## Element Selectors Ki Grouping

```css
h1, h2, h3, p {
    text-align: center;
    border: 2px solid yellow;
    border-radius: 10px;
    padding: 10px;
}
```

Har comma ek naya selector shuru karta hai. Comma bhoolne par selector ka matlab badal kar descendant selector ban sakta hai.

---

## Seekha Kya?

- Grouping se repeated CSS kam hoti hai.
- Element, class aur ID selectors ko group kiya ja sakta hai.
- Is file mein class grouping aur element grouping same result dikhati hain.
- Real project mein same declarations ko ek grouped rule mein rakhna zyada saaf hota hai.

## Browser Mein Result

Is practice mein headings aur paragraphs ko same type ki box styling milti hai.

Result:

- Text center align hota hai.
- Border yellow hota hai.
- Corners rounded hote hain.
- Padding ki wajah se content border se chipakta nahi.

## Grouping Selector Ka Faida

Agar hume `h1`, `h2`, `h3`, aur `p` sab par same CSS lagani ho, to alag alag rules likhne ki zaroorat nahi.

Clean tareeqa:

```css
h1, h2, h3, p {
  text-align: center;
}
```

## Common Mistakes

- Comma ke bajaye space likh dena.
- Grouping mein incomplete selector likhna.
- Har selector ke liye same declarations repeat karna.

## Best Practice

Sirf woh selectors group karo jin ka design waqai same ho.

Jis element ka design different ho, us ke liye separate rule likho.
