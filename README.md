# VibeBox

Vibe-generated HTML tools designed to improve everyday workflows and quality of life.

Every tool is a single self-contained static HTML file — no build step, no install, no server. Anything a tool needs beyond plain HTML/CSS/JS (frameworks, icon sets, fonts) is pulled from a CDN at runtime, so the whole site runs entirely in the browser and deploys as-is to GitHub Pages.

🔗 **Live site:** https://zero41120.github.io/VibeBox/

## Tools

| Tool | Description |
| --- | --- |
| [WCAG Color Contrast Checker](wcag_contrast_eyedropper_tool.html) | Pick colors from any image with an eyedropper and check WCAG 2.1 contrast compliance in real time. |
| [Region Average Color Picker](region_average_color_picker.html) | Pan & zoom any image with [OpenSeadragon](https://openseadragon.github.io/), draw a rectangle or freehand region, and get its average color. |
| [Palette Maker](palette_maker.html) | Build, randomize, and extract color palettes from images, then save, share via URL, and export a palette card PNG. |

Browse them all from the [index page](index.html), which lists every tool with a short description and a link to open it.

## Adding a new tool

1. Create a new self-contained `.html` file at the repo root (e.g. `my_new_tool.html`). Pull in any needed libraries via CDN `<script>`/`<link>` tags — don't add a build step or local dependencies.
2. Register it in the `tools` array in `index.html` so it shows up on the homepage.
3. Add a row to the table above in this README.

## Deployment

The site is static and deploys directly via [GitHub Pages](https://pages.github.com/) from this repository — no build pipeline required. `index.html` at the repo root is the entry point.

## License

[MIT](LICENSE)
