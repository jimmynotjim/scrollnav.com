---
title: Setup
type: guide
order: 3
---

scrollnav works by scanning a single passed [HTML Element](https://developer.mozilla.org/en-US/docs/Web/API/Element) for section
landmarks--by default `h2` elements--that it then uses to generate the
navigation schema.

## Page markup

The content should be wrapped in a container to avoid including unintended
landmarks in the nav. If we were to look at a typical document, it might look
like this:

```html
  <div class="main-content">
    <h2>First section</h2>
    ...
    <h2>Second section</h2>
    ...
    <h2>Third section</h2>
    ...
  </div>
```

## Initialize

Next, we'll save the `.main-content` container Element to a variable and then
pass it on to scrollnav. In this example we'll use `.querySelector()` but you
could also use `.getElementByID()` or `.getElementByClassName()`.

```js
const content = document.querySelector('.main-content');
scrollnav.init(content);
```

scrollnav will then loop through the the `h2` elements, add an ID if they don't
already have one, build the nav, and then inject it just before the
`.main-content` Node. The result for our example document would look like this:

```html
<nav class="scroll-nav">
  <ol class="scroll-nav__list">
    <li class="scroll-nav__item">
      <a class="scroll-nav__link" href="#scroll-nav__1">
        First heading
      <a>
    </li>
    ...
  </ol>
</nav>
<div class="main-content">
  <h2 id="scroll-nav__1">First Heading</h2>
  ...
</div>
```
