# JLDN Generational Versioning Schema Knowledge Base

> **Specification:** Generational Versioning Schema (GVS)  
> **Generation Epoch:** `2607.2.0-s`  
> **Author:** Jeff Langdon (JL Design Network)  
> **Status:** Active Standard  

Welcome to the official documentation and specification wiki for the **JLDN Generational Versioning Schema (GVS)**, the generational versioning standard combining historical context, feature iteration, and precise lifecycle and support tracking into a single string (`[YYMM].[SUBVERSION].[REVISION]-[TAG]`).

---

## 📚 Documentation Index

| Document | Description | Target |
| :--- | :--- | :--- |
| **GVS Specification** | Master technical specification: format positions, 8 lifecycle compound tags, and regex standard. | [Specification](specification.md) |
| **Usage & CI/CD Integration** | Automated regular expressions, Bash/Python/PHP validation scripts, and changelog guidelines. | [Usage Guide](usage.md) |
| **Strategic Roadmap** | Generational horizons and future CLI / Git hook tooling roadmap. | [Roadmap](../.dev/ROADMAP.md) |
| **Release History** | Chronological specification release changelog. | [Changelog](../CHANGELOG.md) |

---

## 🎯 Format Overview

```
                          GVS FORMAT DECOMPOSITION
               ┌───────┬────────────┬──────────┬──────────────┐
               │ 2607  │     2      │    0     │     -s       │
               ├───────┼────────────┼──────────┼──────────────┤
               │ Epoch │ Subversion │ Revision │ Lifecycle    │
               │ (YYMM)│ (Feature)  │ (Patch)  │ & Support    │
               └───────┴────────────┴──────────┴──────────────┘
```

- **Format:** `[YYMM].[SUBVERSION].[REVISION]-[TAG]` (e.g., `2607.2.0-s`).
- **Validation Regex:** `^(\d{2}(?:0[1-9]|1[0-2]))\.(\d+)\.(\d+)-(a|as|b|bs|l|s|ts|z)$`
- **Natively Sortable:** Greek-derived compound tags (`-a` to `-z`) guarantee chronological alphabetical sorting.
