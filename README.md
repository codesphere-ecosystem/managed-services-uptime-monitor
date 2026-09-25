[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

# Uptime Kuma Template

A [Codesphere](https://codesphere.com) deployment template for [Uptime Kuma](https://github.com/louislam/uptime-kuma), a self-hosted monitoring tool for tracking uptime of websites, APIs, and other services with alerting.

This repository defines a ready-to-use Codesphere Landscape (`ci.main.yml`) and a Codesphere Managed Services catalog entry (`provider.yml`) that deploys the official `louislam/uptime-kuma` container image, so it can be launched on Codesphere with one click.

## Deploying

The template is published as a Codesphere Managed Services catalog entry (see [`provider.yml`](provider.yml)). Deploy it from the Codesphere Managed Services catalog, or reference this repository's `gitUrl` directly when configuring a Landscape.

The deployment:

* runs the `louislam/uptime-kuma` container (see `provider.yml` for the currently pinned version),
* exposes Uptime Kuma's web UI on port `3001`,
* persists monitor data under `data/` via a workspace volume mount.

## Third-Party Software

This template deploys the unmodified [Uptime Kuma](https://github.com/louislam/uptime-kuma) container image. Uptime Kuma is © Louis Lam and contributors, licensed under the [MIT License](https://github.com/louislam/uptime-kuma/blob/master/LICENSE). This repository does not vendor or redistribute Uptime Kuma's source code — the image is pulled from its public registry at deploy time.

## License

The contents of this repository (the `ci.main.yml` pipeline, `provider.yml` catalog manifest, and any other files here) are licensed under the Apache License, Version 2.0 — see the [LICENSE](LICENSE) file for details. This does not extend to Uptime Kuma itself, which remains under its own MIT license as noted above.

## Community & Contributions

Please review our [Code of Conduct](CODE_OF_CONDUCT.md) to understand our community expectations.
We welcome contributions! All contributions to this project must be made in accordance with the Developer Certificate of Origin (DCO). See our full [Contributing Guidelines](CONTRIBUTING.md) for details.

## Maintainers

This repository is maintained by Codesphere SE. At least two senior Codesphere officers hold administrative access to this repository in addition to the day-to-day maintainers, so that departure of any single maintainer does not result in loss of control over the project. Maintainer access is revoked and reassigned promptly when a maintainer leaves the company.
