# Portfolio Pages PRD Review

Date: 2026-06-22
Branch: `feature/portfolio-pages`
Commit: `977dac4`
Repo: `Kev-Hamm/kevcreates-portfolio`

## Objective

Move the misplaced portfolio design branch into the actual portfolio repo, then decide how to merge the current GitHub Pages implementation with the two feature-branch design artifacts.

## Current State

The live GitHub Pages site matches `index.html` on `origin/master`.

Current hosted page strengths:

- Clear Fiverr buyer positioning: AI manga and comic pages with human planning and QA proof.
- Strong first-scroll relevance: comic samples, QA-checked headline, package hints, Fiverr CTA.
- Good buyer objection handling: workflow, QA checks, packages, FAQ, commercial/right-scope language.
- Uses real portfolio images and lightbox behavior rather than abstract service copy.
- Good conversion path from proof to services to Fiverr.

Current hosted page weaknesses:

- Visual identity is polished but somewhat generic compared with the stronger Persona/manga direction.
- The hero can feel dense because proof, samples, and CTAs all compete early.
- The offer is manga/comic-specific, which is good for the current Fiverr launch, but it does not represent the broader AI tooling/dashboard skill set.

## Feature Branch Artifacts

The feature branch adds:

- `design/portfolio-a-chronicle-v1.html`
- `design/portfolio-fiverr-v1.html`

### Chronicle Concept

Strengths:

- Strongest visual personality: manga panel grid, speed lines, high-energy system-builder framing.
- Better fit for Kev as an AI architect and world-builder identity.
- Strong section rhythm: hero, Living World panel, selected work, expertise, contact.

Weaknesses:

- Poor fit as the immediate Fiverr gig landing page because the offer is broad and not buyer-specific.
- Does not foreground the actual comic/manga deliverables or QA proof.
- Less direct conversion value for a Fiverr visitor trying to decide whether to buy a comic page package.

### Fiverr Services Concept

Strengths:

- Clear simple service structure and pricing card pattern.
- Easy to scan and less visually risky than Chronicle.
- Could provide useful patterns for future non-comic service pages.

Weaknesses:

- Too generic for the current portfolio.
- Says "web apps, AI tools, and dashboards" rather than manga/comic pages.
- Placeholder-like trust/results copy is weaker than the current page's actual samples.
- Generic Fiverr link should not replace current specific seller/profile CTAs.

## Recommended Direction

Do not replace the current hosted page with either branch artifact directly.

Use a merge strategy:

1. Keep the current `index.html` as the production baseline.
2. Borrow visual energy from Chronicle selectively.
3. Borrow only the clean service-card clarity from Fiverr Services if needed.
4. Keep the page focused on the current revenue target: Fiverr manga/comic page buyers.

## Product Requirements

### Primary User

A Fiverr buyer who wants an AI-assisted manga/comic page or short comic scene and needs confidence that Kev can deliver readable, consistent, quality-checked pages.

### Primary Goal

Convert a visitor into a Fiverr inquiry/order by showing:

- Real page samples.
- Clear package scope.
- A credible production workflow.
- QA/proof value.
- Safe commercial and style-boundary language.

### Non-Goals

- Do not turn the main page into a broad personal portfolio yet.
- Do not lead with dashboards, AI tools, or Living World unless a separate route/page is added.
- Do not replace concrete image proof with abstract panels or generic service copy.

## Proposed Implementation Plan

### Phase 1: Keep Production Stable

- Keep current `index.html` live.
- Leave `design/` artifacts as reference pages on the branch.
- Do not merge Chronicle or Fiverr Services into `index.html` wholesale.

### Phase 2: Visual Identity Upgrade

Apply Chronicle-inspired styling to the current page:

- Add subtle manga panel framing around hero samples and proof sections.
- Add restrained speed-line or screentone accents behind section headers.
- Use sharper section dividers inspired by Chronicle, but keep current content hierarchy.
- Preserve current responsive behavior and image-first proof.

Acceptance criteria:

- First viewport still shows comic/manga proof and Fiverr CTA.
- Mobile text and sample images do not overlap.
- Page remains clearly about manga/comic page production.

### Phase 3: Service Clarity Upgrade

Use the Fiverr Services concept only for package-card clarity:

- Improve Basic/Standard package cards with clearer scope, revision, deliverable, and buyer-fit labels.
- Avoid generic "web apps / dashboards" language on the main page.
- Keep current Fiverr-specific CTA URLs.

Acceptance criteria:

- Buyer can understand the difference between 1-page starter and 3-4 page scene in under 10 seconds.
- No placeholder pricing or fake trust language.

### Phase 4: Optional Separate Architect Page

If Kev wants the broader AI architect identity public, create a separate route/file:

- `architect.html` or `systems.html`
- Based on Chronicle.
- Linked softly from footer or nav as "Systems Work" rather than competing with the Fiverr page.

Acceptance criteria:

- Main page remains conversion-focused.
- Architect page can carry Living World/OpenClaw/world-builder proof without confusing Fiverr buyers.

## Merge Decision

Recommended merge outcome:

- Merge the branch as reference artifacts and PRD documentation.
- Open a follow-up implementation branch for the actual `index.html` upgrade.
- Do not deploy `design/portfolio-a-chronicle-v1.html` or `design/portfolio-fiverr-v1.html` as the homepage.

## Risks

- Over-styling could reduce buyer trust if it feels more like a game UI than a service portfolio.
- Broad AI architect positioning could dilute the Fiverr comic offer.
- Generic pricing cards could conflict with actual Fiverr package pricing if not kept in sync.

## Final Recommendation

Production should be "current page plus Chronicle flavor," not "Chronicle replacement."

The current site has the right offer, proof, and conversion path. Chronicle has the stronger visual signature. The best direction is to keep the current buyer-focused structure and selectively import Chronicle's manga-panel energy into the hero, proof, and section transitions.
