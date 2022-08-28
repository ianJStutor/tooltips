# Tooltips

## Ian Marshall

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

### Live Site

> [https://ianjstutor.github.io/tooltips/](https://ianjstutor.github.io/tooltips/)

### Description

Front-end widget for showing tooltips. Built with vanilla JavaScript, my favorite flavor!

### Usage

Include both <code>tooltips.css</code> and <code>tooltips.js</code> in your project. Link the CSS to your HTML document, import the JS into your main JavaScript file and call <code>initTooltips()</code>. In your HTML, add the <code>data-tooltip</code> attribute to any element that needs a tooltip.

#### HTML

```html
<head>
    <link rel="stylesheet" href="tooltips.css" />
    <script defer type="module" src="main.js"></script>
</head>
<body>
    <img src="lucy.png" alt="My dog Lucy" data-tooltip="My dog Lucy" />
</body>
```

#### JavaScript

```js
//main.js
import { initTooltips } from "./tooltips.js";
initTooltips();
```

### Documentation

#### Module Export

```js
export { initTooltips };
```

#### Public Method

```js
function initTooltips(root = document) {}
```

The <code>root</code> is an HTML element that defines the scope within which to look for elements containing the <code>data-tooltip</code> attribute. <code>root</code> defaults to <code>document</code>, meaning the module will look throughout the entire HTML document for tooltips.
