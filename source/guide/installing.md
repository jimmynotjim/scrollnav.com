---
title: Installing
slug: installing
type: guide
order: 2
---

The compiled, production ready plugin is available in the `/dist` directory.
Only use the code in the `/src` directory if you plan to compile the plugin from
source as part of your project's build process.

<p class="article-note">_Building from source assumes an intermediate level of
knowledge about build tooling. If you have trouble compiling the plugin on your
own please use the provided compiled files or seek help from
[Stack Overflow](https://stackoverflow.com/search?tab=newest&q=scrollnav.js)_
</p>

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

Install with [Yarn](https://yarnpkg.com/en/)

```bash
yarn add scrollnav
```

Install with [NPM](https://www.npmjs.com/)

```bash
npm install scrollnav
```

Install with [Bower](https://bower.io/)

```bash
bower install scrollnav --save
```

<p class="article-note">_The folks from Bower no longer recommend using Bower.
Luckily they've created
[a guide to migrating to Yarn](https://bower.io/blog/2017/how-to-migrate-away-from-bower/)._
</p>
