# @kjosul/prettier-config

Kjosul's [Prettier](https://prettier.io) config.

## Installation

Add the following line to your `.npmrc` file:

```sh
@kjosul:registry=https://npm-proxy.fury.io/kjosul/
```

Then, install the package:

```sh
npm i -D @kjosul/prettier-config
```

## Usage

Based on your requirements, select either the [default configuration](#default-configuration) or the [custom configuration](#custom-configuration).

### Default configuration

If the default configuration meets your requirements, simply modify `package.json`:

```jsonc
{
    // ...
    "prettier": "@kjosul/prettier-config"
}
```

### Custom configuration

If you need to override certain properties, utilize a `.prettierrc.cjs` file instead:

```js
const prettierConfig = require('@kjosul/prettier-config');

module.exports = {
    ...prettierConfig,

    plugins: ['prettier-plugin-tailwindcss'],
    tailwindConfig: './tailwind.config.ts',
};
```

> ⚠️ We utilize a `.cjs` configuration for Prettier due to `"type": "module"` declaration in `package.json`.
