# `base-prettier-config`

> Base [Prettier](https://prettier.io) config that suitable for multiple scenarios.

## Usage

**Install**:

```bash
$ yarn add --dev base-prettier-config
```

**Edit `package.json`**:

```jsonc
{
  // ...
  "prettier": "base-prettier-config"
}
```

or

**Add `require('base-prettier-config')` at .prettierrc.js**:

```javascript
module.exports = {
  ...require("base-prettier-config"),
  // Your prettier config
  semi: false,
  // ...
};
```

## Default Config

```json
{
  "$schema": "http://json.schemastore.org/prettierrc",
  "singleQuote": true,
  "trailingComma": "es5",
  "endOfLine": "lf",
  "arrowParens": "avoid",
  "bracketSpacing": true,
  "jsxBracketSameLine": false,
  "jsxSingleQuote": false,
  "printWidth": 80,
  "proseWrap": "preserve",
  "quoteProps": "as-needed",
  "semi": true,
  "tabWidth": 2,
  "useTabs": false,
  "insertPragma": false,
  "htmlWhitespaceSensitivity": "css",
  "vueIndentScriptAndStyle": false,
  "overrides": [
    {
      "files": ["*.wxss", "*.acss"],
      "options": {
        "parser": "css"
      }
    },
    {
      "files": ".prettierrc",
      "options": {
        "parser": "json"
      }
    },
    {
      "files": "*.ejs",
      "options": {
        "parser": "html"
      }
    }
  ]
}
```

You can make appropriate `Config` adjustments according to your own conditions
