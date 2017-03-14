#webpack-config-svg-icon

A config for [Webpack] for loading `.svg` icon files as React components. 

[![license](http://img.shields.io/npm/l/webpack-config-svg-icon.svg?style=flat)](https://www.npmjs.com/package/webpack-config-svg-icon)
[![version](http://img.shields.io/npm/v/webpack-config-svg-icon.svg?style=flat)](https://www.npmjs.com/package/webpack-config-svg-icon)
[![downloads](http://img.shields.io/npm/dm/webpack-config-svg-icon.svg?style=flat)](https://www.npmjs.com/package/webpack-config-svg-icon)

## Usage

Install:

```sh
yarn add webpack-config-svg-icon
```

Add to your `webpack.config.babel.js`:

```js
import svgIcon from `webpack-config-svg-icon`;

svgIcon({/* options */})({
  /* existing webpack configuration */
})
```

### Options

|Name|Default|Description|
|:---|:------|:----------|
|**`iconPath`**|`asset/icon`|...|
|**`test`**|`/\.icon\.svg$/`|...|
|**`replaceColor`**|...|...|
|**`svgo`**|...|...|

## Features

### SVGO

How to configure SVGO...

### SVG -> React component

SVGs become React components...

### Icon Context

How to dynamically add icons...

```jsx
const context = require.context(process.env.ICON_PATH, false, /\.icon\.svg$/);
```

### Replace fill and stroke with `currentColor`

...

```js
svgIcon({replaceColor: /^#(000){1,2}$/})({
  /* existing webpack configuration */
})
```

## Examples

### React `Icon` component

Set up an icon component with display inline-block...

```jsx
<Icon type='type'/>
```

[webpack]: https://webpack.github.io
