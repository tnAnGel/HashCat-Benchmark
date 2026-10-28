# AMD Radeon HD 8250 (Kalindi) — benchmark fragments

- **Версия:** hashcat v5.1.0.
- **Источник:** [raw GitHub Gist](https://gist.github.com/rarecoil/9c8e4ebb33f93d2e90abd49ef5a8bc3a).
- **Примечание:** WPA output is excluded because the source warns the relevant driver may be broken.

| Mode | Hash | Speed |
|---:|---|---:|
| 0 | MD5 | 212.5 MH/s |
| 100 | SHA1 | 66266.6 kH/s |
| 1400 | SHA2-256 | 31404.2 kH/s |
| 1700 | SHA2-512 | 6194.9 kH/s |

```text
Hashmode: 0 - MD5
Speed.#1.........: 212.5 MH/s
Hashmode: 100 - SHA1
Speed.#1.........: 66266.6 kH/s
Hashmode: 1400 - SHA2-256
Speed.#1.........: 31404.2 kH/s
Hashmode: 1700 - SHA2-512
Speed.#1.........: 6194.9 kH/s
```
