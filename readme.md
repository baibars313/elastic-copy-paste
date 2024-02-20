
---
title: elastic-copy-paste
---

# elastic-copy-paste

`elastic-copy-paste` is a simple npm package that provides a function for copying text to the clipboard. It is designed to be versatile and can be easily integrated into any JavaScript project without dependencies on specific UI libraries or frameworks.

## Installation

To install `elastic-copy-paste` in your project, use the following npm command:

```bash
npm install elastic-copy-paste
```

## Usage

```jsx
import copyToClipboard from 'elastic-copy-paste';

const textToCopy = 'Hello, world!';

copyToClipboard(textToCopy)
  .then((success) => {
    if (success) {
      console.log('Text copied successfully!');
    } else {
      console.log('Failed to copy text.');
    }
  })
  .catch((error) => {
    console.error('Error during copy:', error);
  });


## API

### `copyToClipboard(text: string): Promise<boolean>`

This function takes a `text` parameter and returns a promise. It attempts to copy the provided text to the clipboard. The promise resolves to `true` if the operation is successful and `false` otherwise.

## Browser Compatibility

`elastic-copy-paste` relies on the `navigator.clipboard` API, which may not be available in all browsers. Ensure that your target browsers support this API or consider using a polyfill.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```
