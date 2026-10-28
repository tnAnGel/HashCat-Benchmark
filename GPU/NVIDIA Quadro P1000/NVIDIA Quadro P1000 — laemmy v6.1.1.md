# NVIDIA Quadro P1000

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** Quadro P1000 (3996/4039 MB, 5MCU, CUDA 11.4)
- **Версия hashcat / Version:** v6.1.1
- **Источник / Source:** [laemmy](https://gist.github.com/laemmy/baebc8f4d4c016998ec7004ede81ba42)
- **Примечание / Note:** прогон с `--optimized-kernel-enable` (оптимизированные ядра). Устройство #1 (CUDA); OpenCL-дубль и CPU пропущены.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 4803.1 MH/s |
| 100 | SHA1 | 1903.8 MH/s |
| 1400 | SHA2-256 | 692.7 MH/s |
| 1700 | SHA2-512 | 202.4 MH/s |
| 1000 | NTLM | 7827.1 MH/s |
| 3200 | bcrypt | 4562 H/s |
| 1800 | sha512crypt | 34993 H/s |
| 500 | md5crypt | 2201.5 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 98414 H/s |
| 7500 | Kerberos AS-REQ (23) | 63924.7 kH/s |
| 13100 | Kerberos TGS-REP (23) | 63236.6 kH/s |
| 11300 | Bitcoin wallet.dat | 1071 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 61583 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.1.1) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

CUDA API (CUDA 11.4)
====================
* Device #1: Quadro P1000, 3996/4039 MB, 5MCU

OpenCL API (OpenCL 3.0 CUDA 11.4.94) - Platform #1 [NVIDIA Corporation]
=======================================================================
* Device #2: Quadro P1000, skipped

OpenCL API (OpenCL 1.2 pocl 1.6, None+Asserts, LLVM 9.0.1, RELOC, SLEEF, DISTRO, POCL_DEBUG) - Platform #2 [The pocl project]
=============================================================================================================================
* Device #3: pthread-Intel(R) Core(TM) i5-7500 CPU @ 3.40GHz, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........:  4803.1 MH/s (69.72ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........:  1903.8 MH/s (88.05ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:   692.7 MH/s (60.48ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:   202.4 MH/s (51.74ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:    98414 H/s (51.84ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........:  7827.1 MH/s (42.79ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 3000 - LM

Speed.#1.........:  4736.3 MH/s (70.64ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........:  4997.6 MH/s (67.07ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:   386.5 MH/s (54.18ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:   191.2 MH/s (54.65ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........:  2201.5 kH/s (72.00ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:     4562 H/s (25.49ms) @ Accel:2 Loops:32 Thr:12 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:    34993 H/s (57.71ms) @ Accel:4 Loops:512 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........: 63924.7 kH/s (81.93ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........: 63236.6 kH/s (82.82ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    16818 H/s (51.65ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:     7853 H/s (50.00ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:    97119 H/s (50.62ms) @ Accel:32 Loops:31 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:    71107 H/s (71.29ms) @ Accel:4 Loops:4096 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:     9566 H/s (66.85ms) @ Accel:2 Loops:16384 Thr:1024 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:     8433 H/s (73.51ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:    61583 H/s (78.67ms) @ Accel:4 Loops:512 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:     7050 H/s (241.94ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:   530.8 kH/s (49.53ms) @ Accel:16 Loops:249 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     1071 H/s (48.83ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Started: Mon Dec 20 13:02:05 2021
Stopped: Mon Dec 20 13:07:24 2021
```
