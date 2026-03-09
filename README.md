# 🖥️ Norton Commander Theme for Home Assistant

A dark, monochrome theme inspired by Norton Commander and DOS-era file managers. Part of the [btn.ooo](https://btn.ooo) aesthetic.

## Features

- **Dark DOS aesthetic** — deep black backgrounds, muted text, no rounded corners
- **Zero border radius** — sharp edges everywhere, like God intended
- **Monospace DOS font** — uses `Px437_IBM_VGA_8x16.woff2` (requires [card-mod](https://github.com/thomasloven/lovelace-card-mod))
- **Color palette** — carefully chosen accent colors for readability:
  - 🔵 `#5ac8fa` — Primary/active elements
  - 🟢 `#30d158` — On/success states
  - 🔴 `#ff453a` — Errors/alerts
  - 🟠 `#ff9f0a` — Headers/warnings
  - 🟣 `#bf5af2` — Accents
  - 🔷 `#64d2ff` — Secondary info

## Installation

### HACS (recommended)
1. Open HACS → Frontend → ⋮ → Custom repositories
2. Add: `https://github.com/YOUR_USERNAME/ha-theme-norton-commander`
3. Category: Theme
4. Install

### Manual
1. Copy `themes/norton-commander.yaml` to your HA `themes/` directory
2. Add to `configuration.yaml`:
   ```yaml
   frontend:
     themes: !include_dir_merge_named themes/
   ```
3. Restart Home Assistant

### DOS Font (optional, requires card-mod)
1. Install [card-mod](https://github.com/thomasloven/lovelace-card-mod) via HACS
2. Download `Px437_IBM_VGA_8x16.woff2` from [int10h.org](https://int10h.org/oldschool-pc-fonts/)
3. Place it in `/config/www/fonts/`
4. The theme will automatically load it

## Activate
Settings → Appearance → Theme → **Norton Commander**

## Screenshots

*Coming soon*

## Color Reference

| Variable | Color | Use |
|----------|-------|-----|
| `--nc-bg` | `#0a0a0c` | Main background |
| `--nc-bg-card` | `#12121a` | Card background |
| `--nc-border` | `#3a3a3c` | Borders |
| `--nc-text` | `#b0b0b0` | Primary text |
| `--nc-blue` | `#5ac8fa` | Primary accent |
| `--nc-green` | `#30d158` | Success/on |
| `--nc-red` | `#ff453a` | Error/off |
| `--nc-orange` | `#ff9f0a` | Headers/warning |
| `--nc-purple` | `#bf5af2` | Secondary accent |

## License

MIT
