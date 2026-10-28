# NVIDIA GeForce RTX 3070 Ti

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 3070 Ti
- **Версия hashcat / Version:** v6.2.3
- **Источник / Source:** [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 44432.0 MH/s |
| 100 | SHA1 | 13974.3 MH/s |
| 1400 | SHA2-256 | 6072.5 MH/s |
| 1700 | SHA2-512 | 2034.4 MH/s |
| 1000 | NTLM | 82095.9 MH/s |
| 3200 | bcrypt | 68460 H/s |
| 1800 | sha512crypt | 333.4 kH/s |
| 500 | md5crypt | 19687.0 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 716.0 kH/s |
| 7500 | Kerberos AS-REQ (23) | 997.7 MH/s |
| 13100 | Kerberos TGS-REP (23) | 991.0 MH/s |
| 11300 | Bitcoin wallet.dat | 9396 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 541.8 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
CUDA API (CUDA 12.3)
====================
* Device #1: NVIDIA GeForce RTX 3070 Ti, 7108/8191 MB, 48MCU

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 44432.0 MH/s (71.89ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 100 - SHA1

Speed.#1.........: 13974.3 MH/s (229.77ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  6072.5 MH/s (264.57ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  2034.4 MH/s (395.04ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   716.0 kH/s (273.81ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 82095.9 MH/s (38.64ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 3000 - LM

Speed.#1.........: 42349.0 MH/s (74.88ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 43995.5 MH/s (72.60ms) @ Accel:64 Loops:1024 Thr:1024 Vec:2

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  3234.5 MH/s (248.24ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1721.5 MH/s (466.67ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 19687.0 kH/s (154.58ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    68460 H/s (261.75ms) @ Accel:16 Loops:32 Thr:24 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   333.4 kH/s (468.07ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   997.7 MH/s (403.00ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   991.0 MH/s (405.61ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:   121.7 kH/s (274.58ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    70401 H/s (442.68ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   878.9 kH/s (395.70ms) @ Accel:64 Loops:127 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   610.5 kH/s (249.45ms) @ Accel:16 Loops:4096 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    99652 H/s (285.98ms) @ Accel:128 Loops:16384 Thr:128 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    76532 H/s (320.16ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   541.8 kH/s (334.27ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    89441 H/s (732.04ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  4931.3 kH/s (311.05ms) @ Accel:32 Loops:499 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     9396 H/s (426.97ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
```
