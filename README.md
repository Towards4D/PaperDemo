# Towards_4D_Demo — Project Page

Project page for **"Towards Physically Consistent 4D Scene Reconstruction for Driving Simulation"**.

Published at: <https://templlll.github.io/Towards_4D_Demo/> (once GitHub Pages is enabled).

## How to update the page

Everything is static — edit `index.html` and push to `main`; GitHub Pages rebuilds automatically.

| What | Where |
|------|-------|
| Page content (title, abstract, sections, videos) | `index.html` |
| Styles | `static/css/style.css` |
| Teaser / method figures | `static/images/` (currently placeholder SVGs) |
| Result videos | `static/videos/` (drop `.mp4` files here, then reference them in `index.html`) |

### Adding a video

1. Copy the mp4 into `static/videos/`, e.g. `static/videos/nvs_scene00.mp4`.
2. In `index.html`, replace a placeholder card with:

```html
<div class="video-card">
  <video controls muted loop playsinline>
    <source src="static/videos/nvs_scene00.mp4" type="video/mp4">
  </video>
  <p>Scene 00 — novel-view synthesis</p>
</div>
```

### Replacing placeholder figures

- Teaser: overwrite `static/images/teaser_placeholder.svg`, or add `teaser.png` and update the
  `src` in `index.html` (also rewrite the caption).
- Method figure: same, `static/images/method_placeholder.svg`.

### After the paper is accepted

- Re-enable the Paper / arXiv / Code buttons (remove the `disabled` class, set real `href`s).
- Replace "Anonymous Authors" with the real author list and affiliations.
- Update the BibTeX block.
