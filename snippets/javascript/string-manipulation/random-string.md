---
title: Random string
description: Generates a random string of characters of a certain length
author: kruimol
tags: javascript,function,random
---

```js
function makeid(length, characters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789') {
  return Array.from({ length }, () => characters.charAt(Math.floor(Math.random() * characters.length))).join('');
}

console.log(makeid(5, "1234" /* (optional) */));
```
