# Decoration Store

Decoration Store is a website designed and implemented as a project of Module 2 of the Her-Tech JavaScript Bootcamp. It replicates an interior decoration brand site, presenting decorating ideas and home products for purchase.

## Main sections:

- First section with title, slogan and descriptive paragraph, including a featured gallery showcasing decorative elements
- Second section with a product showcase including images, clickable elements, prices and a link for browsing all products to buy

## Technologies Used:

- HTML:

  General structure by sections:

  - main: groups the visual and functional content of the website:
    - decoration-section: includes a centered headline, introductory text and a grid-based gallery
    - products-section: displays featured product with cards made with flexbox, including their name and price, and one final link for the option "Shop All" products

- CSS:

  CSS created in a nested way

  Selectors used:

  - Universal: /\* in reset folder, for margin and padding
  - Tag: main, section, img, p, etc., for global structure
  - Class: .decoration, .text-container, .products-info, .products-name, etc., for semantic and structured styling
  - Combined: .products-section .shop-all a, .img-container img, for targeting elements in nested components

  Pseudo-classes:

  - :hover on elements like .products-name:hover for interactivity

  Layout systems:

  - Grid layout:

    - Used in .img-container for organizing decoration images in both mobile and desktop versions
    - Adjusted with grid-template-columns and grid-template-rows depending on screen size

  - Flexbox layout:
    - Used for product cards, product info alignment, and general responsiveness
    - Properties like flex-wrap, justify-content, align-items or gap, used to create a consistent layout

  Responsive design:

  - Implemented using @media (min-width: 1024px)
  - The structure adapts from a vertical mobile layout to a horizontal desktop layout
  - Text sizes, image heights, and layout alignments are adjusted specifically for desktop

- CSS variables folder:

  - Organisation of colours and sizes (fonts and other properties) for use in cases where they had the same value
  - Examples: --main-background, --products-background, --primary-font, --thin-text

- CSS fonts folder:

  - Custom fonts loaded via @font-face, including variants of "Playfair Display", "Montserrat" and "Libre Baskerville"

- Tools:
  - Developed using Visual Studio Code
  - Files structured into folders: /css, /images, and main index.html
  - Images folder:
    - All images are locally stored in a folder named /images
    - Alt attributes are used for accessibility and clarity
