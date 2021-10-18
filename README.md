# BETA - JetHome Home Assistant Add-ons

![Project Stage][project-stage-shield]
![Maintenance][maintenance-shield]

## WARNING! THIS IS A BETA REPOSITORY

This repository contains edge builds of add-ons. Edge
builds add-ons are based upon the latest development version.

- They may not work at all.
- They might stop working at any time.
- They could have a negative impact on your system.

This repository was created for:

- Anybody willing to test.
- Anybody interested in trying out upcoming add-ons or add-on features.
- Developers.

If you are more interested in stable releases of our add-ons:

<https://github.com/jethome-ru/hassio-repository>

## Installation

Adding this add-ons repository to your Home Assistant instance is
pretty straightforward. In the Home Assistant add-on store,
a possibility to add a repository is provided.

Use the following URL to add this repository:

```txt
https://github.com/jethome-ru/hassio-repository-beta
```

## Add-ons provided by this repository

### &#10003; [JetHome JetHub mqtt-io peripheral exposer][addon-hassio-addon-jethub-mqtt-io]

![Latest Version][hassio-addon-jethub-mqtt-io-version-shield]
![Supports armhf Architecture][hassio-addon-jethub-mqtt-io-armhf-shield]
![Supports armv7 Architecture][hassio-addon-jethub-mqtt-io-armv7-shield]
![Supports aarch64 Architecture][hassio-addon-jethub-mqtt-io-aarch64-shield]
![Supports amd64 Architecture][hassio-addon-jethub-mqtt-io-amd64-shield]
![Supports i386 Architecture][hassio-addon-jethub-mqtt-io-i386-shield]

Expose JetHome JetHub peripheral (relays, inputs, etc..) via mqtt-io

[:books: JetHome JetHub mqtt-io peripheral exposer add-on documentation][addon-doc-hassio-addon-jethub-mqtt-io]

## Releases

Releases are based on [Semantic Versioning][semver], and use the format
of ``MAJOR.MINOR.PATCH``. In a nutshell, the version will be incremented
based on the following:

- ``MAJOR``: Incompatible or major changes.
- ``MINOR``: Backwards-compatible new features and enhancements.
- ``PATCH``: Backwards-compatible bugfixes and package updates.

The beta add-ons will also have an additional beta marker, unless, the
stable release is newer, in that case, the stable release is published
in this channel.

## Support

- [Open an issue for the add-on: JetHome JetHub mqtt-io peripheral exposer][hassio-addon-jethub-mqtt-io-issue]

[addon-hassio-addon-jethub-mqtt-io]: https://github.com/jethome-ru/hassio-addon-jethub-mqtt-io/tree/v0.1.2
[addon-doc-hassio-addon-jethub-mqtt-io]: https://github.com/jethome-ru/hassio-addon-jethub-mqtt-io/blob/v0.1.2/README.md
[hassio-addon-jethub-mqtt-io-issue]: https://github.com/jethome-ru/hassio-addon-jethub-mqtt-io/issues
[hassio-addon-jethub-mqtt-io-version-shield]: https://img.shields.io/badge/version-v0.1.2-blue.svg
[hassio-addon-jethub-mqtt-io-aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[hassio-addon-jethub-mqtt-io-amd64-shield]: https://img.shields.io/badge/amd64-no-red.svg
[hassio-addon-jethub-mqtt-io-armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[hassio-addon-jethub-mqtt-io-armv7-shield]: https://img.shields.io/badge/armv7-no-red.svg
[hassio-addon-jethub-mqtt-io-i386-shield]: https://img.shields.io/badge/i386-no-red.svg

[issue]: https://github.com/jethome-ru/hassio-repository-beta/issues
[license-shield]: https://img.shields.io/github/license/jethome-ru/hassio-repository-beta.svg
[maintenance-shield]: https://img.shields.io/maintenance/yes/2021.svg
[project-stage-shield]: https://img.shields.io/badge/project%20stage-development-yellowgreen.svg
[semver]: http://semver.org/spec/v2.0.0.html