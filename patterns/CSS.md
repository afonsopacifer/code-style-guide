# CSS Code Style Guide

> Tip: Use [csscomb.js](https://github.com/csscomb/csscomb.js) with our [.csscomb.json](.csscomb.json) to auto-format and [CSSLint](https://github.com/CSSLint/csslint) with our [.csslintrc](.csslintrc).

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
/* good */
.btn {
	color: #fff;
}

/* bad */
.btn{
		color: #fff;
}
```

<hr>

### Basic syntax

Always use double quotation marks:

**CSScomb rule:** `"quotes": "double"`

```css
/* good */
.btn {
	background-image: url("textura.jpg");
	font-family: "Helvetica Neue", sans-serif;
}

/* bad */
.btn {
	background-image: url('textura.jpg');
	font-family: 'Helvetica Neue', sans-serif;
}
```

<hr>

Include a space before opening the rule keys:

**CSScomb rule:** `"space-before-opening-brace": " "`

```css
/* good */
.btn {
	color: #fff;
}

/* bad */
.btn{
	color: #fff;
}
```

<hr>

Closes the keys on a new line:

**CSScomb rule:** `"space-before-closing-brace": "\n"`

```css
/* good */
.btn {
	color: #fff;
}

/* bad */
.btn {
	color: #fff;}
```

<hr>

Include a space after the `:` declarations:

**CSScomb rule:** `"space-after-colon": " "`

```css
/* good */
.btn {
	color: #fff;
}

/* bad */
.btn {
	color:#fff;
}
```

<hr>

Always use one `;` At the end of the declarations:

**CSScomb rule:** `"always-semicolon": true`

```css
/* good */
.btn {
	color: #fff;
}

/* bad */
.btn {
	color: #fff
}
```

<hr>

Always keep one declarations per line:

**CSScomb rule:** `"space-after-selector-delimiter": "\n"`

```css
/* good */
.nav,
.footer,
.btn {
	color: #fff;
}

/* bad */
.nav, .footer, .btn {
	color: #fff;
}
```

<hr>

Separate the rules by a blank line:

```css
/* good */
.btn {
	color: #fff;
}

.nav-item {
	color: #fff;
}

/* bad */
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
/* good */
.nav-item {
	color: #fff;
}

/* bad */
.Nav-item {
	color: #fff;
}
```

<hr>

Use dash to separate names:

```css
/* good */
.nav-item {
	color: #fff;
}

/* bad */
.nav_item {
	color: #fff;
}
```

<hr>

Whenever using hexadecimal values ​​always use reduced:

**CSScomb rule:** `"color-shorthand": true`

```css
/* good */
.nav-item {
	color: #fff;
}

/* bad */
.nav-item {
	color: #ffffff;
}
```

<hr>

Do not specify units when the value is zero:

**CSScomb rule:** `"unitless-zero": true` <br>
**CSSLint rule:** `zero-units`

```css
/* good */
.nav-item {
	padding: 0;
}

/* bad */
.nav-item {
	padding: 0px;
}
```

<hr>

Do not use values ​​starting with zero:

**CSScomb rule:** `"leading-zero": false`

```css
/* good */
.nav-item {
	transition: color .3s;
}

/* bad */
.nav-item {
	transition: color 0.3s;
}
```

<hr>

### Selectors

Use function-related names never style:

```css
/* good */
.spacing-default {
	margin-left: 10px;
}

/* bad */
.margin-left {
	margin-left: 10px;
}
```

<hr>

Never use ID for selectors:

**CSSLint rule:** `ids`

```css
/* good */
.btn {
	color: #fff;
}

/* bad */
#btn {
	color: #fff;
}
```

<hr>

### Declarations

Declarations grouped by type:

**CSScomb rule:** `"sort-order": [...]`

```css
/* good */
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

/* bad */
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

```css
/* good */
:root {
	--highlight-color: blue;
	--secondary-color: red;
}

/* bad */
:root {
	--blue: blue;
	--red: red;
}
```

<hr>

### Tips

- Configure your editor to show blank spaces
- Remove blank spaces
- Use a [.editorconfig](.editorconfig) to help keep the code convention:

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
