## Fix for Armbian / HA Supervised installs (issue #2)

On kernel 6.x (e.g. official JetHome Armbian bookworm images) the GPIO sysfs topology changed: the startup GPIO-unexport helper could not resolve the chip base and silently skipped, leaving sysfs-held lines busy — gpio2mqtt then failed with `Device or resource busy`.

- sysfs chip base resolution now handles the modern topology (checks the resolved device directory first), keeps the legacy layouts as fallbacks, and adds a chip-label fallback (label read via the GPIO uAPI ioctl);
- if the base cannot be resolved while the sysfs GPIO interface is active, the helper now fails loudly (listing the configured line offsets, with a manual unexport hint) instead of silently doing nothing.

Testing on a JetHub D1/D1+ with Armbian + HA Supervised is welcome — please report in issue #2.