# CSS Descendant Selector - Mukammal Notes

## Descendant Selector Kya Hai?
Parent element ke andar wale specific elements ko target karta hai. Dono selectors ke beech space rakha jata hai.

```css
parent child {
    property: value;
}
```
**Space = "Ke Andar"**

---

## Practice Files: `01 First/` aur `02 Second/`

### Basic Example:
```html
<div>
    <p>Yeh div ke ANDAR hai - style milegi.</p>
</div>
<p>Yeh div ke BAHAR hai - style nahi milegi.</p>
```

```css
div p {
    color: red;  /* Sirf div ke andar wala p */
}
```

---

## Deep Nesting Bhi Kaam Karta Hai

```html
<section>
    <div>
        <article>
            <p>Yeh bhi mil jayega!</p>
        </article>
    </div>
</section>
```

```css
section p { color: blue; }  /* Kisi bhi depth ka p */
```

---

## Real-World Use Cases

```css
nav a { color: white; text-decoration: none; }
.card p { font-size: 14px; color: #555; }
thead th { background-color: darkblue; color: white; }
```

---

## Descendant vs Child Farq

```css
div p   { }  /* Sab andar wale p (kisi bhi depth) */
div > p { }  /* Sirf seedha bacha p */
```
