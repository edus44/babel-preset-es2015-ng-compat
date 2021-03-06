# babel-preset-es2015-ng-compat

> Babel preset for all es2015 plugins. Removed some problematic plugins.

## Install

```sh
npm install --save-dev babel-preset-es2015-ng-compat
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "presets": ["es2015-ng-compat"]
}
```

### Via CLI

```sh
babel script.js --presets es2015-ng-compat
```

### Via Node API

```javascript
require("babel-core").transform("code", {
  presets: ["es2015-ng-compat"]
});
```

## Options

### `loose`

`boolean`, defaults to `false`.

Enable "loose" transformations for any plugins in this preset that allow them.

### `modules`

`"amd" | "umd" | "systemjs" | "commonjs" | false`, defaults to `"commonjs"`.

Enable transformation of ES6 module syntax to another module type.

Setting this to `false` will not transform modules.

### `spec`

`boolean`, defaults to `false`.

Enable "spec" transformations for any plugins in this preset that allow them.