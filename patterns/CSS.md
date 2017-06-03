# CSS Code Style Guide

> Use [csscomb.js](https://github.com/csscomb/csscomb.js) with our [configuration file](.csscomb.json) to auto-format.

## Table of Contents

- [Indentation](#indentation)
- [Basic syntax](#basic-syntax)
- [Selectors](#selectors)
- [Declarations](#declarations)
- [Custom Properties](#custom-properties)
- [Tips](#tips)

<hr>

### Indentation

Use soft-tabs with two spaces:

**CSScomb rule:** `"block-indent": "  "`

```css
/* bom */
.btn {
	color: #fff;
}

/* ruim */
.btn{
		color: #fff;
}
```

<hr>

### Basic syntax

Always use double quotation marks:

**CSScomb rule:** `"quotes": "double"`

```css
/* bom */
.btn {
	background-image: url("textura.jpg");
	font-family: "Helvetica Neue", sans-serif;
}

/* ruim */
.btn {
	background-image: url('textura.jpg');
	font-family: 'Helvetica Neue', sans-serif;
}
```

<hr>

Include a space before opening the rule keys:

**CSScomb rule:** `"space-before-opening-brace": " "`

```css
/* bom */
.btn {
	color: #fff;
}

/* ruim */
.btn{
	color: #fff;
}
```

<hr>

Closes the keys on a new line:

**CSScomb rule:** `"space-before-closing-brace": "\n"`

```css
/* bom */
.btn {
	color: #fff;
}

/* ruim */
.btn {
	color: #fff;}
```

<hr>

Include a space after the `:` declarations:

**CSScomb rule:** `"space-after-colon": " "`

```css
/* bom */
.btn {
	color: #fff;
}

/* ruim */
.btn {
	color:#fff;
}
```

<hr>

Always use one `;` At the end of the declarations:

**CSScomb rule:** `"always-semicolon": true`

```css
/* bom */
.btn {
	color: #fff;
}

/* ruim */
.btn {
	color: #fff
}
```

<hr>

Always keep one declarations per line:

**CSScomb rule:** `"space-after-selector-delimiter": "\n"`

```css
/* bom */
.nav,
.footer,
.btn {
	color: #fff;
}

/* ruim */
.nav, .footer, .btn {
	color: #fff;
}
```

<hr>

Separate the rules by a blank line:

**CSScomb rule:** ``

```css
/* bom */
.btn {
	color: #fff;
}

.nav-item {
	color: #fff;
}

/* ruim */
.btn {
	color: #fff;
}
.nav-item {
	color: #fff;
}
```

<hr>

Always use lowercase:

**CSScomb rule:** `"element-case": "lower"`

```css
/* bom */
.nav-item {
	color: #fff;
}

/* ruim */
.Nav-item {
	color: #fff;
}
```

<hr>

Use dash to separate names:

**CSScomb rule:** ``

```css
/* bom */
.nav-item {
	color: #fff;
}

/* ruim */
.nav_item {
	color: #fff;
}
```

<hr>

Whenever using hexadecimal values ​​always use reduced:

**CSScomb rule:** `"color-shorthand": true`

```css
/* bom */
.nav-item {
	color: #fff;
}

/* ruim */
.nav-item {
	color: #ffffff;
}
```

<hr>

Do not specify units when the value is zero:

**CSScomb rule:** `"unitless-zero": true`

```css
/* bom */
.nav-item {
	padding: 0;
}

/* ruim */
.nav-item {
	padding: 0px;
}
```

<hr>

Do not use values ​​starting with zero:

**CSScomb rule:** `"leading-zero": false`

```css
/* bom */
.nav-item {
	transition: color .3s;
}

/* ruim */
.nav-item {
	transition: color 0.3s;
}
```

<hr>

### Selectors

Use function-related names never style:

**CSScomb rule:** ``

```css
/* bom */
.spacing-default {
	margin-left: 10px;
}

/* ruim */
.margin-left {
	margin-left: 10px;
}
```

<hr>

### Declarations

Declarations grouped by type:

**CSScomb rule:** `"sort-order": [...]`

```css
/* bom */
.container {
  font-size: 1em;
  font-weight: bold;

  display: grid;
  grid-template-columns: repeat(7, 1fr);
  grid-template-rows: repeat(5, 130px);

  width: 100%;
  height: 100%;

  color: #000;
  border: 1px solid #000;
  background: #ff567e;
}

/* ruim */
.container {
  display: grid;
  font-size: 1em;
  color: #000;
  grid-template-columns: repeat(7, 1fr);
  background: #ff567e;
  grid-template-rows: repeat(5, 130px);
  width: 100%;
  font-weight: bold;
  height: 100%;
  color: #000;
  border: 1px solid #000;
  height: 100%;
}
```

<hr>

### Custom Properties

Use function-related names never style:

**CSScomb rule:** ``

```css
/* bom */
:root {
	--highlight-color: blue;
	--secondary-color: red;
}

/* ruim */
:root {
	--blue: blue;
	--red: red;
}
```

<hr>

### Tips

- Configure your editor to show blank spaces
- Remove blank spaces

<hr>

Use a [.editorconfig](.editorconfig) to help keep the code convention:

```
# editorconfig.org

root = true

[*]
charset = utf-8
insert_final_newline = true
trim_trailing_whitespace = true
end_of_line = lf
indent_style = tab
indent_size = 2
```

<hr>

Never use generic selectors(elements):

```css
/* bom */
.heading {

}

/* ruim */
h1 {

}
```

<hr>

## Contributing

Find on our [roadmap](https://github.com/afonsopacifer/code-style-guide/issues/1) the next steps of the project ;)
<br>
Want to contribute? [Follow these recommendations](https://github.com/afonsopacifer/code-style-guide/blob/master/CONTRIBUTING.md).

## References

- [Idiomatic CSS by necolas](https://github.com/necolas/idiomatic-css/blob/master/translations/pt-BR/README.md)
- [Coding style by LFeh](https://github.com/LFeh/coding-style/blob/master/translations/pt-BR/README.md)
- [Code guide](http://diegoeis.github.io/code-guide/)

## [<-- Back](https://github.com/afonsopacifer/code-style-guide)
