# Architecture: Standard HTML Formats

The ExamNurture Standard HTML Formats repo is built upon a standard structure that ensures consistent visual branding and print-ready quality.

## Template Design Features
1. **Responsive and Adaptive**: All templates are designed with standard screen resolutions in mind while prioritizing A4 print layouts.
2. **Standard CSS**: Using Vanilla CSS variables for theming (Colors: Primary, Secondary, Accent).
3. **Typography**: Utilizing standard professional fonts for clarity and visual hierarchy.

## Native Row Lock Printing Pattern (v1.2.2)
To solve the "Header Overlap" issue in Chromium-based printing (Chrome/Edge/Brave), we have adopted a high-precision table architecture:
1. **Physical Space Reservation**: The entire content is wrapped in a `<table class="print-wrapper-table">`.
2. **Repeating Headers (`<thead>`)**: The slim header bar is placed inside a `<thead>` with `display: table-header-group` and a fixed height of **10mm**. This forces the browser to reserve the top 10mm of every page before starting the text.
3. **Repeating Footers (`<tfoot>`)**: The blue branding bar is placed inside a `<tfoot>` with `display: table-footer-group` (10mm height), ensuring it sits below the text on every page without overlap. (v1.3.0: Associate Content Manager JD integrated).
4. **Body Content (`<tbody>`)**: The JD content grows within the `<tbody>`, allowing Chrome to manage page breaks naturally between the header and footer rows.
5. **Page 1 Branding**: The main Logo Header is positioned within the `tbody` and pulls into the header zone on the first page to cover the thin repeating bar, providing custom branding for the document start.

## Directory Structure
- `/JD`: This directory houses all Job Description html files. Each file contains internal CSS for standalone portability.
- `examnurture_logo.jpg`: The primary brand asset.

## Principles
- No external dependencies (like Bootstrap or Tailwind) unless specified.
- CSS must be clean and linted.
- Accessibility is a priority.
