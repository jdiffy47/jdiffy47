# github-profile

Source of `github.com/jdiffy47` (the profile README). **Public repo.**

- Never add client names, private repo names, credentials, or anything from private work beyond aggregate counts.
- Pushing to `main` publishes the profile. Commit freely; push only when Jake asks.
- Three workflows in `.github/workflows/` regenerate images daily (03:17-03:29 UTC) and on `workflow_dispatch`:
  - `snake.yml` → `output` branch (Platane/snk). README loads it via raw.githubusercontent.
  - `3d-contrib.yml` → commits `profile-3d-contrib/*.svg` to `main`.
  - `metrics.yml` → commits `github-metrics.svg` to `main`. Uses the `METRICS_TOKEN` repo secret (classic PAT, `repo` + `read:user`) so private repos count; falls back to `GITHUB_TOKEN` (public only).
- Because Actions commit to `main`, run `git pull --rebase` before pushing.
- Never hand-edit generated SVGs (`profile-3d-contrib/`, `github-metrics.svg`).
- One accent: `#c2410c` light / `#fb923c` dark. URL-based widgets: capsule-render, readme-typing-svg, skillicons.dev, streak-stats.
- No Claude attribution in commits.
