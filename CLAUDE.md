# CLAUDE.md

## Project Identity

- **Project:** kunjunnys.com
- **Owner:** Anil Kunjunny, Enterprise Transformation Architect
- **Purpose:** Personal website and testbed for a future dynamic personalisation project
- **Current state:** Static HTML/CSS/JS — V1 and V2
- **Target state:** V3 — Next.js dynamic site with a leading question that identifies visitor type and customises the experience accordingly
- **GitHub repo:** kunjunnys.com (already connected)

## Tech Stack

- **Current:** HTML, CSS, JavaScript — static
- **Target:** Next.js, React, Tailwind CSS, Vercel deployment pipeline
- **Node version:** 18 or higher
- **Package manager:** npm

## MCP Servers Connected

- **Filesystem MCP:** reads and writes local project files — use for all file operations
- **Memory MCP:** persistent key-value store across sessions — use to store project decisions and architecture choices
- **GitHub MCP:** connected to kunjunnys.com repo — use to read commits and propose PRs, never push without explicit confirmation
- **Browser MCP:** opens and navigates Chrome — use to test the live site and for research
- **Fetch MCP:** fetches URLs and reads web content — use for documentation and research tasks

## Task Protocol

- Before executing any task, state: (1) what you are about to do, (2) which files will be affected, (3) your estimated token usage.
- If estimated token usage exceeds 5,000 tokens, stop and ask for confirmation before proceeding.
- If a task affects more than 5 files, list all affected files and ask for confirmation before proceeding.
- Always show a diff or summary of changes before writing to any file.

## Git Conventions

- Never push to main without explicit confirmation from Anil.
- Commit message format: `[type]: short description`. Types: feat, fix, docs, style, refactor, chore.
- Always work on a feature branch. Branch naming: `feature/description` or `fix/description`.
- Never delete files without listing them first and getting confirmation.

## Deployment Pipeline

- **Hosting:** Cloudflare Pages (current, static). Vercel planned for V3.
- Never auto-deploy without explicit confirmation.
- Always test locally before any deployment step.

## V3 Vision

- V3 is a dynamic Next.js site that opens with a leading question identifying the visitor type.
- Visitor types to support: Hiring Manager, Recruiter, Consulting Partner, Potential Client, Collaborator.
- Each visitor type gets a customised experience: different content emphasis, different proof points, different call to action.
- This is a testbed for a future commercial personalisation product. Build it as if it will be productised.

## What Never to Do Without Asking

- Never expose API keys, environment variables, or secrets in any file.
- Never push to main branch without explicit confirmation.
- Never delete files without listing them and getting confirmation.
- Never install npm packages without stating what they do and why they are needed.
- Never make assumptions about the deployment pipeline — always ask.
