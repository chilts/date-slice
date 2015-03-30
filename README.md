# Date Slice #

Figure out which time slice a date lands in.

## Synopsis ##

```js
var dateSlice = require('date-slice')
```

This example will figure out the start of any 15s slice:

```js
var quarterMinute = 15 * 1000
var nearest15s = dateSlice.now(quarterMinute)

console.log(nearest15s.toISOString())
// => 2015-03-30T08:36:15.000Z
```

This example will give you the time to the start of the hour:

```js
var hour = 60 * 60 * 1000
var date = new Date('2015-01-03T22:57:45.123Z')

var nearestHour = dateSlice.from(date, hour)

console.log(nearestHour.toISOString())
// => 2015-01-03T22:00:00.000Z
```

## Author ##

Written by [Andrew Chilton](http://chilts.org/) - [Twitter](https://twitter.com/andychilton).

Written for [Tynio](https://tyn.io/).

## License ##

The MIT License (MIT)

Copyright 2015 Tynio Ltd.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

(Ends)
