# Descendant Combinator (Space) - Mukammal Notes

## Kya Hai?

Descendant combinator kisi ancestor ke andar maujood tamam matching descendants ko select karta hai. Dono selectors ke darmiyan space iska symbol hai.

```css
ancestor descendant {
    property: value;
}
```

Space ko **"ke andar"** parhein:

```css
div p {
    color: red;
}
/* div ke andar ke tamam p */
```

Descendant direct child bhi ho sakta hai aur kai levels andar nested bhi.

---

## Sub-folders

| Folder | Kaam |
|--------|------|
| `00 Descendent Combinators/` | Pehli practice |
| `00 Descendent Combinators (2)/` | Doosri practice |

### Practice 1

```css
div p { color: red; }
div h1 { color: blue; }
```

Pehli practice element selectors ke zariye `div` ke andar headings aur paragraphs target karti hai.

### Practice 2

```css
div p { border: 1px solid white; }
div .paragraph { border: 1px solid yellow; }
div #main-heading { border: 1px solid yellow; }
```

Doosri practice dikhati hai ke right side par element, class ya ID selector aa sakta hai.

---

## Direct Aur Deep Descendant

```html
<section>
    <p>Direct child paragraph</p>
    <article>
        <p>Deep nested paragraph</p>
    </article>
</section>
```

```css
section p { color: green; }
```

Dono paragraphs select honge, kyun ke dono `section` ke descendants hain.

---

## Descendant Aur Child Ka Farq

| Selector | Kya Select Karta Hai? |
|----------|------------------------|
| `section p` | Kisi bhi depth ka matching `p` |
| `section > p` | Sirf direct-child `p` |

---

## Multiple Levels

```css
nav ul li a {
    color: white;
}
```

Yeh woh `a` select karta hai jo `li` ke andar, `li` `ul` ke andar, aur `ul` `nav` ke andar ho. Bohat lambi chain fragile ho sakti hai; reusable class aksar zyada asaan hoti hai.

---

## Common Mistakes

- `div,p` grouping hai; `div p` descendant selector hai.
- Space nazar nahi aati, is liye selector ko dhyan se parhein.
- `div p` sirf direct child tak limited nahi hota.
- Bohat broad selector nested components ko bhi unintended style de sakta hai.

---

## Summary

`A B` ka matlab hai: `A` ke andar maujood tamam matching `B` descendants select karo, chahe woh direct children hon ya zyada levels andar.
