# JLDN Generational Versioning Schema Specification

Welcome to the official specification repository for the **JLDN Generational Versioning Schema**.

- **Master Specification File:** [gvs-2607.md](./gvs-2607.md)
- **Author:** Jeff Langdon
- **Schema Format:** `[YYMM].[SUBVERSION].[REVISION]-[TAG]`

## Overview

The JLDN Generational Versioning Schema is a proprietary, generational standard designed to combine historical context, feature iteration, and precise lifecycle and support tracking into a single, chronologically sortable string.

### Format Structure

`[YYMM].[SUBVERSION].[REVISION]-[TAG]`

* **`[YYMM]` (The Epoch):** 4-digit generational marker representing the 2-digit year and 2-digit zero-padded month when the core architecture of the software was born (e.g., `2607` for July 2026).
* **`[SUBVERSION]`:** Incrementing integer tracking backward-compatible feature additions or architectural expansions.
* **`[REVISION]`:** Incrementing integer tracking bug fixes and security patches.
* **`-[TAG]`:** Compound lifecycle tag (`-a`, `-as`, `-b`, `-bs`, `-l`, `-s`, `-ts`, `-z`).

## Regular Expression Validation

```regex
^(\d{2}(?:0[1-9]|1[0-2]))\.(\d+)\.(\d+)-(a|as|b|bs|l|s|ts|z)$
```

## License

Designed and maintained by Jeff Langdon / JL Design Network. All rights reserved.
