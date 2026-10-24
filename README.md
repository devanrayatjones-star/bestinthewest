# Best in the West Barbers: one-page site

`index.html` is the entire site: one file, no build step.

## To finish it
1. Open `index.html` and fill in the `window.SHOP` block near the top. Copy facts exactly as they appear on Instagram.
   `null` = not filled in yet (shows a yellow tag), `false` = the shop doesn't have this.
2. Save the three pinned photos as `photos/pinned-1.jpg`, `pinned-2.jpg`, `pinned-3.jpg` next to the page,
   or paste them in as `data:` URIs so the page stays a single file.
3. Open the page with `?check` on the end of the URL to see the checklist of anything missing or inconsistent.
4. Before going live: remove `<meta name="robots" content="noindex">`, add the canonical link and `og:image`,
   and add the town to the `<title>` and description.
5. Optional: set `formEndpoint` (e.g. a free Formspree form) so bookings arrive by email automatically.
   Without it, customers send their booking to the shop by Instagram DM, WhatsApp, text or email in one tap.
