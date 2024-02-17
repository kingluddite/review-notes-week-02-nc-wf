# Advanced CSS Selectors

Below is an updated version of your HTML with a form added for people to write a review. I've included examples of grouping selectors, pseudo-classes, attribute selectors, and combinators:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Movie Reviews</title>
    <link rel="stylesheet" href="./assets/css/index.css" />
    <style>
      /* Grouping selectors */
      input[type="text"],
      textarea {
        width: 100%;
        padding: 8px;
        margin: 6px 0;
        border: 1px solid #ccc;
        border-radius: 4px;
        box-sizing: border-box;
      }

      /* Pseudo-classes */
      input[type="submit"]:hover {
        background-color: #45a049;
      }

      /* Attribute selectors */
      input[type="text"]:focus,
      textarea:focus {
        border: 1px solid #4caf50;
      }

      /* Combinators */
      label + input[type="text"] {
        margin-top: 10px;
      }

      form {
        margin-top: 20px;
      }
    </style>
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

      <!-- Form for submitting reviews -->
      <form>
        <h2>Write a Review</h2>
        <label for="movieTitle">Movie Title:</label>
        <input type="text" id="movieTitle" name="movieTitle" required />

        <label for="review">Your Review:</label>
        <textarea id="review" name="review" rows="4" required></textarea>

        <input type="submit" value="Submit" />
      </form>
    </div>
  </body>
</html>
```

In this example:

- **Grouping selectors**: The `input[type="text"]` and `textarea` selectors group together to apply styling to both text inputs and textareas.
- **Pseudo-classes**: The `input[type="submit"]:hover` pseudo-class is used to change the background color of the submit button when hovered over.
- **Attribute selectors**: The `input[type="text"]:focus` and `textarea:focus` selectors apply styling to text inputs and textareas when they are in focus.
- **Combinators**: The `label + input[type="text"]` combinator selects text inputs that directly follow a label element and adds margin to them.

These selectors and pseudo-classes help style the form for submitting reviews in the movie review page.
