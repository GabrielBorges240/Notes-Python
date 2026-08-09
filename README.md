# Python Notes — Gabriel Borges

A single-page HTML/CSS/JS app with Python study notes, organized into topic cards. Each card opens a modal with explanations, code examples, and solved exercises.

## Usage

Open the `index.html` file directly in your browser — no server, build step, or dependencies required.

```bash
open index.html   # macOS
# or just double-click the file
```

## Features

- **27 topics** organized into 5 sections: Fundamentals, Data Structures, OOP & Errors, Ecosystem & Backend, and Advanced Features.
- **Real-time search** by title, tag, or keyword (field at the top of the page).
- **Per-topic modal** with:
  - Explanatory sections (text + code)
  - A "heads up" block with common pitfalls
  - Solved exercises with solution and explanation in an expandable `<details>` element
- Accessibility: keyboard navigation, `aria-*` attributes on interactive elements, focus returned to the card when the modal closes, `Esc` closes the modal or clears the search.

## File structure

Everything lives in a single file (`index.html`):

```
<style>   → dark theme, cards, modal, search bar
<body>    → header, search bar, card grids, modal
<script>  → DATA object with each topic's content
          → card and modal rendering
          → search/filter logic
```
