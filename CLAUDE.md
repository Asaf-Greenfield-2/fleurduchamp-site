# CLAUDE.md — Fleur du Champ placeholder site

## Goal
Build a single, polished, on-brand "coming soon" placeholder page for the domain
**fleurduchampdesign.com**, then help me deploy it and point my domain at it. This is
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
I registered **fleurduchampdesign.com** through **Northwest Registered Agent**. DNS
management is included in my Northwest account. Recommend and walk me through the fastest
path to get this static `index.html` live on that domain. Likely the simplest is a free
static host (Cloudflare Pages, Netlify, or Vercel) deployed via CLI, then pointing the
domain through Northwest's DNS.

Please:
1. Pick a deploy target and explain why (favor free, fast, static-friendly).
2. Give me the exact CLI commands to deploy `index.html`, and run them with me.
3. After deploy, tell me the exact DNS records or nameservers I need to enter in my
   Northwest domain dashboard (apex `fleurduchampdesign.com` **and** `www`), in plain steps.
4. Note that I, the owner, will enter those DNS values and any login credentials myself —
   do not ask for my passwords or account logins.
5. Remind me it can take a little while (often under an hour, sometimes longer) for DNS
   changes to propagate, and how to verify the site is live.
