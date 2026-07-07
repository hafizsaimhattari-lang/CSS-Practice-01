# CSS `:focus` Pseudo Class

## `:focus` kya hoti hai?

`:focus` CSS ki pseudo class hai.

Iska use tab hota hai jab koi element user ke focus me aa jaye.

Simple alfaaz me:

Jab user kisi input field, button, select box, textarea, ya link par click karta hai, ya keyboard se `Tab` press karke us element par aata hai, to woh element focused hota hai.

Us focused element ko style dene ke liye hum `:focus` pseudo class use karte hain.

## Basic syntax

```css
selector:focus {
  property: value;
}
```

Iska matlab:

Jab selected element focus me aaye, tab ye CSS apply ho.

Example:

```css
input:focus {
  border: 2px solid blue;
}
```

Yahan jab user input field par click karega ya keyboard se us par aayega, input ka border blue ho jayega.

## `:focus` ka simple HTML example

```html
<input type="text" placeholder="Enter your name">
```

## `:focus` ka simple CSS example

```css
input:focus {
  background-color: lightyellow;
  border: 2px solid blue;
}
```

Result:

Jab input field focus me aayegi, uska background light yellow aur border blue ho jayega.

## `:focus` kis kis element par lag sakti hai?

`:focus` zyada tar interactive elements par use hoti hai.

Interactive element ka matlab:

Woh element jiske sath user interact kar sakta hai.

Common elements:

- `input`
- `textarea`
- `button`
- `select`
- `a`

Example:

```css
textarea:focus {
  background-color: lightyellow;
}

button:focus {
  outline: 3px solid red;
}

a:focus {
  color: green;
}
```

## `:focus` keyboard ke sath bhi kaam karti hai

`:focus` sirf mouse click se nahi chalti.

Agar user keyboard se `Tab` press karke kisi input, button, ya link par aata hai, tab bhi `:focus` apply hoti hai.

Ye accessibility ke liye bohat important hai, kyun ke har user mouse use nahi karta.

## `outline` aur `border` me farq

`:focus` me hum aksar `outline` ya `border` use karte hain.

### `border`

`border` element ke box ka part hota hai.

Example:

```css
input:focus {
  border: 3px solid red;
}
```

Kabhi kabhi border change karne se element ka size thora move ya shift ho sakta hai.

### `outline`

`outline` element ke bahar draw hota hai.

Example:

```css
button:focus {
  outline: 3px solid white;
}
```

`outline` accessibility ke liye useful hota hai kyun ke ye focus ko clearly show karta hai.

## Important accessibility baat

Kabhi bhi bina replacement ke `outline: none;` use nahi karna chahiye.

Galat:

```css
button:focus {
  outline: none;
}
```

Agar outline remove karni ho, to uski jagah koi aur clear focus style deni chahiye.

Theek:

```css
button:focus {
  outline: 3px solid yellow;
}
```

Ya:

```css
input:focus {
  border: 3px solid blue;
  background-color: lightyellow;
}
```

## `:focus` aur `:hover` me farq

`:hover` tab chalta hai jab mouse kisi element ke upar ho.

`:focus` tab chalta hai jab element selected ya active focus state me ho.

Example:

```css
button:hover {
  background-color: yellow;
}

button:focus {
  outline: 3px solid blue;
}
```

Yahan:

- Mouse button ke upar hoga to `:hover` chalega
- Button click hoga ya keyboard se select hoga to `:focus` chalega

## `:focus` aur `:active` me farq

`:active` sirf us waqt hota hai jab user element ko press kar raha hota hai.

`:focus` click ke baad bhi reh sakta hai.

Example:

```css
button:active {
  background-color: green;
}

button:focus {
  outline: 2px solid red;
}
```

Yahan:

- Button press karte waqt `:active` apply hoga
- Button selected/focused rehne par `:focus` apply hoga

## Practice file 01 ka concept

File:

```text
01 Focus Pseudo Class.html
01 Focus-Pseudo-Class.css
```

Is example me:

- Page ka background black hai
- Heading aur paragraph white hain
- Input par focus karne se input ka background black, text white, aur border white hota hai
- Button par focus karne se button ka color bhi change hota hai

Main selector:

```css
.input-field:focus {
  background-color: black;
  color: white;
  border: 5px solid white;
}
```

Iska matlab:

Jab `.input-field` class wala input focus me aaye, tab us par ye styling apply ho.

## Practice file 02 ka concept

File:

```text
02 Focus Pseudo Class.html
02 Focus-Pseudo-Class.css
```

Is example me `:focus`, `:hover`, aur `:active` ka basic comparison hai.

Is file me:

- Input par focus style lagti hai
- Button par hover style lagti hai
- Button par active style lagti hai
- Link par hover aur active state test hoti hai

Main idea:

```css
.input-field:focus {
  background-color: lightgray;
  border: 3px solid red;
}
```

Yahan input click ya keyboard focus par change hota hai.

## Real life use cases

`:focus` ka use forms me bohat hota hai.

Common examples:

- Login form me selected input highlight karna
- Search box active hone par border color change karna
- Button keyboard se select hone par outline show karna
- Contact form me currently active field ko clear banana
- Website accessibility improve karna

## Common mistakes

### Mistake 1: `:focus` ko hover samajhna

`:focus` aur `:hover` same nahi hain.

`:hover` mouse ke liye hota hai.

`:focus` selected element ke liye hota hai.

### Mistake 2: Input par click karna bhool jana

`:focus` style tabhi dikhegi jab input ya button focus me aaye.

### Mistake 3: `outline: none;` laga dena

Ye keyboard users ke liye problem create karta hai.

Agar outline remove karni ho, to custom focus style zaroor deni chahiye.

### Mistake 4: Non-interactive element par focus expect karna

Normal `div` ya `p` by default focusable nahi hotay.

Form elements aur links normally focusable hotay hain.

## Short summary

`:focus` us element ko style karne ke liye use hoti hai jo user ke focus me ho.

Ye click se bhi aa sakta hai aur keyboard `Tab` se bhi.

Forms aur buttons me `:focus` bohat useful hai.

Best practice:

Focus style hamesha clear aur visible honi chahiye.
