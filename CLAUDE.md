# github-profile

Source of `github.com/jdiffy47` (the profile README). **Public repo.**

- Never add client names, private repo names, credentials, or anything from private work beyond aggregate counts.
- Pushing to `main` publishes the profile. Commit freely; push only when Jake asks.
- One workflow, `.github/workflows/snake.yml`, regenerates the contribution snake daily (03:17 UTC) and on `workflow_dispatch`, writing to the `output` branch (Platane/snk). README loads it via raw.githubusercontent. Nothing commits to `main` automatically.
- Tried and dropped on 2026-09-30, don't re-add without asking: lowlighter/metrics (public-only without a PAT) and the 3D contribution graph (Jake didn't want it, even with the radar/counts stripped).
- Profile avatar source is `assets/avatar-cube.svg` (render: `qlmanage -t -s 1024 -o . avatar-cube.svg`). GitHub has no avatar API; Jake uploads the PNG at github.com/settings/profile.
- One accent: `#c2410c` light / `#fb923c` dark. URL-based widgets: capsule-render, readme-typing-svg, skillicons.dev, streak-stats.
- No Claude attribution in commits.
