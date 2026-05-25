# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Purpose

This is a TalTech (Tallinn University of Technology) HTML workshop template. Students fork this repo and build their own webpage during the workshop. All content and comments are written in Estonian.

## Running the project

There is no build step. Open `index.html` directly in a browser, or serve it with any static file server:

```bash
python3 -m http.server 8080
# or
npx serve .
```

## Architecture

This is a purely static site — no framework, no package manager, no bundler.

- `index.html` — the page structure. Uses a base64-encoded inline image for the hero photo and embeds a YouTube iframe. The "Lisainfo" section and the `<button>` click handler are intentionally left empty for students to complete.
- `style.css` — flexbox-based layout. Selectors use `body` for the page shell, `.container` for horizontal flex rows, `.card` for the image grid, and `#id` selectors for specific elements like `#photo` and `#textBox`.
- `script.js` — a stub with an empty `addEventListener("click", ...)` on `#button` for students to fill in.
- `given_template.jpg` — the target design mockup students are building toward.
- `images/` — icons used in the page (`img.png`, `question.png`, `world-wide-web.png`).

## Key conventions

- CSS uses `em` units throughout for sizing.
- The page layout is a vertical flex column (`body`) containing horizontal flex rows (`.container`).
- Workshop materials and slide deck are linked from the README.
