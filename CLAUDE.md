# CLAUDE.md — Fleur du Champ placeholder site

## Goal
Build a single, polished, on-brand "coming soon" placeholder page for the domain
**fleurduchamp.com**, then help me deploy it and point my domain at it. This is
temporary — the full site comes later — but it should already look high-end, not generic.

## What to build
- A **single self-contained `index.html`** file (inline CSS in a `<style>` tag, no build
  step, no framework). It must open and render correctly by double-clicking the file.
- Responsive and mobile-first. Must look good on phones and desktop.
- Fast-loading and accessible (semantic HTML, sufficient color contrast, alt text on any
  imagery, focus states on links).
- Web fonts are fine via Google Fonts `<link>`. No other external dependencies.
- Include `<title>`, meta description, and Open Graph / Twitter meta tags so the link
  previews nicely when shared. Add a simple favicon if easy.
- No tracking scripts, no cookie banner needed (static page, no data collection).

## Brand
- **Name:** Fleur du Champ  (French for "flower of the field")
- **Business:** Luxury interior design studio.
- **Differentiator:** All fabrics and materials are organically and consciously sourced;
  the studio believes in the importance of organic living. This is the core story —
  make it visible, not a footnote.
- **Tagline (use as the hero headline or sub-headline):**
  *Bespoke Interiors that Enhance your Wellbeing*

## Design direction
- Feel: organic luxury — calm, warm, refined, natural. Think soft and editorial, not loud.
- Palette: warm neutrals (cream, oat, stone) with a natural accent (sage/olive or a muted
  earthy clay). Avoid pure white and pure black; use warm off-white and soft charcoal.
- Type: an elegant serif for headings (e.g. Cormorant Garamond, Fraunces, or Playfair
  Display) paired with a clean, quiet sans-serif for body (e.g. Inter or Work Sans).
- Layout: generous whitespace, centered single-column hero, restrained.
- Motion: subtle only (a gentle fade-in is fine). Nothing flashy.
- It's fine to use a soft background texture or a single tasteful botanical/organic
  flourish, but keep it minimal. No stock-photo clutter.

## Content
Use the copy in `placeholder-content.md` (same folder). Keep the bracketed items as
visible placeholders OR, better, wire them up:
- Make the email a `mailto:` link.
- Make the phone a `tel:` link.
- Make the Instagram handle a real link if a handle is provided.
The human (site owner) will fill in real contact details before launch — flag clearly in a
code comment where those values live so they're easy to find and edit.

## Deliverable
- `index.html` in the project root, ready to upload/deploy as-is.

## Deployment + domain connection
The site is deployed as a static page on **GitHub Pages** from the repo
`Asaf-Greenfield-2/fleurduchamp-site` (branch `main`, folder `/`). The custom domain is
**fleurduchamp.com**, which is registered through **Squarespace** (formerly Google
Domains); DNS is managed in the Squarespace domain dashboard.

Operational notes:
1. The deploy target is GitHub Pages — free, fast, static-friendly, no build step.
2. Deploys happen by pushing to `main`. The `CNAME` file in the repo root pins the
   custom domain to `fleurduchamp.com`.
3. DNS for `fleurduchamp.com` is entered in the Squarespace dashboard:
   - Apex `@` → four A records to GitHub Pages: 185.199.108.153, 185.199.109.153,
     185.199.110.153, 185.199.111.153
   - `www` → CNAME to `asaf-greenfield-2.github.io`
4. The owner (Asaf Greenfield) enters all DNS values and account logins himself —
   do not ask for passwords or account credentials.
5. DNS changes typically propagate in under an hour but can take longer. Verify
   propagation with `dig +short fleurduchamp.com` and then load the domain.
6. Enable "Enforce HTTPS" in GitHub Pages settings only AFTER DNS is pointing at
   GitHub and the certificate has provisioned.
