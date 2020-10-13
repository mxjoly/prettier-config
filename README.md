# Prettier Config

A shared [Prettier](https://prettier.io/) config for all the [@mxjoly](https://github.com/mxjoly) packages.

## Installation

```bash
yarn add --dev @mxjoly/prettier-config
```

```bash
npm install --save-dev @mxjoly/prettier-config
```

## Setup

If you want to use this config as base in any of your projects, you need to create a `.prettierrc.js` file in your project folder that re-exports the Prettier config from `@mxjoly/prettier-config`.

You can either do that automatically by running the following command in the root folder of your project (where your `package.json` is):

```bash
# create .prettierrc.js config file
npm @mxjoly/prettier-config
```

or by manually adding the following content:

```js
module.exports = require('@mxjoly/prettier-config');
```

**Important:** filename must be `.prettierrc.js` or `prettier.config.js` or otherwise Prettier will try to parse it as JSON or YML and will fail.

Read the Prettier [docs](https://prettier.io/docs/en/configuration.html#sharing-configurations) on sharing configurations for more info.
