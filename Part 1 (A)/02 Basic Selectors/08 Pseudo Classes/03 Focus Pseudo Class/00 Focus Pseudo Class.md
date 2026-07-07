# CSS `:focus` Pseudo Class

## `:focus` kya hoti hai?

`:focus` ka matlab hai:

Jab user kisi element par click kare, ya keyboard se `Tab` press kar ke us element par aaye, to woh element focus me aa jata hai.

Us focused element ko style dene ke liye CSS me `:focus` use hoti hai.

## Simple example

HTML:

```html
<input type="text" placeholder="Enter your name">
```

CSS:

```css
input:focus {
  border: 2px solid blue;
}
```

Iska matlab:

Jab user input field par click karega, input ka border blue ho jayega.

## `:focus` kahan use hoti hai?

`:focus` zyada tar form elements ke sath use hoti hai.

Jaise:

- input
- textarea
- button
- select
- link

Example:

```css
textarea:focus {
  background-color: lightyellow;
}
```

Jab user textarea par click karega, uska background light yellow ho jayega.

## Button ke sath example

HTML:

```html
<button>Submit</button>
```

CSS:

```css
button:focus {
  outline: 3px solid red;
}
```

Jab button par click hoga ya keyboard se button select hoga, button ke around red outline aa jayegi.

## `:focus` kyun useful hai?

`:focus` se user ko pata chal jata hai ke woh abhi kis field ya button par hai.

Example:

Agar form me 3 input fields hain:

```html
<input type="text" placeholder="Name">
<input type="email" placeholder="Email">
<input type="password" placeholder="Password">
```

CSS:

```css
input:focus {
  background-color: lightblue;
}
```

Ab user jis input par click karega, woh light blue ho jayega.

Is se user ko easily samajh aa jata hai ke woh kis input me typing kar raha hai.

## `:focus` aur `:hover` me farq

`:hover` tab chalta hai jab mouse kisi element ke upar ho.

`:focus` tab chalta hai jab element click ya keyboard se select ho.

Example:

```css
button:hover {
  background-color: black;
  color: white;
}

button:focus {
  outline: 3px solid blue;
}
```

Yahan:

- mouse button ke upar hoga to `:hover` chalega
- button click hoga to `:focus` chalega

## `:focus` aur `:active` me farq

`:active` sirf tab hota hai jab button press ho raha ho.

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

## Complete short example

HTML:

```html
<input type="text" placeholder="Name">
<button>Send</button>
```

CSS:

```css
input:focus {
  border: 2px solid blue;
  background-color: lightyellow;
}

button:focus {
  outline: 3px solid red;
}
```

## Yaad rakhne wali baat

`:focus` ka use tab hota hai jab hume kisi selected input, button, link, ya form element ko style dena ho.

Short line:

`:focus` us element par style lagati hai jo user ne click ya keyboard se select kiya hota hai.
