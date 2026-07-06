# CSS Combinators - Mukammal Notes

> Is folder ka naam `Sibling Combinators` hai, lekin is mein do nesting combinators (` ` aur `>`) aur do sibling combinators (`+` aur `~`) cover kiye gaye hain.

## Sibling Kya Hote Hain?
Jab do ya zyada elements ek hi parent ke andar hon to unhe Sibling (bhai-bhan) kehte hain.

```html
<div>
    <h1>Heading</h1> <!-- Sibling -->
    <p>Para 1</p>    <!-- Sibling -->
    <p>Para 2</p>    <!-- Sibling -->
</div>
```

---

## Folder Structure

```
07 Sibling Combinators/
|-- 01 Descendant combinator (space)/
|-- 02 Child combinator/
|-- 03 Next sibling combinator (+)/
|-- 04 Subsequent-sibling combinator (~)/
```

---

## Char Relationship Combinators

### 1. Descendant Combinator (Space)
```css
div p { color: red; }
/* div ke ANDAR ke SARE p - chahe kitna andar ho */
```

### 2. Child Combinator (>)
```css
div > p { color: blue; }
/* div ke SEEDHE BACHY p sirf */
```

### 3. Next Sibling Combinator (+)
```css
h1 + p { color: green; }
/* h1 ke TURANT baad wala SIRF EK p */
```

### 4. Subsequent Sibling Combinator (~)
```css
h1 ~ p { color: orange; }
/* h1 ke baad ke SARE p siblings */
```

---

## Practice File Se Code (`03 Next sibling combinator (+)/`)

```html
<div><ul><li>Item 1</li><li>Item 2</li></ul></div>
<h1>Adjacent Sibling Combinator Test</h1>
<p>Yeh h1 ke turant baad hai...</p>

<h1 class="main-heading">Test with class</h1>
<p class="paragraph">Yeh class wala para...</p>
```

---

## Quick Reference

| Symbol | Relation | Adjacency | Matches |
|--------|----------|-----------|---------|
| space | Ancestor → descendant | Direct hona zaroori nahi | Andar ke tamam matches |
| `>` | Parent → child | Direct hona zaroori | Direct children |
| `+` | Sibling → sibling | Bilkul foran | Zyada se zyada ek |
| `~` | Sibling → sibling | Beech mein elements ho sakte hain | Baad ke tamam matches |

---

## Same HTML Par Charon Ka Asar

```html
<section>
    <h2>Heading</h2>
    <p>Direct paragraph 1</p>
    <div><p>Nested paragraph</p></div>
    <p>Direct paragraph 2</p>
</section>
```

```css
section p   { } /* Teenon p */
section > p { } /* Dono direct p */
h2 + p      { } /* Sirf direct paragraph 1 */
h2 ~ p      { } /* Dono direct paragraph siblings */
```

`h2 ~ p` nested paragraph ko select nahi karta, kyun ke uska parent `div` hai.

---

## Real-World Use Cases

```css
li + li { border-top: 1px solid gray; }
label + input { margin-left: 10px; }
h2 ~ p { color: #555; }
nav > a { font-weight: bold; }
```

---

## Common Mistakes

- Descendant aur child combinators ko sibling combinators na samjhein.
- `+` aur `~` mein dono matched elements ka parent same hota hai.
- `A + B` aur `A ~ B` sirf `A` ke baad ke elements dekhte hain.
- Selector ki right side wala element hi style hota hai; left side context deta hai.

---

## Summary

Combinator do selectors ke darmiyan HTML relationship batata hai: andar, direct child, foran agla sibling, ya baad ke siblings. Sahi combinator se selector precise aur predictable rehta hai.
