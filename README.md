Kernel v1.1 NDJSON Proof Artifacts

This repository contains two NDJSON exports produced by Kernel v1.1.

Files

kernel-v1.1-clean.ndjson
A normal run demonstrating deterministic ordering with no gaps.

kernel-v1.1-forced-gap.ndjson
A run where one persisted segment was intentionally removed before export.
The kernel emits an explicit gap record and continues exporting without crashing or silently truncating data.

What this demonstrates

Deterministic event ordering

Segmented capture and export

Explicit, first-class gap markers (no silent data loss)

Successful continuation after missing data

These files are intended to be audited directly as independent evidence.
