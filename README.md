# youtube\_project\_website

A simple, static website project that showcases a YouTube-style channel landing page. Built with semantic HTML and modern, modular CSS. Ideal for practising layout, typography, responsive design, and asset organisation.

## Live Demo

👉 [https://yanamak89.github.io/youtube\_project\_website/](https://yanamak89.github.io/youtube_project_website/)

## Preview

Open `index.html` directly in your browser or run a lightweight local server (see below).

## Features

* Clean, semantic HTML structure.
* Modular CSS in `/styles` for easier maintenance.
* Organised assets for icons and channel imagery.
* Starter layout that you can extend into a multi-page site.

## Project structure

```
/
├── channel-pictures/     # Channel cover and profile assets
├── icons/                # UI icons (SVG/PNG)
├── intro-to-html/        # Learning notes or example snippets used in this project
├── styles/               # CSS stylesheets
├── thumnails/            # Video thumbnails (NOTE: consider renaming to `thumbnails/`)
└── index.html            # Main entry page
```

> Tip: If you rename `thumnails` to `thumbnails`, remember to update any paths in `index.html` and CSS.

## Getting started

### Option 1 — Open the file

1. Download or clone the repository.
2. Double-click `index.html` to open it in your browser.

### Option 2 — Run a local server (recommended)

Using VS Code with the **Live Server** extension:

1. Open the project folder in VS Code.
2. Right-click `index.html` → **Open with Live Server**.

Or use Python (already on most systems):

```bash
# from the project root
python3 -m http.server 8000
# then visit http://localhost:8000 in your browser
```

## Customize

* **Branding**: Replace images in `channel-pictures/` and `thumnails/` with your own.
* **Icons**: Add or swap icons in `icons/` and update their `<img>` or `<svg>` references.
* **Styles**: Edit files in `styles/` to change colors, spacing, and layout.
* **Content**: Update titles, descriptions, and links inside `index.html`.

## Responsive design

This project is a great place to practice responsive patterns. Consider adding:

* A fluid grid for thumbnails.
* Flex or Grid-based header that collapses to a mobile-friendly menu.
* Media queries for key breakpoints (e.g., 360px, 768px, 1024px).

## Accessibility

* Ensure all images have descriptive `alt` text.
* Use meaningful headings (`h1` → `h2` → `h3`).
* Maintain sufficient color contrast and visible focus states.

## Deployment (GitHub Pages)

1. Commit and push your latest changes to the `main` branch.
2. In your GitHub repo: **Settings** → **Pages** → **Branch**: `main` (root), then **Save**.
3. Your site will be available at the Pages URL shown in the banner.

## Roadmap / Ideas

* [ ] Rename `thumnails` → `thumbnails` and update references.
* [ ] Add a dedicated `videos.html` page listing all uploads.
* [ ] Extract color variables and spacing scale into a `styles/variables.css` file.
* [ ] Add a dark theme toggle (prefers-color-scheme + CSS variables).
* [ ] Introduce a simple build step (e.g., PostCSS) for minification.

## Attribution & licenses

* Make sure you have rights to use any images, logos, and icons you include. If assets are placeholders, replace them before publishing.

## FAQ

**Can I use a framework?** Yes - you can keep it static or progressively enhance with a JS framework. Keep the accessible HTML as the foundation.

**Where should I put new pages?** Add additional `.html` files in the project root (e.g., `about.html`, `videos.html`) and link to them from the header.

---

### Developer notes

* HTML: validate with the W3C validator.
* CSS: run through a linter/formatter (e.g., Stylelint, Prettier) for consistency.
* Images: compress thumbnails; aim for efficient formats (WebP/AVIF) when possible.
