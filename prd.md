# On-Page SEO Snapshot PRD

This document summarizes the key requirements for the MVP browser extension inspired by the "Detailed SEO Extension". The goal is to provide core on-page SEO information quickly and clearly within the browser.

## Goals
- Deliver a simple Chrome extension for essential on-page SEO checks.
- Offer a clean, fast UI showing the most critical page data.
- Provide a foundation for future features like Firefox support or advanced exports.

## Target Audience
- SEO professionals (beginner to intermediate).
- Digital marketers, website owners, content creators, and developers.

## Repository Structure
The project is organized so that source code and documentation remain easy to
locate. The key top-level folders include:

```
extension/      # Chrome extension source files
  manifest.json # Extension manifest
  popup/        # HTML, JS, and CSS for the popup UI
  icons/        # Extension icons

docs/           # Additional documentation
  prd.md        # This product requirements document

README.md       # Project overview and setup instructions
```

## Feature Set
1. **Overview Tab**
   - Title tag and length.
   - Meta description and length.
   - URL, canonical URL, meta robots info, word count, language, indexability status.
   - Quick links to `robots.txt` and common sitemap locations.
2. **Headings Tab**
   - List of all headings (H1-H6) in order with hierarchy.
3. **Links Tab**
   - Counts of internal/external links.
   - Detailed list with anchor text, type, nofollow status.
   - Basic CSV export.
4. **Images Tab**
   - Number of images and missing ALT text.
   - List with image URLs and ALT text.
   - Basic CSV export.
5. **Schema Tab**
   - Detection of Schema.org markup types.
   - Display raw JSON-LD or microdata snippets.
   - Show hreflang tags.
6. **Social Tab**
   - Detect Open Graph and Twitter Card tags.

## Non-Goals (for MVP)
- Support for browsers other than Chrome.
- User agent switching or advanced data export.
- Extensive link highlighting or external tool integrations.
- Saving reports or user accounts.

## Success Metrics
- Extension installs and active users.
- User ratings and feedback.
- Low bug reports and uninstall rate.

## Future Considerations
- Firefox support and new features based on user feedback.
- Advanced schema validation, link analysis, and comparison tools.
- User settings and customization options.
