# NVIDIA Quadro RTX 5000 with Max-Q Design — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA Quadro RTX 5000 with Max-Q Design | 6.1.1 | 7-Zip | 383100 | 383.1 kH/s | 15th | 5 | 18440 | [hashcat-1.0.x / 4d816a470aafc62c63dfd70a8fde19b749c15898](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4d816a470aafc62c63dfd70a8fde19b749c15898) |
| NVIDIA Quadro RTX 5000 with Max-Q Design | 6.1.1 | MD5 | 24855453333 | 24.855 GH/s | 26th | 5 | 854809991 | [hashcat-1.0.x / 56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| NVIDIA Quadro RTX 5000 with Max-Q Design | 6.1.1 | SHA-512 | 1064300000 | 1.0643 GH/s | 24th | 5 | 60862263 | [hashcat-1.0.x / 7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5) |
| NVIDIA Quadro RTX 5000 with Max-Q Design | 6.1.1 | SHA1 | 8718566667 | 8.7186 GH/s | 27th | 5 | 235672264 | [hashcat-1.0.x / b5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24](https://openbenchmarking.org/test/pts/hashcat%26eval%3Db5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24) |
| NVIDIA Quadro RTX 5000 with Max-Q Design | 6.1.1 | TrueCrypt RIPEMD160 + XTS | 311433 | 311.43 kH/s | 20th | 5 | 15439 | [hashcat-1.0.x / 4845413fe722aca0126f6f9941bf32d6f8aaf6be](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4845413fe722aca0126f6f9941bf32d6f8aaf6be) |

**Aggregate rows in this card:** 5. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
