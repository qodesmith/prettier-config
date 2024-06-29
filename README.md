# How to use

Install this package:

```
bun add -D @qodestack/prettier-config
```

### Option 1 - your project's `package.json`

Add this line to your `package.json` file:

```json
"prettier": "@qodestack/prettier-config"
```

### Option 2 - using `.prettierrc.json`

Add a `.prettierrc.json` file to your project with the following contents:

```json
"@qodestack/prettier-config"
```

### Option 3 - this config + plugins

Use a `.prettierrc.cjs` file with the following content (the plugin used here is just an example):

```javascript
const qodeStackConfig = require('@qodestack/prettier-config')

module.exports = {
  ...qodeStackConfig,
  plugins: ['prettier-plugin-tailwindcss'],
}
```
