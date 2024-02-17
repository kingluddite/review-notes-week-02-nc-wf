# Display none

Whether to use `display: none` (not `display: hidden`) or not depends on the specific use case and desired behavior.

`display: none` is a CSS property that hides the element completely. It removes the element from the flow of the document, meaning it won't take up any space, and it won't be rendered on the page. Essentially, it's as if the element doesn't exist in the HTML.

Here are some common scenarios where `display: none` might be used:

1. **Responsive Design**: You might use `display: none` to hide certain elements on smaller screens to improve the mobile experience. For example, you might hide a sidebar navigation menu on mobile devices where space is limited.

2. **Progressive Enhancement**: You might initially hide certain elements that are part of a more complex interaction or feature and reveal them later using JavaScript or CSS when needed.

3. **Accessibility**: You might hide elements that are purely decorative or redundant for screen readers using `display: none` combined with proper ARIA attributes or roles.

However, there are also cases where using `display: none` should be avoided:

1. **SEO**: Search engines may interpret hidden content as an attempt to manipulate search rankings, which could negatively impact your site's SEO.

2. **Accessibility**: Hiding content that is essential for screen reader users without providing an accessible alternative can make your site less accessible.

3. **Performance**: While hiding elements with `display: none` removes them from the render tree, it doesn't necessarily prevent them from being downloaded, especially for CSS background images. This can impact performance if there are many hidden elements with large images or other resources.

In summary, `display: none` can be a useful tool when used judiciously and with consideration for accessibility, performance, and SEO implications. It's essential to weigh the pros and cons and consider alternative approaches when appropriate.
