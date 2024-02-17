# Recommended Naming Convention for HTML class and id's
Kebab case is another naming convention commonly used for CSS classes. In kebab case, class names are written in all lowercase letters with hyphens `-` separating words. This convention is often preferred for its simplicity and consistency.

Using kebab case can make class names more readable and easier to type, especially for developers who are not familiar with camelCase or BEM conventions. It also aligns well with naming conventions used in HTML attributes and JavaScript.

Here's an example of how you might use kebab case for naming CSS classes:

```html
<div class="card">
  <h2 class="card-title">Title</h2>
  <p class="card-content">Content goes here</p>
  <button class="card-button card-button-primary">Button</button>
</div>
```

In this example:
- `card` is the block.
- `card-title` and `card-content` are elements of the card block.
- `card-button` is an element of the card block, and `card-button-primary` is a modifier that changes the appearance of the button.

### Benefits of Kebab Case:

1. **Simplicity**: Kebab case is straightforward and easy to understand, making it a good choice for small to medium-sized projects or for developers who prefer a simpler naming convention.

2. **Consistency**: Kebab case aligns well with HTML attributes, JavaScript variables, and function names, promoting consistency across different parts of your codebase.

3. **Readability**: Class names written in kebab case are easy to read and interpret, even for developers who are not familiar with complex naming conventions.

However, it's essential to consider the specific needs and preferences of your team and project when choosing a naming convention. Consistency within your codebase is key, so whichever convention you choose, be sure to use it consistently throughout your CSS files.