---
layout: default
title: Zizzla Patterns
---
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
<script>
  function cssPropertyValue(element, property) {
    var element = document.querySelector(element)
    //var style = getComputedStyle(element)
    //console.log(style)
    return cssValue = getComputedStyle(element).getPropertyValue(property)
  }
</script>

## About
Zimplizzity unites

---

## Colors

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

---

## Typography

<div class="h1">h1
  <script>
    var cssValue = cssPropertyValue('.h1', 'font-size');
    document.write(cssValue);
  </script>
</div>
<div class="text-muted">
  <script>
    var cssValue = cssPropertyValue('.h1', 'font-family');
    document.write(cssValue);
  </script>
</div>

<div class="h2">h2
  <script>
    var cssValue = cssPropertyValue('.h2', 'font-size');
    document.write(cssValue);
  </script>
</div>
<div class="text-muted">
  <script>
    var cssValue = cssPropertyValue('.h2', 'font-family');
    document.write(cssValue);
  </script>
</div>

<div class="h3">h3
  <script>
    var cssValue = cssPropertyValue('.h3', 'font-size');
    document.write(cssValue);
  </script>
</div>
<div class="text-muted">
  <script>
    var cssValue = cssPropertyValue('.h3', 'font-family');
    document.write(cssValue);
  </script>
</div>

<div class="p">p
  <script>
    var cssValue = cssPropertyValue('.p', 'font-size');
    document.write(cssValue);
  </script>
</div>
<div class="text-muted">
  <script>
    var cssValue = cssPropertyValue('.p', 'font-family');
    document.write(cssValue);
  </script>
</div>

<div class="text-muted">text-muted
  <script>
    var cssValue = cssPropertyValue('.text-muted', 'font-size');
    document.write(cssValue);
  </script>
</div>
<div class="text-muted">
  <script>
    var cssValue = cssPropertyValue('.text-muted', 'font-family');
    document.write(cssValue);
  </script>
</div>

---

## Grids

### Large devices: col-lg
<div class="text-muted">12 rows is available for <strong>Large</strong> devices: col-lg
</div>

<div class="container">
  <div class="row">
    <div class="col-lg border">
      1 / 12
    </div>
    <div class="col-lg border">
      1 / 12
    </div>
    <div class="col-lg border">
      1 / 12
    </div>
    <div class="col-lg border">
      1 / 12
    </div>
    <div class="col-lg border">
      1 / 12
    </div>
    <div class="col-lg border">
      1 / 12
    </div>
    <div class="col-lg border">
      1 / 12
    </div>
    <div class="col-lg border">
      1 / 12
    </div>
    <div class="col-lg border">
      1 / 12
    </div>
    <div class="col-lg border">
      1 / 12
    </div>
    <div class="col-lg border">
      1 / 12
    </div>
    <div class="col-lg border">
      1 / 12
    </div>
  </div>
</div>

```
<div class="container">
  <div class="row">
    <div class="col-lg border">
      1 / 12
    </div>
    <div class="col-lg border">
      1 / 12
    </div>
    ...
  </div>
</div>
```

### Medium devices: col-md
<div class="text-muted">6 rows is available for <strong>Medium</strong> devices: col-md
</div>

<div class="container">
  <div class="row">
    <div class="col-md border">
      1 / 6
    </div>
    <div class="col-md border">
      1 / 6
    </div>
    <div class="col-md border">
      1 / 6
    </div>
    <div class="col-md border">
      1 / 6
    </div>
    <div class="col-md border">
      1 / 6
    </div>
    <div class="col-md border">
      1 / 6
    </div>
  </div>
</div>

```
<div class="container">
  <div class="row">
    <div class="col-md border">
      1 / 6
    </div>
    <div class="col-md border">
      1 / 6
    </div>
    ...
  </div>
</div>
```
### Small devices: col-sm
<div class="text-muted">3 rows is available for <strong>Small</strong> devices: col-sm
</div>

<div class="container">
  <div class="row">
    <div class="col-sm border">
      1 / 3
    </div>
    <div class="col-sm border">
      1 / 3
    </div>
    <div class="col-sm border">
      1 / 3
    </div>
  </div>
</div>

```
<div class="container">
  <div class="row">
    <div class="col-sm border">
      1 / 3
    </div>
    <div class="col-sm border">
      1 / 3
    </div>
    <div class="col-sm border">
      1 / 3
    </div>
  </div>
</div>
```

### Smallest devices: col

<div class="text-muted">Only 1 row is available for the <strong>Smallest</strong> devices: col
</div>

<div class="container">
  <div class="row">
    <div class="col border">
      1 / 1
    </div>
  </div>
</div>

```
<div class="container">
  <div class="row">
    <div class="col border">
      1 / 1
    </div>
  </div>
</div>
```

---

## Forms

### Email field

<form>
  <label for="inputEmail">Email address</label>
  <input type="email" class="form-control" id="inputEmail" aria-describedby="emailHelp" placeholder="Enter email">
  <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
</form>

```
<form>
  <label for="inputEmail">Email address</label>
  <input type="email" class="form-control" id="inputEmail" aria-describedby="emailHelp" placeholder="Enter email">
  <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
</form>
```

### Phone field

Future feature? [International Telephone Input](https://intl-tel-input.com/)

### Number field

<form>
  <label for="numberInput">Number</label>
  <input type="number" class="form-control" id="numberInput">
</form>

```
<form>
  <label for="numberInput">Number</label>
  <input type="number" class="form-control" id="numberInput">
</form>
```

### Text field

<form>
  <label for="formControlTextarea">Textarea</label>
  <textarea class="form-control" id="formControlTextarea" rows="3"></textarea>
</form>

```
<form>
  <label for="formControlTextarea">Textarea</label>
  <textarea class="form-control" id="formControlTextarea" rows="3"></textarea>
</form>
```

### Grouping and Validating

<form>
  <div class="form-group">
    <label for="validationTextarea1">Textarea 1</label>
    <textarea class="form-control is-invalid" id="validationTextarea1" placeholder="Required textarea" required></textarea>
  </div>
  <div class="form-group">
    <label for="validationTextarea2">Textarea 2</label>
    <textarea class="form-control" id="validationTextarea2" placeholder="Optional textarea"></textarea>
  </div>
</form>

```
<form>
  <div class="form-group">
    <label for="validationTextarea1">Textarea 1</label>
    <textarea class="form-control is-invalid" id="validationTextarea1" placeholder="Required textarea" required></textarea>
  </div>
  <div class="form-group">
    <label for="validationTextarea2">Textarea 2</label>
    <textarea class="form-control" id="validationTextarea2" placeholder="Optional textarea"></textarea>
  </div>
</form>
```

<form>
  <div class="form-row">
    <div class="form-group col-sm">
      <label for="validationInputNumber">Number</label>
      <input type="number" class="form-control is-invalid" id="validationInputNumber" placeholder="Required number" required>
    </div>
    <div class="form-group col-sm">
      <label for="validationInputEmail">Email</label>
      <input type="email" class="form-control is-invalid" id="validationInputEmail" placeholder="Required email" required>
    </div>
    <div class="form-group col-sm">
      <label for="validationInputAddress">Address</label>
      <input type="text" class="form-control is-invalid" id="validationInputAddress" placeholder="Required address (text)" required>
    </div>
  </div>
</form>

```
<form>
  <div class="form-row">
    <div class="form-group col-sm">
      <label for="validationInputNumber">Number</label>
      <input type="number" class="form-control is-invalid" id="validationInputNumber" placeholder="Required number" required>
    </div>
    <div class="form-group col-sm">
      <label for="validationInputEmail">Email</label>
      <input type="email" class="form-control is-invalid" id="validationInputEmail" placeholder="Required email" required>
    </div>
    <div class="form-group col-sm">
      <label for="validationInputAddress">Address</label>
      <input type="text" class="form-control is-invalid" id="validationInputAddress" placeholder="Required address (text)" required>
    </div>
  </div>
</form>
```

---

## Buttons

### Default

<button type="button" class="btn btn-primary">btn-primary</button>
<button type="button" class="btn btn-secondary">btn-secondary</button>
<button type="button" class="btn btn-info">btn-info</button>

```
<button type="button" class="btn btn-primary">btn-primary</button>
<button type="button" class="btn btn-secondary">btn-secondary</button>
<button type="button" class="btn btn-info">btn-info</button>
```

### Block

<button type="button" class="btn btn-primary btn-block">btn-block</button>
<button type="button" class="btn btn-secondary btn-block">btn-block</button>


```
<button type="button" class="btn btn-primary btn-block">btn-block</button>
<button type="button" class="btn btn-secondary btn-block">btn-block</button>
```
