# NVIDIA GeForce GTX 1080 Ti — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA GeForce GTX 1080 Ti | 6.1.1 | 7-Zip | 519433 | 519.43 kH/s | 35th | 3 | 1247 | [hashcat-1.0.x / 4d816a470aafc62c63dfd70a8fde19b749c15898](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4d816a470aafc62c63dfd70a8fde19b749c15898) |
| NVIDIA GeForce GTX 1080 Ti | 6.1.1 | MD5 | 35379155556 | 35.379 GH/s | 50th | 3 | 48243829 | [hashcat-1.0.x / 56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| NVIDIA GeForce GTX 1080 Ti | 6.1.1 | SHA-512 | 1447777778 | 1.4478 GH/s | 48th | 3 | 3473444 | [hashcat-1.0.x / 7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5) |
| NVIDIA GeForce GTX 1080 Ti | 6.1.1 | SHA1 | 12033222222 | 12.033 GH/s | 51st | 3 | 16670877 | [hashcat-1.0.x / b5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24](https://openbenchmarking.org/test/pts/hashcat%26eval%3Db5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24) |
| NVIDIA GeForce GTX 1080 Ti | 6.1.1 | TrueCrypt RIPEMD160 + XTS | 394511 | 394.51 kH/s | 35th | 3 | 1613 | [hashcat-1.0.x / 4845413fe722aca0126f6f9941bf32d6f8aaf6be](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4845413fe722aca0126f6f9941bf32d6f8aaf6be) |
| NVIDIA GeForce GTX 1080 Ti | 6.2.4 | 7-Zip | 484433 | 484.43 kH/s | 26th | 3 | 52106 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA GeForce GTX 1080 Ti | 6.2.4 | MD5 | 34899044444 | 34.899 GH/s | 42nd | 3 | 2033131846 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| NVIDIA GeForce GTX 1080 Ti | 6.2.4 | SHA-512 | 1345721111 | 1.3457 GH/s | 39th | 3 | 116582613 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| NVIDIA GeForce GTX 1080 Ti | 6.2.4 | SHA1 | 12050044444 | 12.05 GH/s | 37th | 3 | 595321039 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA GeForce GTX 1080 Ti | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 377345 | 377.35 kH/s | 32nd | 3 | 12253 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 10. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
