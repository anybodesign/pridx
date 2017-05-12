# Prid'x

A light and simple CSS stylesheet to help you start any responsive web design project. Basically a fluid flex based responsive CSS grid.
Check the [Demo page](https://lab.anybodesign.com/pridx "Demo page of Prid'x").


## Usage

Prid’x is based on a 12 columns layout. The gutters are managed with the columns' padding.

### Layout

Build your grids with `.row` and `.col-x` elements. For example:

```html
<div class="row">
	<div class="col-12"></div>
	<div class="col-6"></div>
	<div class="col-6"></div>
	...
</div>	
```

### Mixed Widths

Columns can be set to a different width under a particular breakpoint. For example, use the class `small-6` to set the width of the column to 50% for small widths. For medium widths you can use `mid-6`. Breakpoints can of course be customized.

```html
<div class="row">
	<div class="col-3 mid-6 small-4"></div>
	<div class="col-3 mid-6 small-8"></div>
</div>
```

### Nesting

Nesting is possible with the class `.nested`

```html
<div class="col-8">
	<div class="row nested">
		<div class="col-6"></div>					
		<div class="col-6"></div>					
		<div class="col-4"></div>					
		<div class="col-4"></div>					
		<div class="col-4"></div>					
	</div>
</div>

<div class="col-4">
	<div class="row nested">
		<div class="col-6"></div>
		<div class="col-6"></div>
	</div>
</div>

```

### Offsets

You can add some left or right margins if needed. For example, add the class `.left-1` if you want a 1 column left margin, or `.right-2` if you want a 2 columns right-margin.

```html

<div class="col-8 right-2"></div>
<div class="col-1 left-1"></div>

```

### No padding! 

Get rid of the margins with the class `.no-padding`

```html

<div class="col-2 no-padding"></div>

```

### Flexbox magic :)

Use extra classes on `.row` elements:

`.x-top` for align-items: flex-start

`.x-middle` for align-items: center

`.x-bottom` for align-items: flex-end

`.x-stretch` for align-items: stretch

`.x-baseline` for align-items: baseline
	
`.x-left` for justify-content: flex-start

`.x-center` for justify-content: center

`.x-right` for justify-content: flex-end

`.x-between` for justify-content: space-between

`.x-around` for justify-content: space-around




## ChangeLog

**v1.7** - 2017, May 12th

- Deleted CSS reset: to be included in the theme
- Removed .colparent class, use row.nested instead
- Spring cleaning and demo page :)

---

**v1.6** - 2017, March 25th

- Deleted (again) specific CSS styles: forms, typography

---

**v1.5** - 2017, January, 27th

- added .nested class for .row

---

**v1.4** - 2017, Juanuary, 20th

- filling with '.col-0' only on large width

---

**v1.3** - 2016, November, 23th

- Removed specific CSS styles: typography/forms (to be included in a theme)

---

**v1.2** - 2016, October, 6th

- Enhanced: Forms - Custom select

---

**v1.1** - 2016, September, 10th

- Enhanced: New Breakpoints

---

**v1.0** - 2016, June, 26th

- Initial Commit