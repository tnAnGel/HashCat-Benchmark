# NVIDIA GeForce RTX 3070 Laptop GPU

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 3070 Laptop GPU
- **Версия hashcat / Version:** v6.2.3
- **Источник / Source:** [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 31878.6 MH/s |
| 100 | SHA1 | 10174.2 MH/s |
| 1400 | SHA2-256 | 4408.2 MH/s |
| 1700 | SHA2-512 | 1481.6 MH/s |
| 1000 | NTLM | 58663.3 MH/s |
| 3200 | bcrypt | 53927 H/s |
| 1800 | sha512crypt | 226.9 kH/s |
| 500 | md5crypt | 14277.9 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 519.7 kH/s |
| 7500 | Kerberos AS-REQ (23) | 685.2 MH/s |
| 13100 | Kerberos TGS-REP (23) | 678.6 MH/s |
| 11300 | Bitcoin wallet.dat | 6777 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 393.4 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
CUDA API (CUDA 12.3)
====================
* Device #1: NVIDIA GeForce RTX 3070 Laptop GPU, 7131/8191 MB, 40MCU

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 31878.6 MH/s (83.42ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 100 - SHA1

Speed.#1.........: 10174.2 MH/s (263.01ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  4408.2 MH/s (303.76ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1481.6 MH/s (452.10ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   519.7 kH/s (314.32ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 58663.3 MH/s (45.06ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 3000 - LM

Speed.#1.........: 30866.8 MH/s (85.57ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 32041.9 MH/s (83.12ms) @ Accel:64 Loops:1024 Thr:1024 Vec:2

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  2318.5 MH/s (288.72ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1254.7 MH/s (266.22ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 14277.9 kH/s (177.62ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    53927 H/s (276.92ms) @ Accel:16 Loops:32 Thr:24 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   226.9 kH/s (286.63ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   685.2 MH/s (244.11ms) @ Accel:512 Loops:256 Thr:32 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   678.6 MH/s (246.36ms) @ Accel:512 Loops:256 Thr:32 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    87774 H/s (317.30ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    51020 H/s (254.32ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   639.4 kH/s (254.11ms) @ Accel:4 Loops:1023 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   449.9 kH/s (299.94ms) @ Accel:16 Loops:4096 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    70982 H/s (287.99ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    55478 H/s (368.23ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   393.4 kH/s (385.64ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    65663 H/s (415.30ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  3565.4 kH/s (239.34ms) @ Accel:64 Loops:249 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     6777 H/s (493.21ms) @ Accel:32 Loops:512 Thr:1024 Vec:1
```
