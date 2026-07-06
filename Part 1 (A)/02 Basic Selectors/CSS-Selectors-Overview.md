# CSS Basic Selectors - Mukammal Overview

## Selectors Kya Hain?
CSS Selector woh tareeqa hai jis se batate hain ke "CSS in elements par lagaao". Is folder mein 7 qisam ke selectors ki practice ki gayi hai.

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
|-- 07 Sibling Combinators/      Bhai-bhan elements
```

---

## Saat Selectors - Ek Nazar Mein

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

/* 7. Sibling Combinators */
h1 + p { color: green; }   /* Next sibling */
h1 ~ p { color: gray; }    /* Subsequent siblings */
div > p { color: blue; }   /* Direct child */
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
| Bhai-bhan elements | Sibling |

---

## CSS Specificity (Kon Jeeta?)
```
!important > Inline > ID > Class > Element > Universal
```
