# NIST CSF 2.0 – Mongolian Translation (Unofficial)

This repository hosts an unofficial Mongolian translation of the NIST Cybersecurity Framework 2.0 (CSF 2.0).

- Static HTML site: open `index.html` in your browser
- Bilingual (MN/EN) with a simple i18n system (`data-i18n` + JS object)
- Accessibility- and SEO-friendly (skip link, ARIA labels, JSON-LD FAQ)
- Downloads (PDF, glossary, poster) will be added later

## Quick start
- No build or dependencies required.
- Just double-click `index.html` or serve it statically with any web server.

## Project structure
- `index.html` – All markup, styles, and scripts live here (single-file site)
- `.github/ISSUE_TEMPLATE/` – Issue forms for bugs, features, and terminology updates

## Internationalization (i18n)
- All translatable text is driven by the `i18n` JS object and `data-i18n` attributes.
- Language is chosen via the select box (persisted in `localStorage`) and can be forced with `?lang=mn|en`.
- The FAQ JSON-LD block is generated dynamically to match the selected language.

## Contributing
We welcome:
- Bugs/content issues (typos, formatting, broken links)
- Feature ideas (layout, downloads, glossary)
- Terminology updates (glossary proposals)

Use GitHub Issues (preferred):
- Open the Issue chooser: https://github.com/happynitron/nist-csf-2.0-mn/issues/new/choose
- Or email: contact@cybersec.mn

## Licensing & attribution
- NIST source material is a work of the U.S. Government (public domain in nature).
- This translation is not endorsed by NIST and is provided for reference only.
- Planned license for the translation: Creative Commons Attribution 4.0 (CC BY 4.0).
  - CC BY 4.0 summary: https://creativecommons.org/licenses/by/4.0/

## Status
- Current: landing page and i18n scaffolding
- Coming soon: PDF translation, glossary export, poster

## Maintainers
- Feedback and contributions are reviewed via Issues. Thank you for helping improve the translation!
