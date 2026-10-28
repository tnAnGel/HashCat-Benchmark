# NVIDIA GeForce RTX 3060 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| eVGA NVIDIA GeForce RTX 3060 | 6.1.1 | 7-Zip | 429197 | 429.2 kH/s | 17th | 5 | 1449 | [hashcat-1.0.x / 4d816a470aafc62c63dfd70a8fde19b749c15898](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4d816a470aafc62c63dfd70a8fde19b749c15898) |
| eVGA NVIDIA GeForce RTX 3060 | 6.1.1 | MD5 | 23299568572 | 23.3 GH/s | 21st | 5 | 643980885 | [hashcat-1.0.x / 56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| eVGA NVIDIA GeForce RTX 3060 | 6.1.1 | SHA-512 | 1035262857 | 1.0353 GH/s | 20th | 5 | 77080213 | [hashcat-1.0.x / 7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5) |
| eVGA NVIDIA GeForce RTX 3060 | 6.1.1 | SHA1 | 7732937143 | 7.7329 GH/s | 17th | 5 | 26830581 | [hashcat-1.0.x / b5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24](https://openbenchmarking.org/test/pts/hashcat%26eval%3Db5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24) |
| eVGA NVIDIA GeForce RTX 3060 | 6.1.1 | TrueCrypt RIPEMD160 + XTS | 300078 | 300.08 kH/s | 14th | 5 | 151 | [hashcat-1.0.x / 4845413fe722aca0126f6f9941bf32d6f8aaf6be](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4845413fe722aca0126f6f9941bf32d6f8aaf6be) |
| eVGA NVIDIA GeForce RTX 3060 | 6.2.4 | 7-Zip | 414253 | 414.25 kH/s | 21st | 16 | 7552 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| eVGA NVIDIA GeForce RTX 3060 | 6.2.4 | MD5 | 24716833334 | 24.717 GH/s | 23rd | 19 | 538085743 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| eVGA NVIDIA GeForce RTX 3060 | 6.2.4 | SHA-512 | 980312963 | 980.31 MH/s | 26th | 19 | 27050779 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| eVGA NVIDIA GeForce RTX 3060 | 6.2.4 | SHA1 | 7703330208 | 7.7033 GH/s | 20th | 17 | 179126765 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| eVGA NVIDIA GeForce RTX 3060 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 289314 | 289.31 kH/s | 16th | 18 | 9540 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 10. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
