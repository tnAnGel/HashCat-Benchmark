# NVIDIA GeForce RTX 2080 SUPER (Host also had TITAN V cards (skipped) — card is device #4)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 2080 SUPER
- **Конфигурация / Setup:** Host also had TITAN V cards (skipped) — card is device #4
- **Версия hashcat / Version:** v5.1.0
- **Источник / Source:** [epixoip](https://gist.github.com/epixoip/47098d25f171ec1808b519615be1b90d)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 40116.1 MH/s |
| 100 | SHA1 | 13988.8 MH/s |
| 1400 | SHA2-256 | 5736.9 MH/s |
| 1700 | SHA2-512 | 1839.9 MH/s |
| 1000 | NTLM | 69962.0 MH/s |
| 3200 | bcrypt | 27477 H/s |
| 1800 | sha512crypt | 201.6 kH/s |
| 2500 | WPA/WPA2 (legacy) | 651.7 kH/s |
| 7500 | Kerberos AS-REQ (23) | 494.4 MH/s |
| 13100 | Kerberos TGS-REP (23) | 493.2 MH/s |
| 11300 | Bitcoin wallet.dat | 8306 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.1.0-1243-gd1f473d6) starting in benchmark mode...

CUDA API (CUDA 10.1)
====================
* Device #1: TITAN V, skipped
* Device #2: Graphics Device, skipped

OpenCL API (OpenCL 1.2 CUDA 10.1.120) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #3: TITAN V, skipped
* Device #4: Graphics Device, 1995/7982 MB allocatable, 48MCU

Benchmark relevant options:
===========================
* --benchmark-all
* --backend-devices=4
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#4.........: 40116.1 MH/s (80.23ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#4.........: 13988.8 MH/s (230.20ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 900 - MD4

Speed.#4.........: 69858.5 MH/s (46.05ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#4.........: 69962.0 MH/s (45.98ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#4.........:  5736.9 MH/s (280.64ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#4.........:  1839.9 MH/s (437.58ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#4.........:   201.6 kH/s (387.86ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#4.........:   651.7 kH/s (300.95ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 3000 - LM

Speed.#4.........: 36468.2 MH/s (88.21ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#4.........:    27477 H/s (150.20ms) @ Accel:8 Loops:32 Thr:11 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#4.........: 40047.2 MH/s (80.37ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#4.........:  2719.7 MH/s (296.02ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#4.........:   494.4 MH/s (407.18ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 10800 - SHA2-384

Speed.#4.........:  1653.6 MH/s (243.41ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#4.........:     8306 H/s (481.62ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#4.........:    50720 H/s (242.06ms) @ Accel:4 Loops:16384 Thr:1024 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#4.........:    66540 H/s (367.82ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#4.........:   493.2 MH/s (408.13ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#4.........:    42443 H/s (770.43ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 14600 - LUKS (Iterations: 163044)

Speed.#4.........:    16639 H/s (296.10ms) @ Accel:32 Loops:512 Thr:1024 Vec:1
```
