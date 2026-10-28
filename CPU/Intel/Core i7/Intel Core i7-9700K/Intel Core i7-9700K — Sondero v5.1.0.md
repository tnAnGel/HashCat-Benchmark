# Intel Core i7-9700K

- **Вендор / Vendor:** Intel
- **Процессор / CPU:** Intel Core i7-9700K CPU @ 3.60GHz
- **Версия hashcat / Version:** v5.1.0
- **Бэкенд / Backend:** OpenCL — `[Intel(R) Corporation]`, устройство `Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz` (Device #2), `--opencl-device-types=1`
- **Источник / Source:** [Sondero, hashcat.net forum, thread «Is any benchmark of INTEL cpu s ?»](https://hashcat.net/forum/thread-9042.html)
- **Примечание / Note:** В прогоне присутствует iGPU Intel UHD Graphics 630 (Device #1), но он `skipped` (драйвер Intel GPU-only сломан) — реальные замеры только у CPU (Device #2, `Speed.#2`). Стандартный `hashcat -b`.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 1037.8 MH/s |
| 100 | SHA1 | 698.1 MH/s |
| 1400 | SHA2-256 | 299.3 MH/s |
| 1700 | SHA2-512 | 88896.9 kH/s |
| 1000 | NTLM | 1854.4 MH/s |
| 3200 | bcrypt | 5957 H/s |
| 1800 | sha512crypt | 6623 H/s |
| 500 | md5crypt | 90104 H/s |
| 7500 | Kerberos AS-REQ (23) | 6539.1 kH/s |
| 13100 | Kerberos TGS-REP (23) | 6174.7 kH/s |
| 11300 | Bitcoin/Litecoin wallet.dat | 400 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 15088 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.1.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #1: Intel's OpenCL runtime (GPU only) is currently broken.
            We are waiting for updated OpenCL drivers from Intel.
            You can use --force to override, but do not report related errors.
OpenCL Platform #1: Intel(R) Corporation
========================================
* Device #1: Intel(R) UHD Graphics 630, skipped.
* Device #2: Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz, 4070/16281 MB allocatable, 8MCU

Benchmark relevant options:
===========================
* --opencl-device-types=1
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#2.........:  1037.8 MH/s (7.92ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 100 - SHA1

Speed.#2.........:  698.1 MH/s (11.99ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 1400 - SHA2-256

Speed.#2.........:  299.3 MH/s (27.92ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 1700 - SHA2-512

Speed.#2.........: 88896.9 kH/s (94.22ms) @ Accel:1024 Loops:1024 Thr:1 Vec:4

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4096)

Speed.#2.........:    30676 H/s (66.24ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 1000 - NTLM

Speed.#2.........:  1854.4 MH/s (4.42ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 3000 - LM

Speed.#2.........:  315.6 MH/s (26.35ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#2.........:  1118.9 MH/s (7.39ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 5600 - NetNTLMv2

Speed.#2.........: 83706.4 kH/s (50.00ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#2.........: 14075.8 kH/s (74.23ms) @ Accel:128 Loops:1024 Thr:1 Vec:8

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#2.........:    90104 H/s (89.52ms) @ Accel:1024 Loops:1000 Thr:1 Vec:8

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#2.........:    5957 H/s (83.98ms) @ Accel:32 Loops:8 Thr:8 Vec:8

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#2.........:    6623 H/s (61.55ms) @ Accel:1024 Loops:256 Thr:1 Vec:4

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.#2.........:  6539.1 kH/s (80.11ms) @ Accel:64 Loops:16 Thr:64 Vec:8

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23

Speed.#2.........:  6174.7 kH/s (84.83ms) @ Accel:64 Loops:16 Thr:64 Vec:8

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#2.........:    5227 H/s (65.10ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 7999)

Speed.#2.........:    5021 H/s (50.79ms) @ Accel:1024 Loops:256 Thr:1 Vec:4

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 35000)

Speed.#2.........:    1153 H/s (51.88ms) @ Accel:1024 Loops:256 Thr:1 Vec:4

Hashmode: 11600 - 7-Zip (Iterations: 524288)

Speed.#2.........:      164 H/s (48.86ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#2.........:    1164 H/s (54.93ms) @ Accel:128 Loops:16384 Thr:1 Vec:8

Hashmode: 13000 - RAR5 (Iterations: 32767)

Speed.#2.........:    3473 H/s (73.61ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 2000)

Speed.#2.........:    15088 H/s (56.41ms) @ Accel:1024 Loops:256 Thr:1 Vec:8

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 6000)

Speed.#2.........:    9988 H/s (68.11ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 500)

Speed.#2.........:  212.2 kH/s (35.99ms) @ Accel:1024 Loops:500 Thr:1 Vec:8

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 199999)

Speed.#2.........:      400 H/s (52.38ms) @ Accel:1024 Loops:512 Thr:1 Vec:4

Started: Sun Mar 15 09:56:00 2020
Stopped: Sun Mar 15 09:59:52 2020
```
