# Cypress K-8 V9 — Release gate status

**Status: NOT production-certified.** This is a QA candidate, not an approved live deployment.

## Verified locally
- Eight HTML pages present.
- Static audit: zero missing relative link targets and zero broken fragment anchors.
- JavaScript parses with `node --check`.
- Contrast fix: activity chips use dark foreground on light backgrounds.
- Added responsive overflow protection and accessible mobile controls.
- English/Spanish toggle remains available on every HTML page, with persistence.

## Blocking release gates
1. Full bilingual translation and human review: the current dictionary only covers a subset of text nodes. All prose, alt text, metadata and dynamic UI must be covered.
2. Chromium visual and interaction tests: Chromium headless execution timed out in this environment. Test at 320, 375, 768, 1024 and 1440px, both languages, keyboard-only, and reduced motion.
3. Official M-DCPS header/menu parity: source uses Angular templates; full rendered menu and external targets have not been independently verified.
4. Live external links and school-specific content (staff, hours, uniform policy, documents) need school owner approval.
5. Automated accessibility audits (axe/WCAG AA), real browser performance (Lighthouse/Core Web Vitals), security and deployment smoke tests remain outstanding.

## Deployment recommendation
Do not publish as a production-certified site until each gate is signed off with dated test evidence.
