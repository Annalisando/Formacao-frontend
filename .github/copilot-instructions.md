# Copilot Instructions

This repository is a static front-end training workspace. Most pages are standalone HTML/CSS/JavaScript examples rather than a single app with a build pipeline.

## Project structure
- `explora-mundo/` is the main demo site. It uses local assets under `assets/css/`, `assets/js/`, `assets/image/`, and a vendored FontAwesome copy in `assets/lib/fontawesome-free/`.
- `HTML/` contains individual HTML exercises. Files are mostly standalone and use relative asset paths.
- `HTML-CSS/` contains layout and CSS examples organized by topic, each with its own `index.html` and `css/style.css`.
- `JAVASCRIPT/` contains standalone demo pages with inline `<script>` examples, such as `10-funcao.html`.

## Key conventions
- No root-level build or package management is present. There is no `package.json`, `npm`, `yarn`, or task runner for the main repo.
- For changes, edit files directly and preview in the browser.
- Preserve Portuguese labels, comments, and text when updating examples.
- Keep relative asset paths intact. Example: `explora-mundo/index.html` references `assets/css/style.css` and `assets/lib/fontawesome-free/css/all.css`.
- Avoid renaming files with spaces or duplicate copy names without verifying usage.

## Workflows
- Use a local browser preview or a simple static server if needed. There is no special build command.
- Do not modify `explora-mundo/assets/lib/fontawesome-free/` unless updating icon assets or valid FontAwesome files.
- If adding interactivity to `explora-mundo/`, prefer external JS in `assets/js/script.js` rather than mixing new scripts in HTML, but note the current demo uses inline scripts in `JAVASCRIPT/` examples.

## What to avoid
- Do not invent hidden test or build steps; the repository is a collection of static educational examples.
- Do not convert the repo into a complex framework project. Keep changes aligned with static HTML/CSS/JS patterns.

## Notes for agents
- The main app-like folder is `explora-mundo/`; all other folders are exercise examples.
- `JAVASCRIPT/10-funcao.html` demonstrates inline prompt-based interaction and should be treated as a self-contained example.
- There is no central CSS file covering the whole repo; each example uses its own stylesheet.

If any part of the structure is unclear, ask for feedback on which folders should be considered main app code versus learning examples.