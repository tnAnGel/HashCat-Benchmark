# NVIDIA GeForce RTX 4080 SUPER — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| ASUS NVIDIA GeForce RTX 4080 SUPER | 6.2.4 | 7-Zip | 1728800 | 1.7288 MH/s | 87th | 5 | 8385 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA GeForce RTX 4080 SUPER | 6.2.4 | 7-Zip | 1716631 | 1.7166 MH/s | 86th | 3 | 30923 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA GeForce RTX 4080 SUPER | 6.2.4 | SHA-512 | 4357227778 | 4.3572 GH/s | 87th | 3 | 351038586 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| ASUS NVIDIA GeForce RTX 4080 SUPER | 6.2.4 | SHA-512 | 4085470000 | 4.0855 GH/s | 87th | 5 | 380132 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| ASUS NVIDIA GeForce RTX 4080 SUPER | 6.2.4 | SHA1 | 32842605000 | 32.843 GH/s | 86th | 5 | 3644791 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA GeForce RTX 4080 SUPER | 6.2.4 | SHA1 | 30956438889 | 30.956 GH/s | 84th | 3 | 23709851 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| ASUS NVIDIA GeForce RTX 4080 SUPER | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 1240316 | 1.2403 MH/s | 85th | 5 | 215 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| NVIDIA GeForce RTX 4080 SUPER | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 1144375 | 1.1444 MH/s | 84th | 3 | 7448 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 8. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
