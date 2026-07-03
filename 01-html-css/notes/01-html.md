# HTML Notes

## What is HTML?
- HTML = HyperText Markup Language
- Gives structure to a webpage.
- Think of it as the skeleton of a website.

---

## Basic Structure

```html
<!DOCTYPE html>
<html>
<head>
  <title>My Page</title>
</head>
<body>

</body>
</html>
```

- `<html>` → Entire webpage
- `<head>` → Information for browser (not shown)
- `<body>` → Visible content

---

## Common Tags

### Headings

```html
<h1>Main Heading</h1>
<h2>Section</h2>
<h3>Subsection</h3>
```

Use only ONE `<h1>` per page.

---

### Paragraph

```html
<p>Hello World</p>
```

---

### Links

```html
<a href="https://example.com">Visit</a>
```

Open in new tab:

```html
<a href="https://example.com"
   target="_blank"
   rel="noopener noreferrer">
```

---

### Images

```html
<img src="image.jpg" alt="Description">
```

Always add `alt`.

---

### Lists

Unordered

```html
<ul>
  <li>Item</li>
</ul>
```

Ordered

```html
<ol>
  <li>Item</li>
</ol>
```

---

### Forms

```html
<form>

<label for="email">Email</label>
<input
  type="email"
  id="email"
  name="email">

<button>Submit</button>

</form>
```

Always connect:

`label for` ↔ `input id`

---

## Semantic Tags

Use these instead of many divs.

```html
<header>
<nav>
<main>
<section>
<footer>
```

Makes HTML meaningful.

---

## id vs class

### id

- Unique
- Used for:
  - Navigation (`href="#projects"`)
  - JavaScript
  - Sometimes CSS

Example

```html
<section id="projects">
```

---

### class

- Reusable
- Mainly for CSS

```html
<div class="card">
```

---

## name

Mostly used in forms.

```html
<input
name="email">
```

The browser sends:

```
email = abc@gmail.com
```

---

## div vs section

### div

Generic container.

```
Just a box.
```

---

### section

Meaningful part of page.

```
About
Projects
Contact
```

Use section for page areas.

Use div to organize things inside.

---

## Good Habits

✅ Semantic HTML

✅ Meaningful class names

✅ One `<h1>` per page

✅ Always use `alt` on images

✅ Connect labels with inputs

✅ Keep indentation clean

---

## Mistakes I Made

❌ IDs with spaces

```html
id="about me"
```

✅

```html
id="about-me"
```

---

❌ Empty ids

```html
<input id="">
```

✅

```html
<input id="email">
```

---

❌ Empty names

```html
name=""
```

Give meaningful names.

---

❌ Empty links

```html
href=""
```

Instead:

```html
href="#projects"
```