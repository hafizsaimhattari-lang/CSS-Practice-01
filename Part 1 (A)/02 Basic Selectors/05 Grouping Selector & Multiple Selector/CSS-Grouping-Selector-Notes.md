# CSS Grouping Selector - Mukammal Notes

## Grouping Selector Kya Hai?
Kai elements par ek jaisi CSS lagani ho to unhe comma (`,`) se group karke style karte hain. Code repeat nahi hota.

```css
selector1, selector2, selector3 {
    property: value;
}
```

---

## Practice 1 (`1st/` folder) - Basic Grouping

### Grouping ke bina (repetition):
```css
h1 { color: blue; font-family: Arial; }
h2 { color: blue; font-family: Arial; }
h3 { color: blue; font-family: Arial; }
p  { color: blue; font-family: Arial; }
```

### Grouping ke sath (clean):
```css
h1, h2, h3, p {
    color: blue;
    font-family: Arial;
}
```

---

## Practice 2 (`2nd/` folder) - Mixed Selectors

Elements, classes aur IDs ek group mein:
```css
h1, .intro, #hero {
    font-size: 24px;
    margin-bottom: 10px;
}
```

---

## Multi-line Style (Zyada Readable)

```css
h1,
h2,
h3,
.highlight {
    font-family: Arial;
    line-height: 1.5;
}
```

---

## Kab Use Karein?
| Situation | Use |
|-----------|-----|
| Kai tags ko ek jaisi font | Grouping |
| Heading + paragraph ek rang | Grouping |
| Kai classes ko reset karna | Grouping |

---

## Yaad Rakho
```
Grouping = Code kam, kaam zyada (DRY Principle)
```
