# Chennai Home Solar website

- `index.html` is the deployable site. It's a single file with no build step, so you can upload it to Netlify, Cloudflare Pages, GitHub Pages or any web host.
- `src/page.html` is the same page in preview (Artifact) format.

## Before going live
1. Fill in the `SITE` settings at the bottom of `index.html`: phone, WhatsApp number, email, address, and `formEndpoint`.
2. Replace every yellow dashed placeholder: years in business, number of homes, vendor registration status, brands, areas served, GSTIN, warranty terms, financing, and the photos and reviews.
3. Set `costPerKwLow` and `costPerKwHigh` to your real pricing. The defaults (₹55k–65k per kW) are a market estimate, not your prices.
4. Have a Tamil speaker check the Tamil tagline.
5. Remove the financing FAQ if you don't offer financing.

## Lead handling
With no endpoint and no WhatsApp number set, the form sends nothing; it only shows a preview message.
- Quickest option: set `whatsapp`. The form then opens a pre-filled WhatsApp chat, but the customer still has to press Send.
- Better option: point `formEndpoint` at a free form backend (Formspree or Web3Forms) or at a Google Apps Script that writes to a Sheet. Then every lead is captured.
