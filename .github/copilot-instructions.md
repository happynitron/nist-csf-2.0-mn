# Copilot Instructions for NIST CSF 2.0 Mongolian Translation Project

## Project Overview
- This is a static landing page for the Mongolian translation of the NIST Cybersecurity Framework 2.0 (CSF 2.0).
- The project is currently a single-file HTML site (`index.html`) with embedded CSS and JavaScript.
- The site is bilingual (Mongolian/English) and uses a custom i18n system via a JS object and `data-i18n` attributes.
- No build system, package manager, or external dependencies are present yet.

## Key Patterns & Conventions
- **Language Switching:**
  - All translatable text is referenced by `data-i18n` attributes and populated from the `i18n` JS object.
  - Language selection is handled by a `<select>` element (`#lang-select`) and persisted in `localStorage`.
  - The page auto-detects language from URL params, browser settings, or previous selection.
- **FAQ Schema:**
  - FAQ content is duplicated in both HTML and a `<script type="application/ld+json">` block for SEO.
  - The JSON-LD FAQ is dynamically updated based on the selected language.
- **Contribution & Licensing:**
  - The translation is unofficial and planned to be released under CC BY 4.0.
  - Contributions are currently accepted via email; GitHub issue tracking is planned but not yet active.
- **Download Links:**
  - PDF, glossary, and poster downloads are stubbed (disabled) and will be enabled in future updates.
- **Accessibility:**
  - Includes skip links, ARIA labels, and keyboard navigation support.

## Developer Workflows
- **No build/test commands required.**
- All changes are made directly to `index.html`.
- For new features (e.g., downloads, glossary), add new sections/cards in the main HTML file.
- For i18n updates, modify the `i18n` JS object and ensure all new UI elements use `data-i18n`.
- For FAQ or SEO changes, update both the HTML FAQ section and the JSON-LD block.

## Integration Points
- External links reference NIST and (future) GitHub repository for contributions.
- No backend, API, or dynamic server logic is present.

## Examples
- To add a new FAQ:
  1. Add a new `<details>` block in the FAQ section.
  2. Add the corresponding question/answer to the `i18n` object for both languages.
  3. Update the JSON-LD FAQ generator in JS to include the new entry.
- To enable downloads:
  1. Replace disabled buttons with `<a>` tags linking to the actual files.
  2. Update the i18n text and button states accordingly.

## File Reference
- Main file: `index.html` (contains all code, styles, and logic)
- Future assets (PDF, glossary, poster) will be added as separate files and linked from the main page.

---
_If any section is unclear or missing, please provide feedback to improve these instructions._
