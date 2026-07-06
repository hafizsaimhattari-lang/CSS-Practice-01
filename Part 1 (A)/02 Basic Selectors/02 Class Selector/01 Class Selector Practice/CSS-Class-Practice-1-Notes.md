# Class Selector - Practice 1

External CSS ke sath class selector ki pehli practice.

## Files
| File | Kaam |
|------|------|
| `01 Class Selector.html` | HTML mein class lagai |
| `01 Class Selector.css` | CSS mein `.class` define ki |

## Code
```html
<h2 class="heading-highlight">Primary Heading</h2>
<p class="paragraph-highlight">This paragraph shares the exact same design.</p>
<p class="paragraph-highlight">This is another paragraph styled simultaneously.</p>
```
```css
body { background-color: black; }
.heading-highlight {
    color: white; background-color: red;
    padding: 10px; border-radius: 5px; text-align: center;
}
.paragraph-highlight {
    color: white; background-color: red;
    padding: 10px; border-radius: 5px; text-align: center;
}
```

**Seekha:** Ek hi class kai elements par apply ho sakti hai.
