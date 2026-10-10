# Lectern

Lectern is a Mac app that presents HTML slide decks with a presenter view like PowerPoint's: the slides fullscreen on the projector, and on your Mac the current slide, the next slide, your speaker notes, a clock and a ribbon of thumbnails. It works best with decks that follow the Presenter Deck spec, which comes with the app as a Claude skill, and also plays reveal.js and other HTML decks.

- **Download:** [Lectern.dmg](https://github.com/victor-shammas/lectern/releases/latest/download/Lectern.dmg) (free; macOS 14 or later, Apple silicon; notarized by Apple; updates itself)
- **Website:** https://victorshammas.com/lectern/
- **Support:** https://victorshammas.com/lectern/support.html or contact+lectern@victorshammas.com
- **Privacy policy:** https://victorshammas.com/lectern/privacy.html

The app's source code is private. This repository holds the releases and the website.

## The website

`docs/` is served by GitHub Pages at https://victorshammas.com/lectern/ (Settings › Pages › Deploy from a branch › `main`, folder `/docs`; no `CNAME` file, the custom domain comes from the `victor-shammas.github.io` user site). It is plain HTML and one stylesheet, with no build step, external fonts, scripts or trackers, in the same design as the Plainview, Gaugeline, Quoth and Staple sites. Its palette matches the app icon: espresso (`#46321F` → `#1C140E`) and amber (`#FFC56A` → `#EE8A25`).

| File | Published URL |
|---|---|
| `docs/index.html` | https://victorshammas.com/lectern/ |
| `docs/support.html` | https://victorshammas.com/lectern/support.html |
| `docs/privacy.html` | https://victorshammas.com/lectern/privacy.html |
| `docs/style.css`, `docs/icon.png` (256 px), `docs/favicon.png` (64 px), `docs/apple-touch-icon.png` (180 px, opaque) | assets |
| `docs/.nojekyll` | tells Pages to serve files as-is |

The download links point to `releases/latest/download/Lectern.dmg`, so every release must attach the DMG under exactly that name. The update feed (`docs/appcast.xml`) is served from the same folder. Keep these paths stable: the app and its update feed rely on them.

The app bar at the bottom of each page lists the other apps; keep it in step with the other sites and with https://victorshammas.com/apps/.
