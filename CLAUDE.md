# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repo Is

A community-sourced job search guide for technical writers, published as a Jekyll GitHub Pages site. The primary content lives in `docs/guide.md`. There is also an RST version (`docs/job-search-ai-era.rst`) intended for submission to the Write the Docs website repo.

## Publishing

The site uses Jekyll with the `minima` theme and is hosted on GitHub Pages. `_config.yml` sets the base URL — update `url` and `baseurl` when deploying under a real username.

## Key Files

- `docs/guide.md` — the canonical Markdown source for the guide (edit content here)
- `docs/job-search-ai-era.rst` — RST version for the Write the Docs website PR
- `docs/coach.html` — standalone Claude artifact for the interactive Job Search Coach
- `HANDOFF_FOR_CLAUDE_CODE.md` — step-by-step instructions for opening a PR against `writethedocs/www`

## Submitting to Write the Docs

See `HANDOFF_FOR_CLAUDE_CODE.md` for the full workflow. The short version:

1. Fork and clone `https://github.com/writethedocs/www`, create branch `add-job-search-ai-era-guide`
2. Copy `docs/job-search-ai-era.rst` → `www/docs/hiring-guide/job-search-ai-era.rst`
3. Add a `toctree` entry in `www/docs/hiring-guide/index.rst`
4. Run `make html` in the WTD repo and fix any RST warnings
5. Commit, push, and open a PR — title and description template are in `HANDOFF_FOR_CLAUDE_CODE.md`

## Content Guidelines (from CONTRIBUTING.md)

- Voice: second person ("you"), direct, practical
- Be specific and actionable — concrete steps over vague advice
- Keep the tone honest; this guide does not sugarcoat the market
- Avoid vendor promotion; tool mentions are fine when genuinely useful
- For substantial additions, open an issue before writing to align on scope
- All contributors who submit accepted changes are credited in the guide's Credits section
