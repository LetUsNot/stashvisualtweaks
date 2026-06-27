# Stash Visual Tweaks

A [Stash](https://github.com/stashapp/stash) UI plugin that polishes list-card presentation: gold star ratings, right-aligned count icons, optional rounded corners, and configurable max cards per row.

## Features

- **Gold star ratings** — Replaces the diagonal red/orange rating ribbon on grid cards with gold stars styled like the performer detail page rating control.
- **Right-aligned popover icons** — Scene count, o-count, tag count, and similar card buttons align to the right edge of the card.
- **Rounded cards** (optional) — Smooths grid card corners on scenes, performers, studios, groups, galleries, and other list cards.
- **Max row counts** (optional) — Limit how many scene, performer, or group cards appear on one row. Narrower layouts can still show fewer, wider cards. Each entity type can use the stock Stash layout or a custom cap (1–10).

## Requirements

- Stash with UI Plugin API support (v0.25+ recommended)
- Uses `PluginApi` patches and settings — no DOM scraping for layout caps

## Installation

1. Clone or download this repository.

2. Copy the plugin folder into your Stash plugins directory:

   | OS | Path |
   |---|---|
   | Windows | `%USERPROFILE%\.stash\plugins\stashvisualtweaks\` |
   | Linux / macOS | `~/.stash/plugins/stashvisualtweaks/` |

   The folder should contain:

   - `stashvisualtweaks.yml`
   - `stashvisualtweaks.js`
   - `stashvisualtweaks.css`

3. In Stash, go to **Settings → Plugins** and click **Reload Plugins**.

4. Enable **Stash Visual Tweaks** if it is not already enabled.

## Settings

Open **Settings → Plugins → Stash Visual Tweaks**:

- **Rounded cards** — Toggle rounded corners on grid cards.
- **Max Scene / Performer / Group Row Count** — Check *Use default* for stock Stash layout, or set a custom max (1–10) per entity type.

CSS tweaks (stars and right-aligned icons) apply whenever the plugin is enabled. Row caps and rounded cards follow these settings.

## License

MIT. See [LICENSE](LICENSE).
