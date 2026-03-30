# Project Status: Standard HTML Formats

Current version: **v1.2.2** (Native Row Lock Update)

## Completed Templates
- [x] Associate Content Manager JD
- [x] CEO JD
- [x] CTO JD
- [x] Operational and Management Head JD (Zero-Overlap Standard Verified)

## Upcoming
- [ ] Employee Onboarding Letter
- [ ] Intern Offer Letter
- [ ] Internal Branding Guidelines

## Printing Standards
- **Note**: As of v1.2.2, all templates must utilize the **Native Row Lock** (10mm slim <thead>/<tfoot>) architecture to ensure headers and footers physically reserve space across multiple pages. This eliminates content overlap issues in Chromium-based PDF generation. Avoid using `position: fixed` for branding zones as it does not reliably reserve content space.

## Version History
- **v1.2.2**: Implemented the **Native Row Lock** system (10mm <thead>/<tfoot>) for absolute zero-overlap printing in Chrome. Added Market Standard Salary point.
- **v1.1.0**: Initial multi-page printing optimization for Operations JD. Standardized "Social Media Handler" terminology.
- **v1.0.0**: Initial push of standardized JDs for ExamNurture.
