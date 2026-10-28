# NVIDIA GeForce GTX 1060 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA GeForce GTX 1060 | 6.1.1 | 7-Zip | 204944 | 204.94 kH/s | 5th | 4 | 5746 | [hashcat-1.0.x / 4d816a470aafc62c63dfd70a8fde19b749c15898](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4d816a470aafc62c63dfd70a8fde19b749c15898) |
| NVIDIA GeForce GTX 1060 | 6.1.1 | MD5 | 13636325000 | 13.636 GH/s | 13th | 4 | 516031074 | [hashcat-1.0.x / 56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| NVIDIA GeForce GTX 1060 | 6.1.1 | SHA-512 | 534742857 | 534.74 MH/s | 10th | 4 | 47273598 | [hashcat-1.0.x / 7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5) |
| NVIDIA GeForce GTX 1060 | 6.1.1 | SHA1 | 4572827381 | 4.5728 GH/s | 11th | 4 | 118570176 | [hashcat-1.0.x / b5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24](https://openbenchmarking.org/test/pts/hashcat%26eval%3Db5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24) |
| NVIDIA GeForce GTX 1060 | 6.1.1 | TrueCrypt RIPEMD160 + XTS | 148583 | 148.58 kH/s | 5th | 4 | 4547 | [hashcat-1.0.x / 4845413fe722aca0126f6f9941bf32d6f8aaf6be](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4845413fe722aca0126f6f9941bf32d6f8aaf6be) |
| NVIDIA GeForce GTX 1060 | 6.2.4 | 7-Zip | 187083 | 187.08 kH/s | 4th | 7 | 4382 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| Gigabyte NVIDIA GeForce GTX 1060 | 6.2.4 | 7-Zip | 179960 | 179.96 kH/s | 4th | 5 | 16283 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA GeForce GTX 1060 | 6.2.4 | MD5 | 12922255102 | 12.922 GH/s | 12th | 7 | 355004173 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| NVIDIA GeForce GTX 1060 | 6.2.4 | SHA-512 | 481636666 | 481.64 MH/s | 12th | 5 | 4241075 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| NVIDIA GeForce GTX 1060 | 6.2.4 | SHA1 | 4479875000 | 4.4799 GH/s | 12th | 6 | 53272671 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA GeForce GTX 1060 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 135115 | 135.12 kH/s | 5th | 6 | 4060 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 11. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
