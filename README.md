# args-checker-js

a lightweight function's arguments checker in javascript. :heavy_check_mark:

### Version
1.0.0

### Installation

```sh
$ bower install args-checker-js
```
---
# The Problem
As we all know, Javascript doesn't suppor strict typing unlike other languages. So in order to force javascript to do so, we'll do something like this:
```javascript
function someFunc(name, history, callback) {
    if (typeof name !== 'string') {
        throw "Argument number 1 must be a string!";
    }
    
    if (typeof history !== 'object') {
        throw "Argument number 2 must be an object!";
    }
    
    if (typeof callback !== 'function') {
        throw "Argument number 3 must be a function!";
    }
}
```

# What args-checker aims to solve
Wouldn't it be cool if javascript did support strict typing? Say, something like this:
```javascript
function someFunc(String name, Object history, Function callback) {
    // do something...
}
```
