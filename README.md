# use-script
The @1ohooks/use-script package provides a custom React hook for dynamically loading JavaScript scripts in your applications.


# @1ohooks/use-script

[![Version](https://img.shields.io/npm/v/@1ohooks/use-script.svg)](https://www.npmjs.org/package/@1ohooks/use-script)
[![Coverage Status](https://coveralls.io/repos/github/1ohooks/use-script/badge.svg?branch=master)](https://coveralls.io/github/1ohooks/use-script?branch=master)
[![Downloads](https://img.shields.io/npm/dm/@1ohooks/use-script.svg)](https://www.npmjs.com/package/@1ohooks/use-script)
[![Try on RunKit](https://badge.runkitcdn.com/@1ohooks/use-script.svg)](https://runkit.com/npm/@1ohooks/use-script)

The `@1ohooks/use-script` package provides a custom React hook for dynamically loading JavaScript scripts in your applications.

## Installation

You can install `@1ohooks/use-script` using npm or yarn:

```sh
npm install @1ohooks/use-script
# or
yarn add @1ohooks/use-script
```

## Documentation

### useScript

The `useScript` hook allows you to dynamically load JavaScript scripts and manage their loading state.

```javascript
import { useScript } from '@1ohooks/use-script';

// Usage example
function MyComponent() {
  const { loaded, error } = useScript('https://example.com/myscript.js');

  if (loaded) {
    // The script has been successfully loaded
  }

  if (error) {
    // An error occurred while loading the script
  }

  return (
    // Your component JSX
  );
}
```

#### Parameters

- `url` (string): The URL of the JavaScript script to load.

#### Return Values

- `loaded` (boolean): Indicates whether the script has been successfully loaded.
- `error` (Error | null): An error object, if an error occurred during script loading; otherwise, `null`.

## Requirements

- React 16 or higher.

## Usage

You can use the `useScript` hook to load external JavaScript scripts dynamically in your React components. This can be helpful for integrating third-party libraries or resources into your application.

For more advanced usage and handling script dependencies, refer to the hook documentation.

Thank you for using `@1ohooks/use-script` to simplify script loading in your React applications. We hope you find it valuable!
