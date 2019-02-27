---
layout: default
title: Zizzla Patterns
---
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
<script>
  function showCss(attribute) {
    const element = document.querySelector(attribute)
    return style = getComputedStyle(element)
  }
</script>

## About
Zimplizzity unites

## Color

<div class="color-swatch bg-primary"></div>

## Typography

## Grid

## Form

## Button
```html_example
<button class="btn btn-primary">Click</button>
<a class="btn btn-secondary" href="#" role="button">Zizzla!</a>

<p>btn-primary:
<script>
showCss('btn-primary');
const color = style.color;
document.write(color);
</script>
```
