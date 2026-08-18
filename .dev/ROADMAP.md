# JLDN Generational Versioning Schema Roadmap

> **Specification:** JLDN Generational Versioning Schema (GVS)  
> **Generation Epoch:** `2607` (Genesis: July 2026)  
> **Author:** Jeff Langdon (JL Design Network)  
> **Status:** Active Standard  

---

## Strategic Vision

The **JLDN Generational Versioning Schema (GVS)** combines historical context, architecture generation, feature iteration, and precise lifecycle/support tracking into a single, chronologically sortable version string (`[YYMM].[SUBVERSION].[REVISION]-[TAG]`).

```
                      GVS EVOLUTION & AUTOMATION ROADMAP
  ┌────────────────────────┐       ┌────────────────────────┐       ┌────────────────────────┐
  │ Generation 2607        │       │ Generation 2608        │       │ Future Tooling         │
  │ Specification Baseline │ ───>  │ Cross-Project Adoption │ ───>  │ Git Hook Bump Daemon   │
  │ 8 Lifecycle Tags & Regx│       │ CI Matrix Integration  │       │ Auto-Changelog Engine  │
  └────────────────────────┘       └────────────────────────┘       └────────────────────────┘
```

---

## Generational Backlogs & Horizons

### Generation 2607 (Active Baseline)
- [x] **Core Generational Specification:** `[YYMM].[SUBVERSION].[REVISION]-[TAG]` format.
- [x] **Compound Tag System:** 8-stage sortable Greek lifecycle tags (`-a`, `-as`, `-b`, `-bs`, `-l`, `-s`, `-ts`, `-z`).
- [x] **Automated Validation Regex:** Strict pattern `^(\d{2}(?:0[1-9]|1[0-2]))\.(\d+)\.(\d+)-(a|as|b|bs|l|s|ts|z)$`.
- [x] **Orange Team Legacy Modernization:** Full baseline scaffolding, in-repo docs wiki, and `.github/` suite.

### Generation 2608+ (Future Tooling)
- [ ] **GVS CLI & Git Hooks:** Standalone `gvs` binary (`gvs bump subversion`, `gvs validate <tag>`).
- [ ] **Multi-Language SDKs:** Python package, Composer package, and NPM library for parsing and sorting GVS version strings.
