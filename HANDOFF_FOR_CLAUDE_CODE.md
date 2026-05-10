# Handoff Notes for Claude Code

## Task
Create a pull request to add the job search guide to the Write the Docs website repo.

## Target repo
https://github.com/writethedocs/www

## Steps

1. **Read the repo's CLAUDE.md first** — follow any project-specific instructions there.

2. **Fork and clone the WTD repo**, create a new branch:
   ```bash
   git checkout -b add-job-search-ai-era-guide
   ```

3. **Copy the RST file** into the hiring guide directory:
   ```
   docs/job-search-ai-era.rst  →  www/docs/hiring-guide/job-search-ai-era.rst
   ```

4. **Update `www/docs/hiring-guide/index.rst`** — add a new section linking to the guide.
   Insert after the existing sections, before the Consulting section:

   ```rst
   Job searching in the AI era
   ---------------------------

   .. toctree::
      :maxdepth: 2

      job-search-ai-era
   ```

5. **Check RST builds cleanly:**
   ```bash
   make html
   ```
   Fix any warnings before committing.

6. **Commit and push:**
   ```bash
   git add docs/hiring-guide/job-search-ai-era.rst docs/hiring-guide/index.rst
   git commit -m "Add job search guide for the AI era (community-sourced from #career-advice)"
   git push origin add-job-search-ai-era-guide
   ```

7. **Open a PR** against `writethedocs/www:main` with:
   - **Title:** Add: The Technical Writer's Edge — Job Search Guide for the AI Era
   - **Description:** (see suggested PR description below)

## Suggested PR description

```
## Summary

Adds a new community-sourced job search guide to the hiring guide section:
**The Technical Writer's Edge: A Job Search Guide for the AI Era**

## Background

This guide was distilled from discussions in the #career-advice channel of the
Write the Docs Slack. It covers practical, actionable advice for technical writers
navigating the job market in an AI-driven hiring landscape.

## What's included

- Building a job profile that works for humans and ATS algorithms
- Tailoring applications with AI tools
- Networking and referral strategies
- Interview preparation
- Demonstrating AI fluency
- Making domain expertise visible (new angle — highlights TW's rapid-learning superpower)
- Job title strategies for better search reach
- References and community credits

## Contributors

Community members from #career-advice: Alison Holloway, Ben Bristow, Bob Watson,
Daryl White, Dori Woodhouse, Heather Firth, JS, Juliette Kernion, LJ, Lois Patterson,
Mike Jang, Sreya Dutta, Zach Elwood, and others.
```
