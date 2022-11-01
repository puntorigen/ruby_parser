# JS Ruby file parser
Simple class for parsing ruby files, getting their methods, arguments, comments and AST.

```js
const ruby = require('ruby_parser');
const parserObj = new ruby();

const parsed = parserObj.parse({
    filePath: 'tests/test.rb',
    // rubyString: `i = 7` // you can use filePath or rubyString
});

const info = parserObj.getInfo();
const methods = parserObj.getMethods();
const comments = parserObj.getComments();
const ast = parserObj.getAst(); // also, parserObj.parse returns the ast
```

