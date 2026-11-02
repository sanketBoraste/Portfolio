# Sanket Sharma — Portfolio

A dark, developer-focused portfolio built with **HTML and CSS only** — no JavaScript, no build step, no frameworks. The visual language is inspired by [coderarmy.in](https://coderarmy.in/): near-black surfaces, purple and gold accents, Poppins typography, glowing cards, and a macOS-style **Live Coding** editor window.

## Live preview

Open `index.html` in a browser, or serve the folder locally:

```bash
# any static server works
npx serve .
# then visit http://localhost:3000
```

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | Single-page portfolio: hero, tech marquee, about, skills, projects, experience, process, testimonials, contact, footer |
| `styles.css` | All styles, tokens, animations and responsive rules |
| `resume.html` | Matching one-page résumé with a print stylesheet (Ctrl/Cmd + P → save as PDF) |

## Features

- **Live Coding hero** — a CSS-drawn editor with traffic lights, line numbers, syntax colours, a blinking caret, sequential line reveal and a "Live Coding" status badge.
- **Text left / editor right hero** at desktop, matching the reference layout; stacks gracefully on smaller screens.
- **CSS-only mobile navigation** using the checkbox pattern (keyboard focusable, animated burger, full-width menu).
- **Pure CSS visuals** — project thumbnails, dashboard mockup, covers and avatars are all built from gradients and elements. No image assets required.
- **Responsive** across desktop, tablet and mobile (breakpoints at 1120, 1024, 900, 860, 640 and 420px).
- **Accessible** — semantic landmarks, visible focus styles, labelled form fields, skip link, reduced-motion support. Lighthouse: **100 accessibility / 100 best practices / 100 SEO**.
- **Animated details** — marquee, skill meters, floating badge, hover lifts and glowing borders, all respecting `prefers-reduced-motion`.

## Sections on `index.html`

1. Sticky header with nav and "Let's talk" CTA
2. Hero — headline, socials, CTAs, stats and the live-coding editor
3. Technology marquee
4. About — profile card + intro, facts and availability
5. Skills — frontend, backend, tools & cloud with meters
6. Selected work — one featured case study + three project cards
7. Experience — timeline, numbers and education
8. Process — Discover → Design → Build → Ship
9. Testimonials
10. Contact — details, socials and a `mailto:` form
11. Footer with quick links and back-to-top

## Customising

Everything is plain HTML/CSS, so edits are straightforward:

1. **Name / role / copy** — search for `Sanket Sharma`, `sanket.dev` and `Full-Stack Developer` in `index.html`, `resume.html` and `README.md`.
2. **Email** — replace `hello@sanket.dev` (hero, contact, form `action` and résumé).
3. **Links** — replace the placeholder social URLs (`https://github.com/`, `https://linkedin.com/`, `https://x.com/`, `https://dribbble.com/`) and the eight project `href="#"` links with real case-study/GitHub URLs.
4. **Colours** — edit the tokens at the top of `styles.css` (`--purple`, `--gold`, `--bg`, `--text`, …).
5. **Fonts** — Poppins + JetBrains Mono are loaded from Google Fonts; swap the `<link>` tags and `--font` / `--mono` variables to change them.
6. **Résumé** — update `resume.html`; the print stylesheet turns it into a clean black-on-white A4 document.
7. **Favicon** — an inline SVG `{ }` mark is embedded in the `<head>`; replace the `data:image/svg+xml` value if you want a custom icon.

## Notes

- The contact form uses `mailto:` so it works without a backend. Point it at a form service (Formspree, Netlify Forms, etc.) if you want in-page delivery.
- The mobile nav closes with the burger; because there is no JavaScript, it stays open after following an in-page link.
- The active nav underline is set on "Home" statically; a real scroll-spy would require JavaScript.

## Tech

- HTML5
- CSS3 — custom properties, Grid, Flexbox, `clamp()`, keyframes, `@media`, `@media print`, `prefers-reduced-motion`
- Google Fonts — Poppins, JetBrains Mono

## Design reference

- Base background: `#0a0c10`
- Purple: `#6b30e3` · Light purple: `#a78bfa`
- Gold: `#f5c842`
- Card surface: `rgba(15, 18, 25, 0.85)` with `rgba(255, 255, 255, 0.08)` borders
- Radius: 18–22px · Typography: Poppins (UI) + JetBrains Mono (code)
