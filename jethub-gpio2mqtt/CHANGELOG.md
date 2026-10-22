## Fix

- **AppArmor profile: scripts now use `rix` instead of `ix`** — `ix` grants the execute transition but not the read permission, and a shebang script is read by its interpreter, so 1.0.1 failed with `/bin/bash: /usr/local/bin/entrypoint.sh: Permission denied` right after start.

This release goes to the **beta** channel first for hardware verification. If you are affected by 1.0.1: update from the beta repository to this version.