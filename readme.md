# x-spreadsheet

[![npm package](https://img.shields.io/npm/v/x-data-spreadsheet.svg)](https://www.npmjs.org/package/x-data-spreadsheet)
[![NPM downloads](http://img.shields.io/npm/dm/x-data-spreadsheet.svg)](https://npmjs.org/package/x-data-spreadsheet)
[![Join the chat at https://gitter.im/x-datav/spreadsheet](https://badges.gitter.im/x-datav/spreadsheet.svg)](https://gitter.im/x-datav/spreadsheet?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

> A web-based JavaScript spreadsheet

<p align="center">
  <a href="https://github.com/myliang/x-spreadsheet">
    <img width="100%" src="https://raw.githubusercontent.com/myliang/x-spreadsheet/master/docs/demo.png">
  </a>
</p>

## CDN
```html
<link rel="stylesheet" href="https://unpkg.com/x-data-spreadsheet@1.0.11/dist/xspreadsheet.css">
<script src="https://unpkg.com/x-data-spreadsheet@1.0.11/dist/xspreadsheet.js"></script>

<script>
   x.spreadsheet('#xspreadsheet');
</script>
```

## Install

```shell
npm install x-data-spreadsheet
```

## Quick Start

```html
<div id="x-spreadsheet-demo"></div>
```

```javascript
import Spreadsheet from "x-data-spreadsheet";
// If you need to override the default options, you can set the override
// const options = {};
// new Spreadsheet('#x-spreadsheet-demo', options);
new Spreadsheet("#x-spreadsheet-demo")
  .loadData({}) // load data
  .change(data => {
    // save data to db
  });
```

```javascript
// default options
{
  showToolbar: true,
  showGrid: true,
  view: {
    height: () => document.documentElement.clientHeight,
    width: () => document.documentElement.clientWidth,
  },
  row: {
    len: 100,
    height: 25,
  },
  col: {
    len: 26,
    width: 100,
    indexWidth: 60,
    minWidth: 60,
  },
  style: {
    bgcolor: '#ffffff',
    align: 'left',
    valign: 'middle',
    textwrap: false,
    strike: false,
    underline: false,
    color: '#0a0a0a',
    font: {
      name: 'Helvetica',
      size: 10,
      bold: false,
      italic: false,
    },
  },
}
```

## Internationalization
[wiki](https://github.com/myliang/x-spreadsheet/wiki/Internationalization)

## Features
  - Undo & Redo
  - Paint format
  - Clear format
  - Format
  - Font
  - Font size
  - Font bold
  - Font italic
  - Underline
  - Strike
  - Text color
  - Fill color
  - Borders
  - Merge cells
  - Align
  - Text wrapping
  - Freeze cell
  - Functions
  - Resize row-height, col-width
  - Copy, Cut, Paste
  - Autofill
  - Insert row, column
  - Delete row, column
  - Data validations

## Development

```sheel
git clone https://github.com/myliang/x-spreadsheet.git
cd x-spreadsheet
npm install
npm run dev
```

Open your browser and visit http://127.0.0.1:8080.

## Browser Support

Modern browsers(chrome, firefox, Safari).

## LICENSE

MIT
