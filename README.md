# TrustCompo Open Hardware Cross Reference

A public GitHub Pages project for hardware engineers and sourcing teams reviewing lifecycle-affected parts, shortlist replacements, and first-pass cross-reference boundaries.

## What this project is for

This repository publishes part-level reference pages that aim to be useful on their own before sending the reader to TrustCompo. Each published page should help a reviewer answer four practical questions:

- what the original part is
- why the part needs attention now
- which candidates belong in a first-pass shortlist
- which checks still need engineering validation before release

## What this project is not

This is not intended to be a thin backlink directory or an automatic equivalence claim engine. The pages here are shortlist and review aids, not design approval documents.

## Public site structure

- `site/parts/<part>/index.html` for part pages
- `site/vendors/<vendor>/index.html` for vendor browse pages
- `site/data/parts/<part>.json` for machine-readable exports
- `site/data/index.json` for the global part index
- `site/data/sync-progress.json` for sync state and repeatability

## Publishing principles

- Prefer real manufacturer part numbers over internal-only product codes in public page titles.
- Publish only pages that have enough public value to help an engineer start review work.
- Keep links to TrustCompo contextual and useful, such as product detail or datasheet follow-through.
- Make validation boundaries explicit so shortlist pages do not read like blanket equivalence promises.
