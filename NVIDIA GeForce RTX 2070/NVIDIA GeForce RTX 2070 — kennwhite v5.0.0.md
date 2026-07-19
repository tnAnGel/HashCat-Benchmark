# NVIDIA GeForce RTX 2070

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 2070
- **Версия hashcat / Version:** v5.0.0
- **Источник / Source:** [kennwhite](https://gist.github.com/kennwhite/caf3a861325122f5ff8ba58e7210c63d)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 26928.4 MH/s |
| 100 | SHA1 | 8944.0 MH/s |
| 1400 | SHA2-256 | 4030.6 MH/s |
| 1700 | SHA2-512 | 1310.3 MH/s |
| 1000 | NTLM | 39964.4 MH/s |
| 3200 | bcrypt | 14274 H/s |
| 1800 | sha512crypt | 192.2 kH/s |
| 500 | md5crypt | 12179.7 kH/s |
| 2500 | WPA/WPA2 (legacy) | 422.0 kH/s |
| 7500 | Kerberos AS-REQ (23) | 346.2 MH/s |
| 13100 | Kerberos TGS-REP (23) | 338.9 MH/s |
| 11300 | Bitcoin wallet.dat | 5950 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 323.4 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.0.0) starting in benchmark mode...

* Device #1: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
OpenCL Platform #1: NVIDIA Corporation
======================================
* Device #1: GeForce RTX 2070, 2048/8192 MB allocatable, 36MCU

OpenCL Platform #2: Intel(R) Corporation
========================================
* Device #2: Intel(R) Core(TM) i7-6700K CPU @ 4.00GHz, skipped.

Benchmark relevant options:
===========================
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 26928.4 MH/s (88.56ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........:  8944.0 MH/s (268.17ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  4030.6 MH/s (297.60ms) @ Accel:256 Loops:512 Thr:256 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1310.3 MH/s (458.34ms) @ Accel:256 Loops:256 Thr:256 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4096)

Speed.#1.........:   422.0 kH/s (346.99ms) @ Accel:256 Loops:256 Thr:256 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 39964.4 MH/s (59.21ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 23951.2 MH/s (99.27ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 23203.5 MH/s (102.90ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  2045.4 MH/s (293.12ms) @ Accel:256 Loops:256 Thr:256 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:   951.2 MH/s (315.83ms) @ Accel:32 Loops:1024 Thr:256 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 12179.7 kH/s (87.06ms) @ Accel:1024 Loops:1000 Thr:32 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    14274 H/s (156.57ms) @ Accel:32 Loops:8 Thr:8 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   192.2 kH/s (308.66ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.#1.........:   346.2 MH/s (434.38ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23

Speed.#1.........:   338.9 MH/s (438.76ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    73017 H/s (339.78ms) @ Accel:256 Loops:256 Thr:256 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 7999)

Speed.#1.........:    65638 H/s (285.73ms) @ Accel:512 Loops:256 Thr:32 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 35000)

Speed.#1.........:    15781 H/s (270.10ms) @ Accel:256 Loops:64 Thr:256 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 524288)

Speed.#1.........:    11711 H/s (390.85ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    47450 H/s (387.41ms) @ Accel:32 Loops:16384 Thr:256 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32767)

Speed.#1.........:    49470 H/s (369.09ms) @ Accel:256 Loops:256 Thr:256 Vec:1

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 2000)

Speed.#1.........:   323.4 kH/s (459.82ms) @ Accel:256 Loops:128 Thr:256 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 6000)

Speed.#1.........:   116.2 kH/s (863.56ms) @ Accel:1024 Loops:512 Thr:32 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 500)

Speed.#1.........:  3074.8 kH/s (359.66ms) @ Accel:256 Loops:250 Thr:256 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 199999)

Speed.#1.........:     5950 H/s (251.12ms) @ Accel:256 Loops:128 Thr:256 Vec:1

Started: Thu Nov 22 22:21:52 2018
Stopped: Thu Nov 22 22:26:50 2018

C:\HashcatGUI_050b1\hashcat-5.0.0>
```
