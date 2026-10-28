# NVIDIA GeForce RTX 4060 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| ASUS NVIDIA GeForce RTX 4060 | 6.2.4 | 7-Zip | 538750 | 538.75 kH/s | 33rd | 5 | — | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| MSI NVIDIA GeForce RTX 4060 | 6.2.4 | 7-Zip | 538311 | 538.31 kH/s | 32nd | 5 | 12506 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| ASUS NVIDIA GeForce RTX 4060 | 6.2.4 | MD5 | 29787116667 | 29.787 GH/s | 33rd | 4 | — | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| MSI NVIDIA GeForce RTX 4060 | 6.2.4 | MD5 | 29442332937 | 29.442 GH/s | 32nd | 6 | 733665312 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| NVIDIA GeForce RTX 4060 | 6.2.4 | MD5 | 29043622222 | 29.044 GH/s | 32nd | 3 | 5846208 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| ASUS NVIDIA GeForce RTX 4060 | 6.2.4 | SHA-512 | 1213550000 | 1.2135 GH/s | 37th | 5 | — | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| MSI NVIDIA GeForce RTX 4060 | 6.2.4 | SHA-512 | 1198430952 | 1.1984 GH/s | 36th | 7 | 28565172 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| ASUS NVIDIA GeForce RTX 4060 | 6.2.4 | SHA1 | 9512350000 | 9.5123 GH/s | 29th | 5 | — | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| MSI NVIDIA GeForce RTX 4060 | 6.2.4 | SHA1 | 9354830000 | 9.3548 GH/s | 28th | 5 | 210949770 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA GeForce RTX 4060 | 6.2.4 | SHA1 | 9284488889 | 9.2845 GH/s | 27th | 3 | 19070522 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| MSI NVIDIA GeForce RTX 4060 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 358275 | 358.27 kH/s | 29th | 7 | 11064 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| ASUS NVIDIA GeForce RTX 4060 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 357007 | 357.01 kH/s | 28th | 5 | — | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 12. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
