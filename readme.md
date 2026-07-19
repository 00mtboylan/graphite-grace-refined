# Graphite Grace: Refined

A modern, refined interpretation of the classic Graphite Grace Firefox theme — layered dark surfaces with subtle blue accents.

## Features

- **Layered graphite UI** — custom header image with repeating dot texture overlay, centered and tiled
- **Soft blue accent** (`#69B2FF`) — used for highlights, focus states, separators, and tab lines
- **Reduced eye strain** — carefully chosen neutral gray palette with no blue cast in backgrounds
- **Dark color scheme** — explicit `color_scheme: dark` for all chrome and content pages via manifest
- **39 themed color properties** — complete coverage of the Firefox theme API including `tab_line`, `tab_background_separator`, `bookmark_text`, `toolbar_vertical_separator`, `ntp_card_background`

## Installation

### Option 1: Install from Firefox Add-ons (recommended)

[![Mozilla Add-on](https://img.shields.io/amo/v/graphite-grace-refined?label=Firefox%20Add-on&logo=firefox)](https://addons.mozilla.org/en-US/firefox/addon/graphite-grace-refined/)

Install directly from [addons.mozilla.org](https://addons.mozilla.org/en-US/firefox/addon/graphite-grace-refined/) — signed and one-click.

### Option 2: Install from file (manual)

1. Download the latest `-amo.zip` from the [Releases page](https://github.com/00mtboylan/graphite-grace-refined/releases)
2. Open Firefox → `about:addons` → gear icon → **Install Add-on From File...**
3. Select the downloaded zip

### Option 3: Temporary install (for testing)

1. Open Firefox and go to `about:debugging#/runtime/this-firefox`
2. Click **Load Temporary Add-on...**
3. Select any file in the project directory (e.g. `manifest.json`)
4. Theme is applied immediately until Firefox closes

## Screenshots

| New Tab | Preferences |
|:-------:|:-----------:|
| ![New Tab](screenshots/screenshot-newtab.png) | ![Preferences](screenshots/screenshot-preferences.png) |

| Sidebar | Popups & Menus |
|:-------:|:--------------:|
| ![Sidebar](screenshots/screenshot-sidebar.png) | ![Popups](screenshots/screenshot-popups.png) |

## Theme Structure

```
Graphite-Grace-Refined/
├── manifest.json        # Theme manifest — installable add-on
├── images/
│   ├── theme_frame.jpg  # Header background image
│   ├── bg-overlay.png   # Subtle dot-grid overlay texture
│   └── icon.svg         # Theme icon for about:addons
├── screenshots/         # Add your screenshots here
└── readme.md
```

## Color Palette

All surface colors use neutral grays (R=G=B) with no blue cast. Blue is reserved for accent elements only.

| Role        | Surface          | Hex         |
|-------------|------------------|-------------|
| Frame       | Main chrome      | `#2F2F2F`   |
|             | Inactive window  | `#292929`   |
| Toolbar     | Navigation bar   | `#2F2F2F`   |
|             | Selected tab     | `#2F2F2F`   |
| Fields      | URL bar bg       | `#222222`   |
|             | URL bar border   | `#484848`   |
|             | Focus border     | `#69B2FF`   |
| Popups      | Panel bg         | `#262626`   |
|             | Panel border     | `#484848`   |
| Sidebar     | Panel bg         | `#2F2F2F`   |
|             | Border           | `#484848`   |
| NTP         | Page background  | `#2F2F2F`   |
|             | Card background  | `#3A3A3A`   |
| Accent      | Highlight        | `#69B2FF`   |
|             | Hover bg         | `rgba(105,178,255,.10)` |
| Text        | Primary          | `#EEEEEE`   |
|             | Muted            | `#B4B4B4`   |

## Requirements

- Firefox 115 or later

## License

MIT
