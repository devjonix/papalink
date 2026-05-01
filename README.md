# PateLink

> **Unified Control Paradigm for Embedded Device Control**

PateLink is a vendor-independent architectural framework designed to
bridge the gap between embedded hardware and high-level software.
By decoupling transport-layer connectivity from semantic-layer control,
PateLink enables a modular, interoperable ecosystem for industrial
automation, scientific instrumentation, and general electronics.

This repository serves as the **central authority** for the PateLink ecosystem.
It contains the official **Device Type Specifications (DTS)** and the
core documentation defining the PateLink paradigm.

## Project Evolution and Concept

The PateLink architecture was established in 2023, originally conceived as
**OpenLink** to provide a unified control foundation for the DEV Joni product
ecosystem (including scientific light sources such as LogLed).
While the project has undergone two renamings - transitioning from **OpenLink**
to **PapaLink**, and finally to **PateLink** - the core operational principle
has remained constant since its inception.

For a deep dive into the theoretical architecture, the distinction between
transport and semantics, and the hierarchical programming model, please refer
to our primary white paper jointly crafted with Alfrisin Oy CEO, Jori-Aleksi:

**[PateLink - Unified Control Paradigm for Embedded Device Control (2026)](docs/patelink_whitepaper_1May2026.pdf)**

This document provides the technical concept level basis for the OSA Dictionary,
the DTS, and the dual-API structure.


## This Repository: DTS & Documentation

This repository is the primary location for:
1. **Device Type Specifications (DTS):** The canonical blueprints for basic Device Types (e.g., motors, sensors, light sources).
2. **Core Documentation:** Technical specifications for the OSA Semantic KV-Table, the PateLink communication protocol and the dual-API approach.
3. **Governance:** Information regarding the standardization and evolution of the PateLink semantic layer.


## Rest of the PateLink Ecosystem

PateLink is implemented across several specialized repositories. Please navigate
to the appropriate repository based on your aims:

### 1. Python Software Development (Host-Side)
If you are building applications that control PateLink-compliant devices:
* **[patelink-python](https://github.com/devjonix/patelink-python):** The Python reference implementation of the **Direct API** (universal access) and the **Driver API** (semantic productivity).

### 2. Arduino Embedded Development (Device-Side)
If you are a manufacturer or engineer implementing PateLink on hardware:
* **[patelink-arduino](https://github.com/devjonix/patelink-arduino):** Implementation guides and libraries for bringing PateLink support to Arduino-compatible microcontrollers.

### 3. PateLink Verification & Testing (Host-Side)
If you need to validate a device's PateLink compliance:
* **[patelink-testpanels](https://github.com/devjonix/patelink-testpanels):** A suite of tools designed to test device discovery, OSA Dictionary integrity, and DTS compliance.



### Contributing to the DTS

We welcome contributions to the DTS to expand the ecosystem and device types
covered by it.


## License & Neutrality

PateLink is an open-source standard. While the project was architected
by Joni Kemppainen, it is developed and maintained as a community-driven
ecosystem.

To ensure long-term vendor neutrality and prevent ecosystem fragmentation,
PateLink DTS is released under the GPLv3-only license. This ensures that the
protocol remains a public good: it cannot be privatized, and all contributors
and adopters have the legal right to implement, modify, and distribute
PateLink-compliant technologies. PateLink is an independent paradigm,
not a proprietary product of any single commercial entity.

Other parts of PateLink implementations (such as PateLink programming APIs
and MCU firwmares) follow their own licenses set by their creators.



