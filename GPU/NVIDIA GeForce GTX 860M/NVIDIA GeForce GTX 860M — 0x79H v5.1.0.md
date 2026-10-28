# NVIDIA GeForce GTX 860M

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 860M (GM107)
- **Версия hashcat / Version:** v5.1.0
- **Источник / Source:** [0x79H](https://gist.github.com/0x79H/5b8bb29c589589032b8adc592bd2a149)

> Примечание: прогон на Windows, ноутбук; в системе также присутствуют Intel HD Graphics 4600 и CPU — они пропущены (skipped), все результаты принадлежат Device #1 (GTX 860M). Набор режимов соответствует hashcat 5.1.0 (режима 22000 в нём нет; WPA представлен режимом 2500).

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 3081.8 MH/s |
| 100 | SHA1 | 1067.4 MH/s |
| 1400 | SHA2-256 | 397.3 MH/s |
| 1700 | SHA2-512 | 139.0 MH/s |
| 1000 | NTLM | 6030.4 MH/s |
| 3200 | bcrypt | 899 H/s |
| 1800 | sha512crypt | 22828 H/s |
| 500 | md5crypt | 1147.2 kH/s |
| 7500 | Kerberos AS-REQ (23) | 27726.7 kH/s |
| 13100 | Kerberos TGS-REP (23) | 28412.1 kH/s |
| 11300 | Bitcoin wallet.dat | 574 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 35432 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
PS D:\Work\hashcat-5.1.0> .\hashcat64.exe -b
hashcat (v5.1.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #1: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
* Device #2: Intel's OpenCL runtime (GPU only) is currently broken.
             We are waiting for updated OpenCL drivers from Intel.
             You can use --force to override, but do not report related errors.
nvmlDeviceGetFanSpeed(): Not Supported

OpenCL Platform #1: NVIDIA Corporation
======================================
* Device #1: GeForce GTX 860M, 512/2048 MB allocatable, 5MCU

OpenCL Platform #2: Intel(R) Corporation
========================================
* Device #2: Intel(R) HD Graphics 4600, skipped.
* Device #3: Intel(R) Core(TM) i7-4710MQ CPU @ 2.50GHz, skipped.

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........:  3081.8 MH/s (52.11ms) @ Accel:256 Loops:128 Thr:1024 Vec:2

Hashmode: 100 - SHA1

Speed.#1.........:  1067.4 MH/s (56.44ms) @ Accel:256 Loops:128 Thr:384 Vec:4

Hashmode: 1400 - SHA2-256

Speed.#1.........:   397.3 MH/s (50.91ms) @ Accel:128 Loops:32 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:   139.0 MH/s (91.76ms) @ Accel:128 Loops:32 Thr:640 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4096)

Speed.#1.........:    54278 H/s (45.63ms) @ Accel:64 Loops:32 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........:  6030.4 MH/s (53.33ms) @ Accel:256 Loops:256 Thr:1024 Vec:4

Hashmode: 3000 - LM

Speed.#1.........:  3313.2 MH/s (48.67ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........:  2601.3 MH/s (46.08ms) @ Accel:512 Loops:128 Thr:384 Vec:4

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:   217.2 MH/s (81.78ms) @ Accel:128 Loops:32 Thr:896 Vec:2

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:   144.2 MH/s (70.13ms) @ Accel:8 Loops:1024 Thr:256 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........:  1147.2 kH/s (66.28ms) @ Accel:1024 Loops:500 Thr:32 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:      899 H/s (42.39ms) @ Accel:8 Loops:4 Thr:8 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:    22828 H/s (86.68ms) @ Accel:512 Loops:128 Thr:32 Vec:1

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.#1.........: 27726.7 kH/s (92.24ms) @ Accel:256 Loops:32 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23

Speed.#1.........: 28412.1 kH/s (89.89ms) @ Accel:256 Loops:32 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:     9166 H/s (46.15ms) @ Accel:64 Loops:32 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 7999)

Speed.#1.........:     6314 H/s (50.64ms) @ Accel:256 Loops:64 Thr:32 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 35000)

Speed.#1.........:     1509 H/s (47.93ms) @ Accel:64 Loops:16 Thr:512 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 524288)

Speed.#1.........:     1143 H/s (102.10ms) @ Accel:256 Loops:64 Thr:768 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:     9226 H/s (50.57ms) @ Accel:4 Loops:16384 Thr:384 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32767)

Speed.#1.........:     4999 H/s (77.84ms) @ Accel:128 Loops:32 Thr:640 Vec:1

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 2000)

Speed.#1.........:    35432 H/s (35.67ms) @ Accel:32 Loops:16 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 6000)

Speed.#1.........:    20153 H/s (167.09ms) @ Accel:512 Loops:256 Thr:32 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 500)

Speed.#1.........:   323.2 kH/s (66.13ms) @ Accel:64 Loops:62 Thr:640 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 199999)

Speed.#1.........:      574 H/s (43.94ms) @ Accel:64 Loops:16 Thr:1024 Vec:1

Started: Fri Jun 07 23:07:10 2019
Stopped: Fri Jun 07 23:14:46 2019
```
