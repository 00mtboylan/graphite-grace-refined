# Graphite Grace: Refined — Project Guide

## Commands

- **Bump version**: Update `manifest.json` → `git add -A` → `git commit -m "message"` → `git push` → `git tag vX.Y.Z` → `git push origin vX.Y.Z`
- **Build AMO zip**: `cd <root> && zip -r /tmp/graphite-grace-refined-amo-vX.Y.Z.zip manifest.json images/`
- **Build full release zip**: `cd <root> && zip -r /tmp/graphite-grace-refined-vX.Y.Z.zip manifest.json images/ chrome/ screenshots/ readme.md LICENSE`
- **Create GitHub release**: Use API — delete old release if re-tagging, then POST new release + upload assets
- **Test locally**: Load `manifest.json` via `about:debugging#/runtime/this-firefox` → Reload after each edit

## Conventions

- All surface colors are neutral grays (R=G=B) — no blue cast
- Blue accent (`#69B2FF`) only for highlights, focus states, separators, tab lines — always use rgba with opacity (0.2–0.6)
- Theme is manifest-only — no chrome/ CSS bundled
- Version format: semver (patch bumps for tweaks, minor for features)
- Commit messages: concise, descriptive, no emoji
- Only one zip asset per GitHub release (`-amo-`); full source via GitHub's "Download ZIP"

## Files

- `manifest.json` — primary config (colors, images, version)
- `images/` — theme_frame.jpg, bg-overlay.png, icon.svg
- `screenshots/` — 4 PNGs for readme gallery
- `readme.md` — documentation
