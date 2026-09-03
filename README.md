# asgaralisha.github.io

Personal portfolio site for **Asgar Ali Sha D** — GenAI Engineer and Full Stack Developer.

**Live:** https://asgard-15.github.io/asgaralisha.github.io/

A single-page static site covering an introduction, current and previous roles, a grouped skills
breakdown, twelve featured projects, and contact details. The downloadable CV is served from
`images/`.

## Stack

- HTML5 and hand-written CSS, all styles inline in `index.html`
- Bootstrap 4.0 (CDN) for the grid, navbar, and modal
- Font Awesome 6.4.2 (CDN) for icons
- jQuery, Popper, and Bootstrap JS (CDN)
- Vanilla JavaScript for smooth scrolling, scroll-spy navigation highlighting, back-to-top, and the
  footer copyright year
- Inline SVG favicon as a data URI — no binary asset required

There is no build step. GitHub Pages serves `main` directly.

## Structure

```
index.html    Whole site: head, inline CSS, all four sections, and page scripts
images/       Profile photo, technology logos, project screenshots, and the CV PDF
```

Sections are `#home`, `#about`, `#portfolio`, and `#contact`, matched by the navbar anchors and the
scroll-spy handler at the bottom of `index.html`.

## Running locally

```bash
python -m http.server 8000
```

Then open http://localhost:8000.

## Maintenance notes

- Projects without a screenshot use `.project-icon`, a gradient panel with a Font Awesome glyph, so
  new entries need no new image asset.
- Technologies without a logo in `images/` use `.skill-chip` text pills; those with a logo use
  `.skill-button` tiles.
- `.skill-card-auto` and `.experience-auto` override the fixed heights of the original cards so
  content is never clipped as it grows.
- Replace `images/Asgar_AI.pdf` whenever the CV changes; both download buttons point at it.

## Contact

- Email — asgar156d@gmail.com
- LinkedIn — https://www.linkedin.com/in/asgar-ali-sha-d-6925691ab/
- GitHub — https://github.com/AsgarD-15
