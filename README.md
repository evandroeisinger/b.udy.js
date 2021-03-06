## b.udy.js  :dog2:

> A micro (**0.8kb**) DOM library! With only two purposes: facilitate the creation and manipulation of DOM elements.

[![npm version](https://badge.fury.io/js/b.udy.js.svg)](http://badge.fury.io/js/b.udy.js) [![Build Status](https://travis-ci.org/evandroeisinger/b.udy.js.svg?branch=master)](https://travis-ci.org/evandroeisinger/b.udy.js)

```shell
npm install b.udy.js
```

### basic usage
```javascript
// load b.udy
var b = require('b.udy');

// to create a element and return it
var element = b('div').element();

// to load a existing element
b(element);

// to set element id
b(element).id('element-id');

// to set element className
b(element).className('element-class other-element-class');

// to add element attribute
b(element).attr('data-type', 'div');

// to remove element attribute
b(element).removeAttr('data-type', 'div');

// to add element listener
b(element).listener('click', clickListener);

// to remove element listener
b(element).removeListener('click', clickListener);

// to set multiple properties
b(element).id('element').className('element-class').listener('click', clickListener);
```

### methods
- b**(nodeType | element)**: Create or load a DOM element;
- b.**element()**: Return the DOM element;
- b.**id(value)**: Set the DOM element id;
- b.**className(value)**: Set the DOM element className;
- b.**attr(key, value)**: Add a attribute to the DOM element;
- b.**removeAttr(key)**: Remove a attribute from the DOM element;
- b.**listener(eventType, callback)**: Add a event listener to the DOM element;
- b.**removeListener(eventType, callback)**: Remove a event listener from the DOM element;

### support
- chrome: **latest**;
- firefox: **latest**;
- safari: **latest**;
- internet explore: **9+**;

---
### contribute
Everyone can contribute! Every contribution will be welcomed!

**Fork it** -> **Branch it** -> **Test it** -> **Push it** -> **Pull Request it**
