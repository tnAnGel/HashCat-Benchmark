# AMD Radeon Pro WX 3200

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon Pro WX 3200
- **Версия hashcat / Version:** v5.1.0
- **Источник / Source:** [rarecoil](https://gist.github.com/rarecoil/41151368c61f6af6cc5b30851794681d)
- **Примечание / Note:** Windows 10. Драйвер сообщает устройство как `gfx804` (Polaris 12) — модель указана автором в заголовке gist. Формат вывода hashcat 5.x (`Hashmode:` / `Speed.#1`). Режим 2500 (WPA-EAPOL-PBKDF2) в выводе присутствует, но строка Speed отсутствует.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 3157.3 MH/s |
| 100 | SHA1 | 1036.6 MH/s |
| 1400 | SHA2-256 | 493.8 MH/s |
| 1700 | SHA2-512 | 124.4 MH/s |
| 1000 | NTLM | 5684.5 MH/s |
| 3200 | bcrypt | 2288 H/s |
| 1800 | sha512crypt | 20285 H/s |
| 500 | md5crypt | 977.4 kH/s |
| 7500 | Kerberos AS-REQ (23) | 30389.7 kH/s |
| 13100 | Kerberos TGS-REP (23) | 30166.0 kH/s |
| 11300 | Bitcoin wallet.dat | 572 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 27791 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.1.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL Platform #1: Advanced Micro Devices, Inc.
================================================
* Device #1: gfx804, 3264/4096 MB allocatable, 10MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........:  3157.3 MH/s (103.86ms) @ Accel:512 Loops:256 Thr:256 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........:  1036.6 MH/s (77.48ms) @ Accel:256 Loops:128 Thr:256 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:   493.8 MH/s (82.51ms) @ Accel:256 Loops:64 Thr:256 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:   124.4 MH/s (81.90ms) @ Accel:128 Loops:32 Thr:256 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4096)

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#1.........:    51056 H/s (98.86ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........:  5684.5 MH/s (56.66ms) @ Accel:512 Loops:256 Thr:256 Vec:1

Hashmode: 3000 - LM

Speed.#1.........:  3165.2 MH/s (49.66ms) @ Accel:64 Loops:1024 Thr:256 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........:  3645.9 MH/s (89.55ms) @ Accel:512 Loops:256 Thr:256 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:   234.8 MH/s (86.95ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:   124.2 MH/s (80.95ms) @ Accel:4 Loops:1024 Thr:256 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........:   977.4 kH/s (121.30ms) @ Accel:768 Loops:250 Thr:64 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:     2288 H/s (66.70ms) @ Accel:16 Loops:4 Thr:8 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:    20285 H/s (49.95ms) @ Accel:128 Loops:64 Thr:64 Vec:1

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.#1.........: 30389.7 kH/s (83.95ms) @ Accel:128 Loops:32 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23

Speed.#1.........: 30166.0 kH/s (84.69ms) @ Accel:128 Loops:32 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:     9745 H/s (42.62ms) @ Accel:128 Loops:32 Thr:256 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 7999)

Speed.#1.........:     4718 H/s (67.01ms) @ Accel:128 Loops:32 Thr:64 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 35000)

Speed.#1.........:     1046 H/s (70.31ms) @ Accel:64 Loops:16 Thr:256 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 524288)

Speed.#1.........:     1486 H/s (79.28ms) @ Accel:384 Loops:64 Thr:256 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:     8212 H/s (76.56ms) @ Accel:4 Loops:16384 Thr:256 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32767)

Speed.#1.........:     6375 H/s (98.75ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 2000)

Speed.#1.........:    27791 H/s (71.82ms) @ Accel:64 Loops:32 Thr:256 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 6000)

Speed.#1.........:    42111 H/s (81.30ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 500)

Speed.#1.........:   403.2 kH/s (85.34ms) @ Accel:128 Loops:62 Thr:256 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 199999)

Speed.#1.........:      572 H/s (90.01ms) @ Accel:128 Loops:32 Thr:256 Vec:1

Started: Fri Sep 20 20:02:39 2019
Stopped: Fri Sep 20 20:08:48 2019
```
