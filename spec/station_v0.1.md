# Tematom Station — v0.1 Specification

Station connects physical sensors and actuators (ESP32-based) with the Tematom AIPS protocol.

## Components
- **Firmware (ESP32):** exposes minimal web UI and sends JSON metrics to daemon.
- **Daemon:** collects, validates, and forwards metrics via HTTP/HTTPS to AIPS endpoint.
- **Bridge:** translates between local HTTP JSON and AI-facing AIPS structures.
- **Extension:** enables direct chat-based interaction with sensors (commands like `.//GET10//`).
- **Safety Layer:** ARM/DISARM mechanism, command TTL, local watchdog.

## Purpose
To provide a lightweight, modular, memory-aware control node usable in both human and AI workflows.

## Dependencies
- curl (C-based daemon)
- JSON/C parser
- ESP-IDF (for firmware)
- Chrome Manifest v3 (for extension)

## Planned Roadmap
- [ ] Autodiscovery of sensors.
- [ ] Secure command confirmation loop.
- [ ] Persistent AIPS event logs.
- [ ] Optional camera integration.

_This file is a live design document. For the canonical data format, see [AIPS](https://aips.tematom.com)._
