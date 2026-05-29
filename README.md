# Standard ExamNurture Formats

Repository for standardized, print-ready document templates used across ExamNurture — Job Descriptions, Official Documents, and Branding Assets. Built with vanilla HTML/CSS (no framework dependencies) and optimised for Chromium-based PDF generation.

> Renamed from **Standard_HTML_Formats** → **Standard_ExamNurture_Formats** to reflect its broader role as ExamNurture's canonical document-format library (not HTML-only).

## Overview
This repository contains high-quality, print-ready HTML templates designed with modern web standards (Vanilla CSS) and responsive layout principles.

## Structure
- `/Job_Description`: Job Description templates (CTO, CEO, Operations, AI Engineer, etc.)
- `examnurture_logo.jpg`: Standard branding assets

## Available Roles
- **AI Engineer Intern** (v1.4.0)
- **Associate Content Manager** (v1.3.0)
- **Operations & Management Head** (v1.2.2)
- **CEO** (v1.0.0)
- **CTO** (v1.0.0)

## How to Use
1. Copy the desired `.html` template.
2. Update the specific details (Role, Responsibilities, Date).
3. Open in a browser to preview or generate a PDF.

## Standards
- **CSS**: Vanilla CSS for maximum flexibility.
- **Fonts**: Modern serif/sans-serif combinations for professional appearance.
- **Printing**: All new templates (v1.2.2+) MUST use the `<table><thead>/<tfoot>` structure for consistent multi-page header/footer repetition without content overlap. Finalized v1.3.0 Associate JD.
- **Compatibility**: Optimized for Chrome and Edge (Webkit-print-color-adjust).

## Printing Standards
- **Note**: As of v1.2.2, all templates must utilize the **Native Row Lock** (10mm slim <thead>/<tfoot>) architecture to ensure headers and footers physically reserve space across multiple pages. This eliminates content overlap issues in Chromium-based PDF generation. Avoid using `position: fixed` for branding zones as it does not reliably reserve content space.
- **Compatibility**: Optimized for Chrome and Edge (Webkit-print-color-adjust).
