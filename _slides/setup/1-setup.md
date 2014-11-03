---
layout: slide
---



--

## Grid System


--

## CSS classes

- Elementary CSS (typos, images, buttons, forms)
- Advanced components (navbar, panels)
- Javascript animation (dropdown, modal,..)

---

## Everything starts with a nice boilerplate!

https://github.com/lewagon/bootstrap-boilerplate

---

## CSS classes

--

## Elementary CSS

http://getbootstrap.com/css/

--

### Typos (alignment)


--

### Typos (list-inline)

```html
<ul class="list-inline">
  <!--Your list-->
</ul>
```


--

### Buttons


```html
<a class="btn">Default</a>
<a class="btn btn-primary">Primary</a>
<a class="btn btn-success">Success</a>
<a class="btn btn-info">Info</a>
```

--

### Images


--

### Forms

Ex: `.form-inline`, `.form-group`, `.form-control`

```html
<form class="form-inline" role="form">
  <div class="form-group">
    <label for="mail">Email</label>
    <input type="email" class="form-control" id="mail" placeholder="Enter email">
    <input type="submit" value="Sign in" class="btn btn-primary">
  </div>
</form>
```



--

## Look in the doc !

http://getbootstrap.com/css/

--

## Advanced components

http://getbootstrap.com/components/

--

### Navbar



--

### Labels


--

Panels, alerts, badges, many more, read the doc

http://getbootstrap.com/components/

---

## Bootstrap grid



--

## Definition

Bootstrap includes a **responsive, mobile first** fluid **grid** system that appropriately scales up to **12 columns** as the **device** size increases.

--

## Responsive



--

## Mobile-first


--

## How it works?

--

## Container first

```html
<div class="container">

  <!--Define a container-->

</div>
```


--

## Then insert rows

```html
<div class="container">

  <div class="row">
    <!-- First row -->
  </div>

</div>
```


--

```html
<div class="container">

  <div class="row">
    <!-- First row -->
  </div>

  <div class="row">
    <!-- Second row -->
  </div>

</div>
```


--

```html
<div class="container">

  <div class="row">
    <!-- First row -->
  </div>

  <div class="row">
    <!-- Second row -->
  </div>

  <div class="row">
    <!-- Third row -->
  </div>

</div>
```


--

## What's in the row ?

```html
<div class="col-xs-6">
</div>
```

- **col**: because it fits a number of columns
- **xs**: screen width
- **6**: number of columns taken by the block (**max 12**)

--

## Media

- **xs**: Extra small devices (Phones < 768px)
- **sm**: Small devices (Tablets > 768px)
- **md**: Medium devices (> 992px)
- **lg**: Large devices (Desktops > 1200px)

--
## Example (2 columns)


--

## Code

```html
<div class="container">
  <div class="row">

    <div class="col-xs-6">
    </div>

    <div class="col-xs-6">
    </div>

  </div>
</div>
```


--

## Mobile first

- if you just give the `.col-xs` classes
- it will apply on all larger screens

--
## Now what happens ?
```html
<div class="container">
  <div class="row">

    <div class="col-xs-6">
    </div>

    <div class="col-xs-6">
    </div>

    <div class="col-xs-6">
    </div>

  </div>
</div>
```

--
## Just return on new line


--

## Responsive example
We want 4 blocks for tablets or larger screens


--
We want 2 rows for mobiles with 2 blocks on each row

--

## How will you do ?

--

## Code

```html
<div class="container">
  <div class="row">
    <div class="col-xs-6 col-sm-3"></div>
    <div class="col-xs-6 col-sm-3"></div>
    <div class="col-xs-6 col-sm-3"></div>
    <div class="col-xs-6 col-sm-3"></div>
  </div>
</div>
```

Yeah baby !

--

## Offsetting blocks


Can we offset a block ?

--

## Yes we can

```html
<div class="container">
  <div class="row">
    <div class="col-sm-offset-4 col-sm-4">
      <!-- Le contenu de la div centrée -->
    </div>
  </div>
</div>
```