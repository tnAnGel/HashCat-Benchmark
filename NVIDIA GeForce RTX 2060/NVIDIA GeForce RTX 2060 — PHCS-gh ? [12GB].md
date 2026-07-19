# NVIDIA GeForce RTX 2060 (12GB)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 2060
- **Конфигурация / Setup:** 12GB
- **Версия hashcat / Version:** ?
- **Источник / Source:** [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 29685.1 MH/s |
| 100 | SHA1 | 9510.3 MH/s |
| 1400 | SHA2-256 | 4114.6 MH/s |
| 1700 | SHA2-512 | 1318.4 MH/s |
| 1000 | NTLM | 53872.5 MH/s |
| 3200 | bcrypt | 32226 H/s |
| 1800 | sha512crypt | 147.8 kH/s |
| 500 | md5crypt | 12626.2 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 469.9 kH/s |
| 7500 | Kerberos AS-REQ (23) | 523.5 MH/s |
| 13100 | Kerberos TGS-REP (23) | 500.2 MH/s |
| 11300 | Bitcoin wallet.dat | 6096 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 354.9 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
CUDA API (CUDA 12.3)
====================
* Device #1: NVIDIA GeForce RTX 2060, 11221/12287 MB, 34MCU

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 29685.1 MH/s (75.96ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 100 - SHA1

Speed.#1.........:  9510.3 MH/s (239.11ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  4114.6 MH/s (276.35ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1318.4 MH/s (431.88ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   469.9 kH/s (294.56ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 53872.5 MH/s (41.38ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 3000 - LM

Speed.#1.........: 24748.8 MH/s (90.80ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 29299.2 MH/s (76.92ms) @ Accel:64 Loops:1024 Thr:1024 Vec:2

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  2101.0 MH/s (270.55ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1073.8 MH/s (263.99ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 12626.2 kH/s (167.38ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    32226 H/s (262.34ms) @ Accel:16 Loops:32 Thr:16 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   147.8 kH/s (374.34ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   523.5 MH/s (271.63ms) @ Accel:512 Loops:256 Thr:32 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   500.2 MH/s (284.21ms) @ Accel:512 Loops:256 Thr:32 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    80376 H/s (294.39ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    44964 H/s (237.33ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   565.3 kH/s (243.11ms) @ Accel:4 Loops:1023 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   433.7 kH/s (277.55ms) @ Accel:16 Loops:4096 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    53379 H/s (324.85ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    50483 H/s (343.50ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   354.9 kH/s (358.76ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    29879 H/s (774.78ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  3159.8 kH/s (335.58ms) @ Accel:32 Loops:499 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     6096 H/s (465.91ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
```
