# JLDN Generational Versioning Schema

[![GVS](https://img.shields.io/badge/GVS-2607.2.0--s-purple?style=flat-square)](https://github.com/JLDesignNetwork/Generational-Versioning-Schema)
[![License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)
[![Buy Me A Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=flat-square&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/jldesignnetwork)

Welcome to the **JLDN Generational Versioning Schema (GVS)** master specification repository (Generational Versioning Schema: `2607.2.0-s`).

---

## Overview

The **JLDN Generational Versioning Schema (GVS)** is a proprietary versioning protocol designed to combine historical context, feature iteration, and precise lifecycle and support tracking into a single, chronologically sortable string.

* **Author:** Jeff Langdon (JL Design Network)
* **Specification Version:** `2607.2.0-s` (Stable Release)
* **Active Generation:** `2607`

---

## 📚 Documentation & Quick Links

- 📄 **[GVS Specification](docs/specification.md):** Complete technical protocol, format positions, and compound lifecycle tags.
- 🛠️ **[Usage Guide & CI Scripts](docs/usage.md):** Automated regex validation patterns for Bash, Python, and PHP.
- 🗺️ **[Strategic Roadmap](.dev/ROADMAP.md):** Generational roadmap and future tooling.
- 📝 **[Changelog](CHANGELOG.md):** Specification release history.

---

## Core Features

- **Format Structure:** `[YYMM].[SUBVERSION].[REVISION]-[TAG]` (e.g. `2607.2.0-s`).
- **Generational Epoch Marker:** Four-digit year/month architecture origin indicator (`2607`).
- **Alphabetically Sortable Compound Tags:** Eight Greek-inspired lifecycle stages (`-a`, `-as`, `-b`, `-bs`, `-l`, `-s`, `-ts`, `-z`).
- **Validation Regular Expression:** `^(\d{2}(?:0[1-9]|1[0-2]))\.(\d+)\.(\d+)-(a|as|b|bs|l|s|ts|z)$`

---

## Funding & Support

If you find this specification or associated developer tooling helpful, consider supporting ongoing development:

[![Buy Me A Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=flat-square&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/jldesignnetwork)

---

## License & Attribution

Licensed under the [MIT License](LICENSE). Designed and maintained by Jeff Langdon / JL Design Network. All rights reserved.
