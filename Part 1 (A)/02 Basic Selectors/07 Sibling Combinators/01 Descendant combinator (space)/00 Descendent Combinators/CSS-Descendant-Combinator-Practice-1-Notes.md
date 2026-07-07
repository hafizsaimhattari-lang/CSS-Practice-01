# Descendant Combinator - Practice 1

Descendant combinator (space) ki pehli practice mein `div` ke andar headings aur paragraphs ko alag styles di gayi hain.

## Files

| File | Kaam |
|------|------|
| `01 Descendent Selector.html` | Multiple `div`, `h1` aur `p` elements |
| `01 Descendent Selector.css` | `div h1` aur `div p` selectors |

## Practice Selectors

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

`div p` ko **div ke andar paragraph** aur `div h1` ko **div ke andar heading** parhein.

## Grouping Bhi Mumkin Hai

```css
div p, div h1 {
    border: 2px solid black;
    padding: 10px;
}
```

Comma ke dono taraf complete selectors likhna zaroori hai.

## Natija

- `div` ke andar sab `p` red hote hain.
- `div` ke andar sab `h1` blue hote hain.
- `div` se bahar ka `p` ya `h1` in rules se match nahi karega.
- Space direct aur deeply nested dono descendants ko select kar sakti hai.

## Practice Ka Purpose

Ye file descendant combinator ka basic behavior repeat karwati hai.

Yahan main focus ye hai ke selector mein space ka matlab hota hai:

```text
andar kahin bhi
```

Example:

```css
div p
```

Iska matlab sirf immediate child nahi, balki `div` ke andar kahin bhi paragraph ho to target ho sakta hai.

## Common Mistakes

- Space ko ignore kar dena.
- `div p` aur `div > p` ko same samajhna.
- Bahar ke paragraph par style apply hone ki expectation rakhna.

## Best Practice

Descendant selectors useful hain, lekin unhein bohat zyada deeply nested mat banao.

Readable selector:

```css
.content p {
  color: red;
}
```
