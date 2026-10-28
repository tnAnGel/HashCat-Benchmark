# AMD Ryzen 5 2400G — benchmark fragments

- **Процессор:** AMD Ryzen 5 2400G.
- **Источники:** [mode 1800 results](https://hashcat.net/forum/thread-8388.html), [mode 2500 results](https://hashcat.net/forum/thread-9054.html).
- **Примечание:** CPU `Speed.#N` results only. The APU integrated-GPU scores and CPU-skipped run are excluded.

| Version | Mode | Hash | CPU speed |
|---|---:|---|---:|
| v5.1.0 | 1800 | sha512crypt | 2530 H/s |
| v5.1.0 | 1800 | sha512crypt | 2592 H/s |
| v5.1.0-1116-g3c603019 | 1800 | sha512crypt | 2484 H/s |
| v5.1.0-1116-g3c603019 | 1800 | sha512crypt | 2586 H/s |
| v5.1.0 | 2500 | WPA-EAPOL-PBKDF2 | 6630 H/s |
| v5.1.0-1755-gddb641b8 | 2500 | WPA-EAPOL-PBKDF2 | 7267 H/s |

```text
Hashmode: 1800 - sha512crypt
Speed.#2.........: 2530 H/s
Hashmode: 2500 - WPA-EAPOL-PBKDF2
Speed.#2.........: 6630 H/s
```
