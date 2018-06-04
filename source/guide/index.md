---
title: Overview
date: 2018-06-03 15:39:20
---

Welcome to the scrollNav documentation. If you have any problems using
scrollNav, take a look at the [troubleshooting guide](tktktk), ask a question
on [Stack Overflow](tktktk), or report an issue on [GitHub](tktktk).

## What is scrollNav?

scrollNav.js is a small (2.4kb gzipped), dependency free JavaScript plugin for
auto generating single page navigation with active highlighting. Useful for
creating a Table of Contents for a large document (think Wikis), navigation for
a single page website, or anything else you might think of.

scrollNav works by scanning a block of content for section landmarks (typically
heading elements) and generating a list of links from those landmarks. It then
tracks the scroll location of the document and highlights the appropriate link.
While previous versions injected wrappers within the content, the current
version (ver 3) takes a much lighter approach, only changing the DOM as
necessary.

## Browser Compatibility

scrollNav supports all [ES5 compatible browsers](https://caniuse.com/#feat=es5)
using polyfills for modern features (IE8 and below are not supported). If you
wish to provide your own polyfills or only support
[ES6 compatible browsers](https://caniuse.com/#feat=arrow-functions), feel free
to compile the plugin from source as part of your project's build process.

_Note: Building from source assumes an intermediate level of knowledge about
build tooling. If you have trouble compiling the plugin on your own please use
the provided compiled files or seek help from Stack Overflow_

## Changelog

v3.0.0 is the current stable release. For detailed changes in each release
please refer to the [release notes](tktktk). Be sure you
[understand the changes](tktktk) before updating, v3 is a complete re-write of
the plugin.

## License

scrollNav is Copyright &copy; 2012-2018 James Wilson, released under the
[MIT license](tktktk). This means you can re-create, edit or share the plugin
as long as you maintain the same open licensing.
