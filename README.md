# Nevin Kadlec Portfolio

A retro CRT-themed GitHub Pages portfolio for **Nevin Kadlec / NK-Forge**.

The site presents an updated professional portfolio inside a full-screen vintage CRT monitor interface. The goal is to keep the nostalgic green-terminal aesthetic while presenting current engineering work, public project highlights, private/in-progress case studies, and contact links in a clean, recruiter-friendly format.

## Live Site

https://nk-forge.github.io/Nevin-Kadlec/

## Purpose

This portfolio is designed to communicate:

* Full-stack software engineering experience
* Practical backend, desktop, automation, and product-building work
* Current NK-Forge project direction
* Public repositories worth reviewing
* Private/in-progress engineering case studies without exposing sensitive code
* A personal visual style that still feels professional

The CRT interface is intentional: the website should feel like the visitor is looking directly into a powered-on retro terminal.

## Current Portfolio Focus

The page highlights four public review paths:

* **Document Dispatch Service** — backend systems
* **Space Marine 2 Mod Loader / Launcher** — real-world desktop software
* **Full-Stack E-Commerce Application** — product delivery
* **ForgeBoard** — full-stack fundamentals

It also lists selected private/in-progress systems:

* **NK-Forge Orchestrator**
* **NK-Forge Classroom**
* **Ember**
* **Email List Cleaner**

## Project Structure

```txt
.
├── index.html
├── resources/
│   ├── css/
│   │   └── index.css
│   └── media/
│       ├── CRTface.png
│       ├── profile_pic.jpg
│       ├── CRT_monitor.png
│       ├── dark_background_1080.jpg
│       └── pixel_crt.png
├── favicon.ico
├── favicon-16x16.png
├── favicon-32x32.png
├── apple-touch-icon.png
├── android-chrome-192x192.png
├── android-chrome-512x512.png
├── site.webmanifest
└── README.md
```

## Key Files

### `index.html`

Contains the portfolio content and semantic layout:

* Header / identity section
* Profile image with Roscoe
* About section
* Quick review path
* Technical focus
* Engineering principles
* Public projects worth reviewing
* Private / in-progress projects
* Contact links

### `resources/css/index.css`

Controls the CRT effect, terminal styling, responsive behavior, and content placement inside the CRT screen.

Important responsibilities:

* Full-screen CRT background
* Green terminal color system
* Scrollable screen overlay
* CRT scanline effect
* Terminal window styling
* Responsive panel layout
* Screen-fit positioning variables

### `resources/media/CRTface.png`

The active full-screen CRT monitor background.

This image is intentionally used as the full browser background so the visitor’s viewport feels like the CRT monitor itself.

### `resources/media/profile_pic.jpg`

Circular profile image of Nevin with Roscoe.

## CRT Background Behavior

The CRT background is applied to the `body` element:

```css
body {
    background: #050705 url("../media/CRTface.png") no-repeat center center fixed;
    background-size: 100vw 100vh;
}
```

`CRTface.png` is intentionally stretched to the browser viewport so the monitor frame reaches every edge of the page.

This avoids black bars or unused space outside the monitor frame.

## CRT Screen Fit

The HTML content is positioned inside the green CRT screen using CSS variables:

```css
:root {
    --screen-left: 7.6vw;
    --screen-top: 10.4vh;
    --screen-width: 84.8vw;
    --screen-height: 65.2vh;
}
```

These values keep the portfolio content inside the green screen area instead of covering the beige bezel or inner CRT frame shadow.

If the background image changes, these four values are the first place to adjust.

## Design Notes

The visual direction is:

* Retro CRT monitor
* Green phosphor terminal display
* Monospace type
* Subtle scanlines
* Scrollable content inside the screen
* Beige monitor frame as the full-page background
* Professional portfolio content presented with a personal NK-Forge identity

The site intentionally avoids outdated wording like “new developer,” coursework framing, or service-shop sales language.

## Local Development

This is a static HTML/CSS site. No build step is required.

Open the project locally with a simple static server.

Example using VS Code Live Server:

```txt
Open index.html with Live Server
```

Example using Python:

```bash
python -m http.server 5500
```

Then visit:

```txt
http://127.0.0.1:5500/index.html
```

## Deployment

This project is intended for GitHub Pages.

Typical deployment flow:

```bash
git add .
git commit -m "feat: refresh portfolio with CRT terminal layout"
git push
```

GitHub Pages serves the site from the configured branch and folder.

## Maintenance Notes

When updating the site:

1. Update portfolio content in `index.html`.
2. Update visual/layout behavior in `resources/css/index.css`.
3. Keep `CRTface.png` as the active CRT background unless replacing the whole visual frame.
4. Re-check the CSS screen-fit variables after changing the background image.
5. Confirm the live site still keeps all content inside the green CRT screen area.

## Credits

Built and maintained by **Nevin Kadlec** under the **NK-Forge** umbrella.

Portfolio: [nevinkadlec.com](https://nevinkadlec.com)
GitHub: [github.com/NK-Forge](https://github.com/NK-Forge)
LinkedIn: [linkedin.com/in/nevin-kadlec](https://www.linkedin.com/in/nevin-kadlec/)
Email: [dev@nkforge.com](mailto:dev@nkforge.com)
