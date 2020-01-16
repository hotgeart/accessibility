# accessibility

This repo is only for me

## Accordion

Check the folder with the edited JS.

## Tablist

https://mynamesleon.github.io/aria-tablist/

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

No solution at the moment
