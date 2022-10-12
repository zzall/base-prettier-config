# `base-prettier-config`

> My personal [Prettier](https://prettier.io) config.

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

** Add `require('base-prettier-config')` at .prettierrc.js**:

```javascript
module.exports = {
	...require("base-prettier-config"),
	semi: false,
	// Your prettier config
};
```
