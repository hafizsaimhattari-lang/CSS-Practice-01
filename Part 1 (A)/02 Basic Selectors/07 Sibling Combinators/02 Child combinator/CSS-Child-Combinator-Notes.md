# Child Combinator (>) - Notes

## Kya Hai?
Child combinator `>` sirf parent ka seedha bacha pakadta hai - andar andar wale nahi.

```css
div > p { color: blue; }
/* Sirf div ka seedha p */
```

## Descendant Se Farq
```css
div p   { }  /* Sab andar wale p (kisi bhi depth pe) */
div > p { }  /* Sirf seedha bacha p */
```

## Example
```html
<div>
    <p>Seedha bacha - MILEGA</p>
    <article>
        <p>Deep nested - NAHI MILEGA (child se)</p>
    </article>
</div>
```
