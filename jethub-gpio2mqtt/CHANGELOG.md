## AppArmor fix for the sysfs base resolution (issue #2 follow-up)

The AppArmor profile did not allow reads under `/sys/devices/**/gpiochip*` and `/sys/devices/**/gpio/` — exactly where the `/sys/bus/gpio/devices` symlinks resolve. The unexport helper's base resolution was silently denied, so the 1.0.3-rc.1 loud error fired even though the resolution logic itself is correct.

Rules verified on hardware (JetHub D1+, Armbian 6.6, HA Supervised).