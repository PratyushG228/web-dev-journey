# CSS Notes

## What is CSS?

CSS styles HTML.

Think:

HTML = Structure

CSS = Appearance

---

## Link CSS

```html
<link rel="stylesheet" href="style.css">
```

---

## Selectors

Tag

```css
p {}
```

Class

```css
.card {}
```

ID

```css
#projects {}
```

---

## Common Properties

### Colors

```css
color:
background-color:
```

---

### Typography

```css
font-family:
font-size:
font-weight:
line-height:
```

---

### Box Model

Every element has:

```
Margin

Border

Padding

Content
```

---

### Spacing

Outside

```css
margin:
```

Inside

```css
padding:
```

---

### Borders

```css
border:
border-radius:
```

---

## Flexbox

Turn parent into flex container.

```css
display:flex;
```

Main properties

```css
display:flex;
flex-direction:
justify-content:
align-items:
gap:
flex-wrap:
```

---

## Parent vs Child

Parent controls layout.

```css
display
flex
justify-content
align-items
gap
```

Child controls itself.

```css
padding
margin
border
background
flex
width
height
```

---

## flex:1

Applied on children.

```css
.card{
    flex:1;
}
```

Makes children share space equally.

---

## Responsive Design

Viewport

```html
<meta name="viewport"
content="width=device-width, initial-scale=1.0">
```

Media Query

```css
@media (max-width:700px){

}
```

Used to change layout on smaller screens.

---

## Smooth Scroll

```css
html{
scroll-behavior:smooth;
}
```

---

## Hover

```css
a:hover{
color:blue;
}
```

Transition

```css
a{
transition:color .3s;
}
```

---

## Specificity

Priority

```
Inline

↓

ID

↓

Class

↓

Tag
```

---

## Inheritance

Usually inherited

- color
- font-family
- font-size
- line-height

Not inherited

- margin
- padding
- border
- width
- height

---

## DevTools

Use Inspect (F12)

Check:

- Box model
- Applied CSS
- Edit styles live

---

## Good Habits

✅ Keep CSS organized

```
Global

Layout

Navigation

Cards

Footer
```

✅ Use classes more than IDs

✅ Use meaningful names

✅ Use `max-width`

```css
margin:0 auto;
```

to center content.

---

## Mistakes I Made

❌

```css
.project-container{
flex:1;
}
```

✅

```css
.project-card{
flex:1;
}
```

---

❌

```css
transition:.5s;
```

✅

```css
transition:color .5s;
```

---

❌

Forgot

```css
gap:
```

between flex items.

---

❌

Forgot

```css
margin:auto;
```

for centered layout.

---

## Folder Structure

```
project/

index.html
style.css

images/
assets/
```