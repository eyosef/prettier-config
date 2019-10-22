# `@blue-raster/br-prettier`

This module was created to keep code formatting consistent across Blue Raster projects.

## Set up

1. Install prettier

```shell

npm install --save-dev --save-exact prettier

```

2. Install this module locally:

```shell

npm install --save-dev @blue-raster/br-prettier

```

Update `package.json` to reference the module;

```jsonc
{
  // ...
  "prettier": "@blue-raster/br-prettier"
  // ...
}
```

## Customize this module

To override the prettier settings, create a `prettierrc.js` file, export the module and include the customizations. You'll need to do the same thing via an `eslintrc.js` file. See below;

```javascript
// prettierrc.js
module.exports = {
  ...require("@blue-raster/br-prettier"),
  semi: false,
}
```

```javascript
// eslintrc.js
module.exports = {
  ...require("@blue-raster/br-prettier"),
  tabWidth: 4,
}
```
