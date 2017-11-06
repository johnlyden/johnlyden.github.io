---
layout: post
title:  "es6 iterating over array indices and elements w/ for...of loop"
date:   2017-07-18 12:45:31 +0530
categories: ["javascript", "code"]
author: "Johnny"
---

Hey - here is a cool little thing you can do with es6!  

Iterating through an array and using both the element and the index of the element is a pretty useful thing.  Here is a way to do it with the <code>Array.prototype.forEach()</code> method:

```javascript
var arr = ['a', 'b', 'c'];
arr.forEach( (elem, index) => {
    console.log('index = '+index+', elem = '+elem);
});
// Output:
// index = 0, elem = a
// index = 1, elem = b
// index = 2, elem = c
```

well, in case you are just over the <code>forEach</code> method, you can pull some fancy moves with the the es6 <code>for...of</code> loop - this loop supports iterating over iterable objects (including Array, Map, Set, String, TypedArray, arguments object). You can create an iterable containing index-element pairs by using another new es6 feature, <code>Array.prototype.entries()</code>.  You can combine this cool new method with another big one people are hyped on, <strong>destructuring</strong>.

```javascript
const arr = ['a', 'b', 'c'];
for (const [index, elem] of arr.entries()) {
    console.log(`index = ${index}, elem = ${elem}`);
}
```

While this looks newer, it is not as performant as the earlier example.  I'll probably keep doing it with <code>forEach</code> tbh.  Peace!
