# HyperTrace

Real-time telemetry overlay app for **Le Mans Ultimate** (Windows).

Draggable, configurable overlays sit directly on top of the game — no
alt-tabbing, no browser window.

This repository hosts **releases only** — downloadable builds, not source
code.

---

## Overlays

| Overlay | Description |
|---|---|
| **Speed & Gear** | Speed, gear and an RPM shift-light bar |
| **Pedals** | Throttle / brake / clutch bars with a trace history |
| **Standings** | Multi-class live standings — gaps, lap times, pit/out badges, tyre compound, manufacturer logo |
| **Relative** | On-track proximity list of the drivers immediately around you, with live gaps |
| **Delta** | Last lap / best lap / live delta-to-best with a gain-loss bar |
| **Tyres** | Per-tyre carcass temperature (colour-coded to each tyre's own optimal window) and wear |
| **Damage** | Top-down car silhouette showing body, wheel, suspension and rear-wing damage at a glance |
| **Fuel Calculator** | Fuel level, per-lap usage, laps remaining, refuel needed and full tanks to the end |
| **VE Calculator** | Same as Fuel Calculator, for cars that run on Virtual Energy (Hypercar, GT3) instead of fuel |
| **Weather** | Air/track temperature, rain, track wetness, and the session forecast |

Overlays appear automatically when you're on track and hide when you're
not. Everything — position, size, opacity, visible columns/rows, colours —
is configurable per overlay, with a live preview right in the settings
dialog.

---

## Requirements

- **Le Mans Ultimate** (Windows)
- In-game: **Settings → Gameplay → Enable Plugins** must be **ON** — this is what publishes the shared memory the app reads. If you just enabled it, **restart the game**; it doesn't take effect on an already-running session.

---

## Download & run

1. Grab the latest release's zip from the [Releases page](../../releases) and extract it anywhere.
2. Run `HyperTrace.exe`. Self-contained — nothing else to install.
3. Launch (or already be in) an LMU session. Overlays appear automatically once the game is on track.

Settings, positions and the enabled/disabled state of each overlay are
saved to `%USERPROFILE%\.hypertrace\config_v2.json` and persist between
launches.

---

## Credits

See [`THIRD_PARTY_NOTICES.md`](THIRD_PARTY_NOTICES.md).
