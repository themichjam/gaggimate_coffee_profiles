# GaggiMate PRO JSON schema notes

This document explains common fields in a GaggiMate PRO profile JSON file in plain language.

## Top-level fields

### `label`
Human-readable profile name shown in profile lists.

### `type`
Profile type identifier (for example, a PRO-style shot profile).

### `description`
Short explanation of the profile intent (bean style, use case, or target cup result).

### `temperature`
Default or global temperature setting used by the profile, if present.

### `utility`
Metadata and utility settings used by profile tooling or UI helpers.

### `phases`
Ordered list of extraction phases. The machine executes these from first to last.

## Phase object fields

Each item in `phases` typically includes some or all of the fields below:

### `name`
Friendly phase name (for example, preinfusion, ramp, hold, finish).

### `phase`
Phase kind or mode identifier used by the controller.

### `valve`
Valve state or command used during the phase.

### `duration`
How long the phase runs, generally in seconds.

### `temperature`
Phase-specific brew temperature target.

### `transition`
How the controller moves into or out of this phase (for example immediate or ramped behavior).

### `pump`
Pump control settings for the phase.

### `targets`
Target values that define what the machine should chase in that phase (for example pressure and/or flow objectives, depending on profile format).

## Notes

- Field availability can vary by firmware/profile export version.
- Keep profile JSON files machine-readable and avoid manual formatting changes unless intended.
- Treat imported profile files as the source of truth when sharing or versioning.
