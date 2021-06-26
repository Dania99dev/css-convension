# CSS3 (v0.1.0)

- **OOCSS** is the preferred methodology (Object-Oriented CSS)
- Classes should be in recursive alphabetical order
- Childs of a class should come after the parent class itself
- Only the direct parent class should be written in selector:

```css
.class {
  /* Some styles */
}
.class .childclass {
  /* Some styles */
}
```

- only 2 "`parent child`" pair can be in selector

- Selecting html tags are only allowed when there are no scoped tags:

```html
<div class="class">
  <h1>Heading</h1>
  <p>Paragraph</p>
</div>
<!-- you can select `.class h1` and `.class p` here -->
```

- Ordering for a style group:

  1. Class
  1. Pseudo-elements
  1. Pseudo-classes

- Order of pseudo-elements:

  1. before
  1. after
  1. first-line
  1. first-letter
  1. selection
  1. marker

- Order of pseudo-classes:
  1. hover
  1. click

---

Order of properties:

```css
.class {
  /* Margin and padding */
  /* Display (Flex, grid, etc.) */
  /* Background */
  /* Shadows */
}
```
