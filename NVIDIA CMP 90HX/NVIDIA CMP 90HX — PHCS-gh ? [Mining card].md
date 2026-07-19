# NVIDIA CMP 90HX (Mining card)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA CMP 90HX
- **Конфигурация / Setup:** Mining card
- **Версия hashcat / Version:** ?
- **Источник / Source:** [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 39746.3 MH/s |
| 100 | SHA1 | 12949.8 MH/s |
| 1400 | SHA2-256 | 5620.3 MH/s |
| 1700 | SHA2-512 | 1883.9 MH/s |
| 1000 | NTLM | 67393.6 MH/s |
| 3200 | bcrypt | 62292 H/s |
| 1800 | sha512crypt | 289.5 kH/s |
| 500 | md5crypt | 18190.6 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 660.1 kH/s |
| 7500 | Kerberos AS-REQ (23) | 914.6 MH/s |
| 13100 | Kerberos TGS-REP (23) | 911.3 MH/s |
| 11300 | Bitcoin wallet.dat | 8619 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 498.6 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
CUDA API (CUDA 12.5)
====================
* Device #1: NVIDIA CMP 90HX, 9914/10088 MB, 50MCU

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 39746.3 MH/s (83.79ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........: 12949.8 MH/s (258.48ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  5620.3 MH/s (297.74ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1883.9 MH/s (443.67ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   660.1 kH/s (309.12ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 67393.6 MH/s (49.22ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 38838.4 MH/s (85.56ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 40939.5 MH/s (81.27ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  2969.9 MH/s (281.74ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1576.4 MH/s (264.97ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 18190.6 kH/s (174.85ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    62292 H/s (299.30ms) @ Accel:16 Loops:32 Thr:24 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   289.5 kH/s (280.71ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   914.6 MH/s (457.85ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   911.3 MH/s (459.73ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:   111.8 kH/s (311.44ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    64813 H/s (250.19ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   809.8 kH/s (167.33ms) @ Accel:8 Loops:511 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   536.1 kH/s (289.94ms) @ Accel:16 Loops:4096 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    89691 H/s (284.74ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    70484 H/s (362.22ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   498.6 kH/s (377.29ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    82041 H/s (415.50ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  4519.9 kH/s (353.03ms) @ Accel:32 Loops:499 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     8619 H/s (242.25ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
```
