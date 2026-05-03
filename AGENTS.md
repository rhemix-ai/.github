# AGENTS.md — rhemix-gh-org

Public GitHub organization profile repository for **rhemix**.

## Purpose

This repo exists only to provide the GitHub organization landing page.

When published as the org-level `.github` repository, GitHub renders:

- `profile/README.md` as the public organization profile
- `README.md` as the repository README for this `.github` repo itself

## Boundaries

- Keep this repo content-focused. It should not contain website build code, package code, sample data, generated artifacts, or configuration copied from sibling repos.
- Do not import, vendor, or reference files from `rhemix-engine`, `rhemix-cs`, `rhemix-profiles`, `rhemix-redteam`, or `rhemix-website`.
- It may describe the public rhemix ecosystem and link to public surfaces such as the website, public repositories, future docs, and contact email.
- No secrets, tokens, private deployment config, analytics IDs, `.env` files, credentials, or private service URLs belong here.
- Avoid operational/internal-only details. The audience is a public GitHub visitor deciding what the organization is about.

## Editing Guidance

- Primary content lives in `profile/README.md`.
- Keep tone aligned with the public website: concise, technical, and product-facing rather than marketing-heavy.
- Prefer stable descriptions over roadmap claims unless explicitly requested.
- If package names or licensing/status claims change, keep this README consistent with the website and public repository state.
- Do not add badges, screenshots, logos, or generated assets unless explicitly requested.

## Verification

There is no build step for this repo.

Before reporting completion, read the Markdown you changed and check that links, headings, and tables render cleanly in GitHub-flavored Markdown.
