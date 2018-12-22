---
title: Customizing
slug: customizing
type: guide
order: 5
---

scrollnav includes some default settings that work for most situations, but if
your project requires a bit more customization, scrollnav can most likely meet
those. To modify the settings or set your own options, pass in a single object
as the second argument like this:

```js
  scrollnav.init(content, {
    key: value
  });
```

## Default settings

The following settings are editable to overwrite the default.

```js
{
  sections: 'selector',
  // string
  //
  // Sets the querySelector for the content's section landmarks, by default
  // it's 'h2'.

  insertTarget: targetNode,
  // HTML Node
  //
  // Sets the target Node for injecting the navigation, by default it's the
  // content Node passed to scrollnav.

  insertLocation: 'relativeLocation'
  // string
  //
  // Sets the injection location relative to the insertTarget, by default it's
  // 'before'.
  //
  // available options are 'append', 'prepend', 'after', or 'before'

  easingStyle: 'easingName',
  // string
  //
  // Sets the easing type for the scroll animation that is triggered by the
  // click event on a nav item, by default it's 'easeOutQuad'.
  //
  // available options are 'linear' 'easeInQuad', 'easeOutQuad',
  // 'easeInOutQuad', 'easeInCubic', 'easeOutCubic', 'easeInOutCubic',
  // 'easeInQuart', 'easeOutQuart', 'easeInOutQuart', 'easeInQuint',
  // 'easeOutQuint', easeInOutQuint

  updateHistory: true
  // boolean
  //
  // Sets the history behavior when a nav item is clicked, by default it's true
}
```

## Additional options

These additional options are editable but are not set by default.

```js
{
  subSections: '...',
  // string
  //
  // Sets the querySelector for the content's sub-section landmarks.

  onScroll: function() {...},
  // function
  //
  // Sets the callback to be triggered after the window scrolls when triggered
  // by the click event on a nav item.

  onInit: function() {...},
  // function
  //
  // Sets the callback to be triggered after the .init() method has completed.

  onUpdatePositions: function() {...},
  // function
  //
  // Sets the callback to be triggered after the .updatePositions() method
  // has completed.

  onDestroy: function() {...},
  // function
  //
  // Sets the callback to be triggered after the .destroy() method has
  // completed.

  debug: false
  // boolean
  //
  // Enables scrollnav's built in debug mode to log errors to the console and
  // display the active area threshold on screen, helpful for when you've hit a
  // snag you can't easily identify.
}
```

## Available methods

In addition to the `.init()` method scrollnav provides two additional public
methods.

### destroy()

To remove the current instance of scrollnav call the destroy method. If you
need to trigger a callback after scrollnav has been removed, use the
`onDestroy` option described above (passed either in the original init or with
the destroy method).

```js
scrollnav.destroy();
```

### updatePositions()

scrollnav doesn't track outside DOM changes. If your page's content is dynamic
and updates after scrollnav is initialized you'll need to recalcuate the
position data with the updatePositions method. If you need to trigger a
callback after the position data has been recalculated, use the
`onUpdatePositions` option described above (passed either in the original init
or with the updatePositions method).

```js
scrollnav.updatePositions();
```
