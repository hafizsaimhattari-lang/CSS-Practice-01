# Descendant Selector - Practice 2

Is practice mein element, class aur ID selectors ko descendant combinator ke sath combine kiya gaya hai.

## Files

| File | Kaam |
|------|------|
| `02 Descendent Selector.html` | HTML structure |
| `02 Descendent Selector.css` | Element, class aur ID descendants ki practice |

---

## HTML Structure

```html
<div>
    <h1 id="main-heading">Descendant Selector Test</h1>
    <p class="paragraph">Paragraph inside div...</p>
</div>
```

## Element Descendants

```css
div p { border: 1px solid white; padding: 10px; }
div h1 { border: 1px solid white; padding: 10px; }
```

## Class Aur ID Descendants

```css
div .paragraph {
    border: 1px solid yellow;
}

div #main-heading {
    border: 1px solid yellow;
}
```

- `div .paragraph` kisi bhi element ko match karega jo `.paragraph` class rakhta ho aur `div` ke andar ho.
- `div #main-heading` us unique ID ko match karega jo `div` ke andar ho.

---

## Cascade Ka Result

Paragraph `div p` aur `div .paragraph` dono se match hota hai. Class selector zyada specific hai, is liye yellow border white border ko override karti hai. Heading par bhi ID wala rule zyada specific hone ki wajah se yellow border jeetta hai.

---

## Seekha Kya?

- Descendant combinator ke dono taraf kisi bhi qisam ka selector aa sakta hai.
- Ek element ek waqt mein multiple rules se match ho sakta hai.
- Conflict ki surat mein specificity aur source order decide karte hain ke kaunsi value apply hogi.

## Browser Mein Result

Is practice mein paragraph aur heading dono `div` ke andar hain.

Result:

- `div p` aur `div h1` basic styling dete hain.
- `.paragraph` class wala selector paragraph ko zyada specific styling deta hai.
- `#main-heading` ID wala selector heading ko zyada specific styling deta hai.

## Specificity Simple Samajh

Specificity ka matlab hai selector ki power.

Generally:

```text
ID selector > Class selector > Element selector
```

Is liye:

- `div #main-heading` zyada strong hai
- `div .paragraph` element selector se zyada strong hai

## Common Mistakes

- ID ko CSS mein `.` se target karna.
- Class ko CSS mein `#` se target karna.
- Specificity conflict samjhe bina sochna ke CSS kaam nahi kar rahi.

## Best Practice

ID selectors ko kam use karo.

Reusable design ke liye classes zyada flexible hoti hain.
