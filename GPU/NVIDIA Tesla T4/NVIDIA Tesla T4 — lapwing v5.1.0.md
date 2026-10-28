# NVIDIA Tesla T4

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Tesla T4
- **Версия hashcat / Version:** v5.1.0
- **Источник / Source:** [lapwing](https://hashcat.net/forum/thread-7990.html)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 21196.7 MH/s |
| 100 | SHA1 | 7063.7 MH/s |
| 1400 | SHA2-256 | 3194.4 MH/s |
| 1700 | SHA2-512 | 1040.9 MH/s |
| 1000 | NTLM | 32286.0 MH/s |
| 3200 | bcrypt | 13413 H/s |
| 1800 | sha512crypt | 126.1 kH/s |
| 500 | md5crypt | 9681.2 kH/s |
| 7500 | Kerberos AS-REQ (23) | 305.9 MH/s |
| 13100 | Kerberos TGS-REP (23) | 304.2 MH/s |
| 11300 | Bitcoin wallet.dat | 4804 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 237.1 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.1.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

nvmlDeviceGetFanSpeed(): Not Supported

OpenCL Platform #1: NVIDIA Corporation
======================================
* Device #1: Tesla T4, 3769/15079 MB allocatable, 40MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........: 21196.7 MH/s (62.95ms) @ Accel:256 Loops:512 Thr:256 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........:  7063.7 MH/s (94.48ms) @ Accel:256 Loops:256 Thr:256 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  3194.4 MH/s (52.20ms) @ Accel:256 Loops:64 Thr:256 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1040.9 MH/s (80.33ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4096)

Speed.#1.........:   326.4 kH/s (62.45ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 32286.0 MH/s (82.69ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 18820.5 MH/s (71.03ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 18596.2 MH/s (71.77ms) @ Accel:256 Loops:512 Thr:256 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  1603.0 MH/s (52.14ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:   796.0 MH/s (52.59ms) @ Accel:4 Loops:1024 Thr:256 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........:  9681.2 kH/s (60.36ms) @ Accel:1024 Loops:500 Thr:32 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    13413 H/s (23.21ms) @ Accel:8 Loops:4 Thr:8 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   126.1 kH/s (64.38ms) @ Accel:256 Loops:128 Thr:32 Vec:1

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.#1.........:   305.9 MH/s (68.46ms) @ Accel:128 Loops:64 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23

Speed.#1.........:   304.2 MH/s (68.83ms) @ Accel:128 Loops:64 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    58891 H/s (58.98ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 7999)

Speed.#1.........:    56566 H/s (92.37ms) @ Accel:256 Loops:128 Thr:32 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 35000)

Speed.#1.........:    12184 H/s (97.50ms) @ Accel:128 Loops:32 Thr:256 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 524288)

Speed.#1.........:     9336 H/s (67.98ms) @ Accel:256 Loops:128 Thr:256 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    31390 H/s (81.44ms) @ Accel:4 Loops:16384 Thr:256 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32767)

Speed.#1.........:    38290 H/s (66.23ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 2000)

Speed.#1.........:   237.1 kH/s (86.66ms) @ Accel:128 Loops:32 Thr:256 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 6000)

Speed.#1.........:   107.0 kH/s (130.45ms) @ Accel:512 Loops:128 Thr:32 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 500)

Speed.#1.........:  2453.1 kH/s (55.24ms) @ Accel:128 Loops:62 Thr:256 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 199999)

Speed.#1.........:     4804 H/s (86.79ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Started: Wed Dec  5 12:53:33 2018
Stopped: Wed Dec  5 12:58:06 2018
```
