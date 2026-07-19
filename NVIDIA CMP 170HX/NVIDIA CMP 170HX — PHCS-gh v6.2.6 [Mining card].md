# NVIDIA CMP 170HX (Mining card)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA CMP 170HX
- **Конфигурация / Setup:** Mining card
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 43380.6 MH/s |
| 100 | SHA1 | 14087.7 MH/s |
| 1400 | SHA2-256 | 6088.3 MH/s |
| 1700 | SHA2-512 | 2053.2 MH/s |
| 1000 | NTLM | 73580.4 MH/s |
| 3200 | bcrypt | 92117 H/s |
| 1800 | sha512crypt | 334.7 kH/s |
| 500 | md5crypt | 18864.4 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 718.7 kH/s |
| 7500 | Kerberos AS-REQ (23) | 1375.1 MH/s |
| 13100 | Kerberos TGS-REP (23) | 1259.1 MH/s |
| 11300 | Bitcoin wallet.dat | 9367 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 531.9 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
CUDA API (CUDA 12.4)
====================
* Device #1: NVIDIA Graphics Device [CMP 170 HX] , 7745/8033 MB, 70MCU

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable


* Hash-Mode 0 (MD5)

Speed.#1.........: 43380.6 MH/s (53.63ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

* Hash-Mode 100 (SHA1)

Speed.#1.........: 14087.7 MH/s (82.90ms) @ Accel:128 Loops:512 Thr:256 Vec:1

* Hash-Mode 1400 (SHA2-256)

Speed.#1.........:  6088.3 MH/s (95.94ms) @ Accel:32 Loops:512 Thr:512 Vec:1

* Hash-Mode 1700 (SHA2-512)

Speed.#1.........:  2053.2 MH/s (71.11ms) @ Accel:16 Loops:512 Thr:256 Vec:1

* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]

Speed.#1.........:   718.7 kH/s (49.38ms) @ Accel:8 Loops:512 Thr:512 Vec:1

* Hash-Mode 1000 (NTLM)

Speed.#1.........: 73580.4 MH/s (31.52ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

* Hash-Mode 3000 (LM)

Speed.#1.........: 41940.1 MH/s (27.63ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)

Speed.#1.........: 44548.3 MH/s (52.13ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

* Hash-Mode 5600 (NetNTLMv2)

Speed.#1.........:  3242.5 MH/s (90.12ms) @ Accel:16 Loops:512 Thr:512 Vec:1

* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)

Speed.#1.........:  1712.6 MH/s (85.21ms) @ Accel:64 Loops:1024 Thr:32 Vec:1

* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]

Speed.#1.........: 18864.4 kH/s (56.12ms) @ Accel:64 Loops:500 Thr:512 Vec:1

* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]

Speed.#1.........:    92117 H/s (50.58ms) @ Accel:2 Loops:32 Thr:40 Vec:1

* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]

Speed.#1.........:   334.7 kH/s (77.39ms) @ Accel:16384 Loops:256 Thr:32 Vec:1

* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)

Speed.#1.........:  1375.1 MH/s (52.99ms) @ Accel:256 Loops:128 Thr:32 Vec:1

* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)

Speed.#1.........:  1259.1 MH/s (57.90ms) @ Accel:256 Loops:128 Thr:32 Vec:1

* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]

Speed.#1.........:   122.2 kH/s (49.59ms) @ Accel:8 Loops:512 Thr:512 Vec:1

* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]

Speed.#1.........:    69408 H/s (81.65ms) @ Accel:8 Loops:256 Thr:512 Vec:1

* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]

Speed.#1.........:   870.9 kH/s (79.09ms) @ Accel:128 Loops:31 Thr:256 Vec:1

* Hash-Mode 11600 (7-Zip) [Iterations: 16384]

Speed.#1.........:   596.7 kH/s (88.03ms) @ Accel:128 Loops:4096 Thr:32 Vec:1

* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]

Speed.#1.........:   104.3 kH/s (84.72ms) @ Accel:8 Loops:16384 Thr:256 Vec:1

* Hash-Mode 13000 (RAR5) [Iterations: 32799]

Speed.#1.........:    76946 H/s (57.87ms) @ Accel:16 Loops:256 Thr:512 Vec:1

* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]

Speed.#1.........:   531.9 kH/s (60.43ms) @ Accel:8 Loops:256 Thr:512 Vec:1

* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]

Speed.#1.........:    89640 H/s (66.34ms) @ Accel:32 Loops:512 Thr:128 Vec:1

* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]

Speed.#1.........:  4872.2 kH/s (45.16ms) @ Accel:32 Loops:124 Thr:512 Vec:1

* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]

Speed.#1.........:     9367 H/s (77.95ms) @ Accel:16 Loops:512 Thr:256 Vec:1
```
