# NVIDIA Quadro RTX 6000

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Quadro RTX 6000
- **Версия hashcat / Version:** v5.1.0
- **Источник / Source:** [clem9669 (gist)](https://gist.github.com/clem9669/e865fceb1babc6ed10b5e2b42e919d2a)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 54595.7 MH/s |
| 100 | SHA1 | 19604.1 MH/s |
| 1400 | SHA2-256 | 8059.7 MH/s |
| 1700 | SHA2-512 | 2603.4 MH/s |
| 1000 | NTLM | 96608.1 MH/s |
| 3200 | bcrypt | 29096 H/s |
| 1800 | sha512crypt | 359.4 kH/s |
| 500 | md5crypt | 23860.4 kH/s |
| 7500 | Kerberos 5 AS-REQ (23) | 760.5 MH/s |
| 13100 | Kerberos 5 TGS-REP (23) | 758.2 MH/s |
| 11300 | Bitcoin/Litecoin wallet.dat | 11782 H/s |
| 6211 | TrueCrypt RIPEMD160 + XTS 512 | 606.6 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
$ hashcat -b 
hashcat (v5.1.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #1: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
OpenCL Platform #1: NVIDIA Corporation
======================================
* Device #1: Quadro RTX 6000, 6055/24220 MB allocatable, 72MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5





Speed.#1.........: 54595.7 MH/s (44.13ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

Hashmode: 100 - SHA1





Speed.#1.........: 19604.1 MH/s (61.47ms) @ Accel:128 Loops:512 Thr:256 Vec:1

Hashmode: 1400 - SHA2-256



Speed.#1.........:  8059.7 MH/s (74.76ms) @ Accel:128 Loops:256 Thr:256 Vec:1

Hashmode: 1700 - SHA2-512



Speed.#1.........:  2603.4 MH/s (57.86ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4096)





Speed.#1.........:   903.1 kH/s (81.25ms) @ Accel:128 Loops:128 Thr:256 Vec:1

Hashmode: 1000 - NTLM



Speed.#1.........: 96608.1 MH/s (24.87ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

Hashmode: 3000 - LM



Speed.#1.........: 50434.7 MH/s (47.74ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS



Speed.#1.........: 55332.4 MH/s (43.47ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

Hashmode: 5600 - NetNTLMv2



Speed.#1.........:  4055.0 MH/s (74.30ms) @ Accel:128 Loops:128 Thr:256 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES



Speed.#1.........:  1988.9 MH/s (75.82ms) @ Accel:8 Loops:1024 Thr:256 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)



Speed.#1.........: 23860.4 kH/s (88.81ms) @ Accel:1024 Loops:1000 Thr:32 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)



Speed.#1.........:    29096 H/s (38.71ms) @ Accel:16 Loops:4 Thr:8 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)



Speed.#1.........:   359.4 kH/s (81.19ms) @ Accel:512 Loops:128 Thr:32 Vec:1

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23



Speed.#1.........:   760.5 MH/s (49.56ms) @ Accel:128 Loops:64 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23



Speed.#1.........:   758.2 MH/s (49.71ms) @ Accel:128 Loops:64 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)



Speed.#1.........:   157.1 kH/s (79.73ms) @ Accel:128 Loops:128 Thr:256 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 7999)



Speed.#1.........:   134.3 kH/s (70.12ms) @ Accel:256 Loops:128 Thr:32 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 35000)



Speed.#1.........:    31903 H/s (67.19ms) @ Accel:128 Loops:32 Thr:256 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 524288)



Speed.#1.........:    21816 H/s (52.56ms) @ Accel:128 Loops:256 Thr:256 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)



Speed.#1.........:    68364 H/s (67.30ms) @ Accel:4 Loops:16384 Thr:256 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32767)



Speed.#1.........:    97349 H/s (94.18ms) @ Accel:128 Loops:128 Thr:256 Vec:1

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 2000)



Speed.#1.........:   606.6 kH/s (51.62ms) @ Accel:128 Loops:32 Thr:256 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 6000)



Speed.#1.........:   236.9 kH/s (106.08ms) @ Accel:512 Loops:128 Thr:32 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 500)



Speed.#1.........:  6023.6 kH/s (40.75ms) @ Accel:128 Loops:62 Thr:256 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 199999)



Speed.#1.........:    11782 H/s (63.80ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Started: Tue Nov 23 12:44:56 2021
Stopped: Tue Nov 23 12:50:30 2021
```
