# CSS Combinators - Mukammal Notes

> Is folder ka naam `Sibling Combinators` hai, lekin is mein do nesting combinators (` ` aur `>`) aur do sibling combinators (`+` aur `~`) cover kiye gaye hain.

## Sibling Kya Hote Hain?
Jab do ya zyada elements ek hi parent ke andar hon to unhe Sibling (bhai-bhan) kehte hain.

```html
<div>
    <h1>Heading</h1>   <- Sibling
    <p>Para 1</p>      <- Sibling
    <p>Para 2</p>      <- Sibling
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

| Symbol | Naam | Matlab |
|--------|------|--------|
| space | Descendant | Andar koi bhi matching descendant |
| `>` | Child | Seedha bacha sirf |
| `+` | Adjacent Sibling | Agla ek bhai |
| `~` | Subsequent Sibling | Baad ke tamam matching siblings |

---

## Real-World Use Cases

```css
li + li { border-top: 1px solid gray; }
label + input { margin-left: 10px; }
h2 ~ p { color: #555; }
nav > a { font-weight: bold; }
```
