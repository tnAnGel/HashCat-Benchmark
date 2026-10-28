# AMD Radeon RX 6900 XT — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| AMD Radeon RX 6900 XT | 6.2.4 | 7-Zip | 1195564 | 1.1956 MH/s | 72nd | 10 | 40732 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| AMD Radeon RX 6900 XT | 6.2.4 | MD5 | 58596096296 | 58.596 GH/s | 65th | 9 | 1383732339 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| AMD Radeon RX 6900 XT | 6.2.4 | SHA-512 | 2650203333 | 2.6502 GH/s | 67th | 10 | 29851771 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| AMD Radeon RX 6900 XT | 6.2.4 | SHA1 | 23063048148 | 23.063 GH/s | 74th | 9 | 375580594 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| AMD Radeon RX 6900 XT | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 703199 | 703.2 kH/s | 60th | 9 | 20963 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 5. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
