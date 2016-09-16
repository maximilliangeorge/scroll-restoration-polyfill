# scroll-restoration-polyfill 

> Prevent the scroll restoration caused by the `popstate` event or back/forward buttons. [Demo](https://rawgit.com/bfred-it/scroll-restoration-polyfill/master/demo.html)

[![gzipped size](https://badges.herokuapp.com/size/github/bfred-it/scroll-restoration-polyfill/gh-pages/dist/scroll-restoration-polyfill.browser.js?gzip=true&label=gzipped%20size)](#readme)
[![Travis build status](https://api.travis-ci.org/bfred-it/scroll-restoration-polyfill.svg?branch=gh-pages)](https://travis-ci.org/bfred-it/scroll-restoration-polyfill)
[![npm version](https://img.shields.io/npm/v/scroll-restoration-polyfill.svg)](https://www.npmjs.com/package/scroll-restoration-polyfill) 

+*Warning:* it works in Chrome, Safari, and Firefox 46+, but there's **no IE/Edge support yet.**

## Usage

The polyfill has no API. Once included, just use the official API as described on [Chrome Developers](https://developers.google.com/web/updates/2015/09/history-api-scroll-restoration):

```js
// Prevent the scroll, always
history.scrollRestoration = 'manual';

// Stop preventing the scroll
history.scrollRestoration = 'auto';
```

## Install

## Load with plain HTML

```html
<script src="dist/scroll-restoration-polyfill.browser.js"></script>
```

## Load with browserify

```sh
npm install --save scroll-restoration-polyfill
```

```js
equire('scroll-restoration-polyfill');
```

## Links

- Specification: http://majido.github.io/scroll-restoration-proposal/history-based-api.html
- Native compatibility table: https://developer.mozilla.org/en/docs/Web/API/History#Browser_compatibility
- Chrome Developers post: https://developers.google.com/web/updates/2015/09/history-api-scroll-restoration


## Dependencies

* [`on-off` <img alt="dependency gzipped size" src="https://badge-size.herokuapp.com/npm-dom/dom-event/master/index.js?compression=gzip&amp;label=size" height="13">](https://www.npmjs.com/package/on-off)
* [`one-event` <img alt="dependency gzipped size" src="https://badge-size.herokuapp.com/bfred-it/one-event/master/dist/one-event.browser.js?compression=gzip&amp;label=size" height="13">](https://github.com/bfred-it/one-event)
* [`get-scroll` <img alt="dependency gzipped size" src="https://badge-size.herokuapp.com/bfred-it/get-scroll/master/dist/get-scroll.browser.js?compression=gzip&amp;label=size" height="13">](https://github.com/bfred-it/get-scroll)

## License

MIT © [Federico Brigante](http://twitter.com/bfred_it)
