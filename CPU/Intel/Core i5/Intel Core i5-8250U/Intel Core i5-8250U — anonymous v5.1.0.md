# Intel Core i5-8250U

- **Вендор / Vendor:** Intel
- **Процессор / CPU:** Intel(R) Core(TM) i5-8250U CPU @ 1.60GHz
- **Версия hashcat / Version:** v5.1.0
- **Бэкенд / Backend:** OpenCL — `[The pocl project]`, устройство `pthread-Intel(R) Core(TM) i5-8250U CPU @ 1.60GHz` (Device #1, 8MCU)
- **Источник / Source:** [Pastebin XVtBm4Fh](https://pastebin.com/XVtBm4Fh)
- **Примечание / Note:** Прогон только на CPU (единственное устройство Device #1). Запущено с `--force` и `--optimized-kernel-enable`. Полный набор режимов (25 алгоритмов). Формат hashcat 5.x (`Speed.#1`). Дата прогона: 12 Jun 2019. Автор анонимный (raw Pastebin).

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 254.6 MH/s |
| 100 | SHA1 | 63856.1 kH/s |
| 1400 | SHA2-256 | 21904.6 kH/s |
| 1700 | SHA2-512 | 6625.3 kH/s |
| 1000 | NTLM | 421.4 MH/s |
| 3200 | bcrypt | 2926 H/s |
| 1800 | sha512crypt | 361 H/s |
| 500 | md5crypt | 19137 H/s |
| 7500 | Kerberos AS-REQ (23) | 1499.7 kH/s |
| 13100 | Kerberos TGS-REP (23) | 1778.2 kH/s |
| 11300 | Bitcoin/Litecoin wallet.dat | 31 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 1998 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.1.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL Platform #1: The pocl project
====================================
* Device #1: pthread-Intel(R) Core(TM) i5-8250U CPU @ 1.60GHz, 4096/13859 MB allocatable, 8MCU

Benchmark relevant options:
===========================
* --force
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........:   254.6 MH/s (32.74ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 100 - SHA1

Speed.#1.........: 63856.1 kH/s (65.52ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

Hashmode: 1400 - SHA2-256

Speed.#1.........: 21904.6 kH/s (95.38ms) @ Accel:1024 Loops:256 Thr:1 Vec:8

Hashmode: 1700 - SHA2-512

Speed.#1.........:  6625.3 kH/s (78.74ms) @ Accel:512 Loops:128 Thr:1 Vec:4

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4096)

Speed.#1.........:     3042 H/s (83.79ms) @ Accel:512 Loops:256 Thr:1 Vec:8

Hashmode: 1000 - NTLM

Speed.#1.........:   421.4 MH/s (19.57ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 3000 - LM

Speed.#1.........: 74411.2 kH/s (111.89ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........:   224.6 MH/s (19.43ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

Hashmode: 5600 - NetNTLMv2

Speed.#1.........: 12929.2 kH/s (80.53ms) @ Accel:512 Loops:256 Thr:1 Vec:8

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  2609.1 kH/s (96.56ms) @ Accel:32 Loops:1024 Thr:1 Vec:8

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........:    19137 H/s (52.50ms) @ Accel:512 Loops:250 Thr:1 Vec:8

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:     2926 H/s (85.27ms) @ Accel:16 Loops:8 Thr:8 Vec:8

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:      361 H/s (72.16ms) @ Accel:256 Loops:64 Thr:1 Vec:4

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.#1.........:  1499.7 kH/s (87.02ms) @ Accel:32 Loops:8 Thr:64 Vec:8

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23

Speed.#1.........:  1778.2 kH/s (73.56ms) @ Accel:32 Loops:8 Thr:64 Vec:8

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:      447 H/s (97.53ms) @ Accel:512 Loops:256 Thr:1 Vec:8

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 7999)

Speed.#1.........:      438 H/s (74.55ms) @ Accel:256 Loops:128 Thr:1 Vec:4

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 35000)

Speed.#1.........:       96 H/s (77.56ms) @ Accel:256 Loops:128 Thr:1 Vec:4

Hashmode: 11600 - 7-Zip (Iterations: 524288)

Speed.#1.........:       10 H/s (96.78ms) @ Accel:512 Loops:128 Thr:1 Vec:8

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:       81 H/s (49.13ms) @ Accel:8 Loops:16384 Thr:1 Vec:8

Hashmode: 13000 - RAR5 (Iterations: 32767)

Speed.#1.........:      267 H/s (59.82ms) @ Accel:512 Loops:128 Thr:1 Vec:8

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 2000)

Speed.#1.........:     1998 H/s (55.46ms) @ Accel:256 Loops:128 Thr:1 Vec:8

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 6000)

Speed.#1.........:     3088 H/s (54.85ms) @ Accel:512 Loops:256 Thr:1 Vec:8

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 500)

Speed.#1.........:    19994 H/s (48.82ms) @ Accel:256 Loops:250 Thr:1 Vec:8

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 199999)

Speed.#1.........:       31 H/s (83.43ms) @ Accel:512 Loops:128 Thr:1 Vec:4

Started: Wed Jun 12 16:33:50 2019
Stopped: Wed Jun 12 16:40:12 2019
```
