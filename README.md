# Hex String Escaper

Escapes hex strings from \"FF\" format to \"\\xFF\" hex equivalent. Useful for dynamically creating hex values (such as for a rgb value).

## Usage

```js
var util = require("util"),
	HexStringEscaper = require("hexstringescaper"),
	hEsc = HexStringEscaper.escaper;

console.log(hEsc["1F"]); // logs a non-readable symbol 

console.log(util.format("This is escaped hex: %s", hEsc["FF"]));
This is escaped hex: ÿ

```
