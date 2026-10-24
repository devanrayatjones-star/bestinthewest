# Best in the West Barbershop: one-page site

`index.html` is the entire site: one file, photos embedded, no build step.

## Editing
All business details live in the `window.SHOP` block near the top of `index.html`
(barbers and their price lists, hours, address, phone, rating, photos). The page is built
from that block, so it can't contradict itself. Facts come from the shop's Instagram
(@bestinthewestbarbers) and its booking page.

Open the page with `?check` on the end of the URL for the built-in report: inconsistencies,
anything missing, things to confirm with the shop, and go-live steps.

## Before going live
- Remove `<meta name="robots" content="noindex">`.
- Add `<link rel="canonical">` and `og:image` once there's a domain.
- Optional: set `formEndpoint` (e.g. a free Formspree form) so booking requests arrive by email.
  Without it, customers send their request to the shop by Instagram DM or text in one tap.
- Confirm the items listed under `confirm` in the SHOP block with the shop.

## Dark / light theme
The glass toggle (header on tablet/desktop, footer on phones) switches the whole page between
the original design and an all-dark version. It starts from the visitor's system setting and
remembers their choice. Theme colours are the `--t-*` variables at the top of the stylesheet.

## Floating navigation
After the hero scrolls away, a floating bar slides in at the bottom with a live WebGL
liquid orb (tap it to book) and Home / Prices / Book / Contact links that highlight the section
in view. three.js loads from jsDelivr only when the bar first appears; if it can't load, a
CSS orb is shown instead. The bar hides while someone is typing in a form.
