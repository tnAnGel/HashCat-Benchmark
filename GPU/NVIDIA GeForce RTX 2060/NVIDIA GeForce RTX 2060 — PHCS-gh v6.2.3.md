# NVIDIA GeForce RTX 2060

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 2060
- **Версия hashcat / Version:** v6.2.3
- **Источник / Source:** [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 27504.1 MH/s |
| 100 | SHA1 | 8691.6 MH/s |
| 1400 | SHA2-256 | 3773.4 MH/s |
| 1700 | SHA2-512 | 1213.7 MH/s |
| 1000 | NTLM | 49801.5 MH/s |
| 3200 | bcrypt | 29168 H/s |
| 1800 | sha512crypt | 193.3 kH/s |
| 500 | md5crypt | 11687.9 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 434.4 kH/s |
| 7500 | Kerberos AS-REQ (23) | 475.3 MH/s |
| 13100 | Kerberos TGS-REP (23) | 455.0 MH/s |
| 11300 | Bitcoin wallet.dat | 5572 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 328.7 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
CUDA API (CUDA 12.3)
====================
* Device #1: NVIDIA GeForce RTX 2060, 5121/6143 MB, 30MCU

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 27504.1 MH/s (72.40ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 100 - SHA1

Speed.#1.........:  8691.6 MH/s (230.83ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  3773.4 MH/s (265.98ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1213.7 MH/s (413.88ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   434.4 kH/s (281.35ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 49801.5 MH/s (39.65ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 3000 - LM

Speed.#1.........: 24103.1 MH/s (82.29ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 26748.2 MH/s (74.52ms) @ Accel:64 Loops:1024 Thr:1024 Vec:2

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  1956.7 MH/s (256.44ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1003.7 MH/s (249.42ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 11687.9 kH/s (160.69ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    29168 H/s (255.87ms) @ Accel:16 Loops:32 Thr:16 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   193.3 kH/s (251.91ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   475.3 MH/s (264.00ms) @ Accel:128 Loops:1024 Thr:32 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   455.0 MH/s (275.66ms) @ Accel:512 Loops:256 Thr:32 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    73631 H/s (282.81ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    41281 H/s (471.61ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   516.0 kH/s (471.13ms) @ Accel:8 Loops:1023 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   421.3 kH/s (258.06ms) @ Accel:16 Loops:4096 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    55185 H/s (515.01ms) @ Accel:128 Loops:16384 Thr:128 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    45917 H/s (333.38ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   328.7 kH/s (342.35ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    27016 H/s (757.18ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  2882.8 kH/s (325.26ms) @ Accel:32 Loops:499 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     5572 H/s (449.38ms) @ Accel:32 Loops:512 Thr:1024 Vec:1
```
