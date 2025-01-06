# How to use

Install this package:

```
bun add -D @qodestack/prettier-config
```

### Option 1 - your project's `package.json` (no plugin support)

Add this line to your `package.json` file:

```json
"prettier": "@qodestack/prettier-config"
```

### Option 2 - plugin support

Use a `prettier.config.js` file with the following content (the plugin used here is just an example):

```javascript
import qodeStackConfig from '@qodestack/prettier-config'

export default {
  ...qodeStackConfig,
  plugins: ['prettier-plugin-tailwindcss'],
}
```

## From the Prettier docs:

https://prettier.io/docs/en/configuration

You can configure Prettier via (in order of precedence):

- A `"prettier"` key in your package.json, or package.yaml file.
- A `.prettierrc` file written in JSON or YAML.
- A `.prettierrc.json`, `.prettierrc.yml`, `.prettierrc.yaml`, or `.prettierrc.json5` file.
- A `.prettierrc.js`, or `prettier.config.js` file that exports an object using `export default` or `module.exports` (depends on - the [type](https://nodejs.org/api/packages.html#type) value in your package.json).
- A `.prettierrc.mjs`, or `prettier.config.mjs` file that exports an object using `export default`.
- A `.prettierrc.cjs`, or `prettier.config.cjs` file that exports an object using `module.exports`.
- A `.prettierrc.toml` file.
