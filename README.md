[![Build Status](https://secure.travis-ci.org/markdalgleish/bespoke-progress.png?branch=master)](https://travis-ci.org/markdalgleish/bespoke-progress) [![Coverage Status](https://coveralls.io/repos/markdalgleish/bespoke-progress/badge.png)](https://coveralls.io/r/markdalgleish/bespoke-progress)

# bespoke-progress

Progress Bar for [Bespoke.js](http://markdalgleish.com/projects/bespoke.js)

## Download

Download the [production version][min] or the [development version][max], or use a [package manager](#package-managers).

[min]: https://raw.github.com/markdalgleish/bespoke-progress/master/dist/bespoke-progress.min.js
[max]: https://raw.github.com/markdalgleish/bespoke-progress/master/dist/bespoke-progress.js

## Usage

This plugin is shipped in a [UMD format](https://github.com/umdjs/umd), meaning that it is available as a CommonJS/AMD module or browser global.

For example, when using CommonJS modules:

```js
var bespoke = require('bespoke'),
  progress = require('bespoke-progress');

bespoke.from('article', [
  progress()
]);
```

When using browser globals:

```js
bespoke.from('article', [
  bespoke.plugins.progress()
]);
```

Two elements will be added to your presentation: a progress bar, and a container for it.

By default, the `.bespoke-progress-bar` element's width will be dynamically set to a percentage width.

If you'd prefer a vertical progress bar, simply specify `'vertical'` as the plugin option:

```js
bespoke.from('article', [
  progress('vertical')
]);
```

### CSS

The following classes are available on the generated progress elements.

<table>
   <tr>
    <td><b>bespoke-progress-parent</b></td>
    <td>The progress bar's parent element</td>
   </tr>
   <tr>
    <td><b>bespoke-progress-bar</b></td>
    <td>The progress bar</td>
   </tr>
</table>

## Package managers

### npm

```bash
$ npm install bespoke-progress
```

### Bower

```bash
$ bower install bespoke-progress
```

## Credits

This plugin was built with [generator-bespokeplugin](https://github.com/markdalgleish/generator-bespokeplugin).

## License

[MIT License](http://en.wikipedia.org/wiki/MIT_License)
