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
