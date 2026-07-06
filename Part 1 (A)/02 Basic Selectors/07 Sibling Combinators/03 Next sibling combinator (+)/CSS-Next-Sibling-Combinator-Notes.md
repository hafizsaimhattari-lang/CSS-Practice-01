# Next Sibling Combinator (+) - Mukammal Notes

## Kya Hai?
Next Sibling Combinator (`+`) sirf ek element ke turant baad aane wale sibling ko target karta hai.

```css
h1 + p { color: green; }
/* h1 ke FORAN baad wala sirf EK p */
```

---

## Hamari Practice File Se Code

```html
<!-- Element selectors ke sath -->
<div><ul><li>Item 1</li><li>Item 2</li></ul></div>
<h1>Adjacent Sibling Combinator Test</h1>
<p>Lorem ipsum... <- Yeh h1 ke turant baad, style milegi</p>

<div><ul>...</ul></div>
<h1>Adjacent Sibling Combinator Test</h1>
<p>Lorem ipsum... <- Phir se ek h1 + p</p>

<!-- Class ke sath -->
<div><ol>...</ol></div>
<h1 class="main-heading">Test</h1>
<p class="paragraph">Lorem... <- .main-heading + .paragraph</p>

<button type="submit">Submit</button>
```

---

## Important Rules
- Dono elements ek hi parent ke under hon
- Sirf AGLA ek element pakadta hai
- Dono adjacent (bilkul sath) hona zaroori

---

## Next (+) vs Subsequent (~)
```css
h1 + p { }  /* Sirf agla ek p */
h1 ~ p { }  /* Baad ke sare p */
```
