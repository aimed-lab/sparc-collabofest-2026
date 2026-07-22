# SPARC Drug Discovery CollaboFest 2026 — Website

A single-page marketing site for the 2026 SPARC Drug Discovery CollaboFest Challenge.

## Files
- **`index.html`** — the complete site. Fully self-contained: all fonts (Fraunces, Hanken Grotesk, IBM Plex Mono) **and all logos** are embedded as base64, all CSS/JS is inline. **No external dependencies, no build step.** Works opened directly from disk or hosted anywhere.
- `fonts/` + `fonts.css` — source font files and the generated base64 stylesheet (reference only; already inlined).
- `logos/` — the SPARC, CCTS, and UAB Medicine logos extracted from the RFA PDF, plus a dark-theme SPARC variant (reference only; already inlined).

## How to deploy
Just upload `index.html` to any static host — it's the only file you need.
- **UAB web / any web server:** drop `index.html` in place.
- **Netlify / Vercel / GitHub Pages / S3:** upload as-is.
- **Preview locally:** double-click `index.html`, or run `python3 -m http.server` in this folder.

## What's on the page
Hero with live award summary + deadline countdown · the challenge (3-step process) · the three pillars (Targets / Chemicals / Patient Cohorts) · the $20,000 service menu (expandable) · eligibility (UAB + CCTS Partner Network) · the seven-part proposal guide · review process & criteria · 2026 timeline · team-readiness tiers · presenters & co-sponsors · FAQ · final call to action.

## Key facts baked in (per the revised RFA)
- **Submission deadline: September 30, 2026** (updated)
- **Winners announced: by October 20, 2026** (updated)
- Info session: July 30, 2026, 10:00 AM CT (Zoom)
- Three teams × up to $20,000 in in-kind SPARC services (not cash)
- Eligibility: ≥1 co-investigator from UAB or the UAB-led CCTS Partner Network
- Presented by SPARC; co-sponsored by DBIDS, the Marnix E. Heersink Institute for Biomedical Innovation, the UAB-led CCTS, and Southern Research
- Contact: Dr. Swathi Thaker — snthaker@uab.edu

## Live links wired in
- **Apply now** → `https://uab.co1.qualtrics.com/jfe/form/SV_cVnlmrmShnzME86` (Qualtrics registration)
- **Download the RFA** → `https://uab.box.com/s/8svh7hk0bj94a5l3f4qvbm9bw86ozes0` (Box)
- **Register for the info session** → `https://uab.zoom.us/meeting/register/vd8u1awQQ6Kqfa7d-oXoEg` (Zoom, Jul 30 · 10 AM CT)
- **SPARC** → `https://sites.uab.edu/sparc/` (header logo, hero, partners band, footer, contact)

## Logos
Real logos extracted from the RFA PDF are used throughout:
- **SPARC** in the header (with a dedicated light-text variant that auto-swaps in dark mode) and as the "Presented by" logo in the partners band — both linked to the SPARC site.
- **CCTS** and **UAB Medicine** logos on the co-sponsor logo wall.
- **DBIDS**, **Heersink Institute**, and **Southern Research** are shown as matching typographic name plates (no standalone logo files were embedded in the PDF). If you have official SVG/PNG assets for these three, drop them into the corresponding `.chip` in the partners band.

## Things you may want to edit
1. **Theme.** Colors are CSS custom properties at the top of the `<style>` block (`--pine`, `--copper`, `--bg`, etc.) for light and dark. Light is the default; adjust once, applies everywhere.
2. **Confirm the URLs** above stay current, and swap in official logo files for DBIDS / Heersink / Southern Research if you get them.

## Design notes
Deep pine green (a nod to UAB green) as the dominant brand color with a copper/gold spark accent on warm bone paper — deliberately steered away from the generic cream+terracotta template look. Expressive Fraunces serif display, IBM Plex Mono technical labels, Hanken Grotesk body. The signature element is a subtle live "knowledge-graph" node network behind the hero — the literal substance of network / systems pharmacology. Light + dark themes, responsive to mobile, keyboard-accessible, and `prefers-reduced-motion` aware.
