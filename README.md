# ACCESSIBILITY

This repo is only for me, don't pull request.

## Hack Focus

Check the folder with the JS + SASS.

## Accordion

Check the folder with the edited JS.

https://github.com/smillart/WAI-ARIA-Patterns-And-Widgets/tree/master/dist/accordion

## Tablist

https://github.com/scottaohara/a11y_tab_widget

## Accessible menu

https://github.com/hotgeart/accessible-menu

Don't forget to add aria-current (for Drupal) :

```js
// add aria-current
if($('#menu-main .menu .is-active').length){
  $('#menu-main .menu .is-active').attr('aria-current', 'page');
}
```

## Slideshow/Slider

No solution at the moment.
