# Next Sibling Combinator (`+`) - Mukammal Notes

## Kya Hai?
Next Sibling Combinator (`+`), jise Adjacent Sibling Combinator bhi kehte hain, pehle selector ke bilkul foran baad aane wala matching sibling select karta hai.

```css
h1 + p { color: green; }
/* h1 ke FORAN baad wala sirf EK p */
```

---

## Basic Example

```html
<h1>Heading</h1>
<p>Yeh select hoga.</p>
<p>Yeh select nahi hoga.</p>
```

```css
h1 + p { color: green; }
```

Pehla `p`, `h1` ka adjacent sibling hai. Doosre `p` se pehle `p` aa gaya, is liye woh `h1 + p` se match nahi hota.

---

## Important Rules

- Dono elements ek hi parent ke under hon
- Sirf foran agla element check hota hai
- Right-side selector ka match hona zaroori hai
- Beech mein koi doosra **element** aaye to match toot jata hai
- Text aur comments element nahi hote, is liye woh adjacency nahi todte

---

## Hamari Practice Files

| File | Kaam |
|------|------|
| `01 Next sibling combinator (+).html` | Element aur class ke sath basic adjacent siblings |
| `01 Next-sibling-combinator-(+).css` | `div + h1`, `h1 + p` aur `br + button` |
| `02 Next sibling combinator (+).html` | Header, paragraph aur main content structure |
| `02 Next-sibling-combinator-(+).css` | Element, ID aur class ke sath doosri practice |

### Practice 1 Ke Selectors

```css
div + h1 { border: 2px solid white; }
h1 + p { color: yellow; }
div + .main-heading { padding: 10px; }
br + button { border: 2px solid white; }
```

- `div + h1`: `div` ke foran baad wala `h1`.
- `h1 + p`: `h1` ke foran baad wala paragraph.
- `div + .main-heading`: `div` ke foran baad `.main-heading` class wala element.
- `br + button`: sirf tab match hoga jab button se bilkul pehle `br` element ho. Practice HTML mein button se pehle ek aur `br` hai, is liye rule match hota hai.

### Practice 2 Ke Selectors

```css
header + p { color: red; }
#first-br + .first-para { border: 2px solid black; }
```

Pehla rule `header` ke foran baad paragraph aur doosra `#first-br` ke foran baad `.first-para` ko select karta hai.

---

## Next (+) vs Subsequent (~)

```css
h1 + p { }  /* Sirf agla ek p */
h1 ~ p { }  /* Baad ke tamam matching p siblings */
```

| Feature | `+` | `~` |
|---------|-----|-----|
| Same parent | Zaroori | Zaroori |
| Bilkul sath | Zaroori | Zaroori nahi |
| Matches | Zyada se zyada ek | Ek ya kai |

---

## Real-World Use Cases

```css
li + li { border-top: 1px solid gray; }
label + input { margin-left: 8px; }
h2 + p { margin-top: 0; }
.field + .field { margin-top: 16px; }
```

---

## Common Mistakes

- `h1 + p` pehle wala ya door ka paragraph select nahi karta.
- Agar beech mein `<span>` aa jaye to `h1 + p` match nahi karega.
- `+` parent-child relation ke liye nahi; dono matched elements siblings hone chahiye.

---

## Summary

`A + B` ka matlab hai: `A` ke bilkul foran baad aane wala `B` select karo. `A` aur `B` ka parent same hona zaroori hai.
