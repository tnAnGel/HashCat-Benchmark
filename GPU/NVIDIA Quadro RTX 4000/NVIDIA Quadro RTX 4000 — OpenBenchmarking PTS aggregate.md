# NVIDIA Quadro RTX 4000 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA Quadro RTX 4000 | 6.1.1 | 7-Zip | 437371 | 437.37 kH/s | 20th | 8 | 10975 | [hashcat-1.0.x / 4d816a470aafc62c63dfd70a8fde19b749c15898](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4d816a470aafc62c63dfd70a8fde19b749c15898) |
| NVIDIA Quadro RTX 4000 | 6.1.1 | TrueCrypt RIPEMD160 + XTS | 321113 | 321.11 kH/s | 22nd | 8 | 7082 | [hashcat-1.0.x / 4845413fe722aca0126f6f9941bf32d6f8aaf6be](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4845413fe722aca0126f6f9941bf32d6f8aaf6be) |
| NVIDIA Quadro RTX 4000 | 6.2.4 | 7-Zip | 437622 | 437.62 kH/s | 23rd | 6 | 5025 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA Quadro RTX 4000 | 6.2.4 | MD5 | 25312366667 | 25.312 GH/s | 26th | 6 | 398464083 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| NVIDIA Quadro RTX 4000 | 6.2.4 | SHA-512 | 1121283333 | 1.1213 GH/s | 33rd | 6 | 52814294 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| NVIDIA Quadro RTX 4000 | 6.2.4 | SHA1 | 8733400000 | 8.7334 GH/s | 25th | 6 | 55209589 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA Quadro RTX 4000 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 314583 | 314.58 kH/s | 23rd | 6 | 3973 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 7. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
