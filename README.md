# THIS IS MY PERSONAL BRANCH OF AN ABANDONED PROJECT.

Use at your own risk. It works for me with my needs. Message me if it helps you,
and I'll think about taking over the maintainer role. I wonder if I'm on the
one using it still...

Original project: https://github.com/SortableJS/knockout-sortablejs

---

knockout-sortablejs fork
-------------------
A Knockout.js binding to [SortableJS](https://github.com/RubaXa/Sortable/).

### Support KnockoutJS

Include [knockout-sortable.js](knockout-sortable.js)

```html
<div data-bind="sortable: {foreach: yourObservableArray, options: {/* sortable options here */}}">
	<!-- optional item template here -->
</div>

<div data-bind="draggable: {foreach: yourObservableArray, options: {/* sortable options here */}}">
	<!-- optional item template here -->
</div>
```

Using this bindingHandler sorts the observableArray when the user sorts the HTMLElements.

The sortable/draggable bindingHandlers supports the same syntax as Knockouts built in [template](http://knockoutjs.com/documentation/template-binding.html) binding except for the `data` option, meaning that you could supply the name of a template or specify a separate templateEngine. The difference between the sortable and draggable handlers is that the draggable has the sortable `group` option set to `{pull:'clone',put: false}` and the `sort` option set to false by default (overridable).

#### Other attributes are:
 * options: an object that contains settings for the underlaying sortable, ie `group`,`handle`, events etc.
 * collection: if your `foreach` array is a computed then you would supply the underlaying observableArray that you would like to sort here.
 * manuallyHandleUpdateEvents: a boolean to turn off the change events on update that other polymer elements listen to.


### NPM

 `npm install knockout-sortablejs`
