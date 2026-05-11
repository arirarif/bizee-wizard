# BizJump V3 Wizard — HTML Mockup

> Click-through prototype of the new wizard. Modeled exactly on Bizee's verified 13-step flow, populated with BizJump's pricing.

---

## How to open

1. Double-click **`index.html`** — it opens in your default browser.
2. No install, no setup, no internet required.
3. Works in Chrome, Edge, Firefox, Safari.

That's it. Single self-contained file.

---

## What's in the mockup

### Homepage hero (the first screen)
- "Start Your Business With Confidence" headline
- "Launch Your LLC in Days" inset card with Entity + State dropdowns and the live state filing fee
- "Start My Business" CTA → enters the wizard

### Wizard (13 steps)
1. **Package Selection** — 4-tier table (Basic $99 / Pro $195 / Premium $295 ⭐ / Enterprise $295+$29/mo) with "Recommended" ribbon on Premium
2. **Company Information** — LLC name, designator, business purpose with live char counter, NAICS industry dropdown
3. **State Filing Time** — Rush ($50, 3-business-day) vs Standard ($0, ~3 weeks) — with calendar-date estimates
4. **Company Address** — Virtual Address with "FIRST MONTH FREE" green badge + Contact Address form (collects Name, Email, Phone, address)
5. **Premium Service Bundle** — $99 upsell card for Basic/Pro buyers (auto-skipped for Premium/Enterprise)
6. **Members Information** — Number of members + per-member Individual/Company toggle, with "Use BizJump address" shortcut
7. **Registered Agent** — Use BizJump (free 1st year, manual renewal at $99/yr) or Own RA
8. **EIN / Tax ID** — Foreign-individual question, SSN/ITIN, IRS contact address
9. **Small Business Banking** — Partner referral card with feature bullets + customer testimonial
10. **Tax Strategy Consultation** — FREE lead-gen opt-in
11. **Business License Research** — $99 paid addon with dynamic "We've identified N licenses for your business in {state}" copy
12. **Order Summary Review** — Read-only with per-section Edit links
13. **Billing & Payment** — Credit card fields + billing address + Terms checkbox + Complete & Pay button (inside the sidebar)
14. **Confirmation** — Welcome screen with order number, business name, total

### Sidebar (right column from Step 2 onward)
- Updates live as user makes selections
- Shows entity, package, state fee, addons, recurring services
- Bizee's "investment ladder" pattern — empty orange squares fill to orange checkmarks as user progresses
- On Step 13 the sidebar gains the Terms checkbox + Complete & Pay button + trust badges

---

## How to test it

1. Open `index.html`
2. On the homepage, pick an entity (default: LLC) and a state (default: Florida — live fee shown)
3. Click "Start My Business"
4. Click "Get Started ★" on the Premium tier (or any tier)
5. Fill in the company name (anything), pick a designator, type a purpose, pick an industry
6. Continue clicking through all 13 steps
7. End at the confirmation screen

Try going **back** at any step using the "‹ Back" button. The state persists.

Try clicking **"Edit"** on the Step 12 review screen — it jumps you back to that step.

---

## What's NOT in this mockup (yet)

This is a click-through prototype, not a working wizard. The following are intentionally not implemented:

- Real payment processing (Stripe Elements is just a styled form)
- Real WordPress / WooCommerce backend
- Real state persistence across page reloads (in-memory only — refresh resets)
- Real email sending / SMS
- Real account creation
- Real form validation beyond minimal "is this filled" checks
- Mobile optimization (it's responsive, but tested on desktop primarily)

These all come in the WordPress plugin build (V3 implementation phase, ~110 hours per `10-build-estimate.md`).

---

## Design source

Every visual decision is documented in the research folder one level up:
- `../10-BIZEE-RESEARCH/12-screenshot-verified-flow.md` — what Bizee actually does, step by step
- `../10-BIZEE-RESEARCH/13-design-system-from-screenshots.md` — colors, typography, spacing tokens
- `../10-BIZEE-RESEARCH/07-bizjump-v3-wizard-spec.md` — full build spec

---

## Iterating on this mockup

If you want changes, just say what you want and we'll edit `index.html` directly. Re-open to test. Once you sign off on the design + flow, we'll build the WordPress plugin from this as the visual reference.
# bizee-wizard
