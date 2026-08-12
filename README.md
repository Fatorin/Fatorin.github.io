# fatorin.github.io

Personal portfolio — Rin Hsu, backend engineer in Taipei.

**Live:** https://fatorin.github.io/

A single self-contained `index.html`: no build step, no dependencies, no framework.
Everything is inline — styles, the language switcher, and the SVG diagrams.
Available in English, 正體中文 and 日本語 via the switcher in the nav.

## Files

| file | purpose |
| --- | --- |
| `index.html` | the portfolio — case studies |
| `resume.html` | the résumé; carries a print stylesheet, so Print → Save as PDF gives a clean two-page document |
| `404.html` | not-found page, same styling |
| `icon.png` | avatar, 800×800 — also the Open Graph preview image |
| `favicon-32.png`, `favicon-180.png` | tab icons, cropped to the face so it reads small |
| `apple-touch-icon.png` | home-screen icon, full illustration |
| `.nojekyll` | tells GitHub Pages to serve the files as-is, skipping Jekyll |
| `robots.txt`, `sitemap.xml` | crawler hints |

## Editing

Open `index.html` in a browser — that's the whole workflow.

Each language lives in a sibling `<span>` tagged `l-en` / `l-zh` / `l-ja`, and CSS
shows one set at a time based on `data-lang` on `<html>`. **When editing copy, change
all three** — a missing sibling leaves a gap for readers of that language.

Diagrams are hand-written inline SVG on an 860-wide `viewBox`. Keep text inside its
box and inside the `viewBox`, and check the page at 375px as well as desktop.
