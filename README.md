# DLR Performance — Static Website

A modern, self-contained static website for **DLR Performance**, a specialist automotive
garage for performance and high-performance vehicles in Edenfield, Bury.

## Contents

```
dlr-performance/
├── index.html          Homepage
├── services.html       Services (diagnostics, timing belts, remapping, servicing, sensors)
├── about.html          About the garage
├── reviews.html        Customer reviews (4.9★ / 104 Google reviews)
├── contact.html        Contact details, opening hours, enquiry form, map
├── privacy.html        Privacy policy
├── terms.html          Terms of website use
├── robots.txt          Crawler directives
├── sitemap.xml         Sitemap
└── assets/
    ├── css/styles.css  All styles (yellow/black DLR brand palette)
    ├── js/main.js      Nav toggle, FAQ accordion, "today" hours highlight
    └── img/
        ├── dlr-logo.png        DLR Performance brand logo (from Facebook)
        └── dlr-premises.jpg    Real photo of the DLR premises (from Google Business Profile, plates excluded)
```

## Brand

The site uses DLR Performance's own brand identity: a yellow (`#FFE600`) and black
motorsport palette, with the business's real logo in the header and favicon.

## Deploy

This is a plain static site — no build step, no backend, no database.

1. Upload the entire `dlr-performance/` folder to any static host
   (Netlify, Vercel, GitHub Pages, Cloudflare Pages, standard web server, S3, etc.).
2. That's it. `index.html` is the entry point.

Everything works offline once deployed except:
- The embedded Google Map on `contact.html` (loads from Google).
- Google Fonts (loaded from Google Fonts CDN; falls back to system fonts if blocked).

**All imagery is self-hosted** in `assets/img/` — the logo, the real premises
photo, and the three atmospheric feature photographs. There are no external
image dependencies, so the site renders fully on any static host.

## Verified business information used

All substantive facts on this site were drawn from authoritative sources and
cross-checked. Nothing was fabricated:

- **Business:** DLR PERFORMANCE LTD (Company No. 11237435), VAT GB 349 302 991
- **Address:** Unit 1A, Bridge Mills, Rochdale Rd, Edenfield, Ramsbottom, Bury BL0 0RE
- **Phone:** 01706 558 485
- **Rating:** 4.9 / 5 from 104 Google reviews (Google Business Profile)
- **Hours:** Mon–Fri 08:30–17:00; Saturday by appointment; Sunday closed
- **Services:** Diagnostics & electrical fault-finding, timing/cam belt replacement,
  performance remapping, sensor/component replacement, specialist servicing & maintenance
- **Accessibility:** Wheelchair-accessible entrance and car park
- **Payments:** Credit cards, debit cards, NFC mobile payments

Sources: Google Business Profile / Google Places, Companies House, HMRC VAT registry,
aggregated Google reviews, and the business's public listings.

## Notes

- MOT testing is **not** claimed for DLR Performance, as it was not confirmed in the
  available sources.
- Customer review text on `reviews.html` is paraphrased to reflect recurring themes
  across the verified Google reviews (clearly labelled as such on the page); individual
  review text is not reproduced verbatim.
- The contact form builds a readable enquiry summary and routes to the verified phone
  number — no unverified email address is used.
