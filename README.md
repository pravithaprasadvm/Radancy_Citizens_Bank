# Citizens Bank - Mortgage Loan Officer Landing Page

A professional, responsive landing page implementation for Citizens Bank Mortgage Loan Officer Careers, built using semantic HTML5, modern CSS3, and a modular SCSS architecture.

---

## Technical Specifications & Compliance

This project strictly adheres to all specified guidelines and constraints:

- **Base Font**: Arial (`Arial, Helvetica, sans-serif`) is used as the base typography across the entire page. Custom web fonts are ignored in favor of native system fonts.
- **HTML5 & CSS3**: Pure semantic HTML5 markup (`<header>`, `<main>`, `<section>`, `<article>`, `<picture>`, `<source>`, `<blockquote>`, `<cite>`, `<footer>`) with modern CSS3 styling (CSS Grid, Flexbox, transitions, object-fit).
- **Responsive SASS Breakpoints**: Responsive design is handled exclusively through SCSS media query mixins (`@mixin respond`) with defined breakpoint tokens (`$mobile: 480px`, `$tablet: 768px`, `$laptop: 1024px`, `$desktop: 1280px`).
- **No Bootstrap**: 100% custom styling with zero third-party CSS or JS frameworks (no Bootstrap, Tailwind, or jQuery).
- **SCSS Architecture**: Clean, modular 7-1 SASS folder pattern with well-documented partials.

---

## Project Structure

```
Redancy/
├── .gitignore               # Git ignore rules for node_modules, cache, and OS files
├── README.md                # Project documentation and specifications
├── package.json             # NPM package file with Sass build/watch scripts
├── index.html               # Main semantic HTML5 landing page
├── css/
│   ├── style.css            # Compiled production CSS
│   └── style.css.map        # Source map for debugging
├── scss/
│   ├── style.scss           # Main SCSS entry point importing all partials
│   ├── _variables.scss      # Colors, typography, container widths, breakpoints
│   ├── _mixins.scss         # Media query mixins (@mixin respond) and utility helpers
│   ├── _base.scss           # CSS reset, body base styles, .container, .btn
│   ├── _header.scss         # Header navigation and Citizens Bank logo
│   ├── _hero.scss           # Hero picture element and responsive image rules
│   ├── _intro.scss          # "Our investment in you" intro section & CTA button
│   ├── _features.scss       # "Get the Citizens advantage" 2x2 grid & dividers
│   ├── _footprint.scss      # Citizens Bank footprint callout box
│   ├── _testimonials.scss   # 3-column loan officer testimonial cards & quotes
│   └── _footer.scss         # Footer, social icons, legal disclaimer & nav links
└── images/
    ├── logo.png             # Citizens Bank header logo
    ├── hero-desktop.jpg     # Desktop hero banner (1280x449)
    ├── hero-mobile.jpg      # Mobile hero banner (320x204)
    ├── ed.jpg               # Testimonial avatar - Ed
    ├── mark.jpg             # Testimonial avatar - Mark
    ├── john.jpg             # Testimonial avatar - John
    ├── icon-facebook.svg    # Footer social icon - Facebook
    ├── icon-twitter.svg     # Footer social icon - Twitter
    ├── icon-linkedin.svg    # Footer social icon - LinkedIn
    └── icon-youtube.svg     # Footer social icon - YouTube
```

---

## Getting Started

### 1. View the Landing Page
Simply open `index.html` in any modern web browser:
```bash
# Example using Windows start
start index.html
```

### 2. Compile SCSS to CSS

To compile the SASS files into CSS:

Using NPM (requires Node.js):
```bash
# One-time build
npm run build:sass

# Watch mode for active development
npm run watch:sass
```

Or directly using Dart Sass CLI:
```bash
# Direct SASS compilation
sass scss/style.scss css/style.css --source-map
```

---

## Responsive Breakpoints

| Breakpoint Variable | Max-Width | Target Viewport |
|---------------------|-----------|-----------------|
| `$mobile`           | `480px`   | Small smartphones |
| `$tablet`           | `768px`   | Tablets & large phones (switches hero to mobile image, 1-col grid) |
| `$laptop`           | `1024px`  | Small desktop / tablets in landscape |
| `$desktop`          | `1280px`  | Standard desktop container ($container-max-width: 1206px) |

---

## Browser Compatibility

- Google Chrome (latest)
- Mozilla Firefox (latest)
- Apple Safari (latest)
- Microsoft Edge (latest)
>>>>>>> 7703668 (Initial commit: Citizens Bank Landing Page with updated logo emblem favicon)
