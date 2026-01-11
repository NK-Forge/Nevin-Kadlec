# Nevin-Kadlec (CRT Portfolio Site)

This repository contains the source code for a retro CRT/terminal-style personal portfolio page.

GitHub Pages Deployment:
[NK-Forge.github.io](https://nk-forge.github.io/Nevin-Kadlec/)

(https://nk-forge.github.io/Nevin-Kadlec/)
---

## Overview

This is a static HTML/CSS site designed to resemble a CRT monitor interface. The layout places scrollable content inside a “screen” region and uses styling (scanlines, glow, terminal cursor) to create a retro terminal feel.

The page includes:
- Intro / About section
- Technical skills
- Professional strengths
- Services offered
- Portfolio note with external GitHub profile link
- Contact links (email, LinkedIn)
- Resume section with project summaries and certifications

---

## Tech Stack

- HTML5
- CSS3 (custom styling and responsive scaling)
- GitHub Pages (static hosting)

No framework or build tooling is required.

---


Notes:
- `index.html` loads the main stylesheet from `resources/css/index.css`.
- The CRT monitor background image is expected at `resources/media/CRT_monitor.png`.
- Favicons are referenced from the project root, and `site.webmanifest` should also live in the root.

---

## Local Development

Because this is a static site, you can open `index.html` directly in a browser.

For best results (especially for local asset paths), run a local server:

```bash
python -m http.server
```

Then open:

```arduino
http://localhost:8000
```

---

## Deployment

This project is deployed via GitHub Pages.

General steps:

1. Push changes to the `main` branch
2. Enable GitHub Pages in the repository settings:
   - Source: `main` branch
   - Folder: `/ (root)`
3. Confirm the live deployment from the link provided.

---

## License

Personal portfolio project.  
Reuse or redistribution should include attribution.

