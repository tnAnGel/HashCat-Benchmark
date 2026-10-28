# NVIDIA Quadro RTX 4000

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Quadro RTX 4000
- **Версия hashcat / Version:** v6.2.1
- **Источник / Source:** [ventaquil](https://gist.github.com/ventaquil/dd40a32b7c1cb3eff6fdacbd30da5580)
- **Нестандартные опции / Non-standard options:** прогон выполнен с `--benchmark-all`, `--backend-devices=1`, `--optimized-kernel-enable`, `--workload-profile=4`

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 25124.9 MH/s |
| 100 | SHA1 | 8668.6 MH/s |
| 1400 | SHA2-256 | 3719.4 MH/s |
| 1700 | SHA2-512 | 1205.4 MH/s |
| 1000 | NTLM | 45905.3 MH/s |
| 3200 | bcrypt | 27977 H/s |
| 1800 | sha512crypt | 183.0 kH/s |
| 500 | md5crypt | 12133.0 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 426.4 kH/s |
| 7500 | Kerberos AS-REQ (23) | 349.5 MH/s |
| 13100 | Kerberos TGS-REP (23) | 348.5 MH/s |
| 11300 | Bitcoin wallet.dat | 5384 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 325.3 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.1) starting in benchmark mode...

CUDA API (CUDA 11.2)
====================
* Device #1: Quadro RTX 4000, 7886/7982 MB, 36MCU

OpenCL API (OpenCL 1.2 CUDA 11.2.162) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #2: Quadro RTX 4000, skipped

Benchmark relevant options:
===========================
* --benchmark-all
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 25124.9 MH/s (95.65ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 10 - md5($pass.$salt)

Speed.#1.........: 25085.0 MH/s (95.80ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 11 - Joomla < 2.5.18

Speed.#1.........: 24514.8 MH/s (98.04ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 12 - PostgreSQL

Speed.#1.........: 24472.4 MH/s (98.21ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 20 - md5($salt.$pass)

Speed.#1.........: 14160.0 MH/s (170.10ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 21 - osCommerce, xt:Commerce

Speed.#1.........: 14171.0 MH/s (169.98ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 22 - Juniper NetScreen/SSG (ScreenOS)

Speed.#1.........: 14145.2 MH/s (170.29ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 23 - Skype

Speed.#1.........: 14113.5 MH/s (170.67ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 24 - SolarWinds Serv-U

Speed.#1.........: 14129.7 MH/s (170.48ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 30 - md5(utf16le($pass).$salt)

Speed.#1.........: 23745.0 MH/s (101.23ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 40 - md5($salt.utf16le($pass))

Speed.#1.........: 14199.1 MH/s (169.64ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 50 - HMAC-MD5 (key = $pass)

Speed.#1.........:  4225.1 MH/s (285.39ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 60 - HMAC-MD5 (key = $salt)

Speed.#1.........:  9095.7 MH/s (265.11ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........:  8668.6 MH/s (278.19ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 101 - nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.#1.........:  8650.9 MH/s (278.76ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 110 - sha1($pass.$salt)

Speed.#1.........:  8727.4 MH/s (276.32ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 111 - nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.#1.........:  8650.6 MH/s (278.78ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 112 - Oracle S: Type (Oracle 11+)

Speed.#1.........:  8711.5 MH/s (276.82ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 120 - sha1($salt.$pass)

Speed.#1.........:  6613.8 MH/s (364.77ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 121 - SMF (Simple Machines Forum) > v1.1

Speed.#1.........:  6603.8 MH/s (365.34ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 122 - macOS v10.4, macOS v10.5, MacOS v10.6

Speed.#1.........:  6593.6 MH/s (365.90ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 124 - Django (SHA-1)

Speed.#1.........:  6584.6 MH/s (366.40ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 125 - ArubaOS

Speed.#1.........:  6579.9 MH/s (366.66ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 130 - sha1(utf16le($pass).$salt)

Speed.#1.........:  8728.5 MH/s (276.29ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 131 - MSSQL (2000)

Speed.#1.........:  8717.8 MH/s (276.63ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 132 - MSSQL (2005)

Speed.#1.........:  8717.3 MH/s (276.63ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 133 - PeopleSoft

Speed.#1.........:  8648.7 MH/s (278.85ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 140 - sha1($salt.utf16le($pass))

Speed.#1.........:  6620.8 MH/s (364.39ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 141 - Episerver 6.x < .NET 4

Speed.#1.........:  6616.7 MH/s (364.62ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 150 - HMAC-SHA1 (key = $pass)

Speed.#1.........:  1936.7 MH/s (311.35ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 160 - HMAC-SHA1 (key = $salt)

Speed.#1.........:  3633.6 MH/s (331.94ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 200 - MySQL323

Speed.#1.........: 64728.0 MH/s (36.82ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 300 - MySQL4.1/MySQL5

Speed.#1.........:  3751.0 MH/s (321.53ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 400 - phpass (Iterations: 2048)

Speed.#1.........:  7301.6 kH/s (157.50ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 12133.0 kH/s (187.16ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 501 - Juniper IVE (Iterations: 1000)

Speed.#1.........: 12127.7 kH/s (187.23ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 600 - BLAKE2b-512

Speed.#1.........:  2045.4 MH/s (294.78ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 900 - MD4

Speed.#1.........: 45813.9 MH/s (52.23ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 45905.3 MH/s (52.12ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1100 - Domain Cached Credentials (DCC), MS Cache

Speed.#1.........: 12052.2 MH/s (199.95ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1300 - SHA2-224

Speed.#1.........:  3624.3 MH/s (332.79ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  3719.4 MH/s (324.26ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1410 - sha256($pass.$salt)

Speed.#1.........:  3714.8 MH/s (324.67ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 1411 - SSHA-256(Base64), LDAP {SSHA256}

Speed.#1.........:  3704.5 MH/s (325.57ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1420 - sha256($salt.$pass)

Speed.#1.........:  3305.6 MH/s (364.92ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1421 - hMailServer

Speed.#1.........:  3303.0 MH/s (365.22ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1430 - sha256(utf16le($pass).$salt)

Speed.#1.........:  3704.5 MH/s (325.58ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1440 - sha256($salt.utf16le($pass))

Speed.#1.........:  3309.4 MH/s (364.51ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1441 - Episerver 6.x >= .NET 4

Speed.#1.........:  3300.5 MH/s (365.49ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1450 - HMAC-SHA256 (key = $pass)

Speed.#1.........:   678.2 MH/s (444.76ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 1460 - HMAC-SHA256 (key = $salt)

Speed.#1.........:  1526.5 MH/s (394.60ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1037.3 MH/s (290.43ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 1600 - Apache $apr1$ MD5, md5apr1, MD5 (APR) (Iterations: 1000)

Speed.#1.........: 12169.9 kH/s (186.53ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1205.4 MH/s (250.02ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 1710 - sha512($pass.$salt)

Speed.#1.........:  1201.1 MH/s (250.93ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 1711 - SSHA-512(Base64), LDAP {SSHA512}

Speed.#1.........:  1204.9 MH/s (250.12ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 1720 - sha512($salt.$pass)

Speed.#1.........:  1143.8 MH/s (263.52ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 1722 - macOS v10.7

Speed.#1.........:  1135.9 MH/s (265.43ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 1730 - sha512(utf16le($pass).$salt)

Speed.#1.........:  1200.1 MH/s (251.20ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 1731 - MSSQL (2012, 2014)

Speed.#1.........:  1196.2 MH/s (251.96ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 1740 - sha512($salt.utf16le($pass))

Speed.#1.........:  1136.7 MH/s (265.17ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 1750 - HMAC-SHA512 (key = $pass)

Speed.#1.........:   253.1 MH/s (297.76ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Hashmode: 1760 - HMAC-SHA512 (key = $salt)

Speed.#1.........:   521.0 MH/s (289.30ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   183.0 kH/s (319.80ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 2000 - STDOUT

Speed.#1.........: 28413.5 GH/s (0.01ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2100 - Domain Cached Credentials 2 (DCC2), MS Cache 2 (Iterations: 10239)

Speed.#1.........:   349.6 kH/s (335.93ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 2400 - Cisco-PIX MD5

Speed.#1.........: 17925.5 MH/s (134.27ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2410 - Cisco-ASA MD5

Speed.#1.........: 16199.5 MH/s (148.63ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#1.........:   427.2 kH/s (344.07ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 2501 - WPA-EAPOL-PMK (Iterations: 0)

Speed.#1.........:   284.5 MH/s (0.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2600 - md5(md5($pass))

Speed.#1.........:  7652.1 MH/s (315.22ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2611 - vBulletin < v3.8.5

Speed.#1.........:  7629.6 MH/s (316.14ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2612 - PHPS

Speed.#1.........:  7617.8 MH/s (316.64ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2711 - vBulletin >= v3.8.5

Speed.#1.........:  5362.6 MH/s (450.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2811 - MyBB 1.2+, IPB2+ (Invision Power Board)

Speed.#1.........:  5808.1 MH/s (415.45ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 25193.5 MH/s (95.18ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 3100 - Oracle H: Type (Oracle 7+)

Speed.#1.........:   399.5 MH/s (377.50ms) @ Accel:64 Loops:64 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    27977 H/s (159.87ms) @ Accel:8 Loops:32 Thr:16 Vec:1

Hashmode: 3710 - md5($salt.md5($pass))

Speed.#1.........:  7140.8 MH/s (337.82ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 3711 - MediaWiki B type

Speed.#1.........:  7129.3 MH/s (338.35ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 3800 - md5($salt.$pass.$salt)

Speed.#1.........: 14202.3 MH/s (169.60ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 3910 - md5(md5($pass).md5($salt))

Speed.#1.........:  5404.4 MH/s (446.52ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4010 - md5($salt.md5($salt.$pass))

Speed.#1.........:  6368.8 MH/s (378.83ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4110 - md5($salt.md5($pass.$salt))

Speed.#1.........:  6797.7 MH/s (354.90ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4300 - md5(strtoupper(md5($pass)))

Speed.#1.........:  7648.9 MH/s (315.34ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4400 - md5(sha1($pass))

Speed.#1.........:  4632.4 MH/s (260.12ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 4500 - sha1(sha1($pass))

Speed.#1.........:  3321.4 MH/s (363.27ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4510 - sha1(sha1($pass).$salt)

Speed.#1.........:  3210.3 MH/s (375.86ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4520 - sha1($salt.sha1($pass))

Speed.#1.........:  1963.5 MH/s (307.10ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 4521 - Redmine

Speed.#1.........:  1958.8 MH/s (307.83ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 4522 - PunBB

Speed.#1.........:  3056.2 MH/s (394.76ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 4700 - sha1(md5($pass))

Speed.#1.........:  4774.8 MH/s (252.56ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 4710 - sha1(md5($pass).$salt)

Speed.#1.........:  4549.0 MH/s (265.12ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 4711 - Huawei sha1(md5($pass).$salt)

Speed.#1.........:  4539.9 MH/s (265.58ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 4800 - iSCSI CHAP authentication, MD5(CHAP)

Speed.#1.........: 15978.4 MH/s (150.68ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4900 - sha1($salt.$pass.$salt)

Speed.#1.........:  6469.0 MH/s (372.95ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 5100 - Half MD5

Speed.#1.........: 16683.1 MH/s (144.38ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 5200 - Password Safe v3 (Iterations: 2049)

Speed.#1.........:  1477.5 kH/s (317.50ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 5300 - IKE-PSK MD5

Speed.#1.........:   997.2 MH/s (302.41ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 5400 - IKE-PSK SHA1

Speed.#1.........:   409.9 MH/s (367.88ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 26633.1 MH/s (90.28ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  1905.1 MH/s (316.62ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 5700 - Cisco-IOS type 4 (SHA256)

Speed.#1.........:  3711.2 MH/s (325.07ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 5800 - Samsung Android Password/PIN (Iterations: 1023)

Speed.#1.........:  6051.5 kH/s (382.54ms) @ Accel:64 Loops:1023 Thr:1024 Vec:1

Hashmode: 6000 - RIPEMD-160

Speed.#1.........:  5743.5 MH/s (420.21ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 6100 - Whirlpool

Speed.#1.........:   314.5 MH/s (479.71ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   325.3 kH/s (419.45ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 6212 - TrueCrypt RIPEMD160 + XTS 1024 bit (Iterations: 1999)

Speed.#1.........:   198.8 kH/s (376.42ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 6213 - TrueCrypt RIPEMD160 + XTS 1536 bit (Iterations: 1999)

Speed.#1.........:   137.0 kH/s (272.32ms) @ Accel:32 Loops:64 Thr:1024 Vec:1

Hashmode: 6221 - TrueCrypt SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:   469.5 kH/s (278.48ms) @ Accel:4 Loops:999 Thr:1024 Vec:1

Hashmode: 6222 - TrueCrypt SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:   221.5 kH/s (282.23ms) @ Accel:2 Loops:999 Thr:1024 Vec:1

Hashmode: 6223 - TrueCrypt SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:   147.3 kH/s (281.23ms) @ Accel:4 Loops:499 Thr:1024 Vec:1

Hashmode: 6231 - TrueCrypt Whirlpool + XTS 512 bit (Iterations: 999)

Speed.#1.........:    36735 H/s (1992.58ms) @ Accel:8 Loops:249 Thr:1024 Vec:1

Hashmode: 6232 - TrueCrypt Whirlpool + XTS 1024 bit (Iterations: 999)

Speed.#1.........:    18291 H/s (1988.45ms) @ Accel:8 Loops:124 Thr:1024 Vec:1

Hashmode: 6233 - TrueCrypt Whirlpool + XTS 1536 bit (Iterations: 999)

Speed.#1.........:    12171 H/s (1492.48ms) @ Accel:8 Loops:62 Thr:1024 Vec:1

Hashmode: 6241 - TrueCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 999)

Speed.#1.........:   598.3 kH/s (341.24ms) @ Accel:32 Loops:249 Thr:1024 Vec:1

Hashmode: 6242 - TrueCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 999)

Speed.#1.........:   317.7 kH/s (329.16ms) @ Accel:32 Loops:124 Thr:1024 Vec:1

Hashmode: 6243 - TrueCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 999)

Speed.#1.........:   272.8 kH/s (264.90ms) @ Accel:32 Loops:62 Thr:1024 Vec:1

Hashmode: 6300 - AIX {smd5} (Iterations: 1000)

Speed.#1.........: 12031.5 kH/s (188.82ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 6400 - AIX {ssha256} (Iterations: 63)

Speed.#1.........: 20048.8 kH/s (104.86ms) @ Accel:64 Loops:63 Thr:1024 Vec:1

Hashmode: 6500 - AIX {ssha512} (Iterations: 63)

Speed.#1.........:  7543.3 kH/s (279.81ms) @ Accel:64 Loops:63 Thr:1024 Vec:1

Hashmode: 6600 - 1Password, agilekeychain (Iterations: 999)

Speed.#1.........:  3499.2 kH/s (219.82ms) @ Accel:64 Loops:499 Thr:1024 Vec:1

Hashmode: 6700 - AIX {ssha1} (Iterations: 63)

Speed.#1.........: 47662.5 kH/s (39.53ms) @ Accel:64 Loops:63 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  2558.3 kH/s (297.09ms) @ Accel:64 Loops:249 Thr:1024 Vec:1

Hashmode: 6900 - GOST R 34.11-94

Speed.#1.........:   224.0 MH/s (336.57ms) @ Accel:64 Loops:32 Thr:1024 Vec:1

Hashmode: 7000 - FortiGate (FortiOS)

Speed.#1.........:  7570.0 MH/s (318.71ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   513.3 kH/s (283.80ms) @ Accel:4 Loops:1023 Thr:1024 Vec:1

Hashmode: 7200 - GRUB 2 (Iterations: 1023)

Speed.#1.........:   513.4 kH/s (189.32ms) @ Accel:8 Loops:511 Thr:1024 Vec:1

Hashmode: 7300 - IPMI2 RAKP HMAC-SHA1

Speed.#1.........:  1104.7 MH/s (272.93ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 7400 - sha256crypt $5$, SHA256 (Unix) (Iterations: 5000)

Speed.#1.........:   321.5 kH/s (363.38ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 7401 - MySQL $A$ (sha256crypt) (Iterations: 5000)

Speed.#1.........:   300.9 kH/s (387.75ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   349.5 MH/s (431.57ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 7700 - SAP CODVN B (BCODE)

Speed.#1.........:  2306.1 MH/s (261.41ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 7701 - SAP CODVN B (BCODE) from RFC_READ_TABLE

Speed.#1.........:  2443.8 MH/s (493.78ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 7800 - SAP CODVN F/G (PASSCODE)

Speed.#1.........:  1341.2 MH/s (449.89ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 7801 - SAP CODVN F/G (PASSCODE) from RFC_READ_TABLE

Speed.#1.........:  1349.0 MH/s (447.21ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 7900 - Drupal7 (Iterations: 16384)

Speed.#1.........:    63808 H/s (288.32ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 8000 - Sybase ASE

Speed.#1.........:   452.5 MH/s (333.03ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 8100 - Citrix NetScaler (SHA1)

Speed.#1.........:  7354.8 MH/s (328.06ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 8200 - 1Password, cloudkeychain (Iterations: 39999)

Speed.#1.........:    13202 H/s (285.44ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 8300 - DNSSEC (NSEC3)

Speed.#1.........:  3168.4 MH/s (380.83ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 8400 - WBB3 (Woltlab Burning Board)

Speed.#1.........:  1336.6 MH/s (451.44ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 8500 - RACF

Speed.#1.........:  2399.6 MH/s (502.91ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 8600 - Lotus Notes/Domino 5

Speed.#1.........:   194.8 MH/s (387.16ms) @ Accel:32 Loops:64 Thr:1024 Vec:1

Hashmode: 8700 - Lotus Notes/Domino 6

Speed.#1.........: 64204.9 kH/s (293.46ms) @ Accel:16 Loops:32 Thr:1024 Vec:1

Hashmode: 8800 - Android FDE <= 4.3 (Iterations: 1999)

Speed.#1.........:   872.3 kH/s (334.34ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 8900 - scrypt (Iterations: 16384)

Speed.#1.........:     1216 H/s (41.28ms) @ Accel:36 Loops:1024 Thr:32 Vec:1

Hashmode: 9000 - Password Safe v2 (Iterations: 1000)

Speed.#1.........:   460.0 kH/s (152.53ms) @ Accel:256 Loops:1000 Thr:12 Vec:1

Hashmode: 9100 - Lotus Notes/Domino 8 (Iterations: 4999)

Speed.#1.........:   699.9 kH/s (332.33ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 9200 - Cisco-IOS $8$ (PBKDF2-SHA256) (Iterations: 19999)

Speed.#1.........:    71454 H/s (421.98ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 9300 - Cisco-IOS $9$ (scrypt) (Iterations: 16384)

Speed.#1.........:    14249 H/s (2.60ms) @ Accel:36 Loops:1024 Thr:32 Vec:1

Hashmode: 9400 - MS Office 2007 (Iterations: 50000)

Speed.#1.........:   143.7 kH/s (335.34ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 9500 - MS Office 2010 (Iterations: 100000)

Speed.#1.........:    71635 H/s (336.29ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 9600 - MS Office 2013 (Iterations: 100000)

Speed.#1.........:    10837 H/s (278.14ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 9700 - MS Office <= 2003 $0/$1, MD5 + RC4

Speed.#1.........:   315.9 MH/s (477.56ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 9710 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.#1.........:   342.7 MH/s (440.17ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 9720 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.#1.........:  2120.8 MH/s (284.27ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 9800 - MS Office <= 2003 $3/$4, SHA1 + RC4

Speed.#1.........:   352.5 MH/s (427.91ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 9810 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.#1.........:   375.8 MH/s (401.42ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 9820 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.#1.........:  3499.4 MH/s (344.77ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 9900 - Radmin2

Speed.#1.........:  9301.9 MH/s (259.30ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 10000 - Django (PBKDF2-SHA256) (Iterations: 9999)

Speed.#1.........:   142.1 kH/s (414.25ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 10100 - SipHash

Speed.#1.........: 29403.1 MH/s (81.74ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 10200 - CRAM-MD5

Speed.#1.........:  4205.2 MH/s (286.82ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 10300 - SAP CODVN H (PWDSALTEDHASH) iSSHA-1 (Iterations: 1023)

Speed.#1.........:  5788.3 kH/s (399.34ms) @ Accel:64 Loops:1023 Thr:1024 Vec:1

Hashmode: 10400 - PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.#1.........:   394.7 MH/s (382.18ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 10410 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.#1.........:   408.7 MH/s (369.07ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 10420 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.#1.........:  8080.8 MH/s (298.54ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 10500 - PDF 1.4 - 1.6 (Acrobat 5 - 8) (Iterations: 70)

Speed.#1.........: 18728.4 kH/s (118.59ms) @ Accel:1024 Loops:70 Thr:64 Vec:1

Hashmode: 10600 - PDF 1.7 Level 3 (Acrobat 9)

Speed.#1.........:  3692.4 MH/s (326.72ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 10700 - PDF 1.7 Level 8 (Acrobat 10 - 11) (Iterations: 64)

Speed.#1.........:    65452 H/s (281.21ms) @ Accel:8 Loops:4 Thr:1024 Vec:1

Hashmode: 10800 - SHA2-384

Speed.#1.........:  1188.9 MH/s (253.59ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 10900 - PBKDF2-HMAC-SHA256 (Iterations: 999)

Speed.#1.........:  1426.8 kH/s (409.12ms) @ Accel:16 Loops:999 Thr:1024 Vec:1

Hashmode: 10901 - RedHat 389-DS LDAP (PBKDF2-HMAC-SHA256) (Iterations: 8191)

Speed.#1.........:   174.5 kH/s (421.69ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 11000 - PrestaShop

Speed.#1.........: 10074.3 MH/s (239.30ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 11100 - PostgreSQL CRAM (MD5)

Speed.#1.........:  7452.3 MH/s (323.67ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 11200 - MySQL CRAM (SHA1)

Speed.#1.........:  2181.2 MH/s (276.48ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     5384 H/s (279.30ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 11400 - SIP digest authentication (MD5)

Speed.#1.........:  3593.2 MH/s (335.66ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11500 - CRC32

Speed.#1.........:  7581.3 MH/s (158.82ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   435.3 kH/s (321.79ms) @ Accel:16 Loops:4096 Thr:1024 Vec:1

Hashmode: 11700 - GOST R 34.11-2012 (Streebog) 256-bit, big-endian

Speed.#1.........: 45631.5 kH/s (413.12ms) @ Accel:8 Loops:64 Thr:1024 Vec:1

Hashmode: 11750 - HMAC-Streebog-256 (key = $pass), big-endian

Speed.#1.........: 16186.5 kH/s (291.01ms) @ Accel:8 Loops:16 Thr:1024 Vec:1

Hashmode: 11760 - HMAC-Streebog-256 (key = $salt), big-endian

Speed.#1.........: 22394.7 kH/s (420.98ms) @ Accel:2 Loops:128 Thr:1024 Vec:1

Hashmode: 11800 - GOST R 34.11-2012 (Streebog) 512-bit, big-endian

Speed.#1.........: 45689.7 kH/s (412.67ms) @ Accel:8 Loops:64 Thr:1024 Vec:1

Hashmode: 11850 - HMAC-Streebog-512 (key = $pass), big-endian

Speed.#1.........: 14177.1 kH/s (332.42ms) @ Accel:4 Loops:32 Thr:1024 Vec:1

Hashmode: 11860 - HMAC-Streebog-512 (key = $salt), big-endian

Speed.#1.........: 18631.5 kH/s (252.75ms) @ Accel:2 Loops:64 Thr:1024 Vec:1

Hashmode: 11900 - PBKDF2-HMAC-MD5 (Iterations: 999)

Speed.#1.........:  8564.0 kH/s (260.37ms) @ Accel:64 Loops:999 Thr:1024 Vec:1

Hashmode: 12000 - PBKDF2-HMAC-SHA1 (Iterations: 999)

Speed.#1.........:  3479.7 kH/s (221.39ms) @ Accel:64 Loops:499 Thr:1024 Vec:1

Hashmode: 12001 - Atlassian (PBKDF2-HMAC-SHA1) (Iterations: 9999)

Speed.#1.........:   352.4 kH/s (333.77ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 12100 - PBKDF2-HMAC-SHA512 (Iterations: 999)

Speed.#1.........:   526.2 kH/s (276.72ms) @ Accel:4 Loops:999 Thr:1024 Vec:1

Hashmode: 12200 - eCryptfs (Iterations: 65536)

Speed.#1.........:    16394 H/s (280.56ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 12300 - Oracle T: Type (Oracle 12+) (Iterations: 4095)

Speed.#1.........:   129.1 kH/s (284.49ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 12400 - BSDi Crypt, Extended DES (Iterations: 2194)

Speed.#1.........:  1843.4 kH/s (422.29ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    58877 H/s (312.63ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 12600 - ColdFusion 10+

Speed.#1.........:  2018.7 MH/s (298.69ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 12700 - Blockchain, My Wallet (Iterations: 9)

Speed.#1.........: 81348.7 kH/s (11.89ms) @ Accel:64 Loops:9 Thr:1024 Vec:1

Hashmode: 12800 - MS-AzureSync PBKDF2-HMAC-SHA256 (Iterations: 99)

Speed.#1.........: 11671.8 kH/s (177.11ms) @ Accel:64 Loops:99 Thr:1024 Vec:1

Hashmode: 12900 - Android FDE (Samsung DEK) (Iterations: 4095)

Speed.#1.........:   321.0 kH/s (456.82ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    39977 H/s (457.87ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   348.5 MH/s (432.74ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 13200 - AxCrypt 1 (Iterations: 10467)

Speed.#1.........:   100.4 kH/s (1148.16ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 13300 - AxCrypt 1 in-memory SHA1

Speed.#1.........:  8047.0 MH/s (299.71ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    30576 H/s (803.09ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 13500 - PeopleSoft PS_TOKEN

Speed.#1.........:  6210.0 MH/s (388.62ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 13600 - WinZip (Iterations: 999)

Speed.#1.........:  3441.7 kH/s (333.58ms) @ Accel:32 Loops:999 Thr:1024 Vec:1

Hashmode: 13711 - VeraCrypt RIPEMD160 + XTS 512 bit (Iterations: 655330)

Speed.#1.........:     1065 H/s (209.73ms) @ Accel:32 Loops:250 Thr:1024 Vec:1

Hashmode: 13712 - VeraCrypt RIPEMD160 + XTS 1024 bit (Iterations: 655330)

Speed.#1.........:      605 H/s (184.02ms) @ Accel:32 Loops:125 Thr:1024 Vec:1

Hashmode: 13713 - VeraCrypt RIPEMD160 + XTS 1536 bit (Iterations: 655330)

Speed.#1.........:      419 H/s (131.19ms) @ Accel:32 Loops:62 Thr:1024 Vec:1

Hashmode: 13721 - VeraCrypt SHA512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:     1068 H/s (137.76ms) @ Accel:4 Loops:1000 Thr:1024 Vec:1

Hashmode: 13722 - VeraCrypt SHA512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      508 H/s (142.80ms) @ Accel:32 Loops:62 Thr:1024 Vec:1

Hashmode: 13723 - VeraCrypt SHA512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      339 H/s (213.85ms) @ Accel:32 Loops:62 Thr:1024 Vec:1

Hashmode: 13731 - VeraCrypt Whirlpool + XTS 512 bit (Iterations: 499999)

Speed.#1.........:       74 H/s (993.91ms) @ Accel:8 Loops:250 Thr:1024 Vec:1

Hashmode: 13732 - VeraCrypt Whirlpool + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:       37 H/s (988.39ms) @ Accel:8 Loops:125 Thr:1024 Vec:1

Hashmode: 13733 - VeraCrypt Whirlpool + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:       25 H/s (737.80ms) @ Accel:2 Loops:250 Thr:1024 Vec:1

Hashmode: 13741 - VeraCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 327660)

Speed.#1.........:     2145 H/s (213.35ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 13742 - VeraCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 327660)

Speed.#1.........:     1210 H/s (188.39ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 13743 - VeraCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 327660)

Speed.#1.........:      837 H/s (135.77ms) @ Accel:32 Loops:64 Thr:1024 Vec:1

Hashmode: 13751 - VeraCrypt SHA256 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:     1422 H/s (206.63ms) @ Accel:16 Loops:500 Thr:1024 Vec:1

Hashmode: 13752 - VeraCrypt SHA256 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      749 H/s (196.27ms) @ Accel:8 Loops:500 Thr:1024 Vec:1

Hashmode: 13753 - VeraCrypt SHA256 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      500 H/s (146.95ms) @ Accel:8 Loops:250 Thr:1024 Vec:1

Hashmode: 13761 - VeraCrypt SHA256 + XTS 512 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     3553 H/s (211.70ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 13762 - VeraCrypt SHA256 + XTS 1024 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     1863 H/s (202.00ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 13763 - VeraCrypt SHA256 + XTS 1536 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     1238 H/s (151.77ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 13771 - VeraCrypt Streebog-512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:       29 H/s (640.73ms) @ Accel:1 Loops:500 Thr:1024 Vec:1

Hashmode: 13772 - VeraCrypt Streebog-512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:       14 H/s (637.29ms) @ Accel:1 Loops:250 Thr:1024 Vec:1

Hashmode: 13773 - VeraCrypt Streebog-512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:       10 H/s (478.13ms) @ Accel:1 Loops:125 Thr:1024 Vec:1

Hashmode: 13800 - Windows Phone 8+ PIN/password

Speed.#1.........:   921.4 MH/s (327.31ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 13900 - OpenCart

Speed.#1.........:  2114.8 MH/s (285.09ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 14000 - DES (PT = $salt, key = $pass)

Speed.#1.........: 24521.2 MH/s (97.97ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 14100 - 3DES (PT = $salt, key = $pass)

Speed.#1.........:  2467.4 MH/s (489.13ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 14400 - sha1(CX)

Speed.#1.........:   410.9 MH/s (367.03ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 14600 - LUKS (Iterations: 163044)

Speed.#1.........:    10769 H/s (343.37ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 14700 - iTunes backup < 10.0 (Iterations: 9999)

Speed.#1.........:   175.9 kH/s (342.24ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 14800 - iTunes backup >= 10.0 (Iterations: 9999999)

Speed.#1.........:      142 H/s (423.89ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 14900 - Skip32 (PT = $salt, key = $pass)

Speed.#1.........:  4813.9 MH/s (13.43ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 15000 - FileZilla Server >= 0.9.55

Speed.#1.........:  1103.3 MH/s (273.28ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 15100 - Juniper/NetBSD sha1crypt (Iterations: 19999)

Speed.#1.........:   176.7 kH/s (340.82ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 15200 - Blockchain, My Wallet, V2 (Iterations: 4999)

Speed.#1.........:   348.1 kH/s (345.81ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    73188 H/s (341.45ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 15400 - ChaCha20

Speed.#1.........:  4893.6 MH/s (493.26ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 15500 - JKS Java Key Store Private Keys (SHA1)

Speed.#1.........:  8216.5 MH/s (293.61ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 15600 - Ethereum Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1023)

Speed.#1.........:  1266.7 kH/s (367.18ms) @ Accel:64 Loops:255 Thr:1024 Vec:1

Hashmode: 15700 - Ethereum Wallet, SCRYPT (Iterations: 262144)

Speed.#1.........:        0 H/s (10.14ms) @ Accel:1 Loops:1024 Thr:4 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    41300 H/s (282.65ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 16000 - Tripcode

Speed.#1.........:   156.4 MH/s (482.21ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 16100 - TACACS+

Speed.#1.........: 14605.4 MH/s (164.97ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 16200 - Apple Secure Notes (Iterations: 19999)

Speed.#1.........:    65832 H/s (456.14ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 16300 - Ethereum Pre-Sale Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1999)

Speed.#1.........:   647.0 kH/s (446.46ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 16400 - CRAM-MD5 Dovecot

Speed.#1.........: 24874.3 MH/s (96.62ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 16500 - JWT (JSON Web Token)

Speed.#1.........:   632.7 MH/s (476.79ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 16600 - Electrum Wallet (Salt-Type 1-3)

Speed.#1.........:   467.3 MH/s (322.73ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 16700 - FileVault 2 (Iterations: 19999)

Speed.#1.........:    65860 H/s (455.90ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 16800 - WPA-PMKID-PBKDF2 (Iterations: 4095)

Speed.#1.........:   430.7 kH/s (341.28ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 16801 - WPA-PMKID-PMK (Iterations: 0)

Speed.#1.........:   257.5 MH/s (0.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 16900 - Ansible Vault (Iterations: 9999)

Speed.#1.........:   131.4 kH/s (457.03ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 17200 - PKZIP (Compressed)

Speed.#1.........:  3882.4 MH/s (155.06ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 17210 - PKZIP (Uncompressed)

Speed.#1.........:  1426.1 MH/s (211.25ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 17220 - PKZIP (Compressed Multi-File)

Speed.#1.........:  6177.8 MH/s (195.02ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 17225 - PKZIP (Mixed Multi-File)

Speed.#1.........:  7534.0 MH/s (320.24ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 17230 - PKZIP (Mixed Multi-File Checksum-Only)

Speed.#1.........:  7378.4 MH/s (326.93ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 17300 - SHA3-224

Speed.#1.........:   851.9 MH/s (354.04ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 17400 - SHA3-256

Speed.#1.........:   840.7 MH/s (358.81ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 17500 - SHA3-384

Speed.#1.........:   840.5 MH/s (358.78ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 17600 - SHA3-512

Speed.#1.........:   840.2 MH/s (359.02ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 17700 - Keccak-224

Speed.#1.........:   850.5 MH/s (354.65ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 17800 - Keccak-256

Speed.#1.........:   841.2 MH/s (358.56ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 17900 - Keccak-384

Speed.#1.........:   840.9 MH/s (358.62ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 18000 - Keccak-512

Speed.#1.........:   840.1 MH/s (358.95ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 18100 - TOTP (HMAC-SHA1)

Speed.#1.........:  1622.5 MH/s (371.82ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 18200 - Kerberos 5, etype 23, AS-REP

Speed.#1.........:   347.9 MH/s (433.59ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 18300 - Apple File System (APFS) (Iterations: 19999)

Speed.#1.........:    65838 H/s (456.05ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 18400 - Open Document Format (ODF) 1.2 (SHA-256, AES) (Iterations: 99999)

Speed.#1.........:    17485 H/s (344.82ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 18500 - sha1(md5(md5($pass)))

Speed.#1.........:  3149.1 MH/s (383.08ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 18600 - Open Document Format (ODF) 1.1 (SHA-1, Blowfish) (Iterations: 1023)

Speed.#1.........:   590.4 kH/s (307.19ms) @ Accel:1024 Loops:1023 Thr:12 Vec:1

Hashmode: 18700 - Java Object hashCode()

Speed.#1.........:   107.9 GH/s (21.82ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 18800 - Blockchain, My Wallet, Second Password (SHA256) (Iterations: 9999)

Speed.#1.........:   303.7 kH/s (387.64ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 18900 - Android Backup (Iterations: 9999)

Speed.#1.........:   176.2 kH/s (341.61ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 19000 - QNX /etc/shadow (MD5) (Iterations: 1000)

Speed.#1.........: 36210.6 kH/s (54.15ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 19100 - QNX /etc/shadow (SHA256) (Iterations: 1000)

Speed.#1.........: 16336.1 kH/s (131.82ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 19200 - QNX /etc/shadow (SHA512) (Iterations: 1000)

Speed.#1.........:  9002.0 kH/s (241.35ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 19300 - sha1($salt1.$pass.$salt2)

Speed.#1.........:   947.9 MH/s (318.09ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 19500 - Ruby on Rails Restful-Authentication

Speed.#1.........:   114.3 MH/s (329.68ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 19600 - Kerberos 5, etype 17, TGS-REP (Iterations: 4095)

Speed.#1.........:   859.4 kH/s (340.28ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 19700 - Kerberos 5, etype 18, TGS-REP (Iterations: 4095)

Speed.#1.........:   424.6 kH/s (344.81ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 19800 - Kerberos 5, etype 17, Pre-Auth (Iterations: 4095)

Speed.#1.........:   860.3 kH/s (340.33ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 19900 - Kerberos 5, etype 18, Pre-Auth (Iterations: 4095)

Speed.#1.........:   429.3 kH/s (342.35ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 20011 - DiskCryptor SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:   468.8 kH/s (278.94ms) @ Accel:4 Loops:999 Thr:1024 Vec:1

Hashmode: 20012 - DiskCryptor SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:   223.7 kH/s (187.42ms) @ Accel:4 Loops:499 Thr:1024 Vec:1

Hashmode: 20013 - DiskCryptor SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:   147.1 kH/s (281.41ms) @ Accel:4 Loops:499 Thr:1024 Vec:1

Hashmode: 20200 - Python passlib pbkdf2-sha512 (Iterations: 24999)

Speed.#1.........:    21180 H/s (284.68ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 20300 - Python passlib pbkdf2-sha256 (Iterations: 28999)

Speed.#1.........:    48869 H/s (425.25ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 20400 - Python passlib pbkdf2-sha1 (Iterations: 130999)

Speed.#1.........:    26844 H/s (342.16ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 20500 - PKZIP Master Key

Speed.#1.........: 89175.4 MH/s (26.69ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 20510 - PKZIP Master Key (6 byte optimization)

Speed.#1.........: 17035.1 MH/s (141.39ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 20600 - Oracle Transportation Management (SHA256) (Iterations: 999)

Speed.#1.........:  3013.5 kH/s (387.03ms) @ Accel:32 Loops:999 Thr:1024 Vec:1

Hashmode: 20710 - sha256(sha256($pass).$salt)

Speed.#1.........:  1110.7 MH/s (271.45ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 20711 - AuthMe sha256

Speed.#1.........:  1105.8 MH/s (272.68ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 20800 - sha256(md5($pass))

Speed.#1.........:  2792.6 MH/s (432.05ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 20900 - md5(sha1($pass).md5($pass).sha1($pass))

Speed.#1.........:  2616.4 MH/s (461.26ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 21000 - BitShares v0.x - sha512(sha512_bin(pass))

Speed.#1.........:   544.9 MH/s (276.63ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 21100 - sha1(md5($pass.$salt))

Speed.#1.........:  4816.3 MH/s (250.38ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 21200 - md5(sha1($salt).md5($pass))

Speed.#1.........:  5892.7 MH/s (409.48ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 21300 - md5($salt.sha1($salt.$pass))

Speed.#1.........:  3415.7 MH/s (353.00ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 21400 - sha256(sha256_bin($pass))

Speed.#1.........:  1499.4 MH/s (402.31ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 21500 - SolarWinds Orion (Iterations: 999)

Speed.#1.........:    65645 H/s (276.52ms) @ Accel:8 Loops:62 Thr:1024 Vec:1

Hashmode: 21501 - SolarWinds Orion v2 (Iterations: 999)

Speed.#1.........:    65506 H/s (277.15ms) @ Accel:8 Loops:62 Thr:1024 Vec:1

Hashmode: 21600 - Web2py pbkdf2-sha512 (Iterations: 999)

Speed.#1.........:   524.1 kH/s (278.03ms) @ Accel:4 Loops:999 Thr:1024 Vec:1

Hashmode: 21700 - Electrum Wallet (Salt-Type 4) (Iterations: 1023)

Speed.#1.........:   360.6 kH/s (284.07ms) @ Accel:4 Loops:1023 Thr:1024 Vec:1

Hashmode: 21800 - Electrum Wallet (Salt-Type 5) (Iterations: 1023)

Speed.#1.........:   361.2 kH/s (284.13ms) @ Accel:4 Loops:1023 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   426.4 kH/s (344.73ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 22001 - WPA-PMK-PMKID+EAPOL (Iterations: 0)

Speed.#1.........:   253.1 MH/s (0.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 22100 - BitLocker (Iterations: 1048576)

Speed.#1.........:     1479 H/s (389.05ms) @ Accel:4 Loops:4096 Thr:1024 Vec:1

Hashmode: 22200 - Citrix NetScaler (SHA512)

Speed.#1.........:  1194.5 MH/s (252.31ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 22300 - sha256($salt.$pass.$salt)

Speed.#1.........:  3264.0 MH/s (369.58ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 22301 - Telegram Mobile App Passcode (SHA256)

Speed.#1.........:  3249.1 MH/s (371.36ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 22400 - AES Crypt (SHA256) (Iterations: 8191)

Speed.#1.........:   337.7 kH/s (431.97ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 22500 - MultiBit Classic .key (MD5)

Speed.#1.........:   500.3 MH/s (301.39ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 22600 - Telegram Desktop < v2.1.14 (PBKDF2-HMAC-SHA1) (Iterations: 3999)

Speed.#1.........:   124.8 kH/s (293.99ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 22700 - MultiBit HD (scrypt) (Iterations: 16384)

Speed.#1.........:     1261 H/s (41.33ms) @ Accel:36 Loops:1024 Thr:32 Vec:1

Hashmode: 22911 - RSA/DSA/EC/OpenSSH Private Keys ($0$)

Speed.#1.........:   529.0 MH/s (284.91ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 22921 - RSA/DSA/EC/OpenSSH Private Keys ($6$)

Speed.#1.........:  1718.9 MH/s (350.87ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 22931 - RSA/DSA/EC/OpenSSH Private Keys ($1, $3$)

Speed.#1.........:   682.5 MH/s (442.09ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 22941 - RSA/DSA/EC/OpenSSH Private Keys ($4$)

Speed.#1.........:   566.7 MH/s (265.93ms) @ Accel:64 Loops:64 Thr:1024 Vec:1

Hashmode: 22951 - RSA/DSA/EC/OpenSSH Private Keys ($5$)

Speed.#1.........:   476.7 MH/s (316.28ms) @ Accel:64 Loops:64 Thr:1024 Vec:1

Hashmode: 23001 - SecureZIP AES-128

Speed.#1.........:   677.3 MH/s (445.45ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 23002 - SecureZIP AES-192

Speed.#1.........:   533.3 MH/s (282.69ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 23003 - SecureZIP AES-256

Speed.#1.........:   455.3 MH/s (331.14ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 23100 - Apple Keychain (Iterations: 999)

Speed.#1.........:  1746.0 kH/s (266.79ms) @ Accel:64 Loops:249 Thr:1024 Vec:1

Hashmode: 23200 - XMPP SCRAM PBKDF2-SHA1 (Iterations: 4095)

Speed.#1.........:   859.7 kH/s (340.94ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 23300 - Apple iWork (Iterations: 3999)

Speed.#1.........:   887.1 kH/s (330.13ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 23400 - Bitwarden (Iterations: 99999)

Speed.#1.........:    13286 H/s (451.93ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 23500 - AxCrypt 2 AES-128 (Iterations: 999)

Speed.#1.........:    47019 H/s (260.69ms) @ Accel:4 Loops:999 Thr:1024 Vec:1

Hashmode: 23600 - AxCrypt 2 AES-256 (Iterations: 999)

Speed.#1.........:    22952 H/s (534.74ms) @ Accel:4 Loops:999 Thr:1024 Vec:1

Hashmode: 23700 - RAR3-p (Uncompressed) (Iterations: 262144)

Speed.#1.........:    58729 H/s (313.41ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 23800 - RAR3-p (Compressed) (Iterations: 262144)

Speed.#1.........:    58832 H/s (312.87ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 23900 - BestCrypt v3 Volume Encryption (Iterations: 1)

Speed.#1.........:  2409.7 kH/s (472.59ms) @ Accel:32 Loops:1 Thr:1024 Vec:1

Hashmode: 24100 - MongoDB ServerKey SCRAM-SHA-1 (Iterations: 9999)

Speed.#1.........:   348.6 kH/s (337.39ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 24200 - MongoDB ServerKey SCRAM-SHA-256 (Iterations: 14999)

Speed.#1.........:    87452 H/s (457.80ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 24300 - sha1($salt.sha1($pass.$salt))

Speed.#1.........:  3087.8 MH/s (390.69ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 24410 - PKCS#8 Private Keys (PBKDF2-HMAC-SHA1 + 3DES/AES) (Iterations: 2047)

Speed.#1.........:   849.2 kH/s (344.68ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 24420 - PKCS#8 Private Keys (PBKDF2-HMAC-SHA256 + 3DES/AES) (Iterations: 2047)

Speed.#1.........:   689.2 kH/s (425.03ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 24500 - Telegram Desktop >= v2.1.14 (PBKDF2-HMAC-SHA512) (Iterations: 99999)

Speed.#1.........:     1740 H/s (433.17ms) @ Accel:4 Loops:512 Thr:1024 Vec:1

Hashmode: 24600 - SQLCipher (Iterations: 63999)

Speed.#1.........:    27445 H/s (342.66ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 24700 - Stuffit5

Speed.#1.........:  9146.4 MH/s (263.63ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 24800 - Umbraco HMAC-SHA1

Speed.#1.........:  1752.6 MH/s (344.11ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 24900 - Dahua Authentication MD5

Speed.#1.........: 13741.6 MH/s (175.30ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 25300 - MS Office 2016 - SheetProtection (Iterations: 100000)

Speed.#1.........:    10701 H/s (281.66ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 25400 - PDF 1.4 - 1.6 (Acrobat 5 - 8) - edit password (Iterations: 70)

Speed.#1.........: 18753.9 kH/s (118.67ms) @ Accel:1024 Loops:70 Thr:64 Vec:1

Hashmode: 25500 - Stargazer Stellar Wallet XLM (Iterations: 4095)

Speed.#1.........:   347.5 kH/s (420.35ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 25900 - KNX IP Secure - Device Authentication Code (Iterations: 65535)

Speed.#1.........:    20096 H/s (455.85ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 26000 - Mozilla key3.db

Speed.#1.........:   118.8 MH/s (317.30ms) @ Accel:32 Loops:32 Thr:1024 Vec:1

Hashmode: 26100 - Mozilla key4.db (Iterations: 9999)

Speed.#1.........:   142.2 kH/s (413.92ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 99999 - Plaintext

Speed.#1.........: 45335.7 MH/s (52.78ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Started: Wed Jun  9 17:22:16 2021

Stopped: Wed Jun  9 18:22:22 2021
```
