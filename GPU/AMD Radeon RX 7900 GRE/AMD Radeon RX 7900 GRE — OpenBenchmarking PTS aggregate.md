# AMD Radeon RX 7900 GRE — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| AMD Radeon RX 7900 GRE | 6.2.4 | 7-Zip | 1065031 | 1.065 MH/s | 62nd | 9 | 7111 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| AMD Radeon RX 7900 GRE | 6.2.4 | MD5 | 51301147619 | 51.301 GH/s | 58th | 7 | 2863741235 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| AMD Radeon RX 7900 GRE | 6.2.4 | SHA-512 | 2373040000 | 2.373 GH/s | 61st | 10 | 61328547 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| AMD Radeon RX 7900 GRE | 6.2.4 | SHA1 | 21584620370 | 21.585 GH/s | 66th | 9 | 615881309 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |

**Aggregate rows in this card:** 4. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
