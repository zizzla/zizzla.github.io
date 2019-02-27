---
layout: default
title: Zizzla Patterns
---
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
<script>
  function cssPropertyValue(element, property) {
    var element = document.querySelector(element)
    return cssValue = getComputedStyle(element).getPropertyValue(property)
  }
</script>

## About
Zimplizzity unites

## Color
<div class="card-deck">
  <div class="card text-white bg-primary">
    <div class="card-body">
      <h5 class="card-title">bg-primary</h5>
      <p class="card-text">
        <script>
          var cssValue = cssPropertyValue('.bg-primary', 'background-color');
          document.write(cssValue);
        </script>
      </p>
    </div>
  </div>
  <div class="card text-white bg-secondary">
    <div class="card-body">
      <h5 class="card-title">bg-secondary</h5>
      <p class="card-text">
        <script>
          var cssValue = cssPropertyValue('.bg-secondary', 'background-color');
          document.write(cssValue);
        </script>
      </p>
    </div>
  </div>
  <div class="card text-white bg-info">
    <div class="card-body">
      <h5 class="card-title">bg-info</h5>
      <p class="card-text">
        <script>
          var cssValue = cssPropertyValue('.bg-info', 'background-color');
          document.write(cssValue);
        </script>
      </p>
    </div>
  </div>
</div>

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
