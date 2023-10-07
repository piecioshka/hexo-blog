---
title: "IIFE: Pros & Cons"
subtitle: "A few words to explain that technique"
date: Fri, 01 Jun 2018 22:17:23 +0200
tags:
    - javascript
---

In this article we spend some time to describe what is `IIFE` _[ifi]_ and why each
Junior Developer should know this as quick as he can.

This is simple listing of JavaScript code:

```js
(function () {
    'use strict';

    function foo() {
        console.log('bar');
    }

    foo();
})();
```

You can see that the whole code is wrapped by a function in round brackets,
and immediately invoked with another pair of round brackets.

This syntax is called `Immediately Invoke Function Expression` - `IIFE`

## Pros

- function wraps some code which could define variable, so it is defines in
    a local scope
- without any _module definition_ variable define in global namespace,
    which is called _anti-pattern_

## Cons

- each wrap generates indentation
- when project does not have any module
