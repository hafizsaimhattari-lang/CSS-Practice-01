# Practice 02 - Focus, Hover, Active

## Is practice ka maqsad

Is practice ka maqsad `:focus`, `:hover`, aur `:active` ko compare karna hai.

Ye teeno pseudo classes user interaction ke sath kaam karti hain, lekin teeno ka kaam different hota hai.

## Files

```text
02 Focus Pseudo Class.html
02 Focus-Pseudo-Class.css
```

## HTML file me kya hai?

HTML file me ye elements hain:

```html
<h1>Pseudo Classes Test</h1>
<input type="text" placeholder="Click Here" class="input-field">
<button type="button">Hover / Click Me</button>
<a href="#">Simple Link</a>
```

Is code me:

- `input` focus test ke liye hai
- `button` hover aur active test ke liye hai
- `a` link hover aur active test ke liye hai

## CSS me `:focus`

```css
.input-field:focus {
  background-color: lightgray;
  border: 3px solid red;
}
```

Iska matlab:

Jab input field focus me hogi, uska background light gray aur border red ho jayega.

## CSS me `:hover`

```css
button:hover {
  background-color: yellow;
  border: 3px solid green;
  border-radius: 10px;
}
```

Iska matlab:

Jab mouse button ke upar hoga, button ka background yellow aur border green ho jayega.

## CSS me `:active`

```css
button:active {
  background-color: blue;
  color: white;
  border: 3px solid yellow;
  border-radius: 10px;
}
```

Iska matlab:

Jab user button ko press kar raha hoga, button blue ho jayega.

## Link states

```css
a:hover {
  color: red;
}

a:active {
  color: white;
}
```

Iska matlab:

- Link par mouse hover hoga to color red ho jayega
- Link click/press hoga to color white ho jayega

## `:focus`, `:hover`, aur `:active` ka farq

| Pseudo Class | Kab chalti hai? | Example |
| --- | --- | --- |
| `:focus` | Jab element selected/focused ho | Input field click ya Tab se select |
| `:hover` | Jab mouse element ke upar ho | Button par mouse le jana |
| `:active` | Jab element press ho raha ho | Button click hold karna |

## Practice result

Is practice ke baad clear hota hai ke:

- `:focus` selected element ke liye hoti hai
- `:hover` mouse over ke liye hoti hai
- `:active` click/press moment ke liye hoti hai

Short line:

`:focus` selection ke liye, `:hover` mouse ke liye, aur `:active` pressing ke liye hoti hai.

