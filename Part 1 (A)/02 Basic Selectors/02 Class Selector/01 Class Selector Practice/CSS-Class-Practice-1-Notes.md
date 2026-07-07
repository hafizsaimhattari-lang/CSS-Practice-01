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

---

## Har Selector Ka Result

| Selector | Target | Result |
|----------|--------|--------|
| `body` | Poora document body | Black background |
| `.heading-highlight` | Class wali heading | White text, red box |
| `.paragraph-highlight` | Dono class wale paragraphs | Same reusable styling |

`paragraph-highlight` ek hi class name hai jo do `<p>` elements par reuse hua. Browser dono ko same declarations deta hai.

---

## Class Selector Ka Pattern

```html
<element class="class-name">Content</element>
```

```css
.class-name {
    property: value;
}
```

HTML mein class ke sath dot nahi lagta; dot sirf CSS selector mein lagta hai.

---

## Seekha Kya?

- Ek class kai elements par apply ho sakti hai.
- Class name HTML aur CSS mein exact same hona chahiye.
- External stylesheet `<link>` se connect hoti hai.
- Similar styles ko reusable class banana repeated inline CSS se behtar hai.

## Browser Mein Result

Jab page browser mein open hota hai:

- Body ka background black hota hai.
- Heading red background ke sath center mein show hoti hai.
- Dono paragraphs bhi same red box style lete hain.
- Is se clear hota hai ke ek class ko baar baar reuse kiya ja sakta hai.

## Common Mistakes

- HTML mein `class="heading-highlight"` likhna aur CSS mein `.heading-hilight` likh dena.
- CSS selector mein dot (`.`) bhool jana.
- Class name mein space use karna, jaise `heading highlight`; is ka matlab do alag classes hota hai.
- Same styling ko baar baar alag selectors mein repeat karna.

## Best Practice

Agar multiple elements ka design same hai, to class selector use karo.

Class ka naam meaningful rakho, jaise:

```html
<p class="paragraph-highlight">Text</p>
```

Is se baad mein code padhna easy hota hai.
