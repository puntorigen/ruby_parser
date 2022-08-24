# JS Ruby file parser
Simple class for parsing ruby files, getting their methods, arguments, comments and AST.

```js
const ruby = require('ruby_parser');
const parser = new ruby('tests/test.rb');

const info = parser.getInfo();
const methods = parser.getMethods();
const comments = parser.getComments();
const ast = parser.getAst();
```

