# GitHub Repository Settings

This document lists the recommended manual GitHub settings for
`TrustCompo/open-hardware-cross-reference`.

## About Section

Open the GitHub repository page:

https://github.com/TrustCompo/open-hardware-cross-reference

On the repository home page, find the right sidebar section named **About**.
Click the small gear icon or **Edit repository details** button in that section.

Recommended values:

- **Description**: Open hardware cross-reference pages for lifecycle-affected components, replacement shortlists, and engineering validation boundaries.
- **Website**: https://trustcompo.github.io/open-hardware-cross-reference/
- **Topics**:
  - hardware
  - electronics
  - components
  - electronic-components
  - cross-reference
  - replacement-parts
  - bom-management
  - lifecycle-management
  - obsolete-parts
  - supply-chain

Enable these checkboxes if available:

- **Use your GitHub Pages website**
- **Releases**
- **Packages**: leave disabled unless the project starts publishing packages

## Pages

Go to **Settings -> Pages**.

Recommended values:

- **Source**: GitHub Actions
- Confirm the published URL is:
  https://trustcompo.github.io/open-hardware-cross-reference/

The repository already has `.github/workflows/deploy-pages.yml`, so the Pages
deployment should run from GitHub Actions after pushes to `master`.

## General Features

Go to **Settings -> General**.

Recommended values:

- **Issues**: enabled
- **Discussions**: optional, enable if you want broader engineering Q&A
- **Projects**: optional
- **Wiki**: disabled unless maintainers plan to keep it updated
- **Sponsorships**: disabled unless TrustCompo wants a sponsorship surface

## Pull Requests

Go to **Settings -> General -> Pull Requests**.

Recommended values:

- Enable **Allow squash merging**
- Disable merge methods the team does not use
- Enable **Automatically delete head branches**
- Enable **Always suggest updating pull request branches** if available

## Security

Go to **Settings -> Security** or the repository **Security** tab.

Recommended values:

- Enable **Private vulnerability reporting** if available
- Enable **Dependabot alerts**
- Enable **Secret scanning** if available for the organization plan
- Keep `SECURITY.md` updated with the preferred reporting channel

## Branch Protection

Go to **Settings -> Branches** and add a branch protection rule for `master`
when more contributors start submitting changes.

Suggested baseline:

- Require a pull request before merging
- Require approvals from at least one maintainer
- Require status checks to pass before merging
- Require conversation resolution before merging
- Do not allow force pushes

For a small maintainer-only project, this can wait until external contribution
volume increases.

## Google Search Console

Add the GitHub Pages property:

https://trustcompo.github.io/open-hardware-cross-reference/

Submit this sitemap:

https://trustcompo.github.io/open-hardware-cross-reference/sitemap.xml

After publishing, use URL Inspection for:

- https://trustcompo.github.io/open-hardware-cross-reference/
- a few important part pages
- one vendor page

If Google shows the GitHub `/security` page instead of the Pages site, request
indexing for the Pages homepage and make sure the repository About website field
points to the Pages URL.

## External Links

To help search engines identify the canonical public site, link to the GitHub
Pages homepage from:

- TrustCompo main website
- TrustCompo help center or engineering content
- relevant documentation pages
- public posts that introduce the open cross-reference project

Use the Pages URL as the primary link target:

https://trustcompo.github.io/open-hardware-cross-reference/
