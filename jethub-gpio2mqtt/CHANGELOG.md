## What's changed

- **gpio2mqtt daemon bumped to 0.2.1**:
  - epoch-tagged GPIO state events (#105) — cleaner state/change semantics across reconnects;
  - fix: cancellable, tracked timers for `TimedSetOutput` — no more leaked/stuck timed outputs (#103);
  - `serde_yaml` replaced with the maintained `serde_yaml_ng` fork (#104).
- Includes everything from 0.1.0-rc.3: the fixed legacy-addon startup guard (correct Supervisor endpoints, reason logged for every skip).
