## JetHome peripheral exposer — beta

Rename release: the add-on is now **JetHome peripheral exposer** (no uppercase acronym in the name).

Based on the [gpio2mqtt](https://github.com/jethome-iot/gpio2mqtt) daemon (binary **0.2.0**). It coexists with the legacy `jethub-mqtt-io` add-on and refuses to start while that one is running (both claim the same GPIO lines).

### Highlights

- **New MQTT topic / entity structure by default** (`legacy_mqttio: false`): entities are grouped under a JetHub device with modern discovery payloads (`origin` block, availability list, `has_entity_name`-friendly short entity names). Set `mqtt.legacy_mqttio: true` to get the old mqtt-io entity IDs back.
- **JetHub D3 (J310) support**: UXM1–4 RESET/MODE control lines on the TCA6408A I2C port expander, gpiochip auto-resolved at startup.
- **Restore after power cycle**: `restore_mode` option (`restore`/`off`/`on`, default `restore`) — output states survive restarts via MQTT retained messages (gpio2mqtt #96).
- **Reliable MQTT lifecycle** (gpio2mqtt 0.2.0): everything is published strictly after ConnAck and re-published on every reconnect; HA birth message handled; input states retained — fixes the legacy add-on issues #49/#50.
- **Startup guard**: checks via the Supervisor API that the legacy `jethub-mqtt-io` add-on is not running.

### Migration from jethub-mqtt-io

1. Install this add-on (keep both stopped).
2. Stop & disable `jethub-mqtt-io`.
3. Start this add-on; new entities appear under a JetHub device — update automations and dashboards accordingly.

Full documentation: [DOCS.md](https://github.com/jethome-hassio-addons/addon-jethub-gpio2mqtt/blob/main/jethub-gpio2mqtt/DOCS.md)
