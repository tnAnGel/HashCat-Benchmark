# NVIDIA GeForce RTX 4070 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| ASUS NVIDIA GeForce RTX 4070 | 6.2.4 | 7-Zip | 1025013 | 1.025 MH/s | 59th | 8 | 3595 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA GeForce RTX 4070 | 6.2.4 | 7-Zip | 993572 | 993.57 kH/s | 57th | 4 | 91292 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| ASUS NVIDIA GeForce RTX 4070 | 6.2.4 | MD5 | 57922550000 | 57.923 GH/s | 63rd | 5 | 2188439730 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| NVIDIA GeForce RTX 4070 | 6.2.4 | MD5 | 56042334921 | 56.042 GH/s | 60th | 3 | 2300081737 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| ASUS NVIDIA GeForce RTX 4070 | 6.2.4 | SHA-512 | 2394862500 | 2.3949 GH/s | 62nd | 8 | 75381033 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| NVIDIA GeForce RTX 4070 | 6.2.4 | SHA-512 | 2387491667 | 2.3875 GH/s | 61st | 4 | 123277781 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| ASUS NVIDIA GeForce RTX 4070 | 6.2.4 | SHA1 | 19199704167 | 19.2 GH/s | 59th | 8 | 1020906764 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA GeForce RTX 4070 | 6.2.4 | SHA1 | 18103608333 | 18.104 GH/s | 55th | 4 | 333090873 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| ASUS NVIDIA GeForce RTX 4070 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 721054 | 721.05 kH/s | 62nd | 8 | 32570 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| NVIDIA GeForce RTX 4070 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 681328 | 681.33 kH/s | 57th | 4 | 14835 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 10. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
