# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨





CODE
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Responsive Webpage with Flexbox & Grid</title>
  <style>
    /* Reset and base styles */
    * {
      box-sizing: border-box;
    }
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      line-height: 1.6;
    }

    /* Container */
    .container {
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }

    /* Header */
    header {
      background: #4CAF50;
      color: white;
      padding: 1rem;
      text-align: center;
      font-size: 1.5rem;
      font-weight: bold;
    }

    /* Main content area using Grid */
    main {
      display: grid;
      grid-template-columns: 3fr 1fr;
      gap: 1rem;
      padding: 1rem;
      flex-grow: 1;
      background: #f4f4f4;
    }

    /* Article */
    article {
      background: white;
      padding: 1rem;
      border-radius: 5px;
    }

    /* Sidebar */
    aside {
      background: white;
      padding: 1rem;
      border-radius: 5px;
    }

    /* Footer using Flexbox */
    footer {
      background: #333;
      color: white;
      padding: 1rem;
      text-align: center;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    /* Responsive adjustments */
    @media (max-width: 768px) {
      main {
        grid-template-columns: 1fr;
      }
      footer {
        flex-direction: column;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <header>My Responsive Site</header>
    <main>
      <article>
        <h2>Main Content</h2>
        <p>
          This is the main content area. It takes up the majority of space on larger screens.
          Resize the browser to see how the layout changes responsively.
        </p>
      </article>
      <aside>
        <h3>Sidebar</h3>
        <p>
          Sidebar content, such as navigation links, ads, or additional info.
        </p>
      </aside>
    </main>
    <footer>
      <p>&copy; 2025 My Responsive Site. All rights reserved.</p>
    </footer>
  </div>
</body>
</html>

