# Iron Pump Nutrition

Single-page static site (index.html) for a supplement brand, styled with a
Nike-inspired design system.

- Path: D:\Vyzma\clients\iron-pump-nutrition
- Reference: @DESIGN.md — Nike-inspired monochrome design DNA (Futura display, Helvetica Now body, pill buttons, no shadows)
- Repo: git-tracked, in sync with origin/master as of 2026-09-23
- Local dev server: `http://localhost:3333/`
- Products: 4 Pre-Workouts (Hellfire Punch, Blue Rage, Inferno Punch, Blue Raspberry) + 4 Whey Proteins
- WhatsApp ordering number: +91 83175 64213 (used across all CTA buttons, modal, floating widget)

## What's Done (as of 2026-09-23)
- 12 high-res pre-workout images integrated across all 4 flavors, bottle shots normalized to identical 245.3px height on pure #FFFFFF canvas
- On-card pill thumbnail switcher (Front Bottle / Directions & Benefits / Nutrition Facts) per pre-workout product
- Full lightbox product modal: name, tag, rating, pricing, discount badges, flavor selector, gallery with thumbnail nav, keyboard controls (Esc/Left/Right), mobile swipe
- WhatsApp direct order wired to +918317564213 with per-product pre-filled messages, across CTAs/modal/floating widget
- Full-card click-to-modal on all 8 products, with WhatsApp CTA clicks isolated (don't trigger modal)
- Fixed modal non-opening bug: `#product-modal` was below script tags in DOM order; moved modal markup above scripts, made modal handler a standalone script with document-level event delegation

## What's Pending
- **Deploy to Vercel** — local changes are committed-but-not-pushed... actually not yet committed (see below). Waiting on Teja's go-ahead.
- Mobile device live verification: modal swipe gestures + WhatsApp pre-filled messages on a real phone browser
- Skill gap flagged 3x across projects (SYSTEM, Aman Coach, Iron Pump): proposed `vyzma-whatsapp` skill for phone normalization, wa.me encoding, button/card event isolation. Teja hasn't decided yet.

## Git State (2026-09-23)
- Branch up to date with origin/master
- Uncommitted: assets/images/product1-4.png (modified), index.html (modified)
- Untracked: 12 new flavor jpegs (blue-rage-1/2/3, blue-raspberry-1/2/3, hellfire-punch-1/2/3, inferno-punch-1/2/3)
- Nothing pushed yet — commit + push + Vercel deploy all still pending Teja's confirmation

## Vercel
- No canonical Vercel project mapping recorded in root CLAUDE.md for this client yet — confirm project name before first deploy.
