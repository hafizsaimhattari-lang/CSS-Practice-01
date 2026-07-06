# Child Combinator (`>`) - Mukammal Notes

## Kya Hai?

Child combinator (`>`) parent ke sirf **direct child** ko select karta hai. Zyada andar nested descendant is selector se select nahi hota.

```css
parent > child {
    property: value;
}
```

`>` ko Roman Urdu mein **"ka seedha bacha"** parh sakte hain.

```css
div > p {
    color: blue;
}
/* div ka direct-child p */
```

---

## Hamari Practice Files

| File | Kaam |
|------|------|
| `01 Child-Combinator.html` | Direct aur nested children ki basic HTML structure |
| `01 Child-Combinator.css` | Element aur class selectors ke sath `>` ki practice |

### Practice HTML

```html
<section class="parent-box">
    <h2>Direct Child Heading</h2>
    <p>Yeh direct child hai.</p>

    <div class="nested-box">
        <p>Yeh nested paragraph hai.</p>
    </div>
</section>
```

### Practice CSS Ki Samajh

```css
.parent-box > h2 {
    color: yellow;
}

.parent-box > p {
    color: skyblue;
}
```

- `h2` aur pehla `p`, `.parent-box` ke direct children hain; dono select honge.
- `.nested-box` ke andar wala `p`, `.parent-box` ka direct child nahi; woh select nahi hoga.

```css
header > h1 { color: red; }
.family-list > li { color: chartreuse; }
```

Pehla rule `header` ka direct `h1` aur doosra rule list ke direct `li` children select karta hai.

---

## Zaroori Rules

- Left side par parent ka selector hota hai.
- Right side par required direct child ka selector hota hai.
- Beech mein koi aur wrapper aa jaye to match toot jata hai.
- Element, class aur ID kisi bhi selector ke sath use ho sakte hain.
- Whitespace optional hai, lekin `parent > child` likhna zyada readable hai.

---

## Descendant Se Farq

```css
div p   { }  /* Sab andar wale p (kisi bhi depth pe) */
div > p { }  /* Sirf seedha bacha p */
```

### Example

```html
<div>
    <p>Direct child - dono selectors se milega.</p>
    <article>
        <p>Nested - sirf descendant selector se milega.</p>
    </article>
</div>
```

---

## Selector Chain

```css
main > section > p {
    color: green;
}
```

Is mein `section`, `main` ka direct child aur `p`, `section` ka direct child hona chahiye.

---

## Real-World Use Cases

```css
nav > a { text-decoration: none; }
.card > .title { font-weight: bold; }
ul > li { margin-bottom: 8px; }
form > label { display: block; }
```

Child combinator tab useful hai jab component ke sirf apne direct elements style karne hon aur nested components ko bachana ho.

---

## Common Mistakes

```css
/* Agar p div ke andar kisi article mein hai to yeh match nahi karega */
div > p { color: red; }

/* Deep nested p bhi chahiye to space use karo */
div p { color: red; }
```

- `>` ko arrow samajh kar direction ulta na likho: pehle parent, phir child.
- Child combinator sibling ko select nahi karta; yeh parent-child relation ke liye hai.

---

## Summary

`A > B` ka matlab hai: woh `B` select karo jo `A` ka bilkul direct child ho. Agar `B` kisi aur element ke andar nested ho to woh match nahi karega.
