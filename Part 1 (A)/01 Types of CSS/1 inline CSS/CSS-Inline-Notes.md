# 🎨 Inline CSS - Mukammal Notes

## 📚 Inline CSS Kya Hai?
Inline CSS mein `style=""` attribute **seedha HTML tag ke andar** likha jata hai. Koi alag file ya `<style>` block nahi hota — CSS directly tag ke saath hoti hai.

---

## ✍️ Hamari Practice File: `01 Inline CSS.html`

```html
<!-- h1 ko inline CSS se blue, center aur yellow background diya -->
<h1 style="color: blue; text-align: center; background-color: yellow;">
    Yeh Inline CSS Hai!
</h1>

<!-- paragraph ko green aur bold kiya -->
<p style="color: green; font-weight: bold;">
    Isme har line ko alag se design dena parta hai, jo aagay ja kar azaab ban jata hai!
</p>
```

### Is file mein yeh CSS properties use hui hain:
| Property | Value | Kaam |
|----------|-------|------|
| `color` | `blue`, `green` | Text ka rang |
| `text-align` | `center` | Text ko center karna |
| `background-color` | `yellow` | Peeche ka rang |
| `font-weight` | `bold` | Text bold karna |

---

## ✅ Inline CSS Ke Fayde
- Chhoti testing ke liye jaldi kaam karta hai
- Sirf ek element ko specific style deni ho toh useful

## ❌ Inline CSS Ke Nuqsanat
- **Maintainability zero** — 100 elements hoon toh 100 jagah likhna padega
- HTML code garba aur bhari ho jata hai
- **Professional projects mein bilkul use nahi hoti**
- CSS reuse nahi ho sakti

---

## 🔑 Yaad Rakho
```
Inline CSS = Sabse buri practice
Sirf seekhne ke liye padho, real kaam mein mat use karo!
```
