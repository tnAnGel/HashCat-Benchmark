# NVIDIA GeForce RTX 2070 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| ASUS NVIDIA GeForce RTX 2070 | 6.1.1 | 7-Zip | 501632 | 501.63 kH/s | 32nd | 13 | 2442 | [hashcat-1.0.x / 4d816a470aafc62c63dfd70a8fde19b749c15898](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4d816a470aafc62c63dfd70a8fde19b749c15898) |
| ASUS NVIDIA GeForce RTX 2070 | 6.1.1 | MD5 | 29905043590 | 29.905 GH/s | 39th | 13 | 251095361 | [hashcat-1.0.x / 56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| ASUS NVIDIA GeForce RTX 2070 | 6.1.1 | SHA-512 | 1244927839 | 1.2449 GH/s | 37th | 13 | 47597869 | [hashcat-1.0.x / 7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5) |
| ASUS NVIDIA GeForce RTX 2070 | 6.1.1 | SHA1 | 9544720513 | 9.5447 GH/s | 37th | 13 | 37326400 | [hashcat-1.0.x / b5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24](https://openbenchmarking.org/test/pts/hashcat%26eval%3Db5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24) |
| ASUS NVIDIA GeForce RTX 2070 | 6.1.1 | TrueCrypt RIPEMD160 + XTS | 357368 | 357.37 kH/s | 32nd | 13 | 1215 | [hashcat-1.0.x / 4845413fe722aca0126f6f9941bf32d6f8aaf6be](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4845413fe722aca0126f6f9941bf32d6f8aaf6be) |
| ASUS NVIDIA GeForce RTX 2070 | 6.2.4 | 7-Zip | 491946 | 491.95 kH/s | 28th | 7 | 417 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| ASUS NVIDIA GeForce RTX 2070 | 6.2.4 | MD5 | 30865231250 | 30.865 GH/s | 36th | 4 | 446862500 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| ASUS NVIDIA GeForce RTX 2070 | 6.2.4 | SHA-512 | 1230900000 | 1.2309 GH/s | 38th | 7 | 6173735 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| ASUS NVIDIA GeForce RTX 2070 | 6.2.4 | SHA1 | 10170057143 | 10.17 GH/s | 31st | 7 | 444437628 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| ASUS NVIDIA GeForce RTX 2070 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 365643 | 365.64 kH/s | 29th | 7 | 10922 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 10. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
