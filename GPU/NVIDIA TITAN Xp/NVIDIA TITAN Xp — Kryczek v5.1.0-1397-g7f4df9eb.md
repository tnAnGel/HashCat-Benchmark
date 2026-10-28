# NVIDIA TITAN Xp

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA TITAN Xp
- **Версия hashcat / Version:** v5.1.0-1397-g7f4df9eb
- **Источник / Source:** [Kryczek](https://hashcat.net/forum/thread-8662.html)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 40378.4 MH/s |
| 100 | SHA1 | 13359.0 MH/s |
| 1400 | SHA2-256 | 4939.4 MH/s |
| 1700 | SHA2-512 | 1597.0 MH/s |
| 1000 | NTLM | 71313.5 MH/s |
| 3200 | bcrypt | 35113 H/s |
| 1800 | sha512crypt | 235.5 kH/s |
| 500 | md5crypt | 15702.8 kH/s |
| 7500 | Kerberos AS-REQ (23) | 470.2 MH/s |
| 13100 | Kerberos TGS-REP (23) | 474.1 MH/s |
| 11300 | Bitcoin wallet.dat | 7272 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 440.7 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.1.0-1397-g7f4df9eb) starting in benchmark mode...

CUDA API (CUDA 10.2)
====================
* Device #1: TITAN Xp, 12196 MB, 30MCU

OpenCL API (OpenCL 1.2 CUDA 10.2.120) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #2: TITAN Xp, skipped

Benchmark relevant options:
===========================
* --benchmark-all
* --backend-devices=1
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 40378.4 MH/s (98.75ms) @ Accel:128 Loops:1024 Thr:1024 Vec:8

Hashmode: 10 - md5($pass.$salt)

Speed.#1.........: 40474.7 MH/s (98.94ms) @ Accel:128 Loops:1024 Thr:1024 Vec:8

Hashmode: 11 - Joomla < 2.5.18

Speed.#1.........: 39238.3 MH/s (102.07ms) @ Accel:128 Loops:1024 Thr:1024 Vec:8

Hashmode: 12 - PostgreSQL

Speed.#1.........: 39021.0 MH/s (102.30ms) @ Accel:128 Loops:1024 Thr:1024 Vec:8

Hashmode: 20 - md5($salt.$pass)

Speed.#1.........: 23831.4 MH/s (168.43ms) @ Accel:128 Loops:1024 Thr:1024 Vec:4

Hashmode: 21 - osCommerce, xt:Commerce

Speed.#1.........: 23576.0 MH/s (170.07ms) @ Accel:128 Loops:1024 Thr:1024 Vec:4

Hashmode: 22 - Juniper NetScreen/SSG (ScreenOS)

Speed.#1.........: 23099.1 MH/s (173.55ms) @ Accel:128 Loops:1024 Thr:1024 Vec:4

Hashmode: 23 - Skype

Speed.#1.........: 23440.7 MH/s (171.05ms) @ Accel:128 Loops:1024 Thr:1024 Vec:4

Hashmode: 30 - md5(utf16le($pass).$salt)

Speed.#1.........: 39604.0 MH/s (100.77ms) @ Accel:128 Loops:1024 Thr:1024 Vec:4

Hashmode: 40 - md5($salt.utf16le($pass))

Speed.#1.........: 23462.8 MH/s (171.07ms) @ Accel:128 Loops:1024 Thr:1024 Vec:4

Hashmode: 50 - HMAC-MD5 (key = $pass)

Speed.#1.........:  6079.2 MH/s (330.69ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 60 - HMAC-MD5 (key = $salt)

Speed.#1.........: 12257.6 MH/s (325.89ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........: 13359.0 MH/s (300.85ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 101 - nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.#1.........: 13364.2 MH/s (300.80ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 110 - sha1($pass.$salt)

Speed.#1.........: 13467.9 MH/s (298.45ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 111 - nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.#1.........: 13359.0 MH/s (300.93ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 112 - Oracle S: Type (Oracle 11+)

Speed.#1.........: 13467.1 MH/s (298.50ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 120 - sha1($salt.$pass)

Speed.#1.........: 11067.3 MH/s (363.30ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 121 - SMF (Simple Machines Forum) > v1.1

Speed.#1.........: 11058.7 MH/s (363.66ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 122 - macOS v10.4, macOS v10.5, MacOS v10.6

Speed.#1.........: 11033.0 MH/s (364.15ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 124 - Django (SHA-1)

Speed.#1.........: 11031.9 MH/s (364.51ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 125 - ArubaOS

Speed.#1.........: 11026.6 MH/s (364.65ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 130 - sha1(utf16le($pass).$salt)

Speed.#1.........: 13473.9 MH/s (297.78ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 131 - MSSQL (2000)

Speed.#1.........: 13461.5 MH/s (298.08ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 132 - MSSQL (2005)

Speed.#1.........: 13465.7 MH/s (298.15ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 133 - PeopleSoft

Speed.#1.........: 13376.3 MH/s (300.55ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 140 - sha1($salt.utf16le($pass))

Speed.#1.........: 11059.0 MH/s (363.63ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 141 - Episerver 6.x < .NET 4

Speed.#1.........: 11045.5 MH/s (363.52ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 150 - HMAC-SHA1 (key = $pass)

Speed.#1.........:  2899.8 MH/s (346.44ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 160 - HMAC-SHA1 (key = $salt)

Speed.#1.........:  5602.7 MH/s (358.74ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 200 - MySQL323

Speed.#1.........: 80207.1 MH/s (49.20ms) @ Accel:128 Loops:1024 Thr:1024 Vec:8

Hashmode: 300 - MySQL4.1/MySQL5

Speed.#1.........:  6032.3 MH/s (333.12ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 400 - phpass (Iterations: 2048)

Speed.#1.........: 10654.7 kH/s (178.81ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 15702.8 kH/s (241.00ms) @ Accel:128 Loops:1000 Thr:1024 Vec:1

Hashmode: 501 - Juniper IVE (Iterations: 1000)

Speed.#1.........: 15668.1 kH/s (240.97ms) @ Accel:128 Loops:1000 Thr:1024 Vec:1

Hashmode: 600 - BLAKE2b-512

Speed.#1.........:  2621.1 MH/s (382.89ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 900 - MD4

Speed.#1.........: 70266.0 MH/s (56.40ms) @ Accel:128 Loops:1024 Thr:1024 Vec:8

Hashmode: 1000 - NTLM

Speed.#1.........: 71313.5 MH/s (55.91ms) @ Accel:128 Loops:1024 Thr:1024 Vec:8

Hashmode: 1100 - Domain Cached Credentials (DCC), MS Cache

Speed.#1.........: 19512.3 MH/s (205.81ms) @ Accel:128 Loops:1024 Thr:1024 Vec:4

Hashmode: 1300 - SHA2-224

Speed.#1.........:  4799.4 MH/s (416.59ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  4939.4 MH/s (407.11ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1410 - sha256($pass.$salt)

Speed.#1.........:  4951.4 MH/s (406.05ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1411 - SSHA-256(Base64), LDAP {SSHA256}

Speed.#1.........:  4938.2 MH/s (407.13ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1420 - sha256($salt.$pass)

Speed.#1.........:  4396.5 MH/s (457.11ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1421 - hMailServer

Speed.#1.........:  4407.2 MH/s (456.25ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1430 - sha256(utf16le($pass).$salt)

Speed.#1.........:  4951.6 MH/s (405.99ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1440 - sha256($salt.utf16le($pass))

Speed.#1.........:  4407.3 MH/s (456.21ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1441 - Episerver 6.x >= .NET 4

Speed.#1.........:  4406.0 MH/s (456.33ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1450 - HMAC-SHA256 (key = $pass)

Speed.#1.........:  877.9 MH/s (285.65ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 1460 - HMAC-SHA256 (key = $salt)

Speed.#1.........:  2041.6 MH/s (245.80ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1385.5 MH/s (361.15ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1600 - Apache $apr1$ MD5, md5apr1, MD5 (APR) (Iterations: 1000)

Speed.#1.........: 14923.1 kH/s (241.65ms) @ Accel:128 Loops:1000 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1597.0 MH/s (314.61ms) @ Accel:128 Loops:128 Thr:1024 Vec:1

Hashmode: 1710 - sha512($pass.$salt)

Speed.#1.........:  1603.5 MH/s (312.97ms) @ Accel:128 Loops:128 Thr:1024 Vec:1

Hashmode: 1711 - SSHA-512(Base64), LDAP {SSHA512}

Speed.#1.........:  1573.2 MH/s (316.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1720 - sha512($salt.$pass)

Speed.#1.........:  1401.0 MH/s (358.72ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 1722 - macOS v10.7

Speed.#1.........:  1411.0 MH/s (356.22ms) @ Accel:128 Loops:128 Thr:1024 Vec:1

Hashmode: 1730 - sha512(utf16le($pass).$salt)

Speed.#1.........:  1579.2 MH/s (316.73ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1731 - MSSQL (2012, 2014)

Speed.#1.........:  1577.2 MH/s (316.79ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1740 - sha512($salt.utf16le($pass))

Speed.#1.........:  1413.2 MH/s (355.68ms) @ Accel:128 Loops:128 Thr:1024 Vec:1

Hashmode: 1750 - HMAC-SHA512 (key = $pass)

Speed.#1.........:  307.9 MH/s (408.12ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 1760 - HMAC-SHA512 (key = $salt)

Speed.#1.........:  709.7 MH/s (353.91ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:  235.5 kH/s (412.45ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 2000 - STDOUT

Speed.#1.........: 33925.5 MH/s (118.13ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 2100 - Domain Cached Credentials 2 (DCC2), MS Cache 2 (Iterations: 10239)

Speed.#1.........:  540.0 kH/s (362.23ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2400 - Cisco-PIX MD5

Speed.#1.........: 28064.7 MH/s (142.69ms) @ Accel:128 Loops:1024 Thr:1024 Vec:8

Hashmode: 2410 - Cisco-ASA MD5

Speed.#1.........: 28173.3 MH/s (142.46ms) @ Accel:128 Loops:1024 Thr:1024 Vec:4

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#1.........:  674.6 kH/s (362.64ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2501 - WPA-EAPOL-PMK (Iterations: 0)

Speed.#1.........:  328.3 MH/s (0.00ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 2600 - md5(md5($pass))

Speed.#1.........: 10903.1 MH/s (367.66ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 2611 - vBulletin < v3.8.5

Speed.#1.........: 10860.9 MH/s (369.60ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 2612 - PHPS

Speed.#1.........: 10871.6 MH/s (369.81ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 2711 - vBulletin >= v3.8.5

Speed.#1.........:  7562.2 MH/s (265.67ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2811 - MyBB 1.2+, IPB2+ (Invision Power Board)

Speed.#1.........:  8032.1 MH/s (250.14ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 31559.2 MH/s (63.13ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 3100 - Oracle H: Type (Oracle 7+)

Speed.#1.........:  709.5 MH/s (354.23ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    35113 H/s (159.64ms) @ Accel:32 Loops:16 Thr:12 Vec:1

Hashmode: 3710 - md5($salt.md5($pass))

Speed.#1.........: 10084.0 MH/s (398.75ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 3711 - MediaWiki B type

Speed.#1.........: 10081.3 MH/s (397.78ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 3800 - md5($salt.$pass.$salt)

Speed.#1.........: 23806.0 MH/s (168.56ms) @ Accel:128 Loops:1024 Thr:1024 Vec:4

Hashmode: 3910 - md5(md5($pass).md5($salt))

Speed.#1.........:  7613.0 MH/s (263.89ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4010 - md5($salt.md5($salt.$pass))

Speed.#1.........:  9134.8 MH/s (440.21ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 4110 - md5($salt.md5($pass.$salt))

Speed.#1.........:  9868.0 MH/s (407.52ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 4300 - md5(strtoupper(md5($pass)))

Speed.#1.........: 10877.7 MH/s (369.71ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 4400 - md5(sha1($pass))

Speed.#1.........:  7167.0 MH/s (280.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4500 - sha1(sha1($pass))

Speed.#1.........:  5407.5 MH/s (371.62ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4520 - sha1($salt.sha1($pass))

Speed.#1.........:  3417.3 MH/s (294.07ms) @ Accel:128 Loops:256 Thr:1024 Vec:1

Hashmode: 4521 - Redmine

Speed.#1.........:  3417.2 MH/s (294.01ms) @ Accel:128 Loops:256 Thr:1024 Vec:1

Hashmode: 4522 - PunBB

Speed.#1.........:  5079.3 MH/s (395.72ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 4700 - sha1(md5($pass))

Speed.#1.........:  7363.1 MH/s (272.86ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4710 - sha1(md5($pass).$salt)

Speed.#1.........:  6892.6 MH/s (290.25ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4711 - Huawei sha1(md5($pass).$salt)

Speed.#1.........:  6908.0 MH/s (290.50ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 4800 - iSCSI CHAP authentication, MD5(CHAP)

Speed.#1.........: 27332.6 MH/s (146.75ms) @ Accel:128 Loops:1024 Thr:1024 Vec:8

Hashmode: 4900 - sha1($salt.$pass.$salt)

Speed.#1.........: 10833.2 MH/s (370.37ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 5100 - Half MD5

Speed.#1.........: 22363.9 MH/s (179.43ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 5200 - Password Safe v3 (Iterations: 2049)

Speed.#1.........:  1960.2 kH/s (165.56ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 5300 - IKE-PSK MD5

Speed.#1.........:  1322.0 MH/s (380.15ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 5400 - IKE-PSK SHA1

Speed.#1.........:  567.5 MH/s (442.87ms) @ Accel:128 Loops:64 Thr:1024 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 39340.3 MH/s (101.80ms) @ Accel:128 Loops:1024 Thr:1024 Vec:2

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  2776.0 MH/s (361.88ms) @ Accel:128 Loops:256 Thr:1024 Vec:1

Hashmode: 5700 - Cisco-IOS type 4 (SHA256)

Speed.#1.........:  4936.0 MH/s (407.35ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 5800 - Samsung Android Password/PIN (Iterations: 1023)

Speed.#1.........:  9599.2 kH/s (396.53ms) @ Accel:128 Loops:1023 Thr:1024 Vec:1

Hashmode: 6000 - RIPEMD-160

Speed.#1.........:  7771.2 MH/s (258.46ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 6100 - Whirlpool

Speed.#1.........:  370.8 MH/s (338.83ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:  440.7 kH/s (263.57ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 6212 - TrueCrypt RIPEMD160 + XTS 1024 bit (Iterations: 1999)

Speed.#1.........:  244.5 kH/s (459.49ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 6213 - TrueCrypt RIPEMD160 + XTS 1536 bit (Iterations: 1999)

Speed.#1.........:  185.0 kH/s (336.45ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 6221 - TrueCrypt SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:  641.1 kH/s (345.30ms) @ Accel:8 Loops:999 Thr:1024 Vec:1

Hashmode: 6222 - TrueCrypt SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:  310.3 kH/s (349.48ms) @ Accel:4 Loops:999 Thr:1024 Vec:1

Hashmode: 6223 - TrueCrypt SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:  206.4 kH/s (229.04ms) @ Accel:16 Loops:124 Thr:1024 Vec:1

Hashmode: 6231 - TrueCrypt Whirlpool + XTS 512 bit (Iterations: 999)

Speed.#1.........:    56730 H/s (716.05ms) @ Accel:4 Loops:499 Thr:1024 Vec:1

Hashmode: 6232 - TrueCrypt Whirlpool + XTS 1024 bit (Iterations: 999)

Speed.#1.........:    28414 H/s (1068.12ms) @ Accel:16 Loops:62 Thr:1024 Vec:1

Hashmode: 6233 - TrueCrypt Whirlpool + XTS 1536 bit (Iterations: 999)

Speed.#1.........:    18575 H/s (819.40ms) @ Accel:4 Loops:124 Thr:1024 Vec:1

Hashmode: 6241 - TrueCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 999)

Speed.#1.........:  911.6 kH/s (262.06ms) @ Accel:128 Loops:62 Thr:1024 Vec:1

Hashmode: 6242 - TrueCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 999)

Speed.#1.........:  515.3 kH/s (461.21ms) @ Accel:128 Loops:62 Thr:1024 Vec:1

Hashmode: 6243 - TrueCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 999)

Speed.#1.........:  303.3 kH/s (294.92ms) @ Accel:32 Loops:124 Thr:1024 Vec:1

Hashmode: 6300 - AIX {smd5} (Iterations: 1000)

Speed.#1.........: 15651.8 kH/s (241.12ms) @ Accel:128 Loops:1000 Thr:1024 Vec:1

Hashmode: 6400 - AIX {ssha256} (Iterations: 63)

Speed.#1.........: 25507.3 kH/s (134.40ms) @ Accel:128 Loops:63 Thr:1024 Vec:1

Hashmode: 6500 - AIX {ssha512} (Iterations: 63)

Speed.#1.........:  9484.1 kH/s (351.04ms) @ Accel:128 Loops:63 Thr:1024 Vec:1

Hashmode: 6600 - 1Password, agilekeychain (Iterations: 999)

Speed.#1.........:  5367.2 kH/s (354.46ms) @ Accel:64 Loops:999 Thr:1024 Vec:1

Hashmode: 6700 - AIX {ssha1} (Iterations: 63)

Speed.#1.........: 58116.3 kH/s (43.81ms) @ Accel:128 Loops:63 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  3714.6 kH/s (257.01ms) @ Accel:32 Loops:499 Thr:1024 Vec:1

Hashmode: 6900 - GOST R 34.11-94

Speed.#1.........:  372.0 MH/s (337.78ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 7000 - FortiGate (FortiOS)

Speed.#1.........: 11839.8 MH/s (339.53ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:  670.9 kH/s (355.54ms) @ Accel:8 Loops:1023 Thr:1024 Vec:1

Hashmode: 7200 - GRUB 2 (Iterations: 1023)

Speed.#1.........:  680.9 kH/s (354.50ms) @ Accel:8 Loops:1023 Thr:1024 Vec:1

Hashmode: 7300 - IPMI2 RAKP HMAC-SHA1

Speed.#1.........:  1709.2 MH/s (294.01ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 7400 - sha256crypt $5$, SHA256 (Unix) (Iterations: 5000)

Speed.#1.........:  425.7 kH/s (461.57ms) @ Accel:128 Loops:256 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:  470.2 MH/s (267.09ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 7700 - SAP CODVN B (BCODE)

Speed.#1.........:  2568.5 MH/s (391.24ms) @ Accel:128 Loops:256 Thr:1024 Vec:1

Hashmode: 7701 - SAP CODVN B (BCODE) from RFC_READ_TABLE

Speed.#1.........:  2785.7 MH/s (360.85ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 7800 - SAP CODVN F/G (PASSCODE)

Speed.#1.........:  1316.0 MH/s (381.47ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 7801 - SAP CODVN F/G (PASSCODE) from RFC_READ_TABLE

Speed.#1.........:  1499.0 MH/s (335.22ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 7900 - Drupal7 (Iterations: 16384)

Speed.#1.........:    87278 H/s (351.50ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 8000 - Sybase ASE

Speed.#1.........:  638.0 MH/s (393.52ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 8100 - Citrix NetScaler

Speed.#1.........: 12287.3 MH/s (327.20ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 8200 - 1Password, cloudkeychain (Iterations: 39999)

Speed.#1.........:    12543 H/s (250.30ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 8300 - DNSSEC (NSEC3)

Speed.#1.........:  5412.3 MH/s (371.43ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 8400 - WBB3 (Woltlab Burning Board)

Speed.#1.........:  2148.6 MH/s (467.33ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 8500 - RACF

Speed.#1.........:  3994.7 MH/s (251.46ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 8600 - Lotus Notes/Domino 5

Speed.#1.........:  333.9 MH/s (376.26ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 8700 - Lotus Notes/Domino 6

Speed.#1.........:  110.4 MH/s (284.32ms) @ Accel:1 Loops:1024 Thr:1024 Vec:1

Hashmode: 8800 - Android FDE <= 4.3 (Iterations: 1999)

Speed.#1.........:  1370.9 kH/s (353.62ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 8900 - scrypt (Iterations: 1)

Speed.#1.........:  649.7 kH/s (5.54ms) @ Accel:16 Loops:1 Thr:16 Vec:1

Hashmode: 9000 - Password Safe v2 (Iterations: 1000)

Speed.#1.........:  740.1 kH/s (153.64ms) @ Accel:512 Loops:1000 Thr:12 Vec:1

Hashmode: 9100 - Lotus Notes/Domino 8 (Iterations: 4999)

Speed.#1.........:  1103.5 kH/s (349.95ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 9200 - Cisco-IOS $8$ (PBKDF2-SHA256) (Iterations: 19999)

Speed.#1.........:    94682 H/s (264.56ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 9300 - Cisco-IOS $9$ (scrypt) (Iterations: 1)

Speed.#1.........:    27806 H/s (113.18ms) @ Accel:16 Loops:1 Thr:8 Vec:1

Hashmode: 9400 - MS Office 2007 (Iterations: 50000)

Speed.#1.........:  221.4 kH/s (360.74ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 9500 - MS Office 2010 (Iterations: 100000)

Speed.#1.........:  110.9 kH/s (361.90ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 9600 - MS Office 2013 (Iterations: 100000)

Speed.#1.........:    14669 H/s (342.59ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 9700 - MS Office <= 2003 $0/$1, MD5 + RC4

Speed.#1.........:  420.9 MH/s (298.37ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 9710 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.#1.........:  514.8 MH/s (244.05ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 9720 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #2

Speed.#1.........:  3253.3 MH/s (308.07ms) @ Accel:128 Loops:256 Thr:1024 Vec:1

Hashmode: 9800 - MS Office <= 2003 $3/$4, SHA1 + RC4

Speed.#1.........:  486.8 MH/s (257.98ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 9810 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.#1.........:  533.2 MH/s (471.57ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 9820 - MS Office <= 2003 $3, SHA1 + RC4, collider #2

Speed.#1.........:  5791.2 MH/s (347.03ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 9900 - Radmin2

Speed.#1.........: 13540.9 MH/s (296.83ms) @ Accel:128 Loops:1024 Thr:1024 Vec:4

Hashmode: 10000 - Django (PBKDF2-SHA256) (Iterations: 9999)

Speed.#1.........:  188.8 kH/s (259.10ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 10100 - SipHash

Speed.#1.........: 43089.6 MH/s (92.50ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 10200 - CRAM-MD5

Speed.#1.........:  6076.6 MH/s (330.80ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 10300 - SAP CODVN H (PWDSALTEDHASH) iSSHA-1 (Iterations: 1023)

Speed.#1.........:  9393.1 kH/s (406.35ms) @ Accel:128 Loops:1023 Thr:1024 Vec:1

Hashmode: 10400 - PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.#1.........:  561.6 MH/s (447.72ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 10410 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.#1.........:  606.3 MH/s (414.65ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 10420 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #2

Speed.#1.........: 11748.5 MH/s (341.96ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 10500 - PDF 1.4 - 1.6 (Acrobat 5 - 8) (Iterations: 70)

Speed.#1.........: 25274.3 kH/s (71.40ms) @ Accel:1024 Loops:70 Thr:64 Vec:1

Hashmode: 10600 - PDF 1.7 Level 3 (Acrobat 9)

Speed.#1.........:  4951.4 MH/s (406.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 10700 - PDF 1.7 Level 8 (Acrobat 10 - 11) (Iterations: 64)

Speed.#1.........:    82595 H/s (371.42ms) @ Accel:16 Loops:4 Thr:1024 Vec:1

Hashmode: 10800 - SHA2-384

Speed.#1.........:  1522.2 MH/s (329.91ms) @ Accel:128 Loops:128 Thr:1024 Vec:1

Hashmode: 10900 - PBKDF2-HMAC-SHA256 (Iterations: 999)

Speed.#1.........:  1860.9 kH/s (259.33ms) @ Accel:16 Loops:999 Thr:1024 Vec:1

Hashmode: 11000 - PrestaShop

Speed.#1.........: 13403.1 MH/s (299.66ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 11100 - PostgreSQL CRAM (MD5)

Speed.#1.........: 10689.0 MH/s (376.10ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 11200 - MySQL CRAM (SHA1)

Speed.#1.........:  3782.1 MH/s (265.55ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:    7272 H/s (344.42ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 11400 - SIP digest authentication (MD5)

Speed.#1.........:  4664.6 MH/s (430.96ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 11500 - CRC32

Speed.#1.........:  6994.7 MH/s (287.25ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:  489.4 kH/s (249.40ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 11700 - GOST R 34.11-2012 (Streebog) 256-bit, big-endian

Speed.#1.........: 77563.2 kH/s (404.89ms) @ Accel:4 Loops:256 Thr:1024 Vec:1

Hashmode: 11750 - HMAC-Streebog-256 (key = $pass), big-endian

Speed.#1.........: 27163.9 kH/s (288.99ms) @ Accel:1 Loops:256 Thr:1024 Vec:1

Hashmode: 11760 - HMAC-Streebog-256 (key = $salt), big-endian

Speed.#1.........: 37196.1 kH/s (422.36ms) @ Accel:2 Loops:256 Thr:1024 Vec:1

Hashmode: 11800 - GOST R 34.11-2012 (Streebog) 512-bit, big-endian

Speed.#1.........: 77528.8 kH/s (405.23ms) @ Accel:1 Loops:1024 Thr:1024 Vec:1

Hashmode: 11850 - HMAC-Streebog-512 (key = $pass), big-endian

Speed.#1.........: 24013.2 kH/s (327.00ms) @ Accel:2 Loops:128 Thr:1024 Vec:1

Hashmode: 11860 - HMAC-Streebog-512 (key = $salt), big-endian

Speed.#1.........: 31187.7 kH/s (251.49ms) @ Accel:1 Loops:256 Thr:1024 Vec:1

Hashmode: 11900 - PBKDF2-HMAC-MD5 (Iterations: 999)

Speed.#1.........: 11907.7 kH/s (310.75ms) @ Accel:128 Loops:999 Thr:1024 Vec:1

Hashmode: 12000 - PBKDF2-HMAC-SHA1 (Iterations: 999)

Speed.#1.........:  5355.7 kH/s (351.07ms) @ Accel:64 Loops:999 Thr:1024 Vec:1

Hashmode: 12001 - Atlassian (PBKDF2-HMAC-SHA1) (Iterations: 9999)

Speed.#1.........:  556.3 kH/s (351.42ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 12100 - PBKDF2-HMAC-SHA512 (Iterations: 999)

Speed.#1.........:  690.1 kH/s (311.39ms) @ Accel:64 Loops:124 Thr:1024 Vec:1

Hashmode: 12200 - eCryptfs (Iterations: 65536)

Speed.#1.........:    22250 H/s (344.38ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 12300 - Oracle T: Type (Oracle 12+) (Iterations: 4095)

Speed.#1.........:  172.1 kH/s (355.11ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 12400 - BSDi Crypt, Extended DES (Iterations: 2194)

Speed.#1.........:  3129.4 kH/s (412.07ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    53047 H/s (289.19ms) @ Accel:8 Loops:16384 Thr:1024 Vec:1

Hashmode: 12600 - ColdFusion 10+

Speed.#1.........:  2933.5 MH/s (342.37ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 12700 - Blockchain, My Wallet (Iterations: 9)

Speed.#1.........: 77893.5 kH/s (15.35ms) @ Accel:128 Loops:9 Thr:1024 Vec:1

Hashmode: 12800 - MS-AzureSync PBKDF2-HMAC-SHA256 (Iterations: 99)

Speed.#1.........: 15856.3 kH/s (209.09ms) @ Accel:128 Loops:99 Thr:1024 Vec:1

Hashmode: 12900 - Android FDE (Samsung DEK) (Iterations: 4095)

Speed.#1.........:  461.4 kH/s (264.40ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    57777 H/s (264.69ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:  474.1 MH/s (264.93ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 13200 - AxCrypt (Iterations: 10467)

Speed.#1.........:  172.0 kH/s (1116.18ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 13300 - AxCrypt in-memory SHA1

Speed.#1.........: 12623.2 MH/s (318.39ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    52420 H/s (780.35ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 13500 - PeopleSoft PS_TOKEN

Speed.#1.........: 10061.2 MH/s (399.74ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 13600 - WinZip (Iterations: 999)

Speed.#1.........:  5159.8 kH/s (360.72ms) @ Accel:64 Loops:999 Thr:1024 Vec:1

Hashmode: 13711 - VeraCrypt RIPEMD160 + XTS 512 bit (Iterations: 655330)

Speed.#1.........:    1390 H/s (268.55ms) @ Accel:16 Loops:500 Thr:1024 Vec:1

Hashmode: 13712 - VeraCrypt RIPEMD160 + XTS 1024 bit (Iterations: 655330)

Speed.#1.........:      691 H/s (270.43ms) @ Accel:8 Loops:500 Thr:1024 Vec:1

Hashmode: 13713 - VeraCrypt RIPEMD160 + XTS 1536 bit (Iterations: 655330)

Speed.#1.........:      487 H/s (383.93ms) @ Accel:8 Loops:500 Thr:1024 Vec:1

Hashmode: 13721 - VeraCrypt SHA512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:    1412 H/s (345.97ms) @ Accel:16 Loops:500 Thr:1024 Vec:1

Hashmode: 13722 - VeraCrypt SHA512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      637 H/s (381.41ms) @ Accel:16 Loops:250 Thr:1024 Vec:1

Hashmode: 13723 - VeraCrypt SHA512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      426 H/s (286.59ms) @ Accel:16 Loops:125 Thr:1024 Vec:1

Hashmode: 13731 - VeraCrypt Whirlpool + XTS 512 bit (Iterations: 499999)

Speed.#1.........:      111 H/s (1101.88ms) @ Accel:4 Loops:500 Thr:1024 Vec:1

Hashmode: 13732 - VeraCrypt Whirlpool + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      57 H/s (1069.40ms) @ Accel:4 Loops:250 Thr:1024 Vec:1

Hashmode: 13733 - VeraCrypt Whirlpool + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      38 H/s (802.51ms) @ Accel:2 Loops:250 Thr:1024 Vec:1

Hashmode: 13741 - VeraCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 327660)

Speed.#1.........:    2790 H/s (274.06ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 13742 - VeraCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 327660)

Speed.#1.........:    1378 H/s (277.98ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 13743 - VeraCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 327660)

Speed.#1.........:      969 H/s (394.95ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 13751 - VeraCrypt SHA256 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:    1953 H/s (250.21ms) @ Accel:16 Loops:500 Thr:1024 Vec:1

Hashmode: 13752 - VeraCrypt SHA256 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      865 H/s (283.22ms) @ Accel:8 Loops:500 Thr:1024 Vec:1

Hashmode: 13753 - VeraCrypt SHA256 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      569 H/s (429.81ms) @ Accel:16 Loops:250 Thr:1024 Vec:1

Hashmode: 13761 - VeraCrypt SHA256 + XTS 512 bit + boot-mode (Iterations: 199999)

Speed.#1.........:    4856 H/s (257.04ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 13762 - VeraCrypt SHA256 + XTS 1024 bit + boot-mode (Iterations: 199999)

Speed.#1.........:    2165 H/s (289.20ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 13763 - VeraCrypt SHA256 + XTS 1536 bit + boot-mode (Iterations: 199999)

Speed.#1.........:    1426 H/s (438.96ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 13771 - VeraCrypt Streebog-512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:      49 H/s (628.86ms) @ Accel:1 Loops:500 Thr:1024 Vec:1

Hashmode: 13772 - VeraCrypt Streebog-512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      24 H/s (1291.63ms) @ Accel:2 Loops:250 Thr:1024 Vec:1

Hashmode: 13773 - VeraCrypt Streebog-512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      16 H/s (934.99ms) @ Accel:4 Loops:62 Thr:1024 Vec:1

Hashmode: 13800 - Windows Phone 8+ PIN/password

Speed.#1.........:  974.1 MH/s (257.76ms) @ Accel:128 Loops:64 Thr:1024 Vec:1

Hashmode: 13900 - OpenCart

Speed.#1.........:  3421.7 MH/s (293.66ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 14000 - DES (PT = $salt, key = $pass)

Speed.#1.........: 31226.6 MH/s (63.82ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 14100 - 3DES (PT = $salt, key = $pass)

Speed.#1.........:  1816.0 MH/s (276.60ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 14400 - sha1(CX)

Speed.#1.........:  564.4 MH/s (445.48ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 14600 - LUKS (Iterations: 163044)

Speed.#1.........:    15562 H/s (395.45ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 14700 - iTunes backup < 10.0 (Iterations: 9999)

Speed.#1.........:  276.1 kH/s (353.58ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 14800 - iTunes backup >= 10.0 (Iterations: 9999999)

Speed.#1.........:      198 H/s (252.35ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 14900 - Skip32 (PT = $salt, key = $pass)

Speed.#1.........:  5225.0 MH/s (12.44ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 15000 - FileZilla Server >= 0.9.55

Speed.#1.........:  1461.9 MH/s (343.70ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 15100 - Juniper/NetBSD sha1crypt (Iterations: 19999)

Speed.#1.........:  277.6 kH/s (361.54ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 15200 - Blockchain, My Wallet, V2 (Iterations: 4999)

Speed.#1.........:  551.2 kH/s (354.51ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:  115.5 kH/s (361.78ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 15400 - ChaCha20

[33mYour device driver installation is probably broken.[0m
[33mSee also: https://hashcat.net/faq/wrongdriver[0m
[33m[0m
Speed.#1.........:  6476.4 MH/s (621.22ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 15500 - JKS Java Key Store Private Keys (SHA1)

Speed.#1.........: 12591.7 MH/s (319.31ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 15600 - Ethereum Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1023)

Speed.#1.........:  1825.2 kH/s (264.27ms) @ Accel:16 Loops:1023 Thr:1024 Vec:1

Hashmode: 15700 - Ethereum Wallet, SCRYPT (Iterations: 1)

Speed.#1.........:        1 H/s (17333.99ms) @ Accel:1 Loops:1 Thr:1 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    38840 H/s (242.46ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 16000 - Tripcode

Speed.#1.........:  276.4 MH/s (454.64ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 16100 - TACACS+

Speed.#1.........: 21025.1 MH/s (190.84ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 16200 - Apple Secure Notes (Iterations: 19999)

Speed.#1.........:    94948 H/s (264.55ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 16300 - Ethereum Pre-Sale Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1999)

Speed.#1.........:  930.0 kH/s (258.33ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 16400 - CRAM-MD5 Dovecot

Speed.#1.........: 39999.9 MH/s (99.99ms) @ Accel:128 Loops:1024 Thr:1024 Vec:8

Hashmode: 16500 - JWT (JSON Web Token)

Speed.#1.........:  325.3 MH/s (386.29ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 16600 - Electrum Wallet (Salt-Type 1-3)

Speed.#1.........:  521.1 MH/s (240.90ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 16700 - FileVault 2 (Iterations: 19999)

Speed.#1.........:    94969 H/s (264.56ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 16800 - WPA-PMKID-PBKDF2 (Iterations: 4095)

Speed.#1.........:  675.8 kH/s (362.29ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 16801 - WPA-PMKID-PMK (Iterations: 0)

Speed.#1.........:  326.8 MH/s (0.00ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 16900 - Ansible Vault (Iterations: 9999)

Speed.#1.........:  189.6 kH/s (258.43ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 17200 - PKZIP (Compressed)

Speed.#1.........:  2363.4 MH/s (212.38ms) @ Accel:128 Loops:128 Thr:1024 Vec:1

Hashmode: 17210 - PKZIP (Uncompressed)

Speed.#1.........:  1657.7 MH/s (151.31ms) @ Accel:128 Loops:64 Thr:1024 Vec:1

Hashmode: 17220 - PKZIP (Compressed Multi-File)

Speed.#1.........:  5516.8 MH/s (181.97ms) @ Accel:128 Loops:256 Thr:1024 Vec:1

Hashmode: 17225 - PKZIP (Mixed Multi-File)

Speed.#1.........:  6704.7 MH/s (299.75ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 17230 - PKZIP (Mixed Multi-File Checksum-Only)

Speed.#1.........: 10940.3 MH/s (367.50ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 17300 - SHA3-224

Speed.#1.........:  1424.3 MH/s (352.23ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 17400 - SHA3-256

Speed.#1.........:  1431.6 MH/s (351.00ms) @ Accel:128 Loops:128 Thr:1024 Vec:1

Hashmode: 17500 - SHA3-384

Speed.#1.........:  1404.8 MH/s (356.95ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 17600 - SHA3-512

Speed.#1.........:  1419.7 MH/s (353.48ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 17700 - Keccak-224

Speed.#1.........:  1420.8 MH/s (352.93ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 17800 - Keccak-256

Speed.#1.........:  1414.4 MH/s (354.95ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 17900 - Keccak-384

Speed.#1.........:  1406.8 MH/s (357.09ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 18000 - Keccak-512

Speed.#1.........:  1431.4 MH/s (350.84ms) @ Accel:128 Loops:128 Thr:1024 Vec:1

Hashmode: 18100 - TOTP (HMAC-SHA1)

Speed.#1.........:  2588.8 MH/s (387.80ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 18200 - Kerberos 5, etype 23, AS-REP

Speed.#1.........:  471.8 MH/s (266.17ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 18300 - Apple File System (APFS) (Iterations: 19999)

Speed.#1.........:    94933 H/s (264.66ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 18400 - Open Document Format (ODF) 1.2 (SHA-256, AES) (Iterations: 99999)

Speed.#1.........:    27611 H/s (362.89ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 18500 - sha1(md5(md5($pass)))

Speed.#1.........:  4773.9 MH/s (421.20ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 18600 - Open Document Format (ODF) 1.1 (SHA-1, Blowfish) (Iterations: 1023)

Speed.#1.........:  897.3 kH/s (189.86ms) @ Accel:1024 Loops:1023 Thr:12 Vec:1

Hashmode: 18700 - Java Object hashCode()

Speed.#1.........:  226.4 GH/s (17.08ms) @ Accel:128 Loops:1024 Thr:1024 Vec:8

Hashmode: 18800 - Blockchain, My Wallet, Second Password (SHA256) (Iterations: 9999)

Speed.#1.........:  405.8 kH/s (241.56ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 18900 - Android Backup (Iterations: 9999)

Speed.#1.........:  276.5 kH/s (354.58ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 19000 - QNX /etc/shadow (MD5) (Iterations: 1000)

Speed.#1.........: 40245.6 kH/s (82.05ms) @ Accel:128 Loops:1000 Thr:1024 Vec:1

Hashmode: 19100 - QNX /etc/shadow (SHA256) (Iterations: 1000)

Speed.#1.........: 20228.1 kH/s (176.94ms) @ Accel:128 Loops:1000 Thr:1024 Vec:1

Hashmode: 19200 - QNX /etc/shadow (SHA512) (Iterations: 1000)

Speed.#1.........: 12156.6 kH/s (290.73ms) @ Accel:128 Loops:1000 Thr:1024 Vec:1

Hashmode: 19300 - sha1($salt1.$pass.$salt2)

Speed.#1.........:  1256.0 MH/s (400.10ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 19500 - Ruby on Rails Restful-Authentication

Speed.#1.........: 79271.6 kH/s (396.24ms) @ Accel:16 Loops:64 Thr:1024 Vec:1

Hashmode: 19600 - Kerberos 5, etype 17, TGS-REP (Iterations: 4095)

Speed.#1.........:  1342.8 kH/s (361.49ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 19700 - Kerberos 5, etype 18, TGS-REP (Iterations: 4095)

Speed.#1.........:  671.4 kH/s (362.64ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 19800 - Kerberos 5, etype 17, Pre-Auth (Iterations: 4095)

Speed.#1.........:  1347.2 kH/s (361.15ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 19900 - Kerberos 5, etype 18, Pre-Auth (Iterations: 4095)

Speed.#1.........:  671.9 kH/s (362.43ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 20011 - DiskCryptor SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:  467.8 kH/s (163.89ms) @ Accel:8 Loops:499 Thr:1024 Vec:1

Hashmode: 20012 - DiskCryptor SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:  229.2 kH/s (196.95ms) @ Accel:8 Loops:249 Thr:1024 Vec:1

Hashmode: 20013 - DiskCryptor SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:  152.2 kH/s (326.86ms) @ Accel:16 Loops:124 Thr:1024 Vec:1

Hashmode: 20200 - Python passlib pbkdf2-sha512 (Iterations: 24999)

Speed.#1.........:    28410 H/s (353.53ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 20300 - Python passlib pbkdf2-sha256 (Iterations: 28999)

Speed.#1.........:    65471 H/s (264.58ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 20400 - Python passlib pbkdf2-sha1 (Iterations: 130999)

Speed.#1.........:    42197 H/s (362.73ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 20500 - PKZIP Master Key

Speed.#1.........:  104.1 GH/s (36.61ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Hashmode: 20510 - PKZIP Master Key (6 byte optimization)

Speed.#1.........: 20934.3 MH/s (95.62ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 20600 - Oracle Transportation Management (SHA256) (Iterations: 999)

Speed.#1.........:  4007.3 kH/s (322.35ms) @ Accel:128 Loops:499 Thr:1024 Vec:1

Hashmode: 20710 - sha256(sha256($pass).$salt)

Speed.#1.........:  415.5 MH/s (302.25ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 20711 - AuthMe sha256

Speed.#1.........:  415.4 MH/s (302.23ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 20800 - sha256(md5($pass))

Speed.#1.........:  3760.5 MH/s (266.80ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 20900 - md5(sha1($pass).md5($pass).sha1($pass))

Speed.#1.........:  4106.5 MH/s (244.35ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 21000 - BitShares v0.x - sha512(sha512_bin(pass))

Speed.#1.........:  649.8 MH/s (386.64ms) @ Accel:128 Loops:64 Thr:1024 Vec:1

Hashmode: 21100 - sha1(md5($pass.$salt))

Speed.#1.........:  7340.2 MH/s (273.01ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 21200 - md5(sha1($salt).md5($pass))

Speed.#1.........:  7029.4 MH/s (285.51ms) @ Accel:128 Loops:512 Thr:1024 Vec:1

Hashmode: 21300 - md5($salt.sha1($salt.$pass))

Speed.#1.........:  3806.2 MH/s (263.99ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 21400 - sha256(sha256_bin(pass))

Speed.#1.........:  2210.0 MH/s (454.99ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 21500 - SolarWinds Orion (Iterations: 999)

Speed.#1.........:  102.4 kH/s (289.96ms) @ Accel:16 Loops:62 Thr:1024 Vec:1

Hashmode: 99999 - Plaintext

Speed.#1.........: 56712.6 MH/s (70.15ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1

Started: Mon Sep 23 16:34:47 2019
Stopped: Mon Sep 23 17:46:21 2019
```
