# AMD Radeon Pro 5500M

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon Pro 5500M (Compute Engine, MacBook Pro 16" i9-9880H, macOS OpenCL)
- **Версия hashcat / Version:** v5.1.0
- **Источник / Source:** [bryanroma](https://gist.github.com/bryanroma/3709dd4910bac2d982d7d016f67b5950)
- **Примечание / Note:** прогон `sudo hashcat -b --force` — многокарточный (Device #2 — Intel UHD Graphics 630 iGPU, Device #3 — Radeon Pro 5500M); в таблице ниже используются только строки `Speed.#3` (5500M). На macOS OpenCL ряд режимов отработал с предупреждением «OpenCL kernel self-test failed» (числа при этом получены). В отличие от существующего прогона Azunyan1111, здесь **bcrypt (3200) собрался и дал число** (10671 H/s), а прогон дошёл до конца (Bitcoin 11300 = 1205 H/s, есть Started/Stopped). Тот же короткий набор режимов v5.1.0, но на один режим (bcrypt) полнее и без обрыва.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 9210.3 MH/s |
| 100 | SHA1 | 3690.3 MH/s |
| 1400 | SHA2-256 | 1478.8 MH/s |
| 1700 | SHA2-512 | 255.7 MH/s (self-test failed) |
| 1000 | NTLM | 14869.4 MH/s |
| 3200 | bcrypt | 10671 H/s (self-test failed) |
| 1800 | sha512crypt | 36445 H/s (self-test failed) |
| 500 | md5crypt | 3741.6 kH/s |
| 2500 | WPA-EAPOL-PBKDF2 | 79477 H/s |
| 7500 | Kerberos AS-REQ (23) | 124.3 MH/s |
| 13100 | Kerberos TGS-REP (23) | 87659.9 kH/s |
| 11300 | Bitcoin wallet.dat | 1205 H/s (self-test failed) |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 109.8 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
# Keep in mind that macOS is moving from opencl to metal. So there is a bug https://github.com/hashcat/hashcat/issues/1847
# Device:  MacBook Pro 16" i9-9880H, 32GB RAM,5500M 4GB

└─[$] <> sudo hashcat -b --force
Password:
hashcat (v5.1.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL Platform #1: Apple
=========================
* Device #1: Intel(R) Core(TM) i9-9880H CPU @ 2.30GHz, skipped.
* Device #2: Intel(R) UHD Graphics 630, 384/1536 MB allocatable, 24MCU
* Device #3: AMD Radeon Pro 5500M Compute Engine, 1020/4080 MB allocatable, 24MCU

Benchmark relevant options:
===========================
* --force
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#2.........:   531.3 MH/s (45.34ms) @ Accel:128 Loops:32 Thr:256 Vec:1
Speed.#3.........:  9210.3 MH/s (86.29ms) @ Accel:256 Loops:512 Thr:256 Vec:1
Speed.#*.........:  9741.6 MH/s

Hashmode: 100 - SHA1

Speed.#2.........:   197.7 MH/s (62.02ms) @ Accel:64 Loops:32 Thr:256 Vec:1
Speed.#3.........:  3690.3 MH/s (53.52ms) @ Accel:256 Loops:128 Thr:256 Vec:1
Speed.#*.........:  3888.0 MH/s

Hashmode: 1400 - SHA2-256

Speed.#2.........: 80925.9 kH/s (75.96ms) @ Accel:64 Loops:16 Thr:256 Vec:1
Speed.#3.........:  1478.8 MH/s (66.98ms) @ Accel:256 Loops:64 Thr:256 Vec:1
Speed.#*.........:  1559.7 MH/s

Hashmode: 1700 - SHA2-512

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#2.........: 12733.8 kH/s (60.63ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#3.........:   255.7 MH/s (97.60ms) @ Accel:128 Loops:32 Thr:256 Vec:1
Speed.#*.........:   268.4 MH/s

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4096)

Speed.#2.........:     8157 H/s (92.27ms) @ Accel:32 Loops:16 Thr:256 Vec:1
Speed.#3.........:    79477 H/s (76.12ms) @ Accel:128 Loops:32 Thr:256 Vec:1
Speed.#*.........:    87635 H/s

Hashmode: 1000 - NTLM

Speed.#2.........:   903.5 MH/s (54.07ms) @ Accel:128 Loops:64 Thr:256 Vec:1
Speed.#3.........: 14869.4 MH/s (53.02ms) @ Accel:256 Loops:512 Thr:256 Vec:1
Speed.#*.........: 15772.9 MH/s

Hashmode: 3000 - LM

Speed.#2.........:   347.7 MH/s (70.53ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  7893.2 MH/s (49.85ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  8240.9 MH/s

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#2.........:   282.8 MH/s (86.86ms) @ Accel:128 Loops:32 Thr:256 Vec:1
Speed.#3.........:  8852.9 MH/s (89.48ms) @ Accel:256 Loops:512 Thr:256 Vec:1
Speed.#*.........:  9135.7 MH/s

Hashmode: 5600 - NetNTLMv2

Speed.#2.........: 43340.3 kH/s (71.14ms) @ Accel:32 Loops:16 Thr:256 Vec:1
Speed.#3.........:   583.0 MH/s (84.87ms) @ Accel:128 Loops:64 Thr:256 Vec:1
Speed.#*.........:   626.4 MH/s

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#2.........: 17477.6 kH/s (356.56ms) @ Accel:1 Loops:1024 Thr:256 Vec:1
Speed.#3.........:   310.1 MH/s (79.90ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   327.6 MH/s

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#2.........:   238.3 kH/s (49.57ms) @ Accel:256 Loops:125 Thr:16 Vec:1
Speed.#3.........:  3741.6 kH/s (47.44ms) @ Accel:512 Loops:500 Thr:32 Vec:1
Speed.#*.........:  3979.9 kH/s

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#2.........:      595 H/s (78.11ms) @ Accel:4 Loops:2 Thr:8 Vec:1
Speed.#3.........:    10671 H/s (69.43ms) @ Accel:16 Loops:8 Thr:8 Vec:1
Speed.#*.........:    11266 H/s

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#2.........:     2284 H/s (67.24ms) @ Accel:128 Loops:32 Thr:8 Vec:1
Speed.#3.........:    36445 H/s (67.33ms) @ Accel:256 Loops:64 Thr:32 Vec:1
Speed.#*.........:    38729 H/s

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.#2.........:  3582.4 kH/s (53.60ms) @ Accel:16 Loops:8 Thr:64 Vec:1
Speed.#3.........:   124.3 MH/s (49.84ms) @ Accel:128 Loops:32 Thr:64 Vec:1
Speed.#*.........:   127.8 MH/s

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23

Speed.#2.........:  4148.7 kH/s (93.19ms) @ Accel:32 Loops:8 Thr:64 Vec:1
Speed.#3.........: 87659.9 kH/s (50.77ms) @ Accel:128 Loops:32 Thr:64 Vec:1
Speed.#*.........: 91808.6 kH/s

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#2.........:     1390 H/s (91.97ms) @ Accel:32 Loops:16 Thr:256 Vec:1
Speed.#3.........:    14025 H/s (73.62ms) @ Accel:128 Loops:32 Thr:256 Vec:1
Speed.#*.........:    15415 H/s

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 7999)

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#2.........:      770 H/s (62.90ms) @ Accel:64 Loops:32 Thr:8 Vec:1
Speed.#3.........:    13483 H/s (57.79ms) @ Accel:128 Loops:64 Thr:32 Vec:1
Speed.#*.........:    14253 H/s

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 35000)

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#2.........:      175 H/s (62.60ms) @ Accel:16 Loops:4 Thr:256 Vec:1
Speed.#3.........:     2833 H/s (62.41ms) @ Accel:64 Loops:16 Thr:256 Vec:1
Speed.#*.........:     3008 H/s

Hashmode: 11600 - 7-Zip (Iterations: 524288)

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#2.........:      246 H/s (95.72ms) @ Accel:64 Loops:32 Thr:256 Vec:1
Speed.#3.........:     4158 H/s (91.39ms) @ Accel:256 Loops:128 Thr:256 Vec:1
Speed.#*.........:     4404 H/s

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#2.........:     1309 H/s (291.43ms) @ Accel:1 Loops:16384 Thr:256 Vec:1
Speed.#3.........:    17374 H/s (85.22ms) @ Accel:4 Loops:16384 Thr:256 Vec:1
Speed.#*.........:    18684 H/s

Hashmode: 13000 - RAR5 (Iterations: 32767)

Speed.#2.........:      856 H/s (54.85ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#3.........:    16590 H/s (91.51ms) @ Accel:128 Loops:64 Thr:256 Vec:1
Speed.#*.........:    17446 H/s

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 2000)

Speed.#2.........:     5833 H/s (65.91ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#3.........:   109.8 kH/s (52.93ms) @ Accel:64 Loops:32 Thr:256 Vec:1
Speed.#*.........:   115.6 kH/s

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 6000)

Speed.#2.........:     2353 H/s (110.32ms) @ Accel:128 Loops:32 Thr:16 Vec:1
Speed.#3.........:   124.7 kH/s (65.05ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#*.........:   127.0 kH/s

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 500)

Speed.#2.........:    55356 H/s (50.00ms) @ Accel:16 Loops:15 Thr:256 Vec:1
Speed.#3.........:  1034.2 kH/s (79.82ms) @ Accel:128 Loops:62 Thr:256 Vec:1
Speed.#*.........:  1089.6 kH/s

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 199999)

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#2.........:       63 H/s (60.82ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#3.........:     1205 H/s (51.08ms) @ Accel:64 Loops:32 Thr:256 Vec:1
Speed.#*.........:     1268 H/s

Started: Thu Apr  9 14:40:14 2020
Stopped: Thu Apr  9 14:46:38 2020
```
