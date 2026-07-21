# AMD Radeon RX 6600

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 6600
- **Версия hashcat / Version:** v6.2.3
- **Источник / Source:** [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 20580.4 MH/s |
| 100 | SHA1 | 8212.5 MH/s |
| 1400 | SHA2-256 | 3517.3 MH/s |
| 1700 | SHA2-512 | 945.5 MH/s |
| 1000 | NTLM | 33616.7 MH/s |
| 3200 | bcrypt | 26007 H/s |
| 1800 | sha512crypt | 144.3 kH/s |
| 500 | md5crypt | 5622.5 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 417.2 kH/s |
| 7500 | Kerberos AS-REQ (23) | 423.9 MH/s |
| 13100 | Kerberos TGS-REP (23) | 410.5 MH/s |
| 11300 | Bitcoin wallet.dat | 4391 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 264.7 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
OpenCL API (OpenCL 2.1 AMD-APP (3592.0)) - Platform #2 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: AMD Radeon RX 6600, 8112/8176 MB (6732 MB allocatable), 14MCU

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 20580.4 MH/s (45.07ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........:  8212.5 MH/s (113.84ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  3517.3 MH/s (266.25ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:   945.5 MH/s (247.61ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   417.2 kH/s (273.65ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 33616.7 MH/s (27.10ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 19695.0 MH/s (46.81ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 22383.8 MH/s (41.41ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  1407.8 MH/s (332.61ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:   785.8 MH/s (297.68ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........:  5622.5 kH/s (155.62ms) @ Accel:1024 Loops:1000 Thr:64 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    26007 H/s (133.49ms) @ Accel:32 Loops:16 Thr:16 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   144.3 kH/s (322.01ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   423.9 MH/s (276.15ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   410.5 MH/s (285.47ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    71519 H/s (272.91ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    32313 H/s (281.01ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   402.6 kH/s (226.06ms) @ Accel:512 Loops:255 Thr:64 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   383.4 kH/s (267.59ms) @ Accel:512 Loops:4096 Thr:64 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    59038 H/s (482.91ms) @ Accel:512 Loops:16384 Thr:64 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    42780 H/s (333.65ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   264.7 kH/s (429.41ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    35946 H/s (1062.13ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  2726.1 kH/s (324.43ms) @ Accel:1024 Loops:499 Thr:64 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     4391 H/s (266.25ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
```
