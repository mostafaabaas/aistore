# AI Store — aistore.design (static landing site)

The e-commerce UGC desk of **influUGC**. Built Nov 6, 2026. **Files only — not deployed.**

## ⚠️ Content model + design direction (owner orders, Nov 5–6, 2026)

- **Content-first (owner update, Nov 6, 00:24):** network sites must NOT be pure
  company brochures. They lead with useful **content** — tips, guides and
  information that search engines and AI answers surface and that brings
  traffic — with influUGC's services and real work woven inside the content,
  and the central CTAs doing the conversion. This site applies the model: the
  homepage carries a full **"Guides for store owners"** section (3 substantive
  starter guides, below) ahead of the services list, and each guide closes with
  a soft woven-in influUGC line + the standard central CTA.
- **Identity (owner order, Nov 5, 23:57):** ALL network satellite sites use the
  main influUGC identity — black background `#000`, neon lime accent `#C8FF00`,
  dark panels, bold heavy typography, the www.influugc.com feel.
- Brand lockup: `AI Store.` wordmark with the subline "UGC for e-commerce by
  influUGC" (Arabic: «UGC للتجارة الإلكترونية من influUGC»).
- Only real company data: est. 2020, Arab League St Agouza (Giza 12651),
  Egypt + Saudi/Gulf, real client names (Riyadh Season, Saudi Tourism
  Authority, flynas, Saudia, realme, Domino's, TikTok Live, Zanussi).
  No prices, no invented figures or conversion statistics, no testimonials,
  no stock imagery (CSS/text only).

## Pages built (3 HTML pages, 2 languages)

| File | What |
|---|---|
| `index.html` | English-first landing (LTR): hero, client proof strip, **Guides for store owners** (3 starter guides, anchor-linked), 5 services (product-page UGC video ads, unboxing/review content, UGC ads & whitelisting, launch seeding, monthly packs), 4-step how-it-works (brief → creators produce → store runs ads), deliverables checklist, why influUGC (with the in-body editorial link to influugc.com), 6-question answer-first FAQ, contact/CTA band, network footer. |
| `ar.html` | Full Arabic mirror (RTL), same structure, guides and FAQ. |
| `404.html` | Branded not-found page (English). |

Plus: `styles.css`, `favicon.svg` (black + lime AI mark), `sitemap.xml`
(hreflang-annotated), `robots.txt`, `llms.txt`.

### The 3 starter guides (on-page sections, both languages)

1. `#guide-brief` — **How to brief a UGC creator for a product video**: the
   one-page brief (product/audience, one problem per video, three must-show
   moments, never-say list, format basics), what to send with it, deliverables
   agreed in writing, and why a word-for-word script kills the format.
2. `#guide-convert` — **What makes a product video convert on TikTok & Reels**:
   open on the product in use, one idea per video, proof over polish, say the
   offer out loud + captions, first frame as thumbnail, rotate angles and keep
   winners. No statistics — mechanics only, with an explicit no-invented-numbers
   line inside the guide itself.
3. `#guide-rights` — **Usage rights & whitelisting, explained for store
   owners**: file delivery ≠ owning every use; usage scope (pages / organic /
   paid, platforms, duration) in writing before production; whitelisting via
   TikTok Spark Ads authorisation and Meta partnership permissions, arranged
   per creator; raw footage in the original brief; a 5-point pre-payment
   checklist.

Each guide ends with a soft woven-in line (influUGC produces exactly this for
stores) + the standard book/WhatsApp CTAs with `utm_source=aistore`.

## SEO / GEO

- Canonical base `https://aistore.design/` (the real domain — unlike
  ugccompany, which temporarily uses its onrender.com base; if this site is
  first deployed to an `onrender.com` URL before the domain attaches, switch
  all canonical/OG/sitemap/robots/llms bases in one pass, same as the
  ugccompany rule in `../DEPLOY.md` §2).
- Title/meta target "UGC for e-commerce" + Egypt / Saudi Arabia in both
  languages; OpenGraph + Twitter cards; hreflang ar/en both ways.
- JSON-LD: `Organization` (with `parentOrganization: influUGC`, postal address,
  areaServed, the four real social profiles), `WebSite`, and `FAQPage` matching
  each page's visible FAQ word for word.

## CTAs (both carry the satellite UTM set)

- Booking → `https://www.influugc.com/book?utm_source=aistore&utm_medium=satellite&utm_campaign=network`
- WhatsApp (client line) → `https://wa.me/201029979797?utm_source=aistore&utm_medium=satellite&utm_campaign=network`
- Footer legal line: "Part of the influUGC network" linking to the hub.

## What remains (not done here) — read the domain items carefully

1. **⚠️ Marketplace listing on this domain (old account):** `aistore.design`
   sits in the OLD Namecheap account (lamarketing0) and currently carries a
   **$56 Namecheap Marketplace listing created Nov 6, 2026**. The classic
   marketplace listing **cannot be removed self-serve** from the panel — it
   must come off before/while the site goes live on the domain, either via a
   **Namecheap support-removal request** or by letting the listing lapse at
   its own expiry (**Nov 20, 2026**). Do not point traffic at a domain that is
   still listed for sale.
2. **⚠️ Renewal:** the domain **expires Dec 2026**. It was sale stock, but now
   that it is a network site it must be **renewed** — do not let it lapse.
   (Renewal is an owner-approved payment; surface it before the expiry, do not
   auto-pay.)
3. **Deploy** — static folder; any static host or a Render Static Site (free
   tier per the network rule). No server/admin in this build: the brief scoped
   a static landing.
4. **Domain attach** — point `aistore.design` DNS at the host (same checklist
   pattern as `../DEPLOY.md` §4: apex A + www CNAME from the host's screen; no
   MX changes — mail stays on influugc.com). Note the domain lives in the old
   Namecheap account, unlike the new-account keepers.
5. After go-live: dedicated Google Search Console property + submit
   `sitemap.xml`; verify both pages return 200, the guides render, and the FAQ
   matches the JSON-LD.

## Deploy status (Nov 6, 2026)

- **Repo**: https://github.com/mostafaabaas/aistore (private, branch `main`) — source pushed Nov 6, 2026.
- **Hosting**: PENDING-DASHBOARD — the Render Static Site service has **not** been created yet.
  Creating it requires the Render dashboard (no Render API key is available to the
  automation): Render Dashboard → New → Static Site → connect this repo — the repo's
  `render.yaml` blueprint pre-fills the service name (`aistore`) and publish path (`.`).
  Expected live URL once created: https://aistore.onrender.com
- **Domain attach**: separate later batch (see "What remains" item 4 above) — and
  the $56 marketplace listing (item 1) + Dec 2026 renewal (item 2) stay open
  until the support-removal/lapse and the owner's renewal decision.
