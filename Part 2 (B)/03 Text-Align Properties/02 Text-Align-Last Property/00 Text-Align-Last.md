# `text-align-last`

## Introduction

`text-align-last` ek CSS property hai jo **sirf paragraph ya text block ki aakhri (last) line** ki alignment ko control karti hai.

Ye property puri paragraph ki alignment change nahi karti, balki sirf last line ki position ko control karti hai.

---

## Syntax

```css
text-align-last: value;
```

---

## Common Values

```css
text-align-last: auto;
text-align-last: left;
text-align-last: right;
text-align-last: center;
text-align-last: justify;
text-align-last: start;
text-align-last: end;
```

---

## Values ki Wazahat

### `auto`

Browser default behavior follow karta hai.

### `left`

Last line ko left side par align karta hai.

### `right`

Last line ko right side par align karta hai.

### `center`

Last line ko center mein align karta hai.

### `justify`

Last line ko bhi justify karne ki koshish karta hai.

### `start`

Last line ko language ki starting side par align karta hai.

* LTR → Left
* RTL → Right

### `end`

Last line ko language ki ending side par align karta hai.

* LTR → Right
* RTL → Left

---

## Kab Use Hoti Hai?

Ye property zyada tar `text-align: justify;` ke sath use ki jati hai, kyun ke `justify` mein aakhri line aksar justify nahi hoti. `text-align-last` us last line ki alignment ko control karne ke liye use hoti hai.

---

## Important Notes

* Ye **sirf last line** par apply hoti hai.
* Puri paragraph ki alignment `text-align` control karta hai.
* Asar tab zyada nazar aata hai jab paragraph multiple lines mein ho.
* Agar paragraph sirf ek line ka ho, to `text-align-last` ka koi khaas visible effect nahi hota.

---

## Summary

* `text-align-last` sirf last line ki alignment control karti hai.
* Ye puri paragraph ki alignment change nahi karti.
* Is ki sab se common values `left`, `right`, `center`, `justify`, `start`, aur `end` hain.
* Ye property zyada tar `text-align: justify;` ke sath use hoti hai.
* Long paragraphs par iska effect sab se clearly nazar aata hai.
