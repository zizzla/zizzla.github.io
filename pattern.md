---
layout: default
title: Zizzla Patterns
---
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
<script>
  function showCss(attribute) {
    const element = document.querySelector(attribute)
    const style = getComputedStyle(element)
    console.log(style)
    return style
  }
</script>

## About
Zimplizzity unites

## Color

<div class="card text-white bg-primary mb-3" style="max-width: 18rem;">
  <!--div class="card-header">Header</div-->
  <div class="card-body">
    <h5 class="card-title">Primary card title</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
</div>
<script>
showCss('.bg-primary');
const color = style.color;
document.write(color);
</script>

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
