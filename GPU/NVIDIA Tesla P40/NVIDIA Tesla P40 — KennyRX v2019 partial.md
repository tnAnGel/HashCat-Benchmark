# NVIDIA Tesla P40

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Tesla P40
- **Версия hashcat / Version:** не указана
- **Источник / Source:** [публичный сырой вывод](https://www.reddit.com/r/hacking/comments/cz6jat/hashcat_benchmark_on_geforce_now/)
- **Параметры / Options:** `-b` (исходные параметры — см. лог)
- **Примечание / Note:** в источнике опубликован фрагмент вывода для одной Tesla P40, но не версия hashcat и не весь исходный stdout. Сохраняется доступный набор из 25 режимов без дополнений; WPA использует старый mode 2500.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 32855.6 MH/s |
| 100 | SHA1 | 11339.3 MH/s |
| 1400 | SHA2-256 | 3956.8 MH/s |
| 1700 | SHA2-512 | 1283.4 MH/s |
| 1000 | NTLM | 56126.1 MH/s |
| 2500 | WPA-EAPOL-PBKDF2 (legacy mode) | 527.4 kH/s |
| 3200 | bcrypt | 18809 H/s |

## Полный доступный сырой вывод / Raw output

```text
OpenCL Platform #1: NVIDIA Corporation
======================================

* Device #1: Tesla P40, 6144/24576 MB allocatable, 30MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5
Speed.#1.........: 32855.6 MH/s (59.28ms) @ Accel:128 Loops:512 Thr:1024 Vec:4

Hashmode: 100 - SHA1
Speed.#1.........: 11339.3 MH/s (86.21ms) @ Accel:256 Loops:256 Thr:512 Vec:2

Hashmode: 1400 - SHA2-256
Speed.#1.........: 3956.8 MH/s (61.48ms) @ Accel:128 Loops:64 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512
Speed.#1.........: 1283.4 MH/s (59.73ms) @ Accel:128 Loops:32 Thr:640 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4096)
Speed.#1.........: 527.4 kH/s (56.26ms) @ Accel:128 Loops:32 Thr:1024 Vec:1

Hashmode: 1000 - NTLM
Speed.#1.........: 56126.1 MH/s (69.61ms) @ Accel:128 Loops:1024 Thr:1024 Vec:2

Hashmode: 3000 - LM
Speed.#1.........: 25822.0 MH/s (76.24ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS
Speed.#1.........: 27994.2 MH/s (69.78ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 5600 - NetNTLMv2
Speed.#1.........: 2342.5 MH/s (51.96ms) @ Accel:128 Loops:32 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES
Speed.#1.........: 1129.1 MH/s (54.79ms) @ Accel:8 Loops:1024 Thr:256 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)
Speed.#1.........: 9874.0 kH/s (74.72ms) @ Accel:1024 Loops:1000 Thr:32 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)
Speed.#1.........: 18809 H/s (48.98ms) @ Accel:16 Loops:8 Thr:8 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)
Speed.#1.........: 166.6 kH/s (72.22ms) @ Accel:512 Loops:128 Thr:32 Vec:1

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23
Speed.#1.........: 373.7 MH/s (83.17ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23
Speed.#1.........: 373.9 MH/s (83.08ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)
Speed.#1.........: 88325 H/s (56.71ms) @ Accel:128 Loops:32 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 7999)
Speed.#1.........: 49797 H/s (78.09ms) @ Accel:256 Loops:128 Thr:32 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 35000)
Speed.#1.........: 16271 H/s (54.05ms) @ Accel:64 Loops:32 Thr:512 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 524288)
Speed.#1.........: 11789 H/s (59.33ms) @ Accel:128 Loops:128 Thr:768 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)
Speed.#1.........: 39596 H/s (72.02ms) @ Accel:4 Loops:16384 Thr:384 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32767)
Speed.#1.........: 43880 H/s (73.65ms) @ Accel:128 Loops:32 Thr:896 Vec:1

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 2000)
Speed.#1.........: 367.6 kH/s (82.29ms) @ Accel:64 Loops:32 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 6000)
Speed.#1.........: 164.5 kH/s (62.68ms) @ Accel:512 Loops:128 Thr:32 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 500)
Speed.#1.........: 2843.7 kH/s (59.11ms) @ Accel:64 Loops:62 Thr:896 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 199999)
Speed.#1.........: 5949 H/s (51.52ms) @ Accel:64 Loops:32 Thr:1024 Vec:1

Started: Tue Sep 03 08:29:05 2019
Stopped: Tue Sep 03 08:38:50 2019
```

