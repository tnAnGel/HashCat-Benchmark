# NVIDIA GeForce GTX 1050 Ti

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 1050 Ti
- **Версия hashcat / Version:** v6.2.3
- **Источник / Source:** [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 5554.2 MH/s |
| 100 | SHA1 | 1605.2 MH/s |
| 1400 | SHA2-256 | 374.6 MH/s |
| 1700 | SHA2-512 | 94840.7 kH/s |
| 1000 | NTLM | 5615.8 MH/s |
| 3200 | bcrypt | 4416 H/s |
| 1800 | sha512crypt | 27780 H/s |
| 500 | md5crypt | 2207.0 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 50866 H/s |
| 7500 | Kerberos AS-REQ (23) | 42203.3 kH/s |
| 13100 | Kerberos TGS-REP (23) | 72462.4 kH/s |
| 11300 | Bitcoin wallet.dat | 429 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 28239 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
CUDA API (CUDA 12.3)
====================
* Device #1: NVIDIA GeForce GTX 1050 Ti, 3370/4095 MB, 6MCU

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........:  5554.2 MH/s (72.30ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 100 - SHA1

Speed.#1.........:  1605.2 MH/s (250.65ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:   374.6 MH/s (537.28ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........: 94840.7 kH/s (530.50ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:    50866 H/s (480.05ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........:  5615.8 MH/s (71.45ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 3000 - LM

Speed.#1.........:  4124.4 MH/s (97.29ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........:  2632.2 MH/s (152.72ms) @ Accel:64 Loops:1024 Thr:1024 Vec:2

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:   148.4 MH/s (677.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:   128.8 MH/s (390.30ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........:  2207.0 kH/s (174.52ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:     4416 H/s (255.12ms) @ Accel:32 Loops:16 Thr:12 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:    27780 H/s (350.10ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........: 42203.3 kH/s (596.09ms) @ Accel:128 Loops:1024 Thr:32 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........: 72462.4 kH/s (347.12ms) @ Accel:128 Loops:1024 Thr:32 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:     9323 H/s (445.63ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:     4248 H/s (458.27ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:    53019 H/s (406.86ms) @ Accel:32 Loops:127 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:    70733 H/s (345.55ms) @ Accel:16 Loops:4096 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    10687 H/s (574.17ms) @ Accel:128 Loops:16384 Thr:128 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:     3575 H/s (424.82ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:    28239 H/s (411.75ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:     3565 H/s (1146.40ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:   219.8 kH/s (285.13ms) @ Accel:32 Loops:249 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:      429 H/s (291.50ms) @ Accel:8 Loops:512 Thr:1024 Vec:1
```
