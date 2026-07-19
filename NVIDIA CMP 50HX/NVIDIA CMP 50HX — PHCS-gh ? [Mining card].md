# NVIDIA CMP 50HX (Mining card)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA CMP 50HX
- **Конфигурация / Setup:** Mining card
- **Версия hashcat / Version:** ?
- **Источник / Source:** [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 44156.8 MH/s |
| 100 | SHA1 | 14760.5 MH/s |
| 1400 | SHA2-256 | 6375.5 MH/s |
| 1700 | SHA2-512 | 2036.5 MH/s |
| 1000 | NTLM | 73927.3 MH/s |
| 3200 | bcrypt | 51206 H/s |
| 1800 | sha512crypt | 295.0 kH/s |
| 500 | md5crypt | 19690.0 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 725.8 kH/s |
| 7500 | Kerberos AS-REQ (23) | 832.6 MH/s |
| 13100 | Kerberos TGS-REP (23) | 802.8 MH/s |
| 11300 | Bitcoin wallet.dat | 9407 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 550.1 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
CUDA API (CUDA 12.5)
====================
* Device #1: NVIDIA CMP 50HX, 9916/10055 MB, 56MCU

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 44156.8 MH/s (84.38ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........: 14760.5 MH/s (254.17ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  6375.5 MH/s (294.44ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  2036.5 MH/s (460.97ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   725.8 kH/s (314.33ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 73927.3 MH/s (50.38ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 39436.6 MH/s (94.43ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 45236.3 MH/s (81.85ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  3214.8 MH/s (291.84ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1652.4 MH/s (283.37ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 19690.0 kH/s (178.45ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    51206 H/s (272.71ms) @ Accel:16 Loops:32 Thr:16 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   295.0 kH/s (308.34ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   832.6 MH/s (281.77ms) @ Accel:128 Loops:1024 Thr:32 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   802.8 MH/s (292.19ms) @ Accel:256 Loops:512 Thr:32 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:   124.7 kH/s (312.42ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    69541 H/s (252.86ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   872.6 kH/s (260.03ms) @ Accel:4 Loops:1023 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   570.4 kH/s (302.49ms) @ Accel:16 Loops:4096 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    90967 H/s (313.06ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    77894 H/s (366.10ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   550.1 kH/s (382.92ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    47706 H/s (798.57ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  4922.6 kH/s (357.25ms) @ Accel:32 Loops:499 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     9407 H/s (248.64ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
```
