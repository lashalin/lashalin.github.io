# Lasha 拉姐说 · personal site

Live: https://lashalin.github.io

A single-page site with no build step. `index.html` holds all markup, styles and scripts; GitHub Pages serves the `main` branch as-is.

## Layout

| Path | What it is |
|---|---|
| `index.html` | The whole page: hero, about, work, projects & events, sports & travel board, beliefs, contact |
| `lasha.jpg` | Portrait in the About section |
| `og.jpg` | Link preview image (1200×630) for LinkedIn / X / WhatsApp |
| `img/` | Compressed photos: `p-*` projects, `e*` events, `s-*` sports, `t*` travel |
| `serve.js` | Local preview server: `node serve.js` → http://localhost:4173 |

## Editing notes

- Chinese and English copy sit side by side as `<span class="zh">` / `<span class="en">`; the 中 / EN toggle switches them.
- Travel photos and map stops live in the `places` and `shots` arrays in the script near the bottom of `index.html`. Add a stop by adding a place (name, lat, lon) and one or more shots that point to it.
- New photos: resize to about 1200px on the long side before adding to `img/`.
- External scripts and fonts: Google Fonts, and the world outline from `echarts@4.9.0/map/js/world.js` on jsDelivr.

## Publish

Commit and push to `main`. Pages rebuilds in a minute or two.
