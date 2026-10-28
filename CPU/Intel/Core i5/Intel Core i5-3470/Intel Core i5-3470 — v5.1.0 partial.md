# Intel Core i5-3470 — benchmark fragments

- **Процессор:** Intel Core i5-3470.
- **Версия:** hashcat v5.1.0.
- **Источник:** [Hashcat Forum — Hashcat running incorrectly and not using GPU](https://hashcat.net/forum/thread-8702.html).
- **Примечание:** результаты ниже — опубликованные benchmark-режимы CPU. Устройство CPU обозначено как Device #1; не включены обычные cracking-скорости.

| Mode | Hash | Speed |
|---:|---|---:|
| 0 | MD5 | 158.8 MH/s |
| 100 | SHA1 | 117.2 MH/s |
| 1400 | SHA2-256 | 51439.7 kH/s |
| 1700 | SHA2-512 | 14678.9 kH/s |
| 2500 | WPA-EAPOL-PBKDF2 | 5451 H/s |
| 1000 | NTLM | 280.7 MH/s |

```text
* Device #1: Intel(R) Core(TM) i5-3470 CPU @ 3.20GHz
Hashmode: 0 - MD5
Speed.#1.........: 158.8 MH/s
Hashmode: 100 - SHA1
Speed.#1.........: 117.2 MH/s
Hashmode: 1400 - SHA2-256
Speed.#1.........: 51439.7 kH/s
Hashmode: 1700 - SHA2-512
Speed.#1.........: 14678.9 kH/s
Hashmode: 2500 - WPA-EAPOL-PBKDF2
Speed.#1.........: 5451 H/s
Hashmode: 1000 - NTLM
Speed.#1.........: 280.7 MH/s
```
