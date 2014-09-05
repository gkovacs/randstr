randstr
=======

A simple function can be used to generate a random string with the specified length. And, the range of the characters is configurable.

Installation
-------

To Install randstr, use [npm](http://github.com/isaacs/npm)

```bash
$ npm install randstr
````

Usage
-----

```js
var randstr = require('randstr');

// By default, randstr will use `A-Za-z0-9` characters to generate
// a random string, and the length of the string is 32.
randstr();
// >> "xtYRPnR8rM0M6izYTNv8gJd07thPIyN9"


// You can set the default length and range of the characters.
randstr.len = 16;
randstr.chars = 'abcdefghijkmn';

randstr();
// >> "cfhaffchimiblalg"


// However, you can still specify the length and the range of the characters
// to override the default settings when the randstr is called.
randstr(6);
// >> "e3pTse"

randstr(6, '0123456789');
// >> "823748"
```

LICENSE
-------
randstr is licensed under the MIT license.