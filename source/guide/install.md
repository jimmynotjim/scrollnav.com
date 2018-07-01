---
title: Install
slug: install
type: guide
order: 2
---

The compiled, production ready plugin is available in the `dist` directory.
Only use the code in the `src` directory if you plan to compile the plugin from
source as part of your project's build process.

_Note: Building from source assumes an intermediate level of knowledge about
build tooling. If you have trouble compiling the plugin on your own please use
the provided compiled files or seek help from Stack Overflow._

## Include directly

Include the minified Universal Module Definition (UMD) files as a script tag to
register scrollnav as a global variable.

### Manual

<a class="btn btn--outline"
href="https://unpkg.com/scrollnav@3.0.0/dist/scrollnav.umd.min.js"
title="Download scrollnav from unpkg.com">
  Download scrollnav v3.0.0
</a>

```html
<script src="[your assets directory]/scrollnav.umd.min.js"></script>
```
### CDN

If you want to leverage the speed and distribution of a CDN scrollnav is
available on [unpkg](https://unpkg.com/scrollnav@3.0.0/) and
[jsdelivr](https://cdn.jsdelivr.net/npm/scrollnav@3.0.0/). The URL is pinned to
v3.0.0 so you'll need to update the script tag whenever a new version is released.

```html
<script src="https://unpkg.com/scrollnav@3.0.0/dist/scrollnav.umd.min.js"></script>
```

## Package manager

*Note: The NPM registry does not allow for capital letters in package names, be
sure to use all lowercase `scrollnav` when searching for or installing
scrollnav from NPM, Yarn, or unpkg*

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
bower install scrollnav --save
```

_Note: The folks from Bower no longer recommend using Bower. Luckily they've
provided
[a guide on how to migrate to Yarn](https://bower.io/blog/2017/how-to-migrate-away-from-bower/)._
