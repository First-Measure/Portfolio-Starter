# First Measure Portfolio — Comprehensive Site Review

Use this protocol for a pre-approval website review. It is a report-only process: do not modify files, write fixes, commit changes, open a pull request, or deploy anything during the review.

Treat approved content and design direction as intentional unless there is evidence of a defect or regression. Inspect the rendered site at widths 1440, 1024, 768, 430, 390, and 360 pixels; do not rely on source inspection alone.

## Review areas

Apply the product-quality requirements in `PORTFOLIO-STANDARDS.md` throughout this review.

### Recruiter scanability and progressive depth

Test the opening experience as a rapid scan. Within approximately 10 seconds, a reviewer should be able to identify who the professional is, what they do, what makes them relevant or distinctive, and which evidence is most worth exploring.

Then test a focused review of approximately two minutes. The strongest work should be meaningfully evaluable without requiring the viewer to read every paragraph or traverse unnecessary sections. Confirm that deeper material remains available through appropriate progressive disclosure rather than becoming unavoidable.

### Value beyond the résumé and profession fit

Confirm that the portfolio adds professional narrative, context, work evidence, process explanation, demonstrations, or other useful depth beyond reproducing résumé content. Evaluate whether its information design, visual language, section emphasis, and evidence presentation reinforce the individual's actual profession, audience, personality, and approved direction.

Do not require every possible section. Flag sections that exist only because they are present in the starter and do not contribute to the professional story.

### Capability demonstration, case studies, and illustrative material

Prefer tangible demonstrations of supported capability over unsupported or repetitive capability lists. Evaluate case studies against the evidence available for context, problem or opportunity, individual role, constraints, approach, important decisions, work performed, deliverables, outcome or impact, and lessons. Missing categories are acceptable when the evidence does not exist.

Confirm that conceptual interfaces, sample workflows, diagrams, reconstructions, and other illustrative materials are clearly identified and cannot reasonably be mistaken for completed client work, measured outcomes, or professional history. Treat ambiguous labeling as a content-evidence issue.


### Responsive layout

Check horizontal overflow, clipping, overlap, unintended wrapping, restrictive heights, grid and flex behavior, incomplete rows, gutters, shared alignment, whitespace, natural panel expansion, section transitions, fixed-header anchors, navigation, mobile-menu behavior, long content, media and code overflow, footer links, and touch targets. Distinguish natural content-driven height differences from defects.

### Visual cohesion

Evaluate the whole composition: hierarchy, typography, spacing rhythm, pacing, alignment, density, repeated patterns, container overuse, surface transitions, accent frequency, relative section importance, and whether the form used to present evidence serves that evidence. Classify technically valid but questionable choices as **Design Judgment**, not defects.

### Design independence

Determine whether the portfolio depends too heavily on First Measure business-site patterns, Portfolio-Starter patterns, another First Measure portfolio, or generic professional-portfolio conventions. Evaluate composition, section grammar, hierarchy, typography treatment, evidence presentation, grid behavior, and interaction patterns—not color difference alone.

Apply the originality check from `portfolio-starter-IMPLEMENTATION-RULES.md`: if colors, candidate name, and copy were removed, would the structure and composition remain distinctive to this portfolio?

### Content and evidence

Do not rewrite approved content. Review whether the strongest evidence has appropriate prominence; evidence is shown where useful; project narratives are clear; metric qualifiers remain visible; individual and team contributions are distinguishable; samples are identified; limitations retain context; and interview-useful evidence is easy to find.

Do not invent missing evidence. Classify an apparently absent approved element as **Possible Regression — Human Context Required** or **Content/Asset Gap**.

### Accessibility and interaction

Check semantic structure, heading hierarchy, keyboard navigation, visible focus, navigation labels and states, appropriate ARIA, meaningful alternative text, contrast, reduced motion, Escape behavior, link/button semantics, touch targets, focus order, zoom behavior, and screen-reader clarity.

### Technical health

Confirm the automated results and inspect for HTML/CSS/JavaScript errors, console warnings, broken links or anchors, missing assets, bad paths, failed document downloads, conflicting rules, excessive overrides, fragile positioning, dead rules, and implementation choices likely to cause responsive regressions. Do not recommend refactoring solely for stylistic preference.

### Regression review

Look for intended content or behavior that may have been removed, overridden, hidden, or altered. Compilation and rendering alone do not prove intent. When evidence is inconclusive, report **Possible Regression — Human Context Required** and do not redesign around the uncertainty.

## Finding format

For every substantiated finding, provide:

- **Severity:** Critical / High / Medium / Low
- **Classification:** Technical Defect / Responsive Defect / Accessibility / Portfolio Strategy / Content-Evidence / Possible Regression / Design Judgment
- **Location:** Page, section, component, selector, file, or code location
- **Viewport:** Affected viewport(s), when applicable
- **Observed:** What actually happens
- **Cause:** Likely implementation cause
- **Recommended direction:** What should be corrected and why

Do not manufacture findings. State when an area was tested and no issue was substantiated.

## Final quality threshold

Before assigning a final status, answer:

- Does the portfolio clearly communicate who this person is professionally?
- Does it demonstrate rather than merely list capability where practical?
- Does it feel individually designed and appropriate to the profession?
- Does it remain faithful to approved evidence and clearly identify illustrative material?
- Does it provide meaningful value beyond the résumé?
- Does it work intentionally on desktop, tablet, and mobile?
- Does it look and behave like a finished professional product?
- Would the individual be comfortable sending it directly to the intended recruiter, hiring manager, professional contact, or prospective client?

Any “no” answer must appear in the report as a substantiated finding or an explicit human decision still required.

## Final report structure

A. Technical defects requiring correction
B. Responsive/mobile issues
C. Accessibility issues
D. Portfolio strategy, scanability, or progressive-depth issues
E. Content/evidence gaps, illustrative-content ambiguity, or possible regressions
F. Design/visual judgments requiring human decision
G. Items tested with no substantiated issue

Finish with one status:

- Ready for human review
- Ready after technical corrections
- Significant correction required

Then identify the three to five highest-priority findings, if any. Stop after the report.
