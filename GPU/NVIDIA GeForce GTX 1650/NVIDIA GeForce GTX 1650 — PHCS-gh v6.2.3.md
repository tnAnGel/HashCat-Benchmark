# NVIDIA GeForce GTX 1650

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 1650
- **Версия hashcat / Version:** v6.2.3
- **Источник / Source:** [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 11622.2 MH/s |
| 100 | SHA1 | 3847.9 MH/s |
| 1400 | SHA2-256 | 1661.4 MH/s |
| 1700 | SHA2-512 | 535.1 MH/s |
| 1000 | NTLM | 19416.4 MH/s |
| 3200 | bcrypt | 12977 H/s |
| 1800 | sha512crypt | 58570 H/s |
| 500 | md5crypt | 5108.7 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 190.7 kH/s |
| 7500 | Kerberos AS-REQ (23) | 214.6 MH/s |
| 13100 | Kerberos TGS-REP (23) | 205.1 MH/s |
| 11300 | Bitcoin wallet.dat | 2374 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 144.6 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
CUDA API (CUDA 12.6)
====================
* Device #1: NVIDIA GeForce GTX 1650, 3296/4095 MB, 14MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 11622.2 MH/s (80.24ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........:  3847.9 MH/s (243.56ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  1661.4 MH/s (282.21ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:   535.1 MH/s (438.32ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   190.7 kH/s (299.27ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 19416.4 MH/s (47.77ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 11112.2 MH/s (83.55ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 11981.7 MH/s (77.82ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:   799.9 MH/s (293.03ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:   451.1 MH/s (259.48ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........:  5108.7 kH/s (171.69ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    12977 H/s (268.86ms) @ Accel:16 Loops:32 Thr:16 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:    58570 H/s (389.19ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   214.6 MH/s (273.05ms) @ Accel:512 Loops:256 Thr:32 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   205.1 MH/s (285.75ms) @ Accel:256 Loops:512 Thr:32 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    32379 H/s (300.03ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    18397 H/s (238.96ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   230.8 kH/s (245.47ms) @ Accel:4 Loops:1023 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   194.8 kH/s (287.34ms) @ Accel:16 Loops:4096 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    20475 H/s (349.25ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    17724 H/s (401.07ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   144.6 kH/s (365.30ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    12168 H/s (783.76ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  1121.0 kH/s (262.29ms) @ Accel:64 Loops:249 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     2374 H/s (246.16ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
```
