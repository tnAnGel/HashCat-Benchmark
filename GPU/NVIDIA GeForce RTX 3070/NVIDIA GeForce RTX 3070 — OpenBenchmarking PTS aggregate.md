# NVIDIA GeForce RTX 3070 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA GeForce RTX 3070 | 6.1.1 | 7-Zip | 687035 | 687.03 kH/s | 57th | 8 | 1251 | [hashcat-1.0.x / 4d816a470aafc62c63dfd70a8fde19b749c15898](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4d816a470aafc62c63dfd70a8fde19b749c15898) |
| NVIDIA GeForce RTX 3070 | 6.1.1 | MD5 | 39128763095 | 39.129 GH/s | 59th | 8 | 718942091 | [hashcat-1.0.x / 56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| NVIDIA GeForce RTX 3070 | 6.1.1 | SHA-512 | 1722116071 | 1.7221 GH/s | 61st | 8 | 101620217 | [hashcat-1.0.x / 7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5) |
| NVIDIA GeForce RTX 3070 | 6.1.1 | SHA1 | 13133998810 | 13.134 GH/s | 59th | 8 | 30140813 | [hashcat-1.0.x / b5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24](https://openbenchmarking.org/test/pts/hashcat%26eval%3Db5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24) |
| NVIDIA GeForce RTX 3070 | 6.1.1 | TrueCrypt RIPEMD160 + XTS | 502951 | 502.95 kH/s | 55th | 8 | 798 | [hashcat-1.0.x / 4845413fe722aca0126f6f9941bf32d6f8aaf6be](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4845413fe722aca0126f6f9941bf32d6f8aaf6be) |
| Gigabyte NVIDIA GeForce RTX 3070 | 6.2.4 | 7-Zip | 1245642 | 1.2456 MH/s | 76th | 4 | 2260 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| ASUS NVIDIA GeForce RTX 3070 | 6.2.4 | 7-Zip | 707706 | 707.71 kH/s | 43rd | 4 | 34938 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA GeForce RTX 3070 | 6.2.4 | 7-Zip | 667084 | 667.08 kH/s | 41st | 21 | 23552 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| Gigabyte NVIDIA GeForce RTX 3070 | 6.2.4 | MD5 | 80013741667 | 80.014 GH/s | 84th | 4 | 228221564 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| NVIDIA GeForce RTX 3070 | 6.2.4 | MD5 | 41225501619 | 41.226 GH/s | 49th | 25 | 1007611524 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| Gigabyte NVIDIA GeForce RTX 3070 | 6.2.4 | SHA-512 | 3653216667 | 3.6532 GH/s | 83rd | 4 | 6071274 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| ASUS NVIDIA GeForce RTX 3070 | 6.2.4 | SHA-512 | 1795185417 | 1.7952 GH/s | 50th | 4 | 49520834 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| NVIDIA GeForce RTX 3070 | 6.2.4 | SHA-512 | 1710009028 | 1.71 GH/s | 48th | 24 | 90152080 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| Gigabyte NVIDIA GeForce RTX 3070 | 6.2.4 | SHA1 | 25073133333 | 25.073 GH/s | 76th | 4 | 13325692 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| ASUS NVIDIA GeForce RTX 3070 | 6.2.4 | SHA1 | 14265858333 | 14.266 GH/s | 46th | 4 | 1126483334 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA GeForce RTX 3070 | 6.2.4 | SHA1 | 12895249242 | 12.895 GH/s | 40th | 22 | 221034560 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| Gigabyte NVIDIA GeForce RTX 3070 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 961175 | 961.17 kH/s | 80th | 4 | 2225 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| ASUS NVIDIA GeForce RTX 3070 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 527072 | 527.07 kH/s | 50th | 4 | 28737 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| NVIDIA GeForce RTX 3070 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 486693 | 486.69 kH/s | 43rd | 25 | 10259 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 19. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
