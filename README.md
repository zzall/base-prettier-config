# `base-prettier-config`

> Base [Prettier](https://prettier.io) config that suitable for multiple scenarios.

## Usage

**Install With Cli**

```bash
yarn add --dev prettier base-prettier-config
echo "module.exports = {
  ...require('base-prettier-config'),
  // Your prettier config
  semi: false,
  // ...
};" >> .prettierrc.js
```

**Install**:

```bash
$ yarn add --dev prettier base-prettier-config
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
  ...require('base-prettier-config'),
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
  "bracketSameLine": false,
  "jsxSingleQuote": true,
  "printWidth": 120,
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
