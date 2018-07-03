---
title: Styling
slug: styling
type: guide
order: 4
---

Congratulations, you should now have an instance of scrollnav on your page, but
wait, why doesn't it look like the examples?

To keep the library simple and avoid inheritence issues, scrollnav doesn't come
bundled with default styles. I've [created a few demos](tktktk) to give you
some general direction, but it's completely up to you to make scrollnav work
for your specific situation.

## Markup structure

scrollnav follows [BEM (Block, Element, Modifier) Methodology](tktktk) for
providing class names to its markup. `scroll-nav` is the block, with `__list`,
`__item`, and `__link` as elements. The structure looks like this.

```css
nav.scroll-nav
  ol.scroll-nav__list
    li.scroll-nav__item.scroll-nav__item--active
      a.scroll-nav__link
```

<p class="article-note">For a good overview on BEM Methodology, read
[MindBEMding - getting your head 'round BEM syntax](tktktk)</p>


## Active highlighting

When a user scrolls the document, scrollnav watches for each section to pass
the threshold of the active area. As that happens the `--active` modifier is
added to the `__item` element (and subsequently removed from previously active
item). Use this to change or udpate the look of the active items in the
nav.

<p class="article-note">To view the location of the active area threshold
within your document enable `debug` mode from scrollnav's list of
[additional options](tktktk).</p>
