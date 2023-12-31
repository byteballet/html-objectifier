# html-objectifier

This Node.js package allows you to effortlessly convert HTML markup into a structured JavaScript object. It's a versatile library that can be used in both Node.js applications and browser environments. Whether you need to process HTML from files or input via a textarea, this library has you covered.

## Features

- Parse HTML markup into a nested object structure.
- Extract tag names, attributes, text content, and styles.
- Handle complex nested HTML elements and structures.
- Designed for ease of use with CLI and browser input support.
- Highly customizable with options for parsing and formatting.

## Installation

You can install this package using npm or yarn:

```bash
npm install html-objectifier
# or
yarn add html-objectifier
```

## Usage

1. Import the library in your Node.js application:

```javascript
//index.js

const html_objectifier = require("html-objectifier");
html_objectifier();
```

2. You can run it as CLI by running `node index.js markup.html`

3. Use the library to convert HTML to an object:

```javascript
const html = "<div><p>Hello, World!</p></div>";
const result = html_objectifier.parseHTML(html);
console.log(JSON.stringify(result));
```

For browser usage, include the library via a script tag and use it in your JavaScript code.

```html
<script src="https://cdn.jsdelivr.net/gh/byteballet/html-objectifier@master/dist/bundled.js"></script>
<script>
  const { parseHTML } = html_objectifier;
  console.log(parseHTML('<!DOCTYPE html><html lang="en"></html>'));
</script>
```

## Contributions

Contributions and feedback are welcome! If you have suggestions, bug reports, or want to contribute code, please open an issue or submit a pull request.

## License

This package is open-source.

## Author

[Byte Ballet]

## Contact

For inquiries, [Talk to Me!](https://github.com/byteballet/byteballet/issues/new?title=I+want+to+talk+to+you&body=Hi,+@byteballet.).
