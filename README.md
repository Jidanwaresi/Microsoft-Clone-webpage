# Microsoft Homepage Clone

A frontend recreation of the Microsoft homepage built using HTML5 and CSS.

This project was created as a hands-on practice project to understand how a complete webpage can be structured using HTML and CSS, and how Flexbox, CSS Grid, spacing, sizing, alignment, and hover effects work together to build a consistent interface.

> This is a learning project and is not affiliated with or endorsed by Microsoft.

---

## Overview

The project recreates a Microsoft-inspired homepage layout with multiple structured sections:

- Navigation bar
- Hero section
- Hero action links
- Product card grid
- Horizontal promotional sections
- Business section
- Social links
- Multi-column footer

The implementation uses HTML for the page structure and CSS for layout, spacing, alignment, sizing, styling, and visual interaction.

No JavaScript is used in this project.

---

## Tech Stack

- HTML5
- CSS
- Remix Icon

---

## HTML Structure

The page is organized using semantic HTML elements such as:

- `header`
- `nav`
- `main`
- `section`
- `footer`

The main content is divided into separate sections for the hero area, hero action links, product cards, horizontal promotional content, business cards, and social links.

The footer contains multiple `.footer-box` sections for different categories.

---

## Key CSS Concepts Implemented

### 1. CSS Flexbox

Flexbox is used in several parts of the interface for directional layouts and alignment.

Examples include:

- Navbar layout
- Left and right navbar groups
- Hero text layout
- Product card content
- Horizontal promotional sections
- Business card content
- Social links
- Footer columns

The project helped me understand how properties such as:

```css
display: flex;
justify-content;
align-items;
gap;
flex-direction;
```

work together through parent-child relationships.

---

### 2. CSS Grid

CSS Grid is used for repeated card layouts.

The product section uses:

```css
display: grid;
grid-template-columns: repeat(4, 1fr);
gap: 2rem;
```

The business section also uses Grid:

```css
display: grid;
grid-template-columns: repeat(4, 1fr);
gap: 1.5rem;
```

This helped me understand how Grid can be used to organize repeated items into multiple columns.

---

### 3. Flexible Product Card Layout

The product cards contain different amounts of text, which can affect the position of the buttons.

The `.product-details` container uses:

```css
display: flex;
flex-direction: column;
flex-grow: 1;
```

and the button uses:

```css
margin-top: auto;
```

This allows the content area to grow and keeps the button positioned toward the bottom of the available card content area.

---

### 4. Business Card Layout

The business cards use a similar vertical Flexbox structure.

The `.business-card` uses:

```css
display: flex;
flex-direction: column;
```

while `.business-details` uses:

```css
flex: 1;
display: flex;
flex-direction: column;
```

The business button uses:

```css
margin-top: auto;
```

This creates a consistent vertical structure for the business cards.

---

### 5. Background Image Handling

The hero section uses a background image with:

```css
background-position: center;
background-size: cover;
```

This controls how the background image is positioned and scaled within the hero section.

---

### 6. Image Sizing

Images inside the product and business sections use:

```css
width: 100%;
height: auto;
```

This keeps the images proportional while allowing them to fill the width of their containing elements.

---

### 7. Hover Effects and Transitions

Hover interactions are implemented using CSS.

The product and business cards use:

```css
transition: all 0.3s ease;
transform: translateY(-5px);
box-shadow: 0 8px 25px rgba(0,0,0,0.15);
```

These effects provide visual feedback when the user hovers over the cards.

Hover styling is also used for navigation links, buttons, and social links.

---

### 8. Spacing and Alignment

The project makes extensive use of:

```css
margin
padding
gap
width
min-height
```

to control spacing, proportions, and positioning between elements.

Working with these properties helped me understand how spacing is affected by the relationship between parent and child elements.

---

## Challenges I Faced

### Matching Layout Spacing

Recreating an existing interface required more attention to spacing and alignment than creating a layout from scratch.

I had to understand how different combinations of:

- `margin`
- `padding`
- `gap`
- `align-items`
- `justify-content`

affect the final layout.

---

### Keeping Card Buttons Consistent

The product cards contain different amounts of content.

Because of that, the buttons could appear at different positions.

Using:

```css
flex-direction: column;
flex-grow: 1;
margin-top: auto;
```

helped maintain a more consistent button position within the cards.

---

### Choosing Between Flexbox and Grid

The project gave me practical experience in deciding where Flexbox and Grid fit better.

For example:

- Flexbox is used for directional alignment inside components.
- Grid is used for repeated card layouts across multiple columns.

This made the distinction between the two layout systems more practical than learning their properties separately.

---

## What I Learned

This project helped me move from learning individual CSS properties to using them together to solve layout problems.

I learned how to:

1. Structure a complete webpage using HTML.
2. Use Flexbox for directional layouts and alignment.
3. Use CSS Grid for repeated multi-column layouts.
4. Manage spacing using margin, padding, and gap.
5. Use parent-child relationships to control layout behavior.
6. Keep buttons consistently positioned inside flexible card layouts.
7. Handle background images using `background-size` and `background-position`.
8. Use transitions, transforms, and box shadows for hover feedback.

The main learning was that frontend development is not only about knowing CSS properties. It is also about understanding how those properties interact with the structure of the page.

---

## Project Structure

```text
Microsoft-Homepage-Clone/
│
├── index.html
├── style.css
├── icons8-microsoft-48.png
│
└── icons/
    ├── icons8-facebook-48.png
    ├── icons8-x-50.png
    └── icons8-youtube-48.png
```

---

## Project Sections

### Navigation Bar

The navigation bar contains:

- Microsoft navigation links
- All Microsoft
- Search
- Cart
- Sign in
- Circular `ME` button

The layout is handled using Flexbox.

---

### Hero Section

The hero section contains:

- `New` label
- Heading
- Description
- `Learn more` button
- Background image

The hero background uses `background-size: cover` and `background-position: center`.

---

### Hero Action Links

The `.hero-btns` section contains links for:

- Shop Microsoft 365
- Shop XBOX
- Get Windows 11
- Shop Surface

The section uses Flexbox for alignment.

---

### Product Section

The `.product-box` section contains four product cards.

Each card contains:

- Product image
- Heading
- Description
- Action button

The cards are arranged using CSS Grid.

---

### Horizontal Promotional Sections

The `.product-box2` section is used for horizontal image-and-content layouts.

Each layout contains:

- Text content
- Description
- Button
- Large supporting image

The `.container` uses Flexbox to place the content and image side by side.

---

### Business Section

The `.business-section` contains four business cards.

Each card contains:

- Image
- Heading
- Description
- Action button

The cards are arranged using CSS Grid.

---

### Social Links

The social section contains links for:

- Facebook
- X
- YouTube

The icons are arranged using Flexbox.

---

### Footer

The footer contains six `.footer-box` columns:

- What's new
- Microsoft Store
- Education
- Business
- Developer & IT
- Company

The footer uses Flexbox to distribute the columns across the available space.

---

## Current Scope

This project focuses on the HTML and CSS implementation of the interface.

The primary purpose was to practice:

- Page structure
- Flexbox
- CSS Grid
- Spacing
- Alignment
- Image sizing
- Background image handling
- Card layouts
- Hover effects

JavaScript functionality is not included in the current implementation.

---

## Future Improvements

Possible future improvements include:

- Responsive layouts for smaller screens
- Mobile navigation
- Interactive navigation behavior
- Further accessibility improvements
- Additional visual refinement

---

## Learning Outcome

This project was an important step in understanding how HTML and CSS work together to build a complete interface.

Instead of looking at CSS properties individually, I practiced thinking about:

- Page structure
- Parent-child relationships
- Layout systems
- Content flow
- Spacing
- Alignment
- Consistency

The project helped me become more comfortable with solving layout problems through CSS rather than relying on manual positioning.

---

## Acknowledgement

Thanks to my frontend mentor, Devendra Dhote, for encouraging a build-first learning approach.

The concepts practiced through tutorials and lab-based exercises helped me understand the logic behind the implementation and work through layout problems independently.

---

## Author

Jidan Waresi

Learning and building frontend projects with HTML and CSS.

---

## License

This project is intended for educational and learning purposes only.
