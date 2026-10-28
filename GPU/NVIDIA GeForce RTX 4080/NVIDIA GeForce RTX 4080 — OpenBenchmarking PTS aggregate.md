# NVIDIA GeForce RTX 4080 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA GeForce RTX 4080 | 6.2.4 | 7-Zip | 1702547 | 1.7025 MH/s | 86th | 15 | 19957 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| ASUS NVIDIA GeForce RTX 4080 | 6.2.4 | 7-Zip | 1669275 | 1.6693 MH/s | 84th | 4 | — | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA GeForce RTX 4080 | 6.2.4 | MD5 | 94350477232 | 94.35 GH/s | 88th | 16 | 2923559665 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| ASUS NVIDIA GeForce RTX 4080 | 6.2.4 | SHA-512 | 3940250000 | 3.9402 GH/s | 86th | 4 | — | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| NVIDIA GeForce RTX 4080 | 6.2.4 | SHA-512 | 3845694048 | 3.8457 GH/s | 85th | 15 | 82521700 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| ASUS NVIDIA GeForce RTX 4080 | 6.2.4 | SHA1 | 31717475000 | 31.717 GH/s | 85th | 4 | — | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA GeForce RTX 4080 | 6.2.4 | SHA1 | 29927393333 | 29.927 GH/s | 82nd | 15 | 724054120 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| ASUS NVIDIA GeForce RTX 4080 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 1200360 | 1.2004 MH/s | 85th | 4 | — | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| NVIDIA GeForce RTX 4080 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 1129802 | 1.1298 MH/s | 83rd | 15 | 13846 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 9. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
