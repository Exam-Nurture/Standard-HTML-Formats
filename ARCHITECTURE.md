# Architecture: Standard HTML Formats

The ExamNurture Standard HTML Formats repo is built upon a standard structure that ensures consistent visual branding and print-ready quality.

## Template Design Features
1. **Responsive and Adaptive**: All templates are designed with standard screen resolutions in mind while prioritizing A4 print layouts.
2. **Standard CSS**: Using Vanilla CSS variables for theming (Colors: Primary, Secondary, Accent).
3. **Typography**: Utilizing standard professional fonts for clarity and visual hierarchy.

## Directory Structure
- `/JD`: This directory houses all Job Description html files. Each file contains internal CSS for standalone portability.
- `examnurture_logo.jpg`: The primary brand asset.

## Principles
- No external dependencies (like Bootstrap or Tailwind) unless specified.
- CSS must be clean and linted.
- Accessibility is a priority.
