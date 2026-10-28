# NVIDIA GeForce RTX 3080 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA GeForce RTX 3080 | 6.1.1 | 7-Zip | 971594 | 971.59 kH/s | 84th | 17 | 31305 | [hashcat-1.0.x / 4d816a470aafc62c63dfd70a8fde19b749c15898](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4d816a470aafc62c63dfd70a8fde19b749c15898) |
| NVIDIA GeForce RTX 3080 | 6.1.1 | MD5 | 55648736415 | 55.649 GH/s | 77th | 17 | 2164411777 | [hashcat-1.0.x / 56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| NVIDIA GeForce RTX 3080 | 6.1.1 | SHA-512 | 2434445938 | 2.4344 GH/s | 81st | 17 | 163931408 | [hashcat-1.0.x / 7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5) |
| NVIDIA GeForce RTX 3080 | 6.1.1 | SHA1 | 18821249020 | 18.821 GH/s | 85th | 17 | 532885375 | [hashcat-1.0.x / b5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24](https://openbenchmarking.org/test/pts/hashcat%26eval%3Db5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24) |
| NVIDIA GeForce RTX 3080 | 6.1.1 | TrueCrypt RIPEMD160 + XTS | 708283 | 708.28 kH/s | 84th | 17 | 21572 | [hashcat-1.0.x / 4845413fe722aca0126f6f9941bf32d6f8aaf6be](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4845413fe722aca0126f6f9941bf32d6f8aaf6be) |
| NVIDIA GeForce RTX 3080 | 6.2.4 | 7-Zip | 982013 | 982.01 kH/s | 56th | 17 | 18114 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA GeForce RTX 3080 | 6.2.4 | MD5 | 60185295357 | 60.185 GH/s | 66th | 20 | 958038535 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| Gigabyte NVIDIA GeForce RTX 3080 Lite Hash Rate | 6.2.4 | SHA-512 | 2676788889 | 2.6768 GH/s | 68th | 3 | 31256578 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| NVIDIA GeForce RTX 3080 | 6.2.4 | SHA-512 | 2398875439 | 2.3989 GH/s | 62nd | 19 | 50167695 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| NVIDIA GeForce RTX 3080 | 6.2.4 | SHA1 | 19055773530 | 19.056 GH/s | 59th | 17 | 262837463 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA GeForce RTX 3080 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 705370 | 705.37 kH/s | 60th | 21 | 17473 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 11. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
