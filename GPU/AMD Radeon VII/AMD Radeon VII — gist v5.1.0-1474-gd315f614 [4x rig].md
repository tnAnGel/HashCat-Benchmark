# AMD Radeon VII (4x rig)

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon VII
- **Конфигурация / Setup:** 4x rig
- **Версия hashcat / Version:** v5.1.0-1474-gd315f614
- **Источник / Source:** [gist](https://gist.github.com/54340280d81528dcb024ef5df2535c86)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 131.8 GH/s |
| 100 | SHA1 | 45841.7 MH/s |
| 1400 | SHA2-256 | 19699.3 MH/s |
| 1700 | SHA2-512 | 5884.9 MH/s |
| 1000 | NTLM | 218.8 GH/s |
| 3200 | bcrypt | 96557 H/s |
| 1800 | sha512crypt | 841.8 kH/s |
| 500 | md5crypt | 49530.1 kH/s |
| 2500 | WPA/WPA2 (legacy) | 2189.9 kH/s |
| 7500 | Kerberos AS-REQ (23) | 1368.8 MH/s |
| 13100 | Kerberos TGS-REP (23) | 1351.4 MH/s |
| 11300 | Bitcoin wallet.dat | 25189 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 1699.7 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.1.0-1474-gd315f614) starting in benchmark mode...

OpenCL API (OpenCL 2.1 AMD-APP (3019.0)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: gfx906+sram-ecc, 16256/16368 MB (13912 MB allocatable), 60MCU
* Device #2: gfx906+sram-ecc, 16256/16368 MB (13912 MB allocatable), 60MCU
* Device #3: gfx906+sram-ecc, 16256/16368 MB (13912 MB allocatable), 60MCU
* Device #4: gfx906+sram-ecc, 16256/16368 MB (13912 MB allocatable), 60MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable
* --workload-profile=3

Hashmode: 0 - MD5

Speed.#1.........: 33117.2 MH/s (60.37ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
Speed.#2.........: 32984.0 MH/s (60.78ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
Speed.#3.........: 32784.1 MH/s (61.16ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
Speed.#4.........: 32923.4 MH/s (60.87ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   131.8 GH/s

Hashmode: 100 - SHA1

Speed.#1.........: 11405.0 MH/s (87.79ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#2.........: 11567.6 MH/s (86.81ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#3.........: 11467.4 MH/s (87.52ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#4.........: 11401.7 MH/s (87.66ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#*.........: 45841.7 MH/s

Hashmode: 1400 - SHA2-256

Speed.#1.........:  4897.5 MH/s (51.07ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#2.........:  4963.7 MH/s (50.28ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#3.........:  4933.2 MH/s (50.76ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#4.........:  4904.8 MH/s (51.10ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#*.........: 19699.3 MH/s

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1450.2 MH/s (86.52ms) @ Accel:16 Loops:512 Thr:256 Vec:1
Speed.#2.........:  1491.5 MH/s (84.12ms) @ Accel:16 Loops:512 Thr:256 Vec:1
Speed.#3.........:  1480.6 MH/s (84.72ms) @ Accel:16 Loops:512 Thr:256 Vec:1
Speed.#4.........:  1462.6 MH/s (85.81ms) @ Accel:16 Loops:512 Thr:256 Vec:1
Speed.#*.........:  5884.9 MH/s

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#1.........:   542.2 kH/s (56.35ms) @ Accel:16 Loops:512 Thr:256 Vec:1
Speed.#2.........:   554.7 kH/s (55.09ms) @ Accel:16 Loops:512 Thr:256 Vec:1
Speed.#3.........:   549.1 kH/s (55.74ms) @ Accel:16 Loops:512 Thr:256 Vec:1
Speed.#4.........:   543.9 kH/s (56.18ms) @ Accel:16 Loops:512 Thr:256 Vec:1
Speed.#*.........:  2189.9 kH/s

Hashmode: 1000 - NTLM

Speed.#1.........: 54900.1 MH/s (73.10ms) @ Accel:256 Loops:1024 Thr:256 Vec:1
Speed.#2.........: 54543.2 MH/s (73.59ms) @ Accel:256 Loops:1024 Thr:256 Vec:1
Speed.#3.........: 54452.1 MH/s (73.70ms) @ Accel:256 Loops:1024 Thr:256 Vec:1
Speed.#4.........: 54949.2 MH/s (73.04ms) @ Accel:256 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   218.8 GH/s

Hashmode: 3000 - LM

Speed.#1.........: 28503.5 MH/s (70.32ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 29106.2 MH/s (68.85ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 29125.6 MH/s (68.81ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 28887.6 MH/s (69.36ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   115.6 GH/s

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 33719.4 MH/s (59.41ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
Speed.#2.........: 33302.3 MH/s (60.21ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
Speed.#3.........: 33111.2 MH/s (60.36ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
Speed.#4.........: 33651.8 MH/s (59.58ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   133.8 GH/s

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  2337.2 MH/s (53.59ms) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#2.........:  2345.0 MH/s (53.39ms) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#3.........:  2339.7 MH/s (53.52ms) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#4.........:  2353.6 MH/s (53.26ms) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#*.........:  9375.6 MH/s

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1079.0 MH/s (57.98ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  1110.7 MH/s (56.28ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  1103.2 MH/s (56.65ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  1091.3 MH/s (57.26ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  4384.1 MH/s

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 12441.2 kH/s (77.42ms) @ Accel:128 Loops:500 Thr:256 Vec:1
Speed.#2.........: 12333.3 kH/s (78.17ms) @ Accel:128 Loops:500 Thr:256 Vec:1
Speed.#3.........: 12283.0 kH/s (78.46ms) @ Accel:128 Loops:500 Thr:256 Vec:1
Speed.#4.........: 12472.6 kH/s (77.29ms) @ Accel:128 Loops:500 Thr:256 Vec:1
Speed.#*.........: 49530.1 kH/s

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    24133 H/s (38.28ms) @ Accel:1 Loops:32 Thr:16 Vec:1
Speed.#2.........:    24148 H/s (38.28ms) @ Accel:1 Loops:32 Thr:16 Vec:1
Speed.#3.........:    24173 H/s (38.28ms) @ Accel:1 Loops:32 Thr:16 Vec:1
Speed.#4.........:    24103 H/s (38.28ms) @ Accel:1 Loops:32 Thr:16 Vec:1
Speed.#*.........:    96557 H/s

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   212.9 kH/s (55.51ms) @ Accel:16 Loops:256 Thr:256 Vec:1
Speed.#2.........:   220.8 kH/s (53.54ms) @ Accel:16 Loops:256 Thr:256 Vec:1
Speed.#3.........:   207.3 kH/s (54.04ms) @ Accel:16 Loops:256 Thr:256 Vec:1
Speed.#4.........:   200.7 kH/s (54.63ms) @ Accel:16 Loops:256 Thr:256 Vec:1
Speed.#*.........:   841.8 kH/s

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   343.5 MH/s (91.16ms) @ Accel:256 Loops:32 Thr:64 Vec:1
Speed.#2.........:   342.9 MH/s (91.51ms) @ Accel:256 Loops:32 Thr:64 Vec:1
Speed.#3.........:   341.2 MH/s (91.93ms) @ Accel:256 Loops:32 Thr:64 Vec:1
Speed.#4.........:   341.3 MH/s (91.92ms) @ Accel:256 Loops:32 Thr:64 Vec:1
Speed.#*.........:  1368.8 MH/s

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   339.3 MH/s (92.48ms) @ Accel:256 Loops:32 Thr:64 Vec:1
Speed.#2.........:   338.3 MH/s (92.73ms) @ Accel:256 Loops:32 Thr:64 Vec:1
Speed.#3.........:   336.7 MH/s (93.17ms) @ Accel:256 Loops:32 Thr:64 Vec:1
Speed.#4.........:   337.2 MH/s (93.06ms) @ Accel:256 Loops:32 Thr:64 Vec:1
Speed.#*.........:  1351.4 MH/s

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    94871 H/s (53.64ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#2.........:    98012 H/s (51.97ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#3.........:    97281 H/s (52.38ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#4.........:    96289 H/s (52.89ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   386.5 kH/s

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    34219 H/s (68.69ms) @ Accel:4 Loops:512 Thr:256 Vec:1
Speed.#2.........:    34113 H/s (68.98ms) @ Accel:4 Loops:512 Thr:256 Vec:1
Speed.#3.........:    33949 H/s (69.01ms) @ Accel:4 Loops:512 Thr:256 Vec:1
Speed.#4.........:    34193 H/s (68.69ms) @ Accel:4 Loops:512 Thr:256 Vec:1
Speed.#*.........:   136.5 kH/s

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   592.2 kH/s (96.54ms) @ Accel:64 Loops:63 Thr:256 Vec:1
Speed.#2.........:   610.3 kH/s (93.62ms) @ Accel:64 Loops:63 Thr:256 Vec:1
Speed.#3.........:   604.7 kH/s (94.43ms) @ Accel:64 Loops:63 Thr:256 Vec:1
Speed.#4.........:   599.0 kH/s (95.26ms) @ Accel:64 Loops:63 Thr:256 Vec:1
Speed.#*.........:  2406.2 kH/s

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   426.1 kH/s (62.20ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#2.........:   417.6 kH/s (63.33ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#3.........:   416.4 kH/s (63.93ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#4.........:   418.9 kH/s (63.50ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  1679.0 kH/s

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    63567 H/s (51.76ms) @ Accel:4 Loops:16384 Thr:256 Vec:1
Speed.#2.........:    70395 H/s (50.68ms) @ Accel:4 Loops:16384 Thr:256 Vec:1
Speed.#3.........:    67208 H/s (50.68ms) @ Accel:4 Loops:16384 Thr:256 Vec:1
Speed.#4.........:    61072 H/s (50.45ms) @ Accel:4 Loops:16384 Thr:256 Vec:1
Speed.#*.........:   262.2 kH/s

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    63305 H/s (58.65ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#2.........:    65270 H/s (56.90ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#3.........:    64910 H/s (57.22ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#4.........:    64394 H/s (57.70ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   257.9 kH/s

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   417.4 kH/s (72.19ms) @ Accel:16 Loops:256 Thr:256 Vec:1
Speed.#2.........:   430.5 kH/s (69.98ms) @ Accel:16 Loops:256 Thr:256 Vec:1
Speed.#3.........:   427.5 kH/s (70.55ms) @ Accel:16 Loops:256 Thr:256 Vec:1
Speed.#4.........:   424.3 kH/s (71.06ms) @ Accel:16 Loops:256 Thr:256 Vec:1
Speed.#*.........:  1699.7 kH/s

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    97835 H/s (104.41ms) @ Accel:256 Loops:64 Thr:256 Vec:1
Speed.#2.........:    96819 H/s (105.48ms) @ Accel:256 Loops:64 Thr:256 Vec:1
Speed.#3.........:    96364 H/s (106.01ms) @ Accel:256 Loops:64 Thr:256 Vec:1
Speed.#4.........:    97761 H/s (104.49ms) @ Accel:256 Loops:64 Thr:256 Vec:1
Speed.#*.........:   388.8 kH/s

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  4079.3 kH/s (46.93ms) @ Accel:64 Loops:124 Thr:256 Vec:1
Speed.#2.........:  4190.4 kH/s (45.69ms) @ Accel:64 Loops:124 Thr:256 Vec:1
Speed.#3.........:  4170.5 kH/s (45.90ms) @ Accel:64 Loops:124 Thr:256 Vec:1
Speed.#4.........:  4140.6 kH/s (46.22ms) @ Accel:64 Loops:124 Thr:256 Vec:1
Speed.#*.........: 16580.8 kH/s

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     6228 H/s (100.57ms) @ Accel:32 Loops:256 Thr:256 Vec:1
Speed.#2.........:     6393 H/s (97.98ms) @ Accel:32 Loops:256 Thr:256 Vec:1
Speed.#3.........:     6312 H/s (99.24ms) @ Accel:32 Loops:256 Thr:256 Vec:1
Speed.#4.........:     6256 H/s (100.14ms) @ Accel:32 Loops:256 Thr:256 Vec:1
Speed.#*.........:    25189 H/s

Started: Wed Dec  4 00:48:10 2019
Stopped: Wed Dec  4 00:56:03 2019
```
