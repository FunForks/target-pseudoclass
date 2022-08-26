# Demonstration of the :target pseudo-class #

The [:target CSS pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:target) represents a unique element (the target element) with an id matching the URL's `fragment`.

This demo contains:
* A `<nav>` bar with links that set the `fragment` in the address bar
* A set of `<section>`s, whose `id`s match the `fragment`s in the links.

The CSS is designed to show only one `<section>` at a time: the one with the same `id` as the `fragment`.

When the page is first loaded, there may be no fragment. In this case, `section:last-child` is shown by default. If `section:last-child` has an older sibling which *does* have the same `id` as the `fragment`, `section:last-child` will be hidden.

[Click here](https://funforks.github.io/target-pseudoclass/) to see a live demo.