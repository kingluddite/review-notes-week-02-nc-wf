# Display in CSS

- Slide #16 in Presentation

Here's your HTML and CSS with shorthand properties and with the addition of examples for `display: inline-block` and `display: block`:

HTML:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Movie Reviews</title>
    <link rel="stylesheet" href="./assets/css/index.css" />
  </head>
  <body>
    <div class="container">
      <h1>Movie Reviews</h1>

      <div class="review">
        <h2>Movie Title 1</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed et urna
          nec odio vestibulum vestibulum. Nulla facilisi. Donec ac diam ligula.
          Vivamus in felis libero.
        </p>
        <p><strong>Rating:</strong> 4/5</p>
      </div>

      <div class="review">
        <h2>Movie Title 2</h2>
        <p>
          Nullam at elit ex. Duis tristique convallis libero, eget suscipit nunc
          sollicitudin et. Curabitur a turpis quis felis consequat vestibulum.
        </p>
        <p><strong>Rating:</strong> 3.5/5</p>
      </div>

      <div class="review">
        <h2>Movie Title 3</h2>
        <p>
          Vestibulum ante ipsum primis in faucibus orci luctus et ultrices
          posuere cubilia Curae; Nam convallis nisi eu tellus bibendum
          malesuada.
        </p>
        <p><strong>Rating:</strong> 5/5</p>
      </div>
    </div>
  </body>
</html>
```

CSS:

```css
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f4f4f4;
}

.container {
  width: 80%;
  margin: 0 auto;
  padding: 20px;
}

h1 {
  text-align: center;
}

.review {
  background-color: #ffffff;
  border-radius: 5px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  padding: 20px;
  margin-bottom: 20px;
}

/* Using display: inline-block */
.review {
  display: inline-block;
  width: 30%; /* Adjust width as needed */
  margin: 10px; /* Add margin to separate reviews */
}

/* Using display: block */
.review {
  display: block;
  margin-top: 20px; /* Add top margin to separate reviews */
}
```

Explanation:

- In the CSS, I've replaced the individual margin and padding properties with shorthand properties for `body` and `.container`.
- For the `.review` class, I've added examples for both `display: inline-block` and `display: block`.
  - With `display: inline-block`, the review elements will flow horizontally and allow other elements to sit next to them. I've set the width to 30% for illustration purposes, but you can adjust it based on your layout requirements.
  - With `display: block`, each review element will start on a new line, effectively stacking them vertically. I've added a top margin to separate the reviews visually.
