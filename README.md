# @kjosul-dev/prettier-config

Kjosul's [Prettier](https://prettier.io) config.

## Installation

```sh
npm i -D @kjosul-dev/prettier-config
```

## Usage

Based on your requirements, select either the [default configuration](#default-configuration) or the [custom configuration](#custom-configuration).

### Default configuration

If the default configuration meets your requirements, simply modify `package.json`:

```jsonc
{
    // ...
    "prettier": "@kjosul-dev/prettier-config"
}
```

### Custom configuration

If you need to override certain properties, utilize a `.prettierrc.js` file instead:

```js
const prettierConfig = require('@kjosul-dev/prettier-config');

module.exports = {
    ...prettierConfig,
    semi: false,
};
```
