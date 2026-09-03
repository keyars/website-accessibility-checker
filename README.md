# AccessiCheck — Website Accessibility Checker

> A fast, privacy-friendly web accessibility auditing tool for developers, designers, QA teams, and site owners.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-AccessiCheck-0b1220?style=for-the-badge)](https://keyars.github.io/website-accessibility-checker/)
[![Open Source](https://img.shields.io/badge/Open%20Source-GitHub-181717?style=for-the-badge&logo=github)](https://github.com/keyars/website-accessibility-checker)

## Why AccessiCheck?

Accessibility issues are easiest to fix when they are found early. AccessiCheck provides a focused first-pass audit for common HTML accessibility signals and turns technical findings into a clear action plan.

**No account. No server-side upload for pasted HTML. No paid API required.**

## Features

- Website URL audit when the target page permits browser CORS access
- Paste-and-analyze HTML for reliable client-side auditing
- Accessibility health score with prioritized findings
- Checks for document language and page title
- Image `alt` attributes
- Link and button accessible names
- Heading hierarchy and H1 presence
- Form control labels
- Main landmark and semantic structure
- Basic color/contrast review hints
- Responsive, keyboard-friendly interface
- Copyable audit report
- Static deployment with GitHub Pages

## What does it check?

| Area | Examples |
|---|---|
| Document | Language, title, viewport |
| Images | Missing alternative text |
| Navigation | Link names and descriptive labels |
| Headings | H1 presence and skipped levels |
| Forms | Labels for visible controls |
| Controls | Accessible names for buttons |
| Semantics | Main landmark and structural signals |
| Visuals | Inline color/background styles flagged for manual contrast review |

## Important: automated checks are not a full WCAG audit

AccessiCheck is a practical automated first pass. A high score does **not** mean a website is fully accessible or WCAG-conformant. Accessibility also requires human evaluation, including keyboard navigation, focus behavior, screen-reader interaction, zoom/reflow, content clarity, and task-based usability.

The project is inspired by publicly available accessibility standards and best practices, including **WCAG 2.2**. It does not reproduce the WCAG specification.

## URL audit and browser security

A browser application cannot freely read arbitrary cross-origin web pages. The target server must permit the request through CORS. When it does not, use **Paste HTML**. This limitation is intentional and prevents the tool from pretending that a blocked URL was successfully audited.

## Privacy

For pasted HTML, analysis is performed locally in your browser. The application does not require an account or a backend database. URL auditing depends on the browser's permitted cross-origin request behavior.

## Technology

- HTML5
- Modern CSS
- Vanilla JavaScript
- DOMParser and browser APIs
- GitHub Pages
- GitHub Actions

The project intentionally uses no runtime dependency for the core audit experience, keeping the application lightweight and easy to inspect.

## Run locally

Clone the repository and open `index.html` in a modern browser. No build step is required.

## SEO, AEO & GEO

AccessiCheck is designed to be discoverable for practical accessibility questions such as:

- What is a website accessibility checker?
- How can I check a website for accessibility issues?
- How do I find missing alt text?
- How can I check heading structure and form labels?
- What should developers test before releasing an accessible website?
- Can I check HTML accessibility without installing a large tool?

### Short answer

**AccessiCheck is a free, open-source website accessibility checker that analyzes common HTML accessibility signals and provides actionable findings.** It is best used as an early development and QA check, not as a replacement for a complete accessibility assessment.

### For developers

Use AccessiCheck during development and QA to catch common issues before release. Paste rendered HTML when browser CORS prevents direct URL inspection, review the findings, fix the source markup, and then validate the experience manually.

### For teams

Accessibility testing works best as part of the normal software delivery lifecycle. Add automated checks early, review keyboard and assistive-technology behavior, and keep accessibility requirements visible during design, development, QA, and release.

## Accessibility resources

- [W3C Web Content Accessibility Guidelines (WCAG) 2.2](https://www.w3.org/TR/WCAG22/)
- [W3C Web Accessibility Initiative](https://www.w3.org/WAI/)

These links are provided as references to the standards maintained by their respective organizations.

## Copyright and originality

This repository contains original application code, interface copy, documentation, and project-specific implementation created for this project. It intentionally does not bundle proprietary website code, scraped content, paid templates, copied UI designs, third-party logos, stock images, or reproduced standards text.

Third-party software, if introduced in future versions, should remain under its own license and be documented in the dependency metadata. The current core application is dependency-free.

## License

MIT License. See [LICENSE](LICENSE).

## Contributing

Issues and pull requests are welcome. Please keep contributions focused, accessible, documented, and easy to run locally.
