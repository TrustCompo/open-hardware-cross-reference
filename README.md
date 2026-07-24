# TrustCompo Open Hardware Cross Reference

A public GitHub Pages project for hardware engineers and sourcing teams reviewing lifecycle-affected parts, shortlist replacements, and first-pass cross-reference boundaries.

Live site: https://trustcompo.github.io/open-hardware-cross-reference/

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
- `docs/GITHUB_REPOSITORY_SETTINGS.md` for recommended GitHub repository, Pages, security, and search settings

## Contributing corrections

Hardware cross-reference data needs careful evidence. If you find an incorrect candidate, missing alternative, stale lifecycle status, broken link, or unclear validation boundary, please open an issue with public supporting references.

Use the templates under `.github/ISSUE_TEMPLATE/` when possible. See `CONTRIBUTING.md` for the evidence expected on part-number, datasheet, package, pinout, parameter, lifecycle, and compliance corrections.

## Publishing principles

- Prefer real manufacturer part numbers over internal-only product codes in public page titles.
- Publish only pages that have enough public value to help an engineer start review work.
- Keep links to TrustCompo contextual and useful, such as product detail or datasheet follow-through.
- Make validation boundaries explicit so shortlist pages do not read like blanket equivalence promises.

## License and disclaimer

The repository is published under the MIT License. The reference content is provided as an engineering shortlist aid only. It is not a design approval, final equivalence claim, manufacturer guarantee, or legal warranty statement.

See `DISCLAIMER.md` for the validation boundary and `SECURITY.md` for sensitive reporting guidance.
