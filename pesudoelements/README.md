#  Pseudo-elements Demo – Favorite Quote Page

  Purpose

- `::before`
- `::after`
- `::first-letter`
- `::first-line`
- `::selection`
- `::placeholder`
::first-letter

 `::before` and `::after`
Add decorative quotation marks before and after the quote.

```css
.fancy-quote::before {
  content: "“";
}
.fancy-quote::after {
  content: "”";
}

Enlarges and colors the first letter of the quote.

.fancy-quote::first-letter {
  font-size: 200%;
  color: #e91e63;
}

::first-line

Styles the first line of the quote differently for emphasis.

.fancy-quote::first-line {
  color: #0078D7;
  font-weight: bold;
}

::selection

Customizes the background and text color when text is selected.

::selection {
  background-color: #ffb74d;
  color: black;
}

::placeholder

Styles the placeholder text in the input field.

input::placeholder {
  font-style: italic;
  color: #888;
}
