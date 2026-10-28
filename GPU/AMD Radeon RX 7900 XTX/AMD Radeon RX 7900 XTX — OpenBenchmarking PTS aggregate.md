# AMD Radeon RX 7900 XTX — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| AMD Radeon RX 7900 XTX | 6.2.4 | 7-Zip | 1449545 | 1.4495 MH/s | 81st | 5 | 85478 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| XFX AMD Radeon RX 7900 XTX | 6.2.4 | 7-Zip | 1424951 | 1.425 MH/s | 81st | 11 | 38214 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| AMD Radeon RX 7900 XTX | 6.2.4 | MD5 | 69855324952 | 69.855 GH/s | 77th | 5 | 1886642606 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| XFX AMD Radeon RX 7900 XTX | 6.2.4 | MD5 | 69059813571 | 69.06 GH/s | 76th | 10 | 814794592 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| AMD Radeon RX 7900 XTX | 6.2.4 | SHA1 | 30261085238 | 30.261 GH/s | 83rd | 5 | 444548120 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| XFX AMD Radeon RX 7900 XTX | 6.2.4 | SHA1 | 29869465152 | 29.869 GH/s | 82nd | 11 | 278324556 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| XFX AMD Radeon RX 7900 XTX | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 926540 | 926.54 kH/s | 79th | 11 | 19301 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| AMD Radeon RX 7900 XTX | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 924501 | 924.5 kH/s | 79th | 5 | 30758 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 8. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
