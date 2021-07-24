bulma-popover
=============

This extension is based on the [bulma-tooltip] extension, but allows for more complex content to be placed in the pop up.
It is styled like Bulma's builtin box element.

[bulma-tooltip]: https://github.com/Wikiki/bulma-tooltip

Core Classes
------------

- `popover` popover wrapper
- `popover-trigger` display popover when this element is focused
- `popover-content` the content of the popover

Modifiers
---------

- `.is-popover-active` can be used to hold the popover open.
  This can be used to trigger the popover from JavaScript.
- `.is-not-popover-hover` can be used to disable popover activation on hover

Positioning
-----------

The popover is positioned above the popover wrapper by default (top).

The following modifiers can be used to set the popover position:

- `is-popover-top`
- `is-popover-right`
- `is-popover-bottom`
- `is-popover-left`

The position can also be set responsively using the following class:

`is-popover-${position}-${breakpoint}`

Where `${position}` is top, right, bottom, or left and `${breakpoint}` is one of [Bulma's breakpoints][bulma-breakpoint].
For example, `is-popover-bottom-desktop` will position the popover below the popover wrapper for desktop (1024 px) and above.

[bulma-breakpoint]: https://bulma.io/documentation/overview/responsiveness/#breakpoints

Example
-------

```html
<div class="popover is-popover-bottom">
  <button class="button is-primary popover-trigger">Table Popover</button>
  <div class="popover-content">
    <table class="table">
      <thead>
        <tr><th>Fruit</th><th>Color</th></tr>
      </thead>
      <tbody>
        <tr><td>Apple</td><td>Red</td></tr>
        <tr><td>Banana</td><td>Yellow</td></tr>
        <tr><td>Cucumber</td><td>Green</td></tr>
      </tbody>
    </table>
  </div>
</div>
```

Variables
---------

Name | Default Value
---- | -------------
`$popover-max-width` | `24rem`
`$popover-color` | `$text`
`$popover-background-color` | `$white`
`$popover-radius` | `$radius-large` (6px)
`$popover-shadow` |
`$popover-caret-shadow` |
