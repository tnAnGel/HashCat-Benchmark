# Intel UHD Graphics 630 — benchmark fragment

- **GPU:** Intel UHD Graphics 630.
- **Версия:** hashcat v6.2.6.
- **Источник:** [Hashcat Forum benchmark post 58417](https://hashcat.net/forum/thread-11394-post-58417.html).
- **Примечание:** опубликованы только отдельные режимы; показатели CPU из той же системы в эту карточку не включаются.

| Mode | Hash | Speed |
|---:|---|---:|
| 0 | MD5 | 388.0 MH/s |
| 1000 | NTLM | 651.0 MH/s |
| 1400 | SHA2-256 | 47.9022 MH/s |
| 1700 | SHA2-512 | 8.6388 kH/s |
| 2500 | WPA-EAPOL-PBKDF2 | 5767 H/s |
| 3200 | bcrypt | 515 H/s |

```text
Hashmode: 0 - MD5
Speed.#1.........: 388.0 MH/s
Hashmode: 1000 - NTLM
Speed.#1.........: 651.0 MH/s
Hashmode: 1400 - SHA2-256
Speed.#1.........: 47.9022 MH/s
Hashmode: 1700 - SHA2-512
Speed.#1.........: 8.6388 kH/s
Hashmode: 2500 - WPA-EAPOL-PBKDF2
Speed.#1.........: 5767 H/s
Hashmode: 3200 - bcrypt
Speed.#1.........: 515 H/s
```
