# NVIDIA GeForce RTX 3090 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA GeForce RTX 3090 | 6.1.1 | 7-Zip | 1150599 | 1.1506 MH/s | 92nd | 17 | 5542 | [hashcat-1.0.x / 4d816a470aafc62c63dfd70a8fde19b749c15898](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4d816a470aafc62c63dfd70a8fde19b749c15898) |
| NVIDIA GeForce RTX 3090 | 6.1.1 | MD5 | 67148389076 | 67.148 GH/s | 95th | 17 | 1213402211 | [hashcat-1.0.x / 56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| NVIDIA GeForce RTX 3090 | 6.1.1 | SHA-512 | 2932751261 | 2.9328 GH/s | 94th | 17 | 147867483 | [hashcat-1.0.x / 7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5) |
| NVIDIA GeForce RTX 3090 | 6.1.1 | SHA1 | 22724054622 | 22.724 GH/s | 93rd | 17 | 105548212 | [hashcat-1.0.x / b5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24](https://openbenchmarking.org/test/pts/hashcat%26eval%3Db5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24) |
| NVIDIA GeForce RTX 3090 | 6.1.1 | TrueCrypt RIPEMD160 + XTS | 850938 | 850.94 kH/s | 94th | 17 | 4786 | [hashcat-1.0.x / 4845413fe722aca0126f6f9941bf32d6f8aaf6be](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4845413fe722aca0126f6f9941bf32d6f8aaf6be) |
| NVIDIA GeForce RTX 3090 | 6.2.4 | 7-Zip | 1120746 | 1.1207 MH/s | 67th | 38 | 31660 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA GeForce RTX 3090 | 6.2.4 | MD5 | 70733634505 | 70.734 GH/s | 78th | 41 | 3184998432 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| NVIDIA GeForce RTX 3090 | 6.2.4 | SHA-512 | 2872803070 | 2.8728 GH/s | 74th | 40 | 122009584 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| ASUS NVIDIA GeForce RTX 3090 | 6.2.4 | SHA1 | 23914853333 | 23.915 GH/s | 75th | 5 | 797038977 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA GeForce RTX 3090 | 6.2.4 | SHA1 | 22198051111 | 22.198 GH/s | 69th | 41 | 1052003460 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| ASUS NVIDIA GeForce RTX 3090 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 869188 | 869.19 kH/s | 76th | 5 | 12683 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| NVIDIA GeForce RTX 3090 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 816757 | 816.76 kH/s | 72nd | 40 | 22454 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 12. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
