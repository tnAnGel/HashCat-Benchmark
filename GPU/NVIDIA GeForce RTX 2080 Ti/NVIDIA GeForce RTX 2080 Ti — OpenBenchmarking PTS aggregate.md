# NVIDIA GeForce RTX 2080 Ti — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA GeForce RTX 2080 Ti | 6.1.1 | 7-Zip | 887858 | 887.86 kH/s | 70th | 19 | 7331 | [hashcat-1.0.x / 4d816a470aafc62c63dfd70a8fde19b749c15898](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4d816a470aafc62c63dfd70a8fde19b749c15898) |
| NVIDIA GeForce RTX 2080 Ti | 6.1.1 | MD5 | 55501722055 | 55.502 GH/s | 77th | 19 | 669105569 | [hashcat-1.0.x / 56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| NVIDIA GeForce RTX 2080 Ti | 6.1.1 | SHA-512 | 2320916792 | 2.3209 GH/s | 75th | 19 | 108646348 | [hashcat-1.0.x / 7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5) |
| NVIDIA GeForce RTX 2080 Ti | 6.1.1 | SHA1 | 17778797243 | 17.779 GH/s | 74th | 19 | 79147800 | [hashcat-1.0.x / b5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24](https://openbenchmarking.org/test/pts/hashcat%26eval%3Db5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24) |
| NVIDIA GeForce RTX 2080 Ti | 6.1.1 | TrueCrypt RIPEMD160 + XTS | 653012 | 653.01 kH/s | 70th | 19 | 4769 | [hashcat-1.0.x / 4845413fe722aca0126f6f9941bf32d6f8aaf6be](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4845413fe722aca0126f6f9941bf32d6f8aaf6be) |
| Zotac NVIDIA GeForce RTX 2080 Ti | 6.2.4 | 7-Zip | 2918144 | 2.9181 MH/s | 95th | 3 | 5691 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| ASUS NVIDIA GeForce RTX 2080 Ti | 6.2.4 | 7-Zip | 854773 | 854.77 kH/s | 51st | 4 | — | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA GeForce RTX 2080 Ti | 6.2.4 | 7-Zip | 829313 | 829.31 kH/s | 49th | 8 | 65743 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| Zotac NVIDIA GeForce RTX 2080 Ti | 6.2.4 | MD5 | 130494289583 | 130.49 GH/s | 92nd | 3 | 210426329 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| NVIDIA GeForce RTX 2080 Ti | 6.2.4 | MD5 | 50719868810 | 50.72 GH/s | 58th | 10 | 5515024539 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| ASUS NVIDIA GeForce RTX 2080 Ti | 6.2.4 | SHA-512 | 2356225000 | 2.3562 GH/s | 60th | 4 | — | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| NVIDIA GeForce RTX 2080 Ti | 6.2.4 | SHA-512 | 2121733333 | 2.1217 GH/s | 56th | 10 | 213556020 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| Zotac NVIDIA GeForce RTX 2080 Ti | 6.2.4 | SHA1 | 64931622222 | 64.932 GH/s | 95th | 3 | 42928265 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| ASUS NVIDIA GeForce RTX 2080 Ti | 6.2.4 | SHA1 | 19593675000 | 19.594 GH/s | 61st | 4 | — | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA GeForce RTX 2080 Ti | 6.2.4 | SHA1 | 16008560000 | 16.009 GH/s | 51st | 10 | 1845259857 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| Zotac NVIDIA GeForce RTX 2080 Ti | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 2395944 | 2.3959 MH/s | 95th | 3 | 17506 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| ASUS NVIDIA GeForce RTX 2080 Ti | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 708860 | 708.86 kH/s | 61st | 4 | — | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| NVIDIA GeForce RTX 2080 Ti | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 582388 | 582.39 kH/s | 53rd | 10 | 52816 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 18. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
