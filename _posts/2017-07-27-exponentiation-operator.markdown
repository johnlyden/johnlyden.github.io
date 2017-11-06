---
layout: post
title:  "Exponentiation operator transform"
date:   2017-07-27 19:45:31 +0530
categories: ["javascript"]
author: "Johnny"
---

Here is a cool feature of es6 involving exponents. In addition to this old shit:
```javascript
Math.pow(4, 3);
// 64
```
you can use this cool new exponentiation operator:
```javascript
// x ** y

let cubed = 4 ** 3;
// same as: 4 * 4 * 4
```
and then you can even do this:
```javascript
// x **= y

let a = 2;
a **= 2;
// same as: a = a * a;

let b = 3;
b **= 3;
// same as: b = b * b * b;
```

works in the Chrome console now - try it out!
