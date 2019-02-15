### pegjs
---
https://github.com/pegjs/pegjs

```
npm install -g pegjs
npm install pegjs
bower install pegjs

pegjs arithmetics.pegjs
pegjs -o arithmetics-parser.js arithmetics.pegjs
```

```js
var peg = require("pegjs");

var parser = peg.generate("start = ('a' / 'b')");

parser.parse("abba");
parser.parse("abcd");
```

```
{
  start: { offset: 23, line: 5, column 6 },
  end: { offset: 23, line: 5, column: 6 }
}
```


