---
title: Overview
slug: overview
type: guide
order: 1
---

## What is scrollnav?

scrollnav.js is a small (2.4kb gzipped), dependency free JavaScript plugin for
auto generating single page navigation with active highlighting (aka
scrollspy). Useful for creating a Table of Contents for a large document (think
Wikis), navigation for a single page website, or anything else you might think
of. This page itself uses scrollnav to create the sub-sections of the Guide
navigation.

scrollnav works by scanning a block of content for section landmarks (typically
heading elements) and generating a list of links from those landmarks. It then
tracks the scroll location of the document and highlights the appropriate link.
While previous versions injected wrappers within the content, the current
version (ver 3) takes a much lighter approach, only changing the DOM as
necessary.

## Browser Compatibility

To keep scrollnav small, default support starts with
[ES6 compatible browsers](https://caniuse.com/#feat=arrow-functions). To support
[ES5 compatible browsers](https://caniuse.com/#feat=es5) you must provide your
own polyfills or rely on a third party library like pollyfills.io. I personally
use the following polyfill.io feature parameters to support scrollnav in
IE 10 & 11.

```hmlt
<script src="https://cdn.polyfill.io/v3/polyfill.min.js?features=default,NodeList.prototype.forEach,Array.prototype.includes"></script>
```

To add your own polyfills you will need to build the project from source.

<p class="article-note">_Building from source assumes an intermediate level of
knowledge about build tooling. If you have trouble compiling the plugin on your
own please use the provided compiled files or seek help from
[Stack Overflow](https://stackoverflow.com/search?tab=newest&q=scrollnav.js)_
</p>

## Changelog

v3.0.1 is the current stable release. For detailed changes in each release
please refer to the
[release notes](https://github.com/jimmynotjim/scrollnav/releases). Be sure you
[understand the changes](tktktk) before updating, v3 is a complete re-write of
the library and requires a small amount of manual work to udpate from v2.

## License

scrollnav is Copyright &copy; 2012-2018 by James Wilson (aka
[@jimmynotjim](https://github.com/jimmynotjim)), released under the
[MIT license](https://github.com/jimmynotjim/scrollnav/blob/master/LICENSE-MIT).
This means you can re-create, edit or share the plugin as long as you maintain
the same open licensing.
