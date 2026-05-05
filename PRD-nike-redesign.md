# PRD — Iron Pump Nutrition × Nike Design System

**Date:** 2026-05-04  
**Project:** iron-pump-nutrition  
**Task:** Apply Nike design language to existing IPN website  
**Status:** Planning

---

## Goal

Redesign `index.html` using Nike's design system (monochrome UI, massive uppercase type, full-bleed photography) while keeping all existing content, products, and IPN brand color (#FFB800 gold accent).

---

## Why

IPN is a premium Indian sports nutrition brand. Nike's design language — stark monochrome, athletic energy, full-bleed imagery, bold display type — directly reinforces the "Unleash The Beast" positioning. Current site is good but can be elevated to premium athletic retail level.

---

## Design Principles (from Nike DESIGN.md)

| Principle | Application to IPN |
|-----------|-------------------|
| Monochrome UI | Pure black (#000) base, white text, zero grey mid-tones |
| Massive uppercase type | Hero headline ≥ 150px Bebas Neue, section titles full-bleed |
| Full-bleed photography | Hero video full viewport, product images edge-to-edge |
| Minimal UI chrome | Remove decorative borders, simplify nav, let content breathe |
| Athletic urgency | Tight letter-spacing, compressed layouts, bold CTAs |
| Color as signal | #FFB800 gold used only for CTAs and key highlights (not decoration) |

---

## Scope

### In Scope
- [ ] Hero section — full-bleed video, massive headline, Nike-style CTA placement
- [ ] Nav — minimal, near-invisible on scroll, bold uppercase links
- [ ] Marquee strip — keep but make bolder/faster
- [ ] Products section — full-bleed card imagery, monochrome hover states
- [ ] Why IPN carousel — simplify chip design, full-bleed card photos
- [ ] Typography scale — increase all display text, tighten letter-spacing
- [ ] Footer — minimal, stripped back

### Out of Scope
- No new pages
- No backend / cart functionality
- No new product content
- No new images (use existing assets)

---

## Content (unchanged)

- Hero: "Unleash The Beast" — keep
- Marquee: FSSAI Certified, Lab Tested, 24g Protein, etc — keep
- Products: 4 pre-workout + 4 whey protein — keep all prices
- Why IPN: 4 features — keep
- Footer: all links — keep

---

## Technical Constraints

- Single HTML file output (`index.html`)
- GSAP + ScrollTrigger — keep all animations
- Google Fonts: Bebas Neue + Oswald — keep
- Assets unchanged: `assets/logo/`, `assets/images/`, `assets/video/`
- No external CSS frameworks

---

## Success Criteria

- [ ] Looks unmistakably premium athletic retail (Nike energy)
- [ ] IPN gold (#FFB800) still present as brand accent
- [ ] All 8 product cards visible and functional
- [ ] Feature carousel still works
- [ ] Responsive on mobile (768px)
- [ ] GSAP animations intact
- [ ] No broken asset paths

---

## Execution Plan

1. Run `npx getdesign@latest add nike` → get `DESIGN.md`
2. Feed DESIGN.md + current `index.html` to ui-builder agent
3. Agent rewrites `index.html` applying Nike system
4. Review in browser, iterate if needed

---

## Reference

- Nike DESIGN.md: `./nike/DESIGN.md` (after getdesign runs)
- Current site: `./index.html`
- Brand color: `#FFB800`
- Logo: `assets/logo/ipn-logo.png`
