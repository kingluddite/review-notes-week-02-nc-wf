# Avoid using !important when possible
Here's an example demonstrating why using `!important` in CSS is generally considered a bad practice:

Suppose we have the following CSS styling:

```css
.button {
  background-color: red !important;
}
```

And later in our stylesheet, we have the following:

```css
.button {
  background-color: green;
}
```

In this case, the background color of all elements with the class `.button` will be overridden by the `!important` declaration, and they will all have a red background color, regardless of any subsequent styling.

Now, let's say we want to introduce a specific style for buttons with the class `.special-button`, and we want them to have a blue background color. We might try to achieve this by adding the following CSS rule:

```css
.special-button {
  background-color: blue !important;
}
```

However, because of the `!important` declaration, this rule will not override the previous rule, and all buttons with the class `.special-button` will also have a red background color.

This example demonstrates how the use of `!important` can lead to issues with specificity and make it difficult to override styles when needed. It can also make your CSS harder to maintain and debug, as it introduces a global scope for styles that cannot be easily overridden.

Instead of relying on `!important`, it's generally better to use specific selectors and avoid excessive specificity in your CSS. This promotes a cleaner and more maintainable codebase and makes it easier to understand and debug stylesheets. If you find yourself needing to use `!important` frequently, it may be a sign that your CSS architecture could benefit from refactoring.