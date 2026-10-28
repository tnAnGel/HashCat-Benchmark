# NVIDIA GeForce GTX 1060 with Max-Q Design

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 1060 with Max-Q Design (мобильный/laptop GPU; Device #3 — 1060 Max-Q, Device #1/#2 — Intel HD 630 и CPU, пропущены)
- **Версия hashcat / Version:** не указана в источнике / not stated (пост 2018 г., старый формат вывода `Speed.Dev.#`)
- **Источник / Source:** [hashcat forum — thread 7695, kevtheskin, 2018-07-28](https://hashcat.net/forum/thread-7695.html)

## Ключевые результаты / Highlights (Device #3 — GTX 1060 Max-Q)

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 9077.2 MH/s |
| 100 | SHA1 | 3560.1 MH/s |
| 1400 | SHA-256 | 1334.9 MH/s |
| 1700 | SHA-512 | 446.6 MH/s |
| 1000 | NTLM | 15332.5 MH/s |
| 3200 | bcrypt | 6855 H/s |
| 1800 | sha512crypt | 57001 H/s |
| 500 | md5crypt | 4145.7 kH/s |
| 2500 | WPA/WPA2 | 165.8 kH/s |
| 7500 | Kerberos AS-REQ (23) | 130.7 MH/s |
| 13100 | Kerberos TGS-REP (23) | 132.5 MH/s |
| 11300 | Bitcoin wallet.dat | 1973 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 114.2 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
OpenCL Platform #1: Intel(R) Corporation
========================================
* Device #1: Intel(R) HD Graphics 630, skipped.
* Device #2: Intel(R) Core(TM) i7-7700HQ CPU @ 2.80GHz, skipped.
OpenCL Platform #2: NVIDIA Corporation
======================================
* Device #3: GeForce GTX 1060 with Max-Q Design, 1536/6144 MB allocatable, 10MCU
Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5
Speed.Dev.#3.....: 9077.2 MH/s (36.87ms) @ Accel:128 Loops:256 Thr:1024 Vec:1

Hashmode: 100 - SHA1
Speed.Dev.#3.....: 3560.1 MH/s (58.61ms) @ Accel:256 Loops:128 Thr:640 Vec:1

Hashmode: 1400 - SHA-256
Speed.Dev.#3.....: 1334.9 MH/s (62.49ms) @ Accel:128 Loops:64 Thr:1024 Vec:1

Hashmode: 1700 - SHA-512
Speed.Dev.#3.....: 446.6 MH/s (58.05ms) @ Accel:128 Loops:32 Thr:640 Vec:1

Hashmode: 2500 - WPA/WPA2 (Iterations: 4096)
Speed.Dev.#3.....: 165.8 kH/s (61.10ms) @ Accel:128 Loops:32 Thr:1024 Vec:1

Hashmode: 1000 - NTLM
Speed.Dev.#3.....: 15332.5 MH/s (43.48ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 3000 - LM
Speed.Dev.#3.....: 8721.5 MH/s (38.34ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS
Speed.Dev.#3.....: 9352.3 MH/s (71.31ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 5600 - NetNTLMv2
Speed.Dev.#3.....: 763.3 MH/s (54.60ms) @ Accel:128 Loops:32 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES
Speed.Dev.#3.....: 374.4 MH/s (55.70ms) @ Accel:8 Loops:1024 Thr:256 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)
Speed.Dev.#3.....: 4145.7 kH/s (38.51ms) @ Accel:1024 Loops:500 Thr:32 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)
Speed.Dev.#3.....: 6855 H/s (22.60ms) @ Accel:16 Loops:4 Thr:8 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)
Speed.Dev.#3.....: 57001 H/s (70.86ms) @ Accel:512 Loops:128 Thr:32 Vec:1

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23
Speed.Dev.#3.....: 130.7 MH/s (40.25ms) @ Accel:128 Loops:64 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23
Speed.Dev.#3.....: 132.5 MH/s (39.59ms) @ Accel:128 Loops:64 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)
Speed.Dev.#3.....: 30018 H/s (57.40ms) @ Accel:128 Loops:32 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 7999)
Speed.Dev.#3.....: 19205 H/s (67.96ms) @ Accel:256 Loops:128 Thr:32 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 35000)
Speed.Dev.#3.....: 5257 H/s (56.53ms) @ Accel:64 Loops:32 Thr:512 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 524288)
Speed.Dev.#3.....: 3801 H/s (62.28ms) @ Accel:256 Loops:64 Thr:768 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)
Speed.Dev.#3.....: 18710 H/s (51.13ms) @ Accel:4 Loops:16384 Thr:384 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32767)
Speed.Dev.#3.....: 15804 H/s (50.04ms) @ Accel:128 Loops:32 Thr:640 Vec:1

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 2000)
Speed.Dev.#3.....: 114.2 kH/s (45.35ms) @ Accel:64 Loops:16 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 6000)
Speed.Dev.#3.....: 62248 H/s (110.44ms) @ Accel:512 Loops:256 Thr:32 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 500)
Speed.Dev.#3.....: 1026.0 kH/s (42.60ms) @ Accel:64 Loops:62 Thr:640 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 199999)
Speed.Dev.#3.....: 1973 H/s (52.66ms) @ Accel:64 Loops:32 Thr:1024 Vec:1
```
