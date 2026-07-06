# CSS Universal Selector (*) - Mukammal Notes

## Universal Selector Kya Hai?
Page ke har ek element ko ek sath select karta hai. `*` (asterisk) ka nishaan use hota hai.

```css
* {
    property: value;
}
```

---

## Hamari Practice File: `01 Univercal Selector.html` + `.css`

### CSS:
```css
/* "Page par jo kuch bhi hai, sab ko pakar lo!" */
* {
    text-align: center;
    color: white;
    background-color: black;
    border: 2px solid white;
    border-radius: 10px;
    padding: 10px;
    text-decoration: underline;
}
```

### HTML:
```html
<h1>Univercal Selector Practice</h1>
<p>Lorem ipsum dolor sit, amet consectetur adipisicing elit...</p>
```

**Natija:** Har element - body, h1, p sab - black background, white text, border, gol corners.

### Properties:
| Property | Value | Kaam |
|----------|-------|------|
| `text-align` | `center` | Sab center |
| `color` | `white` | Sab text safeed |
| `background-color` | `black` | Sab ka background kala |
| `border` | `2px solid white` | Sab ke gird border |
| `border-radius` | `10px` | Sab ke corners gol |
| `padding` | `10px` | Har element ke andar jagah |
| `text-decoration` | `underline` | Sab underline |

---

## Sabse Common Use - CSS Reset

```css
/* Har professional CSS file ke sabse upar */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

Browser ki default margin/padding hatane ke liye use karte hain.

---

## Savdhaani
- Bahut powerful hai - har cheez pakad leta hai
- Mostly sirf CSS reset ke liye use karo
- `*` elements select karta hai, pseudo-elements `::before` aur `::after` ko automatically include nahi karta

```css
*,
*::before,
*::after {
    box-sizing: border-box;
}
```

Yeh common reset elements ke sath generated pseudo-elements ko bhi include karta hai.

---

## Universal Selector Ko Scope Karna

```css
.card * {
    font-family: Arial, sans-serif;
}
```

Yeh poore page ki bajaye `.card` ke andar har descendant element select karta hai.

---

## Inheritance Se Farq

```css
body { color: white; }
```

`color` aksar children ko inherit hoti hai. Is ka matlab yeh nahi ke `body` selector ne har child ko direct select kiya. `* { color: white; }` har element par direct declaration lagata hai, jo later inheritance/overrides par different asar daal sakti hai.

---

## Common Mistakes Aur Summary

- `*` se margin, padding, border aur background sab par lagana unexpected layout bana sakta hai.
- Universal selector ki specificity zero hoti hai; class/ID rules aasani se override karte hain.
- Focused reset ke liye use karein, har visual property globally lagane ke liye nahi.
