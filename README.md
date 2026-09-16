# Louis Jefferson — Portfolio

Personal portfolio for Louis Jefferson — videographer &amp; editor, Gold Coast, Australia.

Static site (plain HTML/CSS/JS, no build step). Hosted on GitHub Pages at
**[louisjefferson.com](https://louisjefferson.com)**.

## Design
Bone paper, big quiet type, edge-to-edge picture. Newsreader (display) + Schibsted Grotesk
(everything else), no accent colour — the photography carries all of it. ~150 words on the
whole page. Play affordance is a cursor-following disc on pointer devices, a small pill on touch.

## Structure
`index.html` is the whole site: hero → clients → work → stills → Ahipara → about → contact.

- `assets/thumbs/` — film stills / covers
- `assets/gallery/web/` — optimized stills for the mosaic (camera originals in `assets/gallery/` are gitignored)
- `assets/case/` — Ahipara screenshots
- `assets/logos/` — client marks, rendered as single-ink silhouettes via `filter: brightness(0)`
- `assets/og-image.jpg` — social share card

## Stubs waiting on assets
- `#shortform` — hidden vertical/reels section. Drop `reel-01..04.mp4` into `assets/shortform/`
  and remove the `hidden` attribute. Clips use `data-src`, so nothing is fetched while it's off.
- A 7th film (BVOD & DRTV) — see the comment at the end of the work section.
- Instagram / Vimeo — see the comment in the contact footer.

## Deploy
Commit and `git push origin main`; GitHub Pages rebuilds automatically.

## Local preview
```
python -m http.server 8777
```
