[![Build Status](https://secure.travis-ci.org/markdalgleish/bespoke-progress.png?branch=master)](https://travis-ci.org/markdalgleish/bespoke-progress)

# bespoke-progress

Progress Bar for [Bespoke.js](http://markdalgleish.com/projects/bespoke.js)

## Download

Download the [production version][min] or the [development version][max], or use a [package manager](#package-managers).

[min]: https://raw.github.com/markdalgleish/bespoke-progress/master/dist/bespoke-progress.min.js
[max]: https://raw.github.com/markdalgleish/bespoke-progress/master/dist/bespoke-progress.js

## Usage

First, include both `bespoke.js` and `bespoke-progress.js` in your page.

Then, simply include the plugin when instantiating your presentation.

```js
bespoke.horizontal.from('article', {
  progress: true
});
```

Two elements will be added to your presentation: a progress bar, and a container for it.

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

### Bower

```bash
$ bower install bespoke-progress
```

### npm

```bash
$ npm install bespoke-progress
```

The bespoke-progress npm package is designed for use with [browserify](http://browserify.org/), e.g.

```js
require('bespoke');
require('bespoke-progress');
```

## Credits

This plugin was built with [generator-bespokeplugin](https://github.com/markdalgleish/generator-bespokeplugin).

## License

[MIT License](http://en.wikipedia.org/wiki/MIT_License)
