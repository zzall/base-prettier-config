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
	semi: false,
	// Your prettier config
};
```
