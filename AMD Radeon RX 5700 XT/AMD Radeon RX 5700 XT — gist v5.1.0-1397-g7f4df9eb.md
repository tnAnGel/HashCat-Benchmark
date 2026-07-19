# AMD Radeon RX 5700 XT

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 5700 XT
- **Версия hashcat / Version:** v5.1.0-1397-g7f4df9eb
- **Источник / Source:** [gist](https://gist.github.com/1225705081391ba8dd3e0f88c004fae6)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 23790.3 MH/s |
| 100 | SHA1 | 9606.5 MH/s |
| 1400 | SHA2-256 | 4052.3 MH/s |
| 1700 | SHA2-512 | 1145.4 MH/s |
| 1000 | NTLM | 38095.7 MH/s |
| 3200 | bcrypt | 18167 H/s |
| 1800 | sha512crypt | 114.7 kH/s |
| 500 | md5crypt | 8992.2 kH/s |
| 2500 | WPA/WPA2 (legacy) | 468.2 kH/s |
| 7500 | Kerberos AS-REQ (23) | 363.7 MH/s |
| 13100 | Kerberos TGS-REP (23) | 387.7 MH/s |
| 11300 | Bitcoin wallet.dat | 5177 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 308.7 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.1.0-1397-g7f4df9eb) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

/sys/bus/pci/devices/0000:23:00.0/hwmon/hwmon0/temp1_input: unexpected data.

OpenCL API (OpenCL 2.1 AMD-APP (2906.7)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: gfx1010, 4048/8176 MB allocatable, 20MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........: 23790.3 MH/s (55.86ms) @ Accel:512 Loops:512 Thr:256 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........:  9606.5 MH/s (69.24ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  4052.3 MH/s (82.13ms) @ Accel:256 Loops:256 Thr:256 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1145.4 MH/s (72.58ms) @ Accel:128 Loops:128 Thr:256 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#1.........:   468.2 kH/s (86.81ms) @ Accel:64 Loops:512 Thr:256 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 38095.7 MH/s (69.84ms) @ Accel:512 Loops:1024 Thr:256 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 22744.9 MH/s (58.24ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 25598.3 MH/s (51.83ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  1455.6 MH/s (57.06ms) @ Accel:16 Loops:1024 Thr:256 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:   876.2 MH/s (94.91ms) @ Accel:16 Loops:1024 Thr:256 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........:  8992.2 kH/s (69.33ms) @ Accel:256 Loops:500 Thr:256 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    18167 H/s (34.03ms) @ Accel:16 Loops:4 Thr:16 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   114.7 kH/s (71.73ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   363.7 MH/s (57.06ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   387.7 MH/s (53.51ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    79615 H/s (87.23ms) @ Accel:128 Loops:256 Thr:256 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    33318 H/s (48.35ms) @ Accel:32 Loops:128 Thr:256 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   488.3 kH/s (81.70ms) @ Accel:8 Loops:1023 Thr:256 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   355.8 kH/s (50.97ms) @ Accel:128 Loops:512 Thr:256 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    43585 H/s (58.31ms) @ Accel:8 Loops:16384 Thr:256 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    51218 H/s (96.43ms) @ Accel:32 Loops:1024 Thr:256 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   308.7 kH/s (64.81ms) @ Accel:32 Loops:256 Thr:256 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    42056 H/s (161.84ms) @ Accel:32 Loops:1024 Thr:256 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  3211.7 kH/s (78.02ms) @ Accel:256 Loops:124 Thr:256 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     5177 H/s (80.37ms) @ Accel:16 Loops:1024 Thr:256 Vec:1

Started: Mon Sep 16 12:02:19 2019
Stopped: Mon Sep 16 12:07:23 2019
```
