# NVIDIA GeForce RTX 5090 Laptop GPU + Intel — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

> **Composite hardware label:** this PTS name combines multiple GPUs. The data are retained as a system-level aggregate and must not be attributed to one GPU.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA GeForce RTX 5090 Laptop GPU + Intel | 7.1.2 | MD5 | 97062633333 | 97.063 GH/s | 89th | 3 | — | [hashcat-1.3.x / 2f1e49c858bdaf551168a2c36422c3bcd6dbf083](https://openbenchmarking.org/test/pts/hashcat%26eval%3D2f1e49c858bdaf551168a2c36422c3bcd6dbf083) |
| NVIDIA GeForce RTX 5090 Laptop GPU + Intel | 7.1.2 | SHA-256 | 13355266667 | 13.355 GH/s | 82nd | 3 | — | [hashcat-1.3.x / bb70ab4002871eaf41c4c257184d478de05cb604](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dbb70ab4002871eaf41c4c257184d478de05cb604) |
| NVIDIA GeForce RTX 5090 Laptop GPU + Intel | 7.1.2 | SHA-512 | 4155966667 | 4.156 GH/s | 78th | 3 | — | [hashcat-1.3.x / ec680f525d7a44fb1c765bf8f3508874a039743e](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dec680f525d7a44fb1c765bf8f3508874a039743e) |
| NVIDIA GeForce RTX 5090 Laptop GPU + Intel | 7.1.2 | SHA1 | 33924400000 | 33.924 GH/s | 79th | 3 | — | [hashcat-1.3.x / eff31b43dba5f679500a7b4a9d777e74ae74d575](https://openbenchmarking.org/test/pts/hashcat%26eval%3Deff31b43dba5f679500a7b4a9d777e74ae74d575) |

**Aggregate rows in this card:** 4. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
