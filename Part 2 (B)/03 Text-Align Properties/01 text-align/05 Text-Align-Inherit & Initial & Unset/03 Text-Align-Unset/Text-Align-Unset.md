# `text-align: unset`

## Introduction

`text-align: unset;` ek CSS keyword value hai jo property ke behavior ko is baat ke mutabiq decide karti hai ke woh property **inherited** hai ya **non-inherited**.

`text-align` ek **inherited property** hai, is liye `text-align: unset;` ka behavior aksar `text-align: inherit;` jaisa hota hai.

---

## Syntax

```css
text-align: unset;
```

---

## Kaise Kaam Karti Hai?

`unset` do tarah se kaam karti hai:

* Agar property inherited ho, to `unset` parent ki value inherit kar leti hai.
* Agar property inherited na ho, to `unset` browser ki default (`initial`) value use karti hai.

Kyun ke `text-align` inherited property hai, is liye `text-align: unset;` parent ki alignment ko follow karta hai.

---

## Kab Use Hoti Hai?

Real-world projects mein `text-align: unset;` ka use bohat kam hota hai.

Developers aksar:

* `text-align: left;`
* `text-align: right;`
* `text-align: center;`
* `text-align: justify;`
* `text-align: start;`
* `text-align: end;`

ya phir zarurat par `inherit` ko prefer karte hain, kyun ke us ka purpose zyada clear hota hai.

---

## Important Note

`text-align: unset;` ko yaad rakhna achha hai, lekin is ki alag se bohat zyada practice karna zaroori nahi hota. Is property ka concept samajhna kaafi hai, kyun ke practical projects mein iska istemal bohat kam dekhne ko milta hai.

---

## Summary

* `unset` ek CSS keyword value hai.
* `text-align` inherited property hai.
* `text-align: unset;` parent ki alignment ko follow karta hai.
* Real projects mein iska use bohat kam hota hai.
* Is property ka concept yaad rakhna practice se zyada important hai.
