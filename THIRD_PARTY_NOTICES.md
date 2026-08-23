# Third-party notices

HyperTrace's original Python implementation (retired to `legacy/hypertrace/`
— see its own git history on the `legacy-python` branch) adapted portions
of its telemetry calculation engine and its overlay visibility engine from
**TinyPedal** (https://github.com/s-victor/TinyPedal), licensed under the
**GNU General Public License v3.0** (full text:
https://www.gnu.org/licenses/gpl-3.0.html).

The current C++/C# app does not contain that adapted code. The
functionally equivalent logic — fuel/energy/battery consumption tracking,
reference-lap-time and session-finish-type derivation, shared-memory field
extraction, and the auto-hide visibility gate — was independently
reimplemented for the rewrite: same observable behavior, different
internal design (see `hypertrace/bridge/src/consumption_tracker.hpp`,
`hypertrace/bridge/src/bridge_core.cpp`, `hypertrace/bridge/src/lmu_bridge.cpp`,
and `hypertrace/overlay/src/SessionActivity.cs`). No GPLv3 obligation
applies to the binary this app distributes.

TinyPedal is credited here as a courtesy, for the historical record of
where the original Python prototype's approach came from — not because
the current app incorporates any of its code.

## License

This file exists to keep that historical acknowledgment in one place
instead of scattered through old commit messages and the changelog.
