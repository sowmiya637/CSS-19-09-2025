 My Cafe – Responsive Layout with Modern CSS

CSS Highlights
1. CSS Variables

Defined in :root for easy reuse and theming:

:root {
  --primary-color: #0078D7;
  --highlight-color: #e91e63;
  --font-color: #292525;
  --bg-color: #fefefe;
  --sidebar-width: 250px;
}

2. Custom Selection Styling
::selection {
  background-color: var(--highlight-color);
  color: white;
}

3. Responsive Typography with clamp()
.hero h1 {
  font-size: clamp(2rem, 5vw, 4rem);
}

4. Button Hover Animation
.cta-button:hover {
  transform: scale(1.05);
}
