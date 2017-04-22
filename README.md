# art-template-loader

[![NPM Version](https://img.shields.io/npm/v/art-template-loader.svg)](https://npmjs.org/package/art-template-loader)
[![Node.js Version](https://img.shields.io/node/v/art-template-loader.svg)](http://nodejs.org/download/)

[art-template](https://github.com/aui/art-template) loader for webpack

## Install

```shell
npm install art-template
npm install art-template-loader --save-dev
```

## Usage

```js
module.exports = {
    // ...
    module: {
        rules: [{
            test: /\.art$/,
            loader: "art-template-loader",
            options: {
                // art-template options (if necessary)
                imports: require.resolve('./template-imports')
            }
        }],
    },
    // ...
}
```

## Debug

```shell
webpack --debug
```

## Options

You can pass [art-template options](https://github.com/aui/art-template)
using standard webpack [loader options](https://webpack.js.org/configuration/module/#useentry).
