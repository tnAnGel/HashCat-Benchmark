# AMD Radeon RX 580 2048SP

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 580 2048SP (32 MCU; 8064/8192 MB)
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [PHCS-gh — полный raw benchmark](https://raw.githubusercontent.com/PHCS-gh/Hashcat-benchmark/main/AMD/AMD%20RX%20580%202048SP%2C%2032MCU)
- **Бэкенд / Backend:** HIP API (HIP 4.4)
- **Параметры / Options:** `--backend-devices=1 --optimized-kernel-enable --workload-profile=4`
- **Примечание / Note:** отдельный SKU 2048SP; не объединять с обычной RX 580.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 10105.8 MH/s |
| 100 | SHA1 | 3561.5 MH/s |
| 1400 | SHA2-256 | 1560.7 MH/s |
| 1700 | SHA2-512 | 430.4 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 177.2 kH/s |
| 1000 | NTLM | 19555.7 MH/s |

## Raw benchmark output

```text
Hashcat 6.2.6
AMD driver Adrenalin 22.5.1
Stock clocks
-----------------------------------------------------------------------------

HIP API (HIP 4.4)
=================
* Device #1: AMD Radeon RX 580 2048SP, 8064/8192 MB, 32MCU

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

* Hash-Mode 0 (MD5)
Speed.#1.........: 10105.8 MH/s (211.24ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

* Hash-Mode 100 (SHA1)
Speed.#1.........: 3561.5 MH/s (300.43ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

* Hash-Mode 1400 (SHA2-256)
Speed.#1.........: 1560.7 MH/s (342.83ms) @ Accel:512 Loops:512 Thr:64 Vec:1

* Hash-Mode 1700 (SHA2-512)
Speed.#1.........: 430.4 MH/s (311.09ms) @ Accel:256 Loops:256 Thr:64 Vec:1

* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
Speed.#1.........: 177.2 kH/s (367.88ms) @ Accel:512 Loops:256 Thr:64 Vec:1

* Hash-Mode 1000 (NTLM)
Speed.#1.........: 19555.7 MH/s (109.01ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

* Hash-Mode 3000 (LM)
Speed.#1.........: 10160.1 MH/s (209.97ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
Speed.#1.........: 10616.8 MH/s (200.99ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

* Hash-Mode 5600 (NetNTLMv2)
Speed.#1.........: 683.6 MH/s (391.49ms) @ Accel:512 Loops:256 Thr:64 Vec:1

* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
Speed.#1.........: 378.4 MH/s (354.21ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
Speed.#1.........: 4146.2 kH/s (477.19ms) @ Accel:1024 Loops:1000 Thr:64 Vec:1

* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
Speed.#1.........: 6275 H/s (314.07ms) @ Accel:8 Loops:16 Thr:16 Vec:1

* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
Speed.#1.........: 74540 H/s (341.91ms) @ Accel:2048 Loops:1024 Thr:64 Vec:1

* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
Speed.#1.........: 128.6 MH/s (260.19ms) @ Accel:256 Loops:64 Thr:64 Vec:1

* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
Speed.#1.........: 111.7 MH/s (299.78ms) @ Accel:256 Loops:64 Thr:64 Vec:1

* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
Speed.#1.........: 30292 H/s (368.38ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
Speed.#1.........: 14262 H/s (361.71ms) @ Accel:256 Loops:128 Thr:64 Vec:1

* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
Speed.#1.........: 180.1 kH/s (320.91ms) @ Accel:256 Loops:127 Thr:64 Vec:1

* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
Speed.#1.........: 198.5 kH/s (311.94ms) @ Accel:128 Loops:4096 Thr:64 Vec:1

* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
Speed.#1.........: 26661 H/s (306.11ms) @ Accel:64 Loops:16384 Thr:64 Vec:1

* Hash-Mode 13000 (RAR5) [Iterations: 32799]
Speed.#1.........: 19439 H/s (419.45ms) @ Accel:256 Loops:512 Thr:64 Vec:1

* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
Speed.#1.........: 105.9 kH/s (315.45ms) @ Accel:256 Loops:128 Thr:64 Vec:1

* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
Speed.#1.........: 33363 H/s (326.90ms) @ Accel:16 Loops:1024 Thr:512 Vec:1

* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
Speed.#1.........: 1245.7 kH/s (272.59ms) @ Accel:512 Loops:249 Thr:64 Vec:1

* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
Speed.#1.........: 2038 H/s (327.91ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
```
