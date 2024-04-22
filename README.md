# @egiftcard/eslint-config

egiftcard ESLint config to enforce coding standards and best practices.

- TypeScript and Jest support
- Seamless Prettier integration
- Separate environments for Node.js and React

## Installation

```bash
yarn add --dev eslint @egiftcard/eslint-config
```

## Usage

> Make sure to include `require('@egiftcard/eslint-config/load')` at the top of your ESLint config. This loads a `@rushstack/eslint-patch/modern-module-resolution` patch so that ESLint loads any plugins installed by this package. 

```js
require('@egiftcard/eslint-config/load')

module.exports = {
  extends: '@egiftcard/eslint-config/node'
}
```

or:

```js
require('@egiftcard/eslint-config/load')

module.exports = {
  extends: '@egiftcard/eslint-config/react'
}
```

#### VSCode

If you're a VSCode user, consider installing the official [ESLint plugin](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) and copying [`./.vscode/settings.json`](.vscode/settings.json#L1-L6) to your own `.vscode/settings.json` configuration file. This will automatically run `eslint --fix` on save.
