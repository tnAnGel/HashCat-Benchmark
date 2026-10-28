# AMD Ryzen Threadripper 3970X

- **Вендор / Vendor:** AMD
- **Процессор / CPU:** AMD Ryzen Threadripper 3970X 32-Core Processor
- **Версия hashcat / Version:** v6.0.0
- **Бэкенд / Backend:** OpenCL API (OpenCL 2.1 WINDOWS) — `[Intel(R) Corporation]` runtime, устройство `AMD Ryzen Threadripper 3970X 32-Core Processor` (Device #1, 64MCU), `--opencl-device-types=1`
- **Источник / Source:** [Sondero, hashcat.net forum, thread «Ryzen 9 3900X vs Core i9-9900K»](https://hashcat.net/forum/thread-9254.html)
- **Примечание / Note:** Чистый прогон только на CPU (Device #1). Замеры получены через Intel OpenCL CPU runtime на Windows. Стандартный `hashcat -b`.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 5384.9 MH/s |
| 100 | SHA1 | 2598.2 MH/s |
| 1400 | SHA2-256 | 983.5 MH/s |
| 1700 | SHA2-512 | 294.1 MH/s |
| 1000 | NTLM | 9552.0 MH/s |
| 3200 | bcrypt | 40807 H/s |
| 1800 | sha512crypt | 29859 H/s |
| 500 | md5crypt | 495.2 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 132.6 kH/s |
| 7500 | Kerberos AS-REQ (23) | 47894.3 kH/s |
| 13100 | Kerberos TGS-REP (23) | 49258.4 kH/s |
| 11300 | Bitcoin/Litecoin wallet.dat | 1474 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 93633 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.0.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL API (OpenCL 2.1 WINDOWS) - Platform #1 [Intel(R) Corporation]
====================================================================
* Device #1: AMD Ryzen Threadripper 3970X 32-Core Processor, 65343/65407 MB (16351 MB allocatable), 64MCU

Benchmark relevant options:
===========================
* --opencl-device-types=1
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........:  5384.9 MH/s (12.32ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 100 - SHA1

Speed.#1.........:  2598.2 MH/s (25.72ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 1400 - SHA2-256

Speed.#1.........:  983.5 MH/s (68.07ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 1700 - SHA2-512

Speed.#1.........:  294.1 MH/s (56.93ms) @ Accel:1024 Loops:256 Thr:1 Vec:4

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:  132.6 kH/s (61.34ms) @ Accel:512 Loops:1024 Thr:1 Vec:8

Hashmode: 1000 - NTLM

Speed.#1.........:  9552.0 MH/s (6.93ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 3000 - LM

Speed.#1.........:  1222.2 MH/s (54.57ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........:  6371.2 MH/s (10.43ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  437.3 MH/s (76.60ms) @ Accel:512 Loops:1024 Thr:1 Vec:8

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........: 56771.9 kH/s (73.60ms) @ Accel:64 Loops:1024 Thr:1 Vec:8

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........:  495.2 kH/s (64.79ms) @ Accel:512 Loops:1000 Thr:1 Vec:8

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    40807 H/s (97.42ms) @ Accel:64 Loops:32 Thr:1 Vec:8

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:    29859 H/s (54.57ms) @ Accel:256 Loops:512 Thr:1 Vec:4

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........: 47894.3 kH/s (87.46ms) @ Accel:4 Loops:256 Thr:64 Vec:8

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........: 49258.4 kH/s (85.03ms) @ Accel:2 Loops:512 Thr:64 Vec:8

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    22554 H/s (60.28ms) @ Accel:512 Loops:1024 Thr:1 Vec:8

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    11239 H/s (57.02ms) @ Accel:512 Loops:256 Thr:1 Vec:4

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:  140.3 kH/s (38.43ms) @ Accel:256 Loops:511 Thr:1 Vec:4

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:    32554 H/s (57.88ms) @ Accel:128 Loops:4096 Thr:1 Vec:8

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    4776 H/s (53.52ms) @ Accel:64 Loops:16384 Thr:1 Vec:8

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    11359 H/s (89.96ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:    93633 H/s (86.38ms) @ Accel:1024 Loops:256 Thr:1 Vec:8

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    12281 H/s (55.49ms) @ Accel:512 Loops:512 Thr:1 Vec:8

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  720.4 kH/s (86.96ms) @ Accel:1024 Loops:499 Thr:1 Vec:8

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:    1474 H/s (56.70ms) @ Accel:1024 Loops:256 Thr:1 Vec:4

Started: Sat Jun 20 17:42:35 2020
Stopped: Sat Jun 20 17:46:08 2020
```
