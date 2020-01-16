
```js
// hack focus

(function(body) {

	var usingMouse;

	var preFocus = function(event) {
		usingMouse = (event.type === 'mousedown');
	};

	var addFocus = function(event) {
		if (usingMouse)
			event.target.classList.add('focus--mouse');
	};

	var removeFocus = function(event) {
		event.target.classList.remove('focus--mouse');
	};

	var bindEvents = function() {
		body.addEventListener('keydown', preFocus);
		body.addEventListener('mousedown', preFocus);
		body.addEventListener('focusin', addFocus);
		body.addEventListener('focusout', removeFocus);
	};

	bindEvents();

})(document.body);
```

```sass
a,
[role="link"],
[role="button"],
input,
select,
button {
  &:focus {
    outline: 0.1875rem solid #2135FC;
    outline-offset: 0.125rem;
  }
}


a,
[role="link"],
[role="button"],
input,
select,
button {
  &.focus--mouse {
    &:focus {
      outline: none;
    }
  }
}
```
