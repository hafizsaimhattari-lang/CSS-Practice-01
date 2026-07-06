# HTML Mein Sibling Kya Hota Hai?

English mein sibling ka matlab bhai ya behan hota hai. HTML mein woh elements siblings hote hain jin ka **immediate parent same** ho.

```html
<main>
    <h1>Heading</h1>
    <p>Paragraph</p>
    <div>Box</div>
</main>
```

Yahan `h1`, `p` aur `div` siblings hain, kyun ke teeno ka parent `main` hai.

---

## Kaun Sibling Nahi Hai?

```html
<main>
    <section>
        <p>Nested paragraph</p>
    </section>
    <h2>Heading</h2>
</main>
```

`section` aur `h2` siblings hain. Lekin nested `p`, `h2` ka sibling nahi, kyun ke `p` ka parent `section` aur `h2` ka parent `main` hai.

---

## Adjacent Sibling (`+`)

`+` sirf foran agla matching sibling select karta hai.

```css
h1 + p {
    color: green;
}
```

Isay yun parhein: **h1 ke bilkul baad wala p**.

```html
<h1>Heading</h1>
<p>Select hoga</p>
<p>Select nahi hoga</p>
```

---

## Subsequent Sibling (`~`)

`~` pehle element ke baad aane wale tamam matching siblings select karta hai. Beech mein doosre elements ho sakte hain.

```css
h1 ~ p {
    color: orange;
}
```

```html
<h1>Heading</h1>
<p>Select hoga</p>
<span>Beech ka element</span>
<p>Yeh bhi select hoga</p>
```

---

## Jaldi Yaad Rakho

| Symbol | Matlab |
|--------|--------|
| `A + B` | `A` ke foran baad wala ek `B` |
| `A ~ B` | `A` ke baad ke tamam matching `B` siblings |

Dono selectors sirf forward direction mein dekhte hain aur matched elements ka parent same hona chahiye.
