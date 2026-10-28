# NVIDIA GeForce RTX 2080 Ti + Intel UHD 630 + NVIDIA GeForce RTX 2080 Ti — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

> **Composite hardware label:** this PTS name combines multiple GPUs. The data are retained as a system-level aggregate and must not be attributed to one GPU.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA GeForce RTX 2080 Ti + Intel UHD 630 + NVIDIA GeForce RTX 2080 Ti | 6.2.4 | 7-Zip | 1515010 | 1.515 MH/s | 82nd | 4 | 26886 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA GeForce RTX 2080 Ti + Intel UHD 630 + NVIDIA GeForce RTX 2080 Ti | 6.2.4 | SHA-512 | 2376373383 | 2.3764 GH/s | 61st | 4 | 125823330 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| NVIDIA GeForce RTX 2080 Ti + Intel UHD 630 + NVIDIA GeForce RTX 2080 Ti | 6.2.4 | SHA1 | 36422491667 | 36.422 GH/s | 87th | 4 | 394000056 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA GeForce RTX 2080 Ti + Intel UHD 630 + NVIDIA GeForce RTX 2080 Ti | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 1349217 | 1.3492 MH/s | 87th | 4 | 13377 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 4. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
