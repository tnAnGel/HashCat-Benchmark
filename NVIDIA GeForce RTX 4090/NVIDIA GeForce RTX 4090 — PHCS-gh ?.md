# NVIDIA GeForce RTX 4090

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 4090
- **Версия hashcat / Version:** ?
- **Источник / Source:** [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 148.0 GH/s |
| 100 | SHA1 | 49207.2 MH/s |
| 1400 | SHA2-256 | 21539.3 MH/s |
| 1700 | SHA2-512 | 7263.4 MH/s |
| 1000 | NTLM | 244.9 GH/s |
| 3200 | bcrypt | 241.8 kH/s |
| 1800 | sha512crypt | 1155.0 kH/s |
| 500 | md5crypt | 64981.0 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 2539.8 kH/s |
| 7500 | Kerberos AS-REQ (23) | 3517.0 MH/s |
| 13100 | Kerberos TGS-REP (23) | 3500.3 MH/s |
| 11300 | Bitcoin wallet.dat | 33409 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 1928.4 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
CUDA API (CUDA 12.3)
====================
* Device #1: NVIDIA GeForce RTX 4090, 23008/24563 MB, 128MCU

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........:   148.0 GH/s (13.81ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........: 49207.2 MH/s (43.04ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........: 21539.3 MH/s (98.96ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  7263.4 MH/s (295.06ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:  2539.8 kH/s (205.16ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........:   244.9 GH/s (8.16ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 3000 - LM

Speed.#1.........:   141.0 GH/s (14.15ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........:   151.7 GH/s (13.44ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........: 11550.5 MH/s (185.16ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  6106.2 MH/s (350.38ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 64981.0 kH/s (28.75ms) @ Accel:16 Loops:1000 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:   241.8 kH/s (395.61ms) @ Accel:32 Loops:32 Thr:24 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:  1155.0 kH/s (359.71ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:  3517.0 MH/s (304.59ms) @ Accel:512 Loops:512 Thr:32 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:  3500.3 MH/s (305.87ms) @ Accel:512 Loops:512 Thr:32 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:   427.1 kH/s (209.01ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:   252.0 kH/s (319.60ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:  3122.2 kH/s (221.50ms) @ Accel:16 Loops:511 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:  1592.1 kH/s (183.01ms) @ Accel:16 Loops:4096 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:   171.0 kH/s (166.58ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:   271.4 kH/s (240.77ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:  1928.4 kH/s (248.14ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:   321.5 kH/s (271.48ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........: 17023.6 kH/s (117.22ms) @ Accel:16 Loops:499 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:    33409 H/s (320.15ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
```
