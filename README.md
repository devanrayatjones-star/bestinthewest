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
