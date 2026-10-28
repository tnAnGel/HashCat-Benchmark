# NVIDIA GeForce GTX 950 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| eVGA NVIDIA GeForce GTX 950 | 6.1.1 | MD5 | 4791888889 | 4.7919 GH/s | 7th | 3 | 74241410 | [hashcat-1.0.x / 56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| eVGA NVIDIA GeForce GTX 950 | 6.1.1 | SHA-512 | 179100000 | 179.1 MH/s | 5th | 3 | 6781674 | [hashcat-1.0.x / 7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5) |
| eVGA NVIDIA GeForce GTX 950 | 6.1.1 | SHA1 | 1678222222 | 1.6782 GH/s | 5th | 3 | 16271664 | [hashcat-1.0.x / b5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24](https://openbenchmarking.org/test/pts/hashcat%26eval%3Db5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24) |

**Aggregate rows in this card:** 3. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
