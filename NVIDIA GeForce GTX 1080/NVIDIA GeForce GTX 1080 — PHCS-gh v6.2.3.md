# NVIDIA GeForce GTX 1080

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 1080
- **Версия hashcat / Version:** v6.2.3
- **Источник / Source:** [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 28122.2 MH/s |
| 100 | SHA1 | 9524.1 MH/s |
| 1400 | SHA2-256 | 3500.1 MH/s |
| 1700 | SHA2-512 | 1005.3 MH/s |
| 1000 | NTLM | 49639.8 MH/s |
| 3200 | bcrypt | 22062 H/s |
| 1800 | sha512crypt | 160.0 kH/s |
| 500 | md5crypt | 11041.9 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 495.9 kH/s |
| 7500 | Kerberos AS-REQ (23) | 411.9 MH/s |
| 13100 | Kerberos TGS-REP (23) | 395.0 MH/s |
| 11300 | Bitcoin wallet.dat | 5319 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 307.5 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
CUDA API (CUDA 12.5)
====================
* Device #1: NVIDIA GeForce GTX 1080, 7187/8191 MB, 20MCU

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 28122.2 MH/s (47.21ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 100 - SHA1

Speed.#1.........:  9524.1 MH/s (140.38ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  3500.1 MH/s (382.91ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1005.3 MH/s (333.28ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   495.9 kH/s (327.93ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 49639.8 MH/s (26.53ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 3000 - LM

Speed.#1.........: 23103.7 MH/s (57.19ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 27200.2 MH/s (48.82ms) @ Accel:64 Loops:1024 Thr:1024 Vec:2

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  1999.3 MH/s (335.15ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:   954.8 MH/s (350.56ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 11041.9 kH/s (112.68ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    22062 H/s (339.43ms) @ Accel:32 Loops:32 Thr:12 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   160.0 kH/s (403.90ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   411.9 MH/s (406.79ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   395.0 MH/s (424.16ms) @ Accel:512 Loops:512 Thr:32 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    84398 H/s (330.04ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    39151 H/s (321.19ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   491.5 kH/s (328.67ms) @ Accel:8 Loops:1023 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   304.4 kH/s (460.22ms) @ Accel:32 Loops:4096 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    46644 H/s (437.68ms) @ Accel:128 Loops:16384 Thr:128 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    42238 H/s (482.88ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   307.5 kH/s (250.12ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    35815 H/s (761.20ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  2651.7 kH/s (467.86ms) @ Accel:64 Loops:499 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     5319 H/s (313.74ms) @ Accel:32 Loops:512 Thr:1024 Vec:1
```
