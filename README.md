# Tooltips

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

## Description

Front-end widget for showing tooltips. Detects mouse or pointer movement--not touch events--so only works on desktop devices. Built with vanilla JavaScript, my favorite flavor!

## Author

> [Ian Marshall](https://ianjstutor.github.io/ian-marshall/)

## Live Site

> [https://ianjstutor.github.io/tooltips/](https://ianjstutor.github.io/tooltips/)

## Usage

1. Include both <code>tooltips.css</code> and <code>tooltips.js</code> in your project.
2. Link the CSS to your HTML document.
3. Import the JS module into your main JavaScript file and call <code>initTooltips()</code>.
4. In your HTML, add the <code>data-tooltip</code> attribute to any element that needs a tooltip.

### HTML

```html
<head>
    <link rel="stylesheet" href="tooltips.css" />
    <script type="module" src="main.js"></script>
</head>
<body>
    <img src="lucy.png" alt="My dog Lucy" data-tooltip="My dog Lucy" />
</body>
```

### JavaScript

```js
//main.js
import { tooltips } from "./tooltips.js";
tooltips();
```

## Documentation

### Module Export

```js
export { initTooltips };
```

### Public Method

```js
function tooltips(root = document) {}
```

The <code>root</code> is an HTML element that defines the scope within which to look for elements containing the <code>data-tooltip</code> attribute. <code>root</code> defaults to <code>document</code>, meaning the module will look throughout the entire HTML document for tooltips.
