# Vue Adapter for Fractal

This adapter lets you use Vue as a template engine in [Fractal](http://fractal.build). It's based on Fractal's [Handlebars adapter](https://github.com/frctl/handlebars). This adapter aims to maintain a Vue flavor rather than achieve complete feature parity with the Handlebars adapter. The goal is to facilitate writing Vue components that can easily be used in other projects.

## Installation

Install the adapter via NPM:

```
npm i --save swey/fractal-vue-adapter
```

#### In your fractal.js just set the engine like this:

```javascript
const Vue = require('vue');

fractal.components.set('engine', '@swey/fractal-vue-adapter');
fractal.components.set('ext', '.(vue|html)');
```

#### In the fractal.js you can also add plugins, e.g.:

```
Vue.use(require('./src/js/plugins/GlobalsPlugin'));
```
