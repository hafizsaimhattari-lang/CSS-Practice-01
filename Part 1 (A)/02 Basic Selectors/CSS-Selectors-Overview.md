# CSS Basic Selectors - Mukammal Overview

## Selectors Kya Hain?
CSS selector browser ko batata hai ke declaration block kin HTML elements par apply karna hai. Is folder mein simple selectors, combinators aur pseudo-classes ke 8 topic groups practice kiye gaye hain.

---

## Folder Structure

```
02 Basic Selectors/
|-- 01 Element Selector/         Tag naam se select
|-- 02 Class Selector/           .className se select
|-- 03 Id Selector/              #idName se select
|-- 04 Univercal Selector/       * se sab kuch
|-- 05 Grouping Selector/        Kai selectors ek sath
|-- 06 Descendent Selector/      Nested elements
|-- 07 Sibling Combinators/      Element relationships
|-- 08 Pseudo Classes/           Element ki state
```

---

## Topics - Ek Nazar Mein

```css
/* 1. Element Selector */
h1 { color: white; background-color: black; }

/* 2. Class Selector */
.heading-highlight { background-color: red; color: white; }

/* 3. ID Selector */
#special-box { border: 3px solid gold; }

/* 4. Universal Selector */
* { margin: 0; padding: 0; box-sizing: border-box; }

/* 5. Grouping Selector */
h1, h2, h3, p { font-family: Arial; }

/* 6. Descendant Selector */
div p { color: red; }

/* 7. Relationship Combinators */
div > p { color: blue; }   /* Direct child */
h1 + p { color: green; }   /* Next sibling */
h1 ~ p { color: gray; }    /* Subsequent siblings */

/* 8. Pseudo Class */
button:hover { background-color: navy; }
```

---

## Konsa Selector Kab?

| Situation | Selector |
|-----------|----------|
| Sab `<p>` tags | Element |
| Kuch khaas elements | Class |
| Ek specific element | ID |
| Sab ko ek style | Universal |
| Kai elements ek jaisi style | Grouping |
| Parent ke andar wale | Descendant |
| Direct child | Child combinator `>` |
| Foran agla sibling | Next sibling `+` |
| Baad ke matching siblings | Subsequent sibling `~` |
| Hover/click jaisi state | Pseudo class |

---

## Selector Ko Kaise Parhein?

Complex selector ko right se left samajhna useful hota hai:

```css
.card > p.highlight:hover { color: red; }
```

Pehle `.highlight:hover` wala `p` dhoondo, phir check karo ke woh `.card` ka direct child hai.

---

## CSS Specificity (Kaunsa Rule Jeetega?)

Basic priority ko is tarah samjhein:

```
Inline style > ID > Class / attribute / pseudo-class > Element / pseudo-element
```

- Universal selector (`*`) aur combinators (` `, `>`, `+`, `~`) specificity add nahi karte.
- Same specificity ho to neeche/later likha rule jeetta hai.
- `!important` normal declarations ko override karta hai, lekin ise routine styling ke liye avoid karein.

```css
p { color: blue; }       /* Element */
.note { color: green; }  /* Class: yeh jeetega */
#intro { color: red; }   /* ID: agar same element par ho to yeh jeetega */
```

---

## Common Mistakes

- `.class` ke dot aur `#id` ke hash ko bhoolna.
- Grouping comma (`h1, p`) aur descendant space (`h1 p`) ko mix karna.
- `>` ko sibling selector kehna; yeh direct child relation hai.
- Selector ko be-wajah bohat lamba banana, jis se reuse aur override mushkil hota hai.

---

## Summary

Simple selectors element ki pehchan batate hain, combinators elements ka relationship, aur pseudo-classes state ya position. In teenon ko combine karke precise selectors bante hain.
