## What's changed

- **gpio2mqtt daemon bumped to 0.2.2**:
  - live interrupt-driven inputs and stale-proof input read ordering (#113) — inputs are no longer polled blindly;
  - the Wirenboard MQTT convention is now functional (#112);
  - config hardening: `timed_set_ms`, `publish_initial` and `tls` are validated honestly, payload precedence fixed (#115);
  - inversion-aware mock event injection for tests (#114).
- Includes rc.6/rc.7 polish: red `[ERROR]` log lines (ANSI), watchdog guidance in the docs.
