# TrustCompo Open Hardware Cross Reference

Public GitHub Pages site for lifecycle-aware hardware cross references, replacement candidates, and evidence-backed lookup pages.

## Purpose

This repository exists to publish useful public reference pages for hardware engineers who need to:

- check whether a part is obsolete, NRND, or otherwise lifecycle-affected
- review candidate replacements by bucket such as `P2P`, `Functional`, and `Similar`
- compare a small set of normalized parameters before moving into deeper design validation
- jump to the matching TrustCompo product page for full detail, pricing, and procurement context

The site is intended to be useful on its own. It is not a thin backlink directory.

## Site Structure

```text
site/
  index.html
  robots.txt
  sitemap.xml
  parts/
  vendors/
  data/
    index.json
    vendors/
    parts/
```

## Publishing Model

Pages are generated from structured lifecycle and cross-reference data after TrustCompo-side catalog updates succeed.

Each part page should include:

- lifecycle status
- evidence summary
- replacement candidates
- comparison notes
- verification reminders
- a canonical link back to the relevant TrustCompo product page

## Initial State

The first commit creates the GitHub Pages scaffold and placeholder indexes so the repository is ready for automated publishing.
