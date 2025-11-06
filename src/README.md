**Version 1.0.0 — November 2025**

TEMATOM Station is a minimal demo showing how the AIPS signal chain works  
from sensor → website → Station (daemon) → Bridge → Chrome Extension → AI.

This release includes:
- `tematomstation.c` — the main daemon that reads live sensor data.
- `tematombridge.c` — Chrome Native Messaging bridge for the extension.
- `TematomSetup v.1.0.exe` — installer (Inno Setup).
- `TematomSetup v.1.0.zip` — archive version of the installer.

### Installation
1. Download the installer from the [Releases](https://github.com/Tematom/Station/releases) page.  
2. Run `tematomsetup.exe` (Administrator privileges required).  
3. The software will be installed to `C:\Tematom` and create a desktop shortcut.  
4. Uninstall via Start Menu → Tematom → Uninstall.

### Description
TEMATOM Station demonstrates a simple, functional example of an AIPS data flow:  
sensor readings are pushed to `sensor.tematom.com`, fetched by the daemon,  
saved as `tematomdata.json`, and displayed through a Chrome extension.

### Project goal
Provide an open, working engineering demo that shows practical  
human–AI interaction and sensor integration principles within the AIPS ecosystem.

---

© TEMATOM / Andrey K. (aka Ded)
