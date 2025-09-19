CSS At-Rules Demonstration

This page demonstrates the use of CSS at-rules within a single responsive HTML page styled like a cafe website.

CSS At-Rules Used
1. @import

Used to import Google Fonts (Poppins):

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap');

2. @font-face

Loads a custom fallback font (Roboto as MyCustomFont):

@font-face {
  font-family: 'MyCustomFont';
  src: url('https://fonts.gstatic.com/s/roboto/v30/KFOmCnqEu92Fr1Mu4mxP.ttf') format('truetype');
}

3. @media

Applies responsive styles for screens 480px wide or smaller:

@media (max-width: 480px) {
  @layer base {
    .container {
      max-width: 90%;
      padding: 10px;
    }
  }
}

4. @keyframes

Defines a simple fade and scale animation:

@keyframes fadeInScale {
  from {
    opacity: 0;
    transform: scale(0.9);
  }
  to {
    opacity: 1;
    transform: scale(1);
  }
}

5. @supports

Checks for CSS variable support and defines custom properties:

@supports (--css: variables) {
  :root {
    --primary-color: #0078D7;
    --bg-color: #ffffff;
  }
}

6. @layer

Organizes CSS into logical layers:

@layer reset, base, components;

reset – removes default browser styles

base – basic layout and typography

components – reusable UI blocks like cards, buttons, forms
