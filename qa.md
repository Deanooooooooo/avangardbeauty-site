# AvangardBeauty QA

- Local site: `sites/avangardbeauty/index.html`
- Target live URL: `https://deanooooooooo.github.io/avangardbeauty-site/`
- Target repo: `https://github.com/Deanooooooooo/avangardbeauty-site`
- QA scripts: `node scripts/qa_avangardbeauty.js`, `node scripts/inspect_avangardbeauty_map.js`

## Gate 1 — source/fact audit
PASS with one blocker noted below.
- Name/category/address/phone: Google Sheet row + Google Maps profile.
- Booking/services/description/hours/payment: Studio24 `https://studio24.bg/12288?m`.
- Instagram: verified by direct profile text matching business, booking link, and Дружба 2 address.
- No official standalone website/domain found; Studio24 is a booking/profile page, not a standalone site.
- No invented prices, certifications, awards, guarantees, review counts, or fake claims in public copy.

## Gate 2 — visual-result image audit
PASS.
- Checked Google Maps photos, Studio24 gallery, Instagram direct handle, Facebook direct handles/search, and Brave searches.
- Site uses the best available Instagram hair/nail result images near the top and Studio24/Maps images for interior/location trust.

## Gate 3 — testimonial audit
[blocked: reviewer names/text unavailable]
- Google Maps public/limited view showed aggregate place information but did not expose named written reviews.
- Studio24 showed aggregate rating/category review signals but no named written review text.
- Instagram includes salon-written captions/social posts but not named third-party testimonial text.
- Public page intentionally contains no testimonial cards, no fake names, no paraphrased reviews, and no visible review counts.

## Gate 4 — copy audit
PASS.
- Bulgarian copy pass completed.
- No numbered service boxes, no source/audit mechanics copy, no TODO/Lorem, no review-count language.

## Gate 5 — link/schema/SEO-head audit
PASS.
- One H1, title/meta description/robots/canonical/OG/twitter tags present.
- HairSalon schema contains NAP, sameAs, hours, map and canonical URL. No `reviewCount`.
- Links checked: phone, Studio24, Instagram, Google Maps navigation, anchors.

## Gate 6 — image/layout audit
PASS.
- All local image paths load.
- Hero/interior/gallery images have deliberate placement.
- Result gallery preserves hair/nail result visibility; no visible letterboxing or repeated hero image.

## Gate 7 — map/local SEO audit
PASS.
- Bottom map/local SEO contact block is directly above footer.
- Exactly one visible Google Maps navigation CTA in contact block.
- Full-page screenshots can show offscreen iframe blank, but scrolled map clip renders visibly: `artifacts/avangardbeauty-map-clip.png`.

## Gate 8 — responsive visual QA
PASS with testimonial blocker above.
- Desktop/mobile screenshots generated: `artifacts/avangardbeauty-desktop-qa.png`, `artifacts/avangardbeauty-mobile-qa.png`.
- Sticky mobile header call button present.
- Footer icon/action system is consistent.

## Gate 9 — final live QA after deploy
PASS with testimonial blocker above.
- Live HTTP 200 confirmed.
- Live HTML contains AvangardBeauty, Studio24, HairSalon schema, canonical, OG image, phone CTA, and map/contact block.
- Live OG image returns HTTP 200.
- Live mobile map clip renders visibly: `artifacts/avangardbeauty-live-map-clip.png`.
