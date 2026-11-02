# Cypress K–8 V10 QA release status

**NOT PRODUCTION-CERTIFIED.**

## Corrections in V10
- Added Spanish translations for important introductory and program descriptions, while retaining the original English for reversibility.
- Added language switching for image alt, title, placeholder, and ARIA label attributes when a translation is available.
- Updated the mobile-menu button label after switching languages.
- Replaced the misleading “Schedule a Tour” call-to-action with “Call to Arrange a Tour,” because its target is a telephone link, not a booking service.
- Preserved V9 contrast, animation and responsive styling changes.

## Checks performed
- JavaScript syntax check: passed (`node --check`).
- Browser tests attempted using installed Chromium and Playwright, both local file and localhost HTTP. Both were blocked by `net::ERR_BLOCKED_BY_ADMINISTRATOR`; no browser test passed. This is an environmental restriction, not evidence the site works.
- Official school reference confirms the address and phone in public M-DCPS materials (5400 SW 112 Ct, Miami, FL 33165; 305-271-1611). Historical publications cannot certify current staff, hours, or current programs.

## Remaining release blockers
1. Full English-to-Spanish translation of all content, including legal/policy material, metadata, accessibility labels, and human editorial review.
2. Successful real-browser test matrix (mobile/desktop, navigation, focus, forms, language persistence, animation, reduced motion, no JS exceptions).
3. WCAG 2.2 AA accessibility audit using a browser, including contrast measurements and keyboard screen-reader checks.
4. Live external-link verification, official M-DCPS dynamic navigation comparison, current personnel/document owner sign-off.
5. Deployment-environment performance, security, analytics/privacy and Lighthouse/Core Web Vitals testing.

Do not describe this package as production-certified or deploy it as an approved official school site without completing these gates.
