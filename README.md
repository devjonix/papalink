# PapaLink

> **Unified Control Paradigm for Embedded Device Control**

PapaLink is a vendor-independent architectural framework designed to
bridge the gap between embedded hardware and high-level software.
By decoupling transport-layer connectivity from semantic-layer control,
PapaLink enables a modular, interoperable ecosystem for industrial
automation, scientific instrumentation, and general electronics.

This repository serves as the **central authority** for the PapaLink ecosystem.
It contains the official **Device Type Specifications (DTS)** and the
core documentation defining the PapaLink paradigm.

## Project Evolution and Concept

The PapaLink architecture was established in 2023, originally conceived as
**OpenLink** to provide a unified control foundation for the DEV Joni product
ecosystem (including scientific light sources such as LogLed).
While the project has undergone two renamings - transitioning from **OpenLink**
to **PapaLink**, and finally to **PapaLink** - the core operational principle
has remained constant since its inception.

For a deep dive into the theoretical architecture, the distinction between
transport and semantics, and the hierarchical programming model, please refer
to our primary white paper jointly crafted with Alfrisin Oy CEO, Jori-Aleksi:

**[PapaLink - Unified Control Paradigm for Embedded Device Control (2026)](docs/papalink_whitepaper_1May2026.pdf)**

This document provides the technical concept level basis for the OSA Dictionary,
the DTS, and the dual-API structure.


## This Repository: DTS & Documentation

This repository is the primary location for:
1. **Device Type Specifications (DTS):** The canonical blueprints for basic Device Types (e.g., motors, sensors, light sources).
2. **Core Documentation:** Technical specifications for the OSA Semantic KV-Table, the PapaLink communication protocol and the dual-API approach.
3. **Governance:** Information regarding the standardization and evolution of the PapaLink semantic layer.


## Rest of the PapaLink Ecosystem

PapaLink is implemented across several specialized repositories. Please navigate
to the appropriate repository based on your aims:

### 1. Python Software Development (Host-Side)
If you are building applications that control PapaLink-compliant devices:
* **[papalink-python](https://github.com/devjonix/papalink-python):** The Python reference implementation of the **Direct API** (universal access) and the **Driver API** (semantic productivity).

### 2. Arduino Embedded Development (Device-Side)
If you are a manufacturer or engineer implementing PapaLink on hardware:
* **[papalink-arduino](https://github.com/devjonix/papalink-arduino):** Implementation guides and libraries for bringing PapaLink support to Arduino-compatible microcontrollers.

### 3. PapaLink Verification & Testing (Host-Side)
If you need to validate a device's PapaLink compliance:
* **[papalink-testpanels](https://github.com/devjonix/papalink-testpanels):** A suite of tools designed to test device discovery, OSA Dictionary integrity, and DTS compliance.



## Contributing to the DTS

We welcome contributions to the DTS to expand the ecosystem and device types
covered by it.


## License & Neutrality

PapaLink is an open-source standard. While the project was architected
by Joni Kemppainen, it is developed and maintained as a community-driven
ecosystem.

To ensure long-term vendor neutrality and prevent ecosystem fragmentation,
PapaLink DTS is released under the GPLv3-only license. This ensures that the
protocol remains a public good: it cannot be privatized, and all contributors
and adopters have the legal right to implement, modify, and distribute
PapaLink-compliant technologies. PapaLink is an independent paradigm,
not a proprietary product of any single commercial entity.

Other parts of PapaLink implementations (such as PapaLink programming APIs
and MCU firwmares) follow their own licenses set by their creators.



