# NVIDIA GeForce RTX 2070 SUPER

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 2070 SUPER
- **Версия hashcat / Version:** v6.0.0
- **Источник / Source:** [Staubgeborener](https://gist.github.com/Staubgeborener/f719af9bee8b8d05f4d0816bf7d6a082)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 34762.3 MH/s |
| 100 | SHA1 | 11034.0 MH/s |
| 1400 | SHA2-256 | 4268.5 MH/s |
| 1700 | SHA2-512 | 1378.6 MH/s |
| 1000 | NTLM | 58309.9 MH/s |
| 3200 | bcrypt | 29993 H/s |
| 1800 | sha512crypt | 159.1 kH/s |
| 500 | md5crypt | 14187.2 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 492.9 kH/s |
| 7500 | Kerberos AS-REQ (23) | 372.8 MH/s |
| 13100 | Kerberos TGS-REP (23) | 357.0 MH/s |
| 11300 | Bitcoin wallet.dat | 6154 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 377.9 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.0.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #1: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
* Device #2: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
CUDA API (CUDA 11.0)
====================
* Device #1: GeForce RTX 2070 SUPER, 6719/8192 MB, 40MCU

OpenCL API (OpenCL 1.2 CUDA 11.0.140) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #2: GeForce RTX 2070 SUPER, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........: 34762.3 MH/s (76.85ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 100 - SHA1

Speed.#1.........: 11034.0 MH/s (60.45ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  4268.5 MH/s (78.00ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1378.6 MH/s (60.43ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   492.9 kH/s (82.78ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 58309.9 MH/s (45.60ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 3000 - LM

Speed.#1.........: 29966.9 MH/s (88.80ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 26620.2 MH/s (100.32ms) @ Accel:64 Loops:1024 Thr:1024 Vec:2

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  2108.5 MH/s (79.17ms) @ Accel:64 Loops:64 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1167.0 MH/s (71.24ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 14187.2 kH/s (88.19ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    29993 H/s (20.66ms) @ Accel:4 Loops:8 Thr:16 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   159.1 kH/s (102.19ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   372.8 MH/s (55.82ms) @ Accel:32 Loops:256 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   357.0 MH/s (58.33ms) @ Accel:16 Loops:512 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    84001 H/s (82.70ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    48762 H/s (64.31ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   612.1 kH/s (52.82ms) @ Accel:4 Loops:255 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   475.1 kH/s (75.04ms) @ Accel:4 Loops:4096 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    44498 H/s (57.34ms) @ Accel:1 Loops:16384 Thr:1024 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    45136 H/s (56.49ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   377.9 kH/s (49.80ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    32230 H/s (211.69ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  2594.7 kH/s (60.80ms) @ Accel:4 Loops:499 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     6154 H/s (67.78ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Started: Sat Jun 27 15:38:02 2020
Stopped: Sat Jun 27 15:42:53 2020
```
