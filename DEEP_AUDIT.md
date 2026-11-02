# V6 Deep Audit

This pass re-audits the original Cypress K-8 navigation supplied from the live site and public M-DCPS/Cypress documents.

## Confirmed source facts incorporated
- Cypress K-8 Center, state school ID 1281, PK–8, 5400 SW 112th Ct, Miami, FL 33165, (305) 271-1611.
- School hours shown in the Cypress Title I parent deck: 8:00 a.m.–3:05 p.m.
- Mission, vision, and the 3 Rs from official SIP/handbook materials.
- Full original navigation hierarchy supplied from the live school site.
- Current program flyers supplied from the school site: Special Education, Gifted, Advanced Academics, Medical Academy.
- Uniform policy and visual guide.
- Title I PFEP, Annual Parent Meeting, SIP, Parent/Student Handbook.
- Published social handles from the 2024–25 handbook: Instagram CYPRESSK8_PTSA_, X @cypress_k8, Facebook cypressk8center.
- Faculty/staff names transcribed from the original Cypress Faculty and Staff graphic. The production site should still validate role/title/contact fields against the district's current HR roster.

## UX treatment
Original destinations are preserved but reorganized by user need. Content-heavy posters/PDFs are converted to readable HTML where appropriate while official source documents remain linked. External services remain external links. A complete `site-directory.html` makes migration coverage auditable.

## Dynamic-link caveat
The public M-DCPS Angular shell does not expose all child URLs to static indexing. For child destinations whose exact current URL cannot be reliably recovered, the redesign preserves the destination and routes through an official Cypress/M-DCPS hub rather than fabricating a URL.
