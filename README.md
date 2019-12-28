# Helper Library
Helper library with public methods

**Project 8** - [Vanilla JS Academy](https://vanillajsacademy.com/) (Fall 2019)


### Part 1

**Helper Library**  [Demo](https://letioneill.github.io/helper-library/01-helper-library.html)

Create a helper library with public methods you can use to:

- Convert a NodeList to an array.
- Get the first matching element in the DOM.
- Get all matching elements in the DOM as an array.
- Add a class to all elements in an array.
- Remove a class from all elements in an array

```
// _.toArray()
var arr = _.toArray(document.querySelectorAll('button'));
console.log('_.toArray()', arr);

// _.get()
var btn = _.get('#button-2');
console.log('_.get()', btn);

// _.get()
var btns = _.getAll('button');
console.log('_.getAll()', btns);

// _.addClass()
_.addClass(btns, 'btn-purple');

// _.removeClass()
_.removeClass(btns, 'btn-blue');
```

### Part 2

**Dom Manipulation Library**  [Demo](https://letioneill.github.io/helper-library/02-dom-manipulation-library.html)

Small DOM manipulation library with public methods you can use to: 

- Get an array of items from the DOM.
- Get the first and last matching items from the DOM.
- Add and remove a class to all matching elements.

Pass in a selector, and then call helper functions on your matching elements. To use it, create new instances of the library like this:

```
// Create new instances
var btns = new $('button');
var list = new $('ul');
Then, I can use the public helper methods like this.

// $.items()
console.log('$.items()', btns.items());
console.log('$.items()', list.items());

// $.first()
console.log('$.first()', btns.first());

// $.last()
console.log('$.last()', btns.last());

// $.addClass()
btns.addClass('btn-purple');

// $.removeClass()
btns.removeClass('btn-blue');
```

### Part 3

**Dom Manipulation Library Chaining**  [Demo](https://letioneill.github.io/helper-library/03-dom-manipulation-library-chaining.html)

Modify DOM manipulation library to support chaining methods. Only works for functions that aren’t already returning something)