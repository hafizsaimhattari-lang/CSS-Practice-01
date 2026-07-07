# Practice 01 - Focus Pseudo Class

## Is practice ka maqsad

Is practice ka maqsad ye samajhna hai ke CSS `:focus` pseudo class input field aur button ke sath kaise kaam karti hai.

## Files

```text
01 Focus Pseudo Class.html
01 Focus-Pseudo-Class.css
```

## HTML file me kya hai?

HTML file me basic structure hai:

```html
<h1>Focus Pseudo Class</h1>
<p>Click on the input field to see the effect of the focus pseudo class.</p>
<input type="text" placeholder="Click here to focus" class="input-field">
<button type="button">Submit</button>
```

Is code me:

- `h1` page ka main title hai
- `p` user ko instruction de raha hai
- `input` focus test ke liye hai
- `button` button focus test ke liye hai
- `class="input-field"` se input ko CSS me target kiya gaya hai

## CSS file me kya hai?

Body ko black background diya gaya hai:

```css
body {
  font-family: Arial, sans-serif;
  background-color: black;
}
```

Heading aur paragraph ko white color diya gaya hai:

```css
h1,
p {
  color: white;
}
```

Input focus state:

```css
.input-field:focus {
  background-color: black;
  color: white;
  border: 5px solid white;
}
```

Iska matlab:

Jab input field par click hoga ya keyboard se focus aayega, input ka background black, text white, aur border white ho jayega.

Button focus state:

```css
button:focus {
  background-color: black;
  color: white;
  border: 2px solid white;
}
```

Iska matlab:

Jab button focus me aayega, uski styling change ho jayegi.

## Important point

`:focus` ke liye element ka selected hona zaroori hai.

Input par click karo ya keyboard se `Tab` press karke input ya button par jao, tab effect clear nazar aayega.

## Practice result

Is practice ke baad samajh aata hai ke:

- `:focus` form elements par kaam karti hai
- Input field focus hone par style change hoti hai
- Button focus hone par style change hoti hai
- Keyboard users ke liye focus style helpful hoti hai

