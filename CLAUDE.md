# github-profile

Source of `github.com/jdiffy47` (the profile README). **Public repo.**

- Never add client names, private repo names, credentials, or anything from private work beyond aggregate counts.
- Pushing to `main` publishes the profile. Commit freely; push only when Jake asks.
- Two workflows in `.github/workflows/` regenerate images daily (03:17-03:23 UTC) and on `workflow_dispatch`:
  - `snake.yml` → `output` branch (Platane/snk). README loads it via raw.githubusercontent.
  - `3d-contrib.yml` → commits `profile-3d-contrib/*.svg` to `main`.
- Because Actions commit to `main`, run `git pull --rebase` before pushing.
- Never hand-edit generated SVGs (`profile-3d-contrib/`).
- lowlighter/metrics was tried and dropped (2026-09-30): without a PAT it only sees public repos, and Jake chose not to add one.
- Profile avatar source is `assets/avatar-cube.svg` (render: `qlmanage -t -s 1024 -o . avatar-cube.svg`). GitHub has no avatar API; Jake uploads the PNG at github.com/settings/profile.
- One accent: `#c2410c` light / `#fb923c` dark. URL-based widgets: capsule-render, readme-typing-svg, skillicons.dev, streak-stats.
- No Claude attribution in commits.
