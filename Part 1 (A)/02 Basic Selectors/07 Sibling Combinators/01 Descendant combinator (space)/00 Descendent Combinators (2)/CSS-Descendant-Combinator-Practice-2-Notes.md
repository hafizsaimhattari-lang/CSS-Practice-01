# Descendant Combinator - Practice 2

Is practice mein descendant combinator ko element, class aur ID selector ke sath use kiya gaya hai.

## Files

| File | Kaam |
|------|------|
| `02 Descendent Selector.html` | ID wali heading aur class wala paragraph |
| `02 Descendent Selector.css` | Chaar descendant selector examples |

## HTML Structure

```html
<div>
    <h1 id="main-heading">Descendant Selector Test</h1>
    <p class="paragraph">Paragraph inside div...</p>
</div>
```

## Practice Selectors

```css
div p { border: 1px solid white; }
div h1 { border: 1px solid white; }
div .paragraph { border: 1px solid yellow; }
div #main-heading { border: 1px solid yellow; }
```

### Har Rule Ka Matlab

| Selector | Target |
|----------|--------|
| `div p` | `div` ke andar har `p` |
| `div h1` | `div` ke andar har `h1` |
| `div .paragraph` | `div` ke andar `.paragraph` class |
| `div #main-heading` | `div` ke andar `#main-heading` ID |

## Specificity Ka Asar

Ek hi paragraph `div p` aur `div .paragraph` dono ko match karta hai. Class wala selector zyada specific hai, is liye uski yellow border jeetti hai. ID wale heading rule mein bhi yahi principle apply hota hai.

## Seekha Kya?

- Space combinator tag, class aur ID sab ke sath kaam karta hai.
- Ek element multiple selectors se match ho sakta hai.
- Specificity conflicting property ka winner decide karti hai.

## Practice Ka Result

Is practice mein same elements par multiple selectors match karte hain.

Paragraph:

```css
div p
div .paragraph
```

Heading:

```css
div h1
div #main-heading
```

Class aur ID selectors zyada specific hain, is liye unki border styling final result mein jeetti hai.

## Specificity Yaad Rakhna

Simple order:

```text
ID > Class > Element
```

Is liye `#main-heading` wali styling normal `h1` selector se stronger hoti hai.

## Common Mistakes

- Specificity ko ignore karna.
- Same property multiple selectors mein likh kar confuse ho jana.
- Class aur ID symbols mix karna.

## Best Practice

Practice ke liye ID selector theek hai, lekin real reusable CSS mein class selector zyada useful hota hai.
