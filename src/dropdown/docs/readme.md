Dropdown is a simple directive which will toggle a dropdown menu on click or programmatically.

This directive is composed by three parts:

* `uib-dropdown` which transforms a node into a dropdown.
* `uib-dropdown-toggle` which allows the dropdown to be toggled via click. This directive is optional.
* `uib-dropdown-menu` which transforms a node into the popup menu.

### uib-dropdown settings

* `append-to`
  _(Default: `null`)_ -
  Appends the inner dropdown-menu to an arbitrary DOM element.

* `auto-close`
  _(Default: `always`)_ -
  Controls the behavior of the menu when clicked.
  * `always` - Automatically closes the dropdown when any of its elements is clicked.
  * `disabled` - Disables the auto close. You can control it manually with `is-open`. It still gets closed if the toggle is clicked, `esc` is pressed or another dropdown is open. It also won't be closed on `$locationchangeSuccess`.
  * `outsideClick` - Closes the dropdown automatically only when the user clicks any element outside the dropdown.
  
* `append-to-body`
  _(Default: `false`)_ -
  Appends the inner dropdown-menu to the body element.

* `is-open`
  _(Default: `false`)_ -
  Defines whether or not the dropdown-menu is open. The `uib-dropdown-toggle` will toggle this attribute on click.
  
* `keyboard-nav`:
  _(Default: `false`)_ -
  Enables navigation of dropdown list elements with the arrow keys.
  
### uib-dropdown-menu settings

* `template-url`
  _(Default: `none`)_ -
  You may specify a template for the dropdown menu. Check the demos for an example.
  
### Default settings `uibDropdownConfig`

* `appendToOpenClass`
  _(Default: `uib-dropdown-open`)_ -
  Class to apply when the dropdown is open and appended to a different DOM element.
  
* `openClass`
  _(Default: `open`)_ -
  Class to apply when the dropdown is open.
