⚠️ **This add-on is deprecated** and replaced by [JetHome peripheral exposer](https://github.com/jethome-hassio-addons/addon-jethub-gpio2mqtt).

This is a text-only maintenance release on top of 0.4.2-rc.2: the deprecation notice in the documentation and add-on description. The daemon (gpio2mqtt 0.1.5), runtime and build environment are unchanged.

**Migration:** install the new add-on, stop and disable this one, start the new one. The new add-on also has a `legacy_mqttio` compatibility switch that reproduces the old entity IDs.