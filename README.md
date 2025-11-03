Tematom Station - а hybrid software–hardware node that bridges real-world sensors, AI assistants, and human operators through AIPS.

Source of truth: this repository (`main` branch)

Canonical protocol: https://aips.tematom.com

Main Site: https://tematom.com (coming soon)

Main Site (AIPS Verison): https://ai.tematom.com

Station operates as the physical and logical endpoint of the Tematom ecosystem:
- **Firmware:** ESP32 microcontroller running minimal web UI and sensor interface.
- **Daemon:** background process polling sensors and pushing AIPS packets.
- **Bridge:** communication layer between Station and AI assistant via AIPS.
- **Extension:** optional Chrome connector for chat-based interaction.
- **Site:** presentation and AI interface mirror.

For details, see `spec/station_v0.1.md` and `docs/architecture_diagram.md`.

Origin project: https://tematom.com  
Maintained by Tematom team  
Concept design: Andrey K. (aka Ded, humanoid) · Bulgaria · 2025

License: MIT.
