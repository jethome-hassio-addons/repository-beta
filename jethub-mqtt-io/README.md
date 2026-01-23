# Home Assistant Add-on: JetHome JetHub peripheral exposer

[![Release][release-shield]][release] ![Project Stage][project-stage-shield] ![Project Maintenance][maintenance-shield]

## About

Expose [JetHome JetHub](http://jethome.com) resources (relays,inputs,etc..) to Home Assistant via gpio2mqtt

**Note**: _All used GPIOs will **disappear** from **/sys/class/gpio** during addon run_

## Supported devices:

### [JetHome JetHub D1/D1+](http://jethome.ru/jethub-d1p) (Basic version with 3 relays, 4 inputs and 1-wire, 1 ZigBee module).

**Exposed peripheral:**

- 3 relays
- 4 inputs
- internal stat LED (green/red)
- (optional) ZigBee module control (BOOT, RESET)

**Note**: _You still need to use HACS Home Assistant [1-Wire via sysbus](https://github.com/thecode/ha-onewire-sysbus) integration to expose 1-Wire device 
like temperature sensors `DS18B20`_

### [JetHome JetHub H1](http://jethome.ru/jethub-h1) (Basic version, ZigBee module)

**Exposed peripheral:**

- internal stat LED
- (optional) modules slot control (BOOT, RESET)

## WARNING! THIS IS A BETA VERSION!

This Home Assistant Add-ons repository contains beta releases of add-ons.

- They might stop working at any time.
- They could have a negative impact on your system.

This repository was created for:

- Anybody willing to test.
- Anybody interested in trying out upcoming add-ons or add-on features.

If you are more interested in stable releases of our add-ons:

<https://github.com/jethome-hassio-addons/repository>


## JetHome resources:

- Documentation - https://docs.jethome.com
- Official website - https://jethome.com
- Telegram news channel - https://t.me/jethome_news
- Telegram official chat - https://t.me/jethomeru
- GitHub: https://github.com/jethome-iot

[maintenance-shield]: https://img.shields.io/maintenance/yes/2026.svg
[project-stage-shield]: https://img.shields.io/badge/project%20stage-production%20ready-brightgreen.svg
[release-shield]: https://img.shields.io/badge/version-v0.4.1-rc.1-blue.svg
[release]: https://github.com/jethome-hassio-addons/addon-jethub-mqtt-io/tree/v0.4.1-rc.1