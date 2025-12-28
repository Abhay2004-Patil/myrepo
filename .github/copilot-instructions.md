<!--
Guidance for AI coding agents (concise, actionable).
This file is generated from repository contents on 2025-12-28.
-->
# Copilot instructions — static single-file site

- **Project type:** Minimal static website. Single entry: [index.html](index.html#L1-L400).
- **Quick preview:** Open `index.html` in a browser or run a simple HTTP server:

  ```bash
  python -m http.server 8000
  # then visit http://localhost:8000
  ```

- **No build/test pipeline detected:** There are no package manifests, CI workflows, or test suites present. Do not add workflow assumptions unless you add supporting files (e.g., `package.json`, GitHub Actions). If you introduce a build step, include clear README instructions.

- **Primary editing rules:**
  - Keep changes minimal and focused to the single file `index.html` unless you intentionally add new assets (create `assets/`, `css/`, `js/` folders).
  - Preserve `<!DOCTYPE html>`, `lang`, `meta charset`, and `meta viewport` tags when modifying the file.
  - The visible version string is in the H1: `This is version V4`. If bumping the version, update that text and the PR description.

- **Adding new assets or features:**
  - Add a top-level README.md explaining any new build or preview commands.
  - If you add JavaScript, prefer `js/` and include script tags at the end of `<body>`.
  - If you add CSS, prefer `css/` and include a link in `<head>`.

- **Commit & PR guidance for AI agents:**
  - Keep commits atomic (e.g., "docs: update version to V5" or "feat: add css/ and basic styles").
  - In PR descriptions, include exact file links to changed lines (e.g., update [index.html](index.html#L1-L40)).

- **When to ask for clarification:**
  - If a task touches more than `index.html` (adding CI, packages, or server code), ask the repo owner for intended runtime, target browser support, and whether to add a README explaining build/test steps.

- **Reference file(s):**
  - [index.html](index.html#L1-L400) — single page content; change version text here.

If anything in this guidance is unclear or you want more detail (for example: recommended folder layout, CSS/JS patterns, or adding CI), tell me which area to expand.
