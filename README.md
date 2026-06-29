# Nevin Kadlec Portfolio

Retro CRT-themed GitHub Pages portfolio for Nevin Kadlec / NK-Forge.

## Files

- `resources/media/CRTface.png` is the full-screen CRT background.
- `resources/media/profile_pic.jpg` is the circular profile photo with Roscoe.
- Main content lives in `index.html`.
- CRT positioning and responsive styling live in `resources/css/index.css`.

## Background behavior

The uploaded `CRTface.png` is square, so the CSS intentionally stretches it with:

```css
background-size: 100vw 100vh;
```

That makes the CRT frame fill the entire browser canvas edge-to-edge instead of leaving black bars.


## CRT screen fit

The HTML overlay is intentionally inset from the screen edges:

```css
--screen-left: 7.6vw;
--screen-top: 10.4vh;
--screen-width: 84.8vw;
--screen-height: 65.2vh;
```

These values keep the content inside the green CRT glass instead of covering the beige bezel or the inner frame shadow.
