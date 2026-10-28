# AMD Radeon RX Vega 10 Graphics — benchmark fragments

- **Версия:** hashcat v6.2.3.
- **Источник:** [Hashcat Forum — thread 10276](https://hashcat.net/forum/thread-10276.html).
- **Примечание:** четыре режимы имеют успешные `Speed` lines; WPA mode завис без результата и не включён.

| Mode | Hash | Speed.#3 |
|---:|---|---:|
| 0 | MD5 | 3595.8 MH/s |
| 100 | SHA1 | 1374.6 MH/s |
| 1400 | SHA2-256 | 560.2 MH/s |
| 1700 | SHA2-512 | 128.1 MH/s |

```text
Hashmode: 0 - MD5
Speed.#3.........: 3595.8 MH/s
Hashmode: 100 - SHA1
Speed.#3.........: 1374.6 MH/s
Hashmode: 1400 - SHA2-256
Speed.#3.........: 560.2 MH/s
Hashmode: 1700 - SHA2-512
Speed.#3.........: 128.1 MH/s
```
