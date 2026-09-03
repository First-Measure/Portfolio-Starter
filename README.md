# First Measure — Neutral Client Portfolio Starter

A private, reusable, dependency-free starter for producing professional client portfolios.

## Purpose

This repository is the approved First Measure baseline for client portfolio sites. It is intentionally neutral: it provides a Modern Studio visual system and adaptable portfolio structure without client content, First Measure sales messaging, pricing, or external service links.

Create a separate repository for every client. Client repositories are independent productions; this repository remains the private master baseline.

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

1. Start from this approved repository.
2. Create a new, separate private repository for the client.
3. Replace every bracketed placeholder in `index.html`.
4. Update the HTML language, title, description, contact routes, and résumé/CV destination.
5. Add only client-approved public assets to the client repository.
6. Review navigation, links, desktop layout, mobile layout, keyboard interaction, and content accuracy.
7. Obtain client approval before deployment.
8. Deploy the client repository through the selected hosting workflow.

## Accessibility and responsive baseline

- Desktop navigation converts to a keyboard-operable mobile menu at 680px.
- The mobile menu updates its accessible name, moves focus to the first navigation link when opened, closes after navigation or outside interaction, and supports Escape.
- In-page sections account for the fixed header when scrolled to.
- Visible keyboard focus styles and reduced-motion support are included.
- Layouts collapse progressively at 1000px, 680px, and 400px.

## Rules

- Do not store client résumés, intake exports, private documents, or confidential materials in this master repository.
- Do not store client-specific content in this master repository.
- Do not publish this repository as a client site.
- Do not retain placeholder email addresses, links, metadata, or copy in a launched client site.
- Treat `main` as the approved starter baseline.
- Keep the template framework-free and dependency-free unless a deliberate production decision changes that standard.

## Design direction

The starter preserves the approved Modern Studio direction: editorial serif display typography, warm paper surfaces, deep navy contrast sections, terracotta accents, fine rules, structured cards, and a calm, professional responsive layout.


## Design independence

Every client production must follow the high-priority [design-independence implementation rules](portfolio-starter-IMPLEMENTATION-RULES.md). Treat the starter as a technical foundation, not a visual template, and complete the required originality check before approval or deployment.  
