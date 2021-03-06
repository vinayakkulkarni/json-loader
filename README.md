[![npm][npm]][npm-url]
[![node][node]][node-url]
[![deps][deps]][deps-url]
[![tests][tests]][tests-url]
[![coverage][cover]][cover-url]
[![chat][chat]][chat-url]

<div align="center">
  <img width="160" height="180"
    src="https://worldvectorlogo.com/logos/json.svg">
  <a href="https://github.com/webpack/webpack">
    <img width="200" height="200"
      src="https://webpack.js.org/assets/icon-square-big.svg">
  </a>
  <h1>JSON Loader</h1>
</div>

**Note: Since webpack v2, JSON files will work by default. You might still want to use this if you use a custom file extension.**

<h2 align="center">Install</h2>

```bash
npm install --save-dev json-loader
```

<h2 align="center">Usage</h2>


### Configuration (recommended)

**webpack.config.js**
```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.json$/,
        use: 'json-loader'
      }
    ]
  }
}
```

```js
import json from 'file.json';
```

### CLI

```bash
webpack --module-bind 'json=json-loader'
```

```js
import json from 'file.json';
```

### Inline

```js
import json from 'json-loader!file.json';
```

<h2 align="center">Maintainer</h2>

<table>
  <tbody>
    <tr>
      <td align="center">
        <img width="150 height="150" src="https://github.com/sokra.png?s=150">
        <br>
        <a href="https://github.com/sokra">Tobias Koppers</a>
      </td>
    <tr>
  <tbody>
</table>

[npm]: https://img.shields.io/npm/v/json-loader.svg
[npm-url]: https://npmjs.com/package/json-loader

[node]: https://img.shields.io/node/v/json-loader.svg
[node-url]: https://nodejs.org

[deps]: https://david-dm.org/webpack/json-loader.svg
[deps-url]: https://david-dm.org/webpack/json-loader

[tests]: http://img.shields.io/travis/webpack/json-loader.svg
[tests-url]: https://travis-ci.org/webpack/json-loader

[cover]: https://coveralls.io/repos/github/webpack/json-loader/badge.svg
[cover-url]: https://coveralls.io/github/webpack/json-loader

[chat]: https://badges.gitter.im/webpack/webpack.svg
[chat-url]: https://gitter.im/webpack/webpack
