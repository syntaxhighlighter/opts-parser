# opts-parser

Parses key/value pairs into hash object.

[![Dependency status](https://david-dm.org/alexgorbatchev/opts-parser.png)](https://david-dm.org/alexgorbatchev/opts-parser)
[![devDependency Status](https://david-dm.org/alexgorbatchev/opts-parser/dev-status.png)](https://david-dm.org/alexgorbatchev/opts-parser#info=devDependencies)
[![Build Status](https://travis-ci.org/alexgorbatchev/opts-parser.png)](https://travis-ci.org/alexgorbatchev/opts-parser)

[![NPM](https://nodei.co/npm/opts-parser.png?downloads=true&stars=true)](https://npmjs.org/package/opts-parser)

## Installation

    npm install opts-parser

## Usage Example

    var opts = require('opts-parser');

    opts.parse("hello: value; foo-bar: [12, "monkeys"]; value: 'value'")

    {
      "hello": "value",
      "foo-bar": [12, "monkeys"],
      "fooBar": [12, "monkeys"],
      "value": "value
    }

Understands the following formats:

- `name: true|false;`
- `name: word;`
- `name: [word, word];`
- `name: "string";`
- `name: 'string';`

## Testing

    npm test

## License

GPL & MIT
