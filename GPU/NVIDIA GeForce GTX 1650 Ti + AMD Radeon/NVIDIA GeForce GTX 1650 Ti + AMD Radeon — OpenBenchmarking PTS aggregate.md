# NVIDIA GeForce GTX 1650 Ti + AMD Radeon — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

> **Composite hardware label:** this PTS name combines multiple GPUs. The data are retained as a system-level aggregate and must not be attributed to one GPU.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA GeForce GTX 1650 Ti + AMD Radeon | 6.2.4 | MD5 | 14966700000 | 14.967 GH/s | 14th | 3 | 116404257 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |

**Aggregate rows in this card:** 1. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
