# First Measure — Neutral Client Portfolio Starter

A reusable, dependency-free starter for producing professional client portfolios.

## Purpose

This repository is the approved First Measure baseline for client portfolio sites. It is intentionally neutral: it provides a Modern Studio visual system and adaptable portfolio structure without client content, First Measure sales messaging, pricing, or external service links.

Create a separate private repository for every client. Client repositories are independent productions; this repository remains the master baseline and must not contain client-specific or confidential material.

## Standards and instruction hierarchy

Every client production must follow the [First Measure Portfolio Standards](PORTFOLIO-STANDARDS.md). Apply repository guidance in this order:

1. `PORTFOLIO-STANDARDS.md` — product quality, content, evidence, experience, and approval requirements
2. `portfolio-starter-IMPLEMENTATION-RULES.md` — high-priority design-independence requirements
3. `AGENTS.md` — implementation workflow, technical constraints, and definition of done
4. `QA-REVIEW.md` — report-only pre-approval review protocol

The standards define outcomes without forcing every profession or client into the same structure.

## Structure

- `index.html` — one-page neutral portfolio structure with clearly marked placeholders
- `styles.css` — Modern Studio design tokens, layout, components, and responsive rules
- `script.js` — accessible mobile navigation behavior
- `assets/images/` — client images and visual assets
- `assets/icons/` — client icons and marks
- `assets/documents/` — client-facing documents, such as a résumé or CV PDF

The `.gitkeep` files only preserve the empty asset folders in Git. Remove them once real assets are added to a client repository.

## Included portfolio areas

The starter supports these adaptable sections:

1. Professional identity and headline
2. Introduction / about
3. Selected work, accomplishments, or case studies
4. Professional experience
5. Skills / expertise
6. Credentials, education, and evidence
7. Optional testimonial
8. Professional approach
9. Contact call to action and footer

Sections may be added, removed, reordered, or adapted when the approved portfolio direction supports it. Preserve the responsive behavior and visual hierarchy unless an intentional, tested client-specific change is required.

## Client production workflow

1. Start from this approved repository and read `PORTFOLIO-STANDARDS.md`, `portfolio-starter-IMPLEMENTATION-RULES.md`, and `AGENTS.md`.
2. Create a new, separate private repository for the client.
3. Establish and obtain approval for a direction based on the client's profession, audience, personality, approved content, and strongest evidence.
4. Adapt, add, remove, or reorder sections so the portfolio adds value beyond the résumé and supports progressive depth.
5. Replace every bracketed placeholder in `index.html`.
6. Update the HTML language, title, description, contact routes, and résumé/CV destination.
7. Add only client-approved public assets and clearly identify any illustrative or reconstructed demonstrations.
8. Run `npm run validate`, then complete the report-only review in `QA-REVIEW.md`.
9. Obtain client approval before deployment.
10. Deploy the client repository through the selected hosting workflow.

## Accessibility and responsive baseline

- Desktop navigation converts to a keyboard-operable mobile menu at 680px.
- The mobile menu updates its accessible name, moves focus to the first navigation link when opened, closes after navigation or outside interaction, and supports Escape.
- In-page sections account for the fixed header when scrolled to.
- Visible keyboard focus styles and reduced-motion support are included.
- Layouts collapse progressively at 1000px, 680px, and 400px.

## Development validation

Use Node.js 20 or newer. After installing dependencies, install Playwright's Chromium browser once and run the single quality gate:

```sh
npm install
npx playwright install chromium
npm run validate
```

`npm run validate` checks HTML structure, local links and assets, browser errors, automated accessibility, navigation behavior, smoke behavior, and horizontal overflow at widths 1440, 1024, 768, 430, 390, and 360 pixels.

The automated gate does not approve portfolio strategy, content, evidence, confidentiality, or visual design. Before client approval or deployment, evaluate the work against [`PORTFOLIO-STANDARDS.md`](PORTFOLIO-STANDARDS.md), use the report-only process in [`QA-REVIEW.md`](QA-REVIEW.md), and complete human review. Repository-wide implementation guidance is in [`AGENTS.md`](AGENTS.md).

## Rules

- Do not store client résumés, intake exports, private documents, or confidential materials in this master repository.
- Do not store client-specific content in this master repository.
- Do not publish this repository as a client site.
- Do not retain placeholder email addresses, links, metadata, or copy in a launched client site.
- Treat `main` as the approved starter baseline.
- Keep the template framework-free and dependency-free unless a deliberate production decision changes that standard.

## Design direction

The starter demonstrates a neutral Modern Studio baseline: editorial serif display typography, warm paper surfaces, deep navy contrast sections, terracotta accents, fine rules, structured cards, and a calm responsive layout. This is scaffolding, not the approved visual direction for every client; each production must establish its own approved, profession-appropriate identity.


## Design independence

Every client production must follow the high-priority [design-independence implementation rules](portfolio-starter-IMPLEMENTATION-RULES.md). Treat the starter as a technical foundation, not a visual template, and complete the required originality check before approval or deployment.  
