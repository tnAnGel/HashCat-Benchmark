# NVIDIA GeForce GTX 770 — 3-GPU benchmark fragment

- **Версия:** hashcat v3.6.0.
- **Источник:** [Hashcat Forum, raw benchmark thread 6708](https://hashcat.net/forum/thread-6708.html).
- **Примечание:** в хосте три GTX 770; скорости ниже оставлены раздельно по устройствам. Это не одиночный GPU-замер.

| Mode | Hash | Speed #1 / #2 / #3 |
|---:|---|---:|
| 900 | MD4 | 6561.4 / 6502.8 / 6427.7 MH/s |
| 0 | MD5 | 3701.8 / 3690.5 / 3666.3 MH/s |
| 100 | SHA1 | 935.7 / 944.1 / 948.1 MH/s |
| 1400 | SHA2-256 | 555.8 / 549.5 / 541.9 MH/s |
| 1700 | SHA2-512 | 110.8 / 108.9 / 108.4 MH/s |

```text
Hash-Mode 0 (MD5)
Speed.#1.........: 3701.8 MH/s
Speed.#2.........: 3690.5 MH/s
Speed.#3.........: 3666.3 MH/s
```
