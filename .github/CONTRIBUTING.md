# Contributing to JLDN Generational Versioning Schema

Thank you for contributing to the **JLDN Generational Versioning Schema (GVS)** specification!

---

## 1. Schema Invariants

1. **Format Regular Expression:** Any modification to the GVS regular expression must maintain 100% backward-compatibility and pass automated CI regex unit tests.
2. **Alphabetical Lifecycle Ordering:** Compound tags must strictly preserve natural alphabetical sorting (`-a` < `-as` < `-b` < `-bs` < `-l` < `-s` < `-ts` < `-z`).
3. **Generational Task Tracking:** All tasks must be recorded in `.dev/[GEN]/backlog.json`.
