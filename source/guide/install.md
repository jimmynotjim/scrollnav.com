---
title: Install
date: 2018-06-03 15:39:20
---

The compiled, production ready plugin is available in the `dist` directory.
Only use the code in the `src` directory if you plan to compile the plugin from
source as part of your project's build process.

_Note: Building from source assumes an intermediate level of knowledge about
build tooling. If you have trouble compiling the plugin on your own please use
the provided compiled files or seek help from Stack Overflow_

## Direct include

Include the minified Universal Module Definition (UMD) files as a script tag to
register scrollNav as a global variable.

### Manual

[Download scrollNav v3.0.0](https://unpkg.com/scrollNav@3.0.0/dist/scrollNav.umd.min.js)

```html
<script src="[your assets directory]/scrollNav.umd.min.js"></script>
```
### CDN

If you want to leverage the speed and distribution of a CDN scrollNav is
available on [unpkg](https://unpkg.com/scrollnav@3.0.0/) and
[jsdelivr](https://cdn.jsdelivr.net/npm/scrollnav@3.0.0/). The URL is pinned to
v3.0.0 so you'll need to update script tag whenever a new version is released.

```html
<script src="https://unpkg.com/scrollNav@3.0.0/dist/scrollNav.umd.min.js"></script>
```

## Package manager

*Note: The NPM registry does not allow for capital letters in package names, be
sure to use all lowercase `scrollnav` when searching for or installing
scrollNav from yarn or NPM*

Install with [Yarn](tktktk)

```bash
yarn add scrollnav
```

Install with [NPM](tktktk)

```bash
npm install scrollnav
```

Install with [Bower](tktktk)

```bash
bower install scrollNav --save
```

_Note: The folks from Bower no longer recommend using Bower. Luckily they've
provided a guide on
[how to migrate to Yarn](https://bower.io/blog/2017/how-to-migrate-away-from-bower/)._


