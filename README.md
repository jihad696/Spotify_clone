# Spotify Clone (UI)

## Project overview
A lightweight static UI that clones the look-and-feel of Spotify's Browse experience. It demonstrates layout patterns for a music streaming web app: navigation, search, browse cards, side panel, and footer.

## Technologies used
- HTML5
- CSS3 (Flexbox and CSS Grid)
- Plain static assets (images, SVG icons)

## Semantic HTML
The project uses semantic HTML elements such as `<header>`, `<nav>`, `<main>`, `<aside>`, `<section>`, and `<footer>` to provide meaningful page structure and improve SEO and assistive technology navigation.

## Accessibility
- Landmarks (`role` attributes and semantic tags) are used for easier navigation by screen readers.
- Visible labels and `aria-label` provided for interactive controls (search, nav links, icons).
- Contrast-conscious color choices are used in the design variables, but final contrast should be validated with automated tools.
- Focusable controls (buttons, links, inputs) use clear visible states and large hit targets where possible.

## Layout techniques
- Flexbox is used for horizontal layouts such as the main navigation and quick action rows.
- CSS Grid is used for the browse card layout and category grids to provide consistent multi-column arrangements.

## Folder structure
- `index.html` — main landing page
- `pages/` — additional pages (e.g., `browse_all.html`)
- `assets/` — images and icons
- `css/` — all stylesheets (reset, variables, layout, components, page-specific)

## How to run
1. Open `index.html` or any page in the `pages/` folder directly in a browser.
2. No build step or server is required for the static UI. For a local static server (recommended for consistent relative paths):

```bash
# using Python 3.x
python -m http.server 8000
# then open http://localhost:8000/pages/browse_all.html
```

## Future improvements
- Consolidate and document design tokens (colors, spacing, typography) in `variables.css`.
- Add unit tests for visual regressions (Percy, Chromatic) if ported to a component-driven framework.
- Improve accessibility: keyboard focus trap tests, screen reader validations, and color contrast tuning.
- Make responsive design strict and consistent across breakpoints (mobile-first approach).
- Convert repeated card markup into templates or components if integrating into a framework.

---
