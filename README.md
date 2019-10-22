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

3. Update `package.json` to reference the module;

```.json
{
  // ...
  "prettier": "@blue-raster/br-prettier"
  // ...
}
```

## Customize this module

1. Delete `"prettier": "@blue-raster/br-prettier"` in your `package.json`
2. Create a `prettier.config.js` file, export the module and include the customizations
   ⋅⋅⋅Note: customizing this file will override eslint customizations. That means there's no need to reference this module in your eslint config files.

```javascript
// prettier.config.js
module.exports = {
  ...require("@blue-raster/br-prettierjs"),
  tabWidth: 10,
}
```
