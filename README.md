oo.js
========

[Simple JavaScript Inheritance](http://ejohn.org/blog/simple-javascript-inheritance/) by John Resig

Customized from the original source to use a config object argument (instead of a standard argument list).

Usage
========

Class.extend()
```
MyClass = Class.extend({
    init: function() {
        // no longer takes params, all params are pre-loaded into class
        _super()
    },
    customFunction: function(){
        // ...
    },
    customMember: 10
});
```

Instantiation
```
// All options are automatically loaded (and override default class options) into the class on initialization
var m = MyClass({
    customMember: 10,
    myFunc: function(){
        // ...
    }
});
```