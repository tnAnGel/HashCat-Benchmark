# NVIDIA Quadro RTX 5000

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Quadro RTX 5000
- **Версия hashcat / Version:** v6.2.1
- **Источник / Source:** [ventaquil](https://gist.github.com/ventaquil/fd403f169da055e9af855c4dc701f9f2)
- **Нестандартные опции / Non-default options:** прогон с `--benchmark-all`, `--backend-devices=1`, `--workload-profile=4` (pure kernels, без `-O`)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 18535.8 MH/s |
| 100 | SHA1 | 9097.1 MH/s |
| 1400 | SHA2-256 | 4240.9 MH/s |
| 1700 | SHA2-512 | 1611.9 MH/s |
| 1000 | NTLM | 22994.1 MH/s |
| 3200 | bcrypt | 38716 H/s |
| 1800 | sha512crypt | 72952 H/s |
| 500 | md5crypt | 1594.2 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 662.0 kH/s |
| 7500 | Kerberos AS-REQ (23) | 460.8 MH/s |
| 13100 | Kerberos TGS-REP (23) | 469.7 MH/s |
| 11300 | Bitcoin wallet.dat | 8269 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 497.1 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.1) starting in benchmark mode...

CUDA API (CUDA 11.2)
====================
* Device #1: Quadro RTX 5000, 16007/16125 MB, 48MCU

OpenCL API (OpenCL 1.2 CUDA 11.2.162) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #2: Quadro RTX 5000, skipped

Benchmark relevant options:
===========================
* --benchmark-all
* --backend-devices=1
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 18535.8 MH/s (173.35ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 10 - md5($pass.$salt)

Speed.#1.........:  3697.1 MH/s (435.21ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11 - Joomla < 2.5.18

Speed.#1.........:  3703.9 MH/s (434.40ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 12 - PostgreSQL

Speed.#1.........:  3706.1 MH/s (434.14ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 20 - md5($salt.$pass)

Speed.#1.........: 16072.1 MH/s (199.99ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 21 - osCommerce, xt:Commerce

Speed.#1.........: 16052.2 MH/s (200.24ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 22 - Juniper NetScreen/SSG (ScreenOS)

Speed.#1.........: 15964.3 MH/s (201.34ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 23 - Skype

Speed.#1.........: 15973.1 MH/s (201.23ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 24 - SolarWinds Serv-U

Speed.#1.........: 15911.0 MH/s (202.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 30 - md5(utf16le($pass).$salt)

Speed.#1.........: 13783.7 MH/s (233.26ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 40 - md5($salt.utf16le($pass))

Speed.#1.........: 15535.5 MH/s (206.91ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 50 - HMAC-MD5 (key = $pass)

Speed.#1.........:  3770.4 MH/s (426.72ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 60 - HMAC-MD5 (key = $salt)

Speed.#1.........: 10956.3 MH/s (293.57ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........:  9097.1 MH/s (353.66ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 101 - nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.#1.........:  9090.5 MH/s (353.91ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 110 - sha1($pass.$salt)

Speed.#1.........:  8298.6 MH/s (387.71ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 111 - nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.#1.........:  8293.0 MH/s (387.99ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 112 - Oracle S: Type (Oracle 11+)

Speed.#1.........:  8274.0 MH/s (388.87ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 120 - sha1($salt.$pass)

Speed.#1.........:  8526.4 MH/s (377.36ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 121 - SMF (Simple Machines Forum) > v1.1

Speed.#1.........:  8499.9 MH/s (378.54ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 122 - macOS v10.4, macOS v10.5, MacOS v10.6

Speed.#1.........:  8473.5 MH/s (379.71ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 124 - Django (SHA-1)

Speed.#1.........:  8456.8 MH/s (380.47ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 125 - ArubaOS

Speed.#1.........:  8453.3 MH/s (380.63ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 130 - sha1(utf16le($pass).$salt)

Speed.#1.........:  8155.9 MH/s (394.52ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 131 - MSSQL (2000)

Speed.#1.........:  8150.5 MH/s (394.77ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 132 - MSSQL (2005)

Speed.#1.........:  8146.9 MH/s (394.96ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 133 - PeopleSoft

Speed.#1.........:  8691.6 MH/s (370.17ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 140 - sha1($salt.utf16le($pass))

Speed.#1.........:  8340.7 MH/s (385.78ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 141 - Episerver 6.x < .NET 4

Speed.#1.........:  8337.0 MH/s (385.94ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 150 - HMAC-SHA1 (key = $pass)

Speed.#1.........:  2283.3 MH/s (352.25ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 160 - HMAC-SHA1 (key = $salt)

Speed.#1.........:  4864.6 MH/s (330.66ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 200 - MySQL323

Speed.#1.........: 98554.5 MH/s (32.26ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 300 - MySQL4.1/MySQL5

Speed.#1.........:  4859.4 MH/s (331.01ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 400 - phpass (Iterations: 2048)

Speed.#1.........: 11006.4 kH/s (136.94ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........:  1594.2 kH/s (243.18ms) @ Accel:8 Loops:1000 Thr:1024 Vec:1

Hashmode: 501 - Juniper IVE (Iterations: 1000)

Speed.#1.........:  1595.5 kH/s (242.92ms) @ Accel:8 Loops:1000 Thr:1024 Vec:1

Hashmode: 600 - BLAKE2b-512

Speed.#1.........:  2806.6 MH/s (286.50ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 900 - MD4

Speed.#1.........: 24012.5 MH/s (133.71ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 22994.1 MH/s (139.65ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1100 - Domain Cached Credentials (DCC), MS Cache

Speed.#1.........: 10971.0 MH/s (293.18ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1300 - SHA2-224

Speed.#1.........:  4257.0 MH/s (377.92ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  4240.9 MH/s (379.38ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1410 - sha256($pass.$salt)

Speed.#1.........:  3956.9 MH/s (406.61ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 1411 - SSHA-256(Base64), LDAP {SSHA256}

Speed.#1.........:  3945.0 MH/s (407.85ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 1420 - sha256($salt.$pass)

Speed.#1.........:  4049.7 MH/s (397.30ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1421 - hMailServer

Speed.#1.........:  4051.4 MH/s (397.12ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1430 - sha256(utf16le($pass).$salt)

Speed.#1.........:  3979.4 MH/s (404.31ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 1440 - sha256($salt.utf16le($pass))

Speed.#1.........:  4058.7 MH/s (396.40ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1441 - Episerver 6.x >= .NET 4

Speed.#1.........:  4053.7 MH/s (396.88ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1450 - HMAC-SHA256 (key = $pass)

Speed.#1.........:   951.9 MH/s (422.54ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 1460 - HMAC-SHA256 (key = $salt)

Speed.#1.........:  1722.0 MH/s (467.23ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1559.3 MH/s (257.71ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 1600 - Apache $apr1$ MD5, md5apr1, MD5 (APR) (Iterations: 1000)

Speed.#1.........:  1590.2 kH/s (243.65ms) @ Accel:8 Loops:1000 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1611.9 MH/s (249.36ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 1710 - sha512($pass.$salt)

Speed.#1.........:   540.5 MH/s (372.06ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 1711 - SSHA-512(Base64), LDAP {SSHA512}

Speed.#1.........:   540.1 MH/s (372.35ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 1720 - sha512($salt.$pass)

Speed.#1.........:  1468.4 MH/s (273.78ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 1722 - macOS v10.7

Speed.#1.........:  1460.1 MH/s (275.34ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 1730 - sha512(utf16le($pass).$salt)

Speed.#1.........:   515.4 MH/s (390.16ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 1731 - MSSQL (2012, 2014)

Speed.#1.........:   514.3 MH/s (391.04ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 1740 - sha512($salt.utf16le($pass))

Speed.#1.........:  1478.4 MH/s (271.92ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 1750 - HMAC-SHA512 (key = $pass)

Speed.#1.........:   128.6 MH/s (390.90ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 1760 - HMAC-SHA512 (key = $salt)

Speed.#1.........:   216.1 MH/s (465.35ms) @ Accel:4 Loops:512 Thr:1024 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:    72952 H/s (267.50ms) @ Accel:32 Loops:64 Thr:1024 Vec:1

Hashmode: 2000 - STDOUT

Speed.#1.........: 42137.4 GH/s (0.01ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2100 - Domain Cached Credentials 2 (DCC2), MS Cache 2 (Iterations: 10239)

Speed.#1.........:   534.3 kH/s (292.77ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 2400 - Cisco-PIX MD5

Speed.#1.........: 27574.7 MH/s (116.38ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2410 - Cisco-ASA MD5

Speed.#1.........: 24931.4 MH/s (128.80ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#1.........:   659.1 kH/s (297.11ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 2501 - WPA-EAPOL-PMK (Iterations: 0)

Speed.#1.........:   232.2 MH/s (0.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2600 - md5(md5($pass))

Speed.#1.........:  3904.5 MH/s (412.07ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2611 - vBulletin < v3.8.5

Speed.#1.........:  3835.0 MH/s (419.54ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2612 - PHPS

Speed.#1.........:  3837.7 MH/s (419.25ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2711 - vBulletin >= v3.8.5

Speed.#1.........:  8287.6 MH/s (388.25ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2811 - MyBB 1.2+, IPB2+ (Invision Power Board)

Speed.#1.........:  7379.3 MH/s (436.09ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 38114.0 MH/s (83.93ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 3100 - Oracle H: Type (Oracle 7+)

Speed.#1.........:   582.0 MH/s (345.48ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    38716 H/s (154.07ms) @ Accel:8 Loops:32 Thr:16 Vec:1

Hashmode: 3710 - md5($salt.md5($pass))

Speed.#1.........:  5314.3 MH/s (302.63ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 3711 - MediaWiki B type

Speed.#1.........:  5310.2 MH/s (302.87ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 3800 - md5($salt.$pass.$salt)

Speed.#1.........: 12574.6 MH/s (255.57ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 3910 - md5(md5($pass).md5($salt))

Speed.#1.........:  7093.9 MH/s (453.64ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4010 - md5($salt.md5($salt.$pass))

Speed.#1.........:  7735.3 MH/s (415.99ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4110 - md5($salt.md5($pass.$salt))

Speed.#1.........:  7649.4 MH/s (420.70ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 4300 - md5(strtoupper(md5($pass)))

Speed.#1.........:  3901.4 MH/s (412.39ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4400 - md5(sha1($pass))

Speed.#1.........:  6142.1 MH/s (261.79ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 4500 - sha1(sha1($pass))

Speed.#1.........:  4563.2 MH/s (352.53ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 4510 - sha1(sha1($pass).$salt)

Speed.#1.........:  4139.3 MH/s (388.66ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 4520 - sha1($salt.sha1($pass))

Speed.#1.........:  2926.9 MH/s (274.71ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 4521 - Redmine

Speed.#1.........:  2915.7 MH/s (275.76ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 4522 - PunBB

Speed.#1.........:  4245.0 MH/s (378.98ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4700 - sha1(md5($pass))

Speed.#1.........:  6388.3 MH/s (251.68ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 4710 - sha1(md5($pass).$salt)

Speed.#1.........:  5553.0 MH/s (289.64ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 4711 - Huawei sha1(md5($pass).$salt)

Speed.#1.........:  5545.3 MH/s (290.01ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 4800 - iSCSI CHAP authentication, MD5(CHAP)

Speed.#1.........:  5446.7 MH/s (295.27ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4900 - sha1($salt.$pass.$salt)

Speed.#1.........:  7521.4 MH/s (427.84ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 5100 - Half MD5

Speed.#1.........: 17598.4 MH/s (182.60ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 5200 - Password Safe v3 (Iterations: 2049)

Speed.#1.........:  2256.3 kH/s (230.37ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 5300 - IKE-PSK MD5

Speed.#1.........:  1409.2 MH/s (285.31ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 5400 - IKE-PSK SHA1

Speed.#1.........:   443.0 MH/s (454.07ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 23101.2 MH/s (139.04ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  2035.1 MH/s (395.30ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 5700 - Cisco-IOS type 4 (SHA256)

Speed.#1.........:  4232.9 MH/s (380.06ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 5800 - Samsung Android Password/PIN (Iterations: 1023)

Speed.#1.........:  7343.5 kH/s (418.24ms) @ Accel:64 Loops:1023 Thr:1024 Vec:1

Hashmode: 6000 - RIPEMD-160

Speed.#1.........:  6981.8 MH/s (460.94ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 6100 - Whirlpool

Speed.#1.........:   131.1 MH/s (383.43ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   497.1 kH/s (362.19ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 6212 - TrueCrypt RIPEMD160 + XTS 1024 bit (Iterations: 1999)

Speed.#1.........:   308.0 kH/s (322.40ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 6213 - TrueCrypt RIPEMD160 + XTS 1536 bit (Iterations: 1999)

Speed.#1.........:   215.2 kH/s (459.58ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 6221 - TrueCrypt SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:   728.8 kH/s (476.63ms) @ Accel:8 Loops:999 Thr:1024 Vec:1

Hashmode: 6222 - TrueCrypt SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:   343.6 kH/s (481.08ms) @ Accel:4 Loops:999 Thr:1024 Vec:1

Hashmode: 6223 - TrueCrypt SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:   225.9 kH/s (321.87ms) @ Accel:16 Loops:124 Thr:1024 Vec:1

Hashmode: 6231 - TrueCrypt Whirlpool + XTS 512 bit (Iterations: 999)

Speed.#1.........:    51981 H/s (1866.80ms) @ Accel:16 Loops:124 Thr:1024 Vec:1

Hashmode: 6232 - TrueCrypt Whirlpool + XTS 1024 bit (Iterations: 999)

Speed.#1.........:    25867 H/s (1869.50ms) @ Accel:16 Loops:62 Thr:1024 Vec:1

Hashmode: 6233 - TrueCrypt Whirlpool + XTS 1536 bit (Iterations: 999)

Speed.#1.........:    17337 H/s (1401.44ms) @ Accel:4 Loops:124 Thr:1024 Vec:1

Hashmode: 6241 - TrueCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 999)

Speed.#1.........:   922.6 kH/s (288.70ms) @ Accel:32 Loops:249 Thr:1024 Vec:1

Hashmode: 6242 - TrueCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 999)

Speed.#1.........:   485.4 kH/s (279.11ms) @ Accel:32 Loops:124 Thr:1024 Vec:1

Hashmode: 6243 - TrueCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 999)

Speed.#1.........:   328.6 kH/s (398.64ms) @ Accel:32 Loops:124 Thr:1024 Vec:1

Hashmode: 6300 - AIX {smd5} (Iterations: 1000)

Speed.#1.........:  1592.9 kH/s (243.40ms) @ Accel:8 Loops:1000 Thr:1024 Vec:1

Hashmode: 6400 - AIX {ssha256} (Iterations: 63)

Speed.#1.........: 29928.7 kH/s (90.49ms) @ Accel:64 Loops:63 Thr:1024 Vec:1

Hashmode: 6500 - AIX {ssha512} (Iterations: 63)

Speed.#1.........: 11269.2 kH/s (241.00ms) @ Accel:64 Loops:63 Thr:1024 Vec:1

Hashmode: 6600 - 1Password, agilekeychain (Iterations: 999)

Speed.#1.........:  5400.1 kH/s (188.76ms) @ Accel:64 Loops:499 Thr:1024 Vec:1

Hashmode: 6700 - AIX {ssha1} (Iterations: 63)

Speed.#1.........: 66005.9 kH/s (35.64ms) @ Accel:64 Loops:63 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  3703.0 kH/s (272.30ms) @ Accel:64 Loops:249 Thr:1024 Vec:1

Hashmode: 6900 - GOST R 34.11-94

Speed.#1.........:   314.8 MH/s (319.28ms) @ Accel:64 Loops:32 Thr:1024 Vec:1

Hashmode: 7000 - FortiGate (FortiOS)

Speed.#1.........:  7835.4 MH/s (410.68ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   797.1 kH/s (486.16ms) @ Accel:8 Loops:1023 Thr:1024 Vec:1

Hashmode: 7200 - GRUB 2 (Iterations: 1023)

Speed.#1.........:   791.0 kH/s (326.76ms) @ Accel:16 Loops:511 Thr:1024 Vec:1

Hashmode: 7300 - IPMI2 RAKP HMAC-SHA1

Speed.#1.........:  1557.5 MH/s (258.09ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 7400 - sha256crypt $5$, SHA256 (Unix) (Iterations: 5000)

Speed.#1.........:   157.6 kH/s (246.53ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 7401 - MySQL $A$ (sha256crypt) (Iterations: 5000)

Speed.#1.........:   142.8 kH/s (268.01ms) @ Accel:64 Loops:64 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   460.8 MH/s (436.51ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 7700 - SAP CODVN B (BCODE)

Speed.#1.........:  2133.7 MH/s (376.99ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 7701 - SAP CODVN B (BCODE) from RFC_READ_TABLE

Speed.#1.........:  2228.9 MH/s (360.86ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 7800 - SAP CODVN F/G (PASSCODE)

Speed.#1.........:  2063.4 MH/s (389.85ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 7801 - SAP CODVN F/G (PASSCODE) from RFC_READ_TABLE

Speed.#1.........:  2070.6 MH/s (388.50ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 7900 - Drupal7 (Iterations: 16384)

Speed.#1.........:    98633 H/s (248.59ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 8000 - Sybase ASE

Speed.#1.........:   703.8 MH/s (285.61ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 8100 - Citrix NetScaler (SHA1)

Speed.#1.........:  7862.7 MH/s (409.25ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 8200 - 1Password, cloudkeychain (Iterations: 39999)

Speed.#1.........:    20437 H/s (491.54ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 8300 - DNSSEC (NSEC3)

Speed.#1.........:   475.1 MH/s (423.28ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 8400 - WBB3 (Woltlab Burning Board)

Speed.#1.........:  1095.8 MH/s (367.02ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 8500 - RACF

Speed.#1.........:  3564.4 MH/s (451.43ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 8600 - Lotus Notes/Domino 5

Speed.#1.........:   272.4 MH/s (369.15ms) @ Accel:32 Loops:64 Thr:1024 Vec:1

Hashmode: 8700 - Lotus Notes/Domino 6

Speed.#1.........: 89802.8 kH/s (279.80ms) @ Accel:16 Loops:32 Thr:1024 Vec:1

Hashmode: 8800 - Android FDE <= 4.3 (Iterations: 1999)

Speed.#1.........:  1339.5 kH/s (288.99ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 8900 - scrypt (Iterations: 16384)

Speed.#1.........:     2439 H/s (25.45ms) @ Accel:48 Loops:1024 Thr:32 Vec:1

Hashmode: 9000 - Password Safe v2 (Iterations: 1000)

Speed.#1.........:   633.9 kH/s (147.54ms) @ Accel:256 Loops:1000 Thr:12 Vec:1

Hashmode: 9100 - Lotus Notes/Domino 8 (Iterations: 4999)

Speed.#1.........:  1062.9 kH/s (290.64ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 9200 - Cisco-IOS $8$ (PBKDF2-SHA256) (Iterations: 19999)

Speed.#1.........:   109.9 kH/s (365.52ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 9300 - Cisco-IOS $9$ (scrypt) (Iterations: 16384)

Speed.#1.........:    28146 H/s (1.75ms) @ Accel:48 Loops:1024 Thr:32 Vec:1

Hashmode: 9400 - MS Office 2007 (Iterations: 50000)

Speed.#1.........:   218.9 kH/s (293.22ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 9500 - MS Office 2010 (Iterations: 100000)

Speed.#1.........:   109.2 kH/s (293.83ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 9600 - MS Office 2013 (Iterations: 100000)

Speed.#1.........:    16728 H/s (480.33ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 9700 - MS Office <= 2003 $0/$1, MD5 + RC4

Speed.#1.........:   440.6 MH/s (456.55ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 9710 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.#1.........:   478.6 MH/s (420.26ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 9720 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #2

Speed.#1.........:  3283.9 MH/s (244.83ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 9800 - MS Office <= 2003 $3/$4, SHA1 + RC4

Speed.#1.........:   502.0 MH/s (400.59ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 9810 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.#1.........:   525.1 MH/s (382.95ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 9820 - MS Office <= 2003 $3, SHA1 + RC4, collider #2

Speed.#1.........:  5407.7 MH/s (297.40ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 9900 - Radmin2

Speed.#1.........:  4500.2 MH/s (357.49ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 10000 - Django (PBKDF2-SHA256) (Iterations: 9999)

Speed.#1.........:   218.6 kH/s (358.92ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 10100 - SipHash

Speed.#1.........: 45173.6 MH/s (70.87ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 10200 - CRAM-MD5

Speed.#1.........:  3767.1 MH/s (427.12ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 10300 - SAP CODVN H (PWDSALTEDHASH) iSSHA-1 (Iterations: 1023)

Speed.#1.........:  8697.1 kH/s (350.73ms) @ Accel:64 Loops:1023 Thr:1024 Vec:1

Hashmode: 10400 - PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.#1.........:   545.6 MH/s (368.58ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 10410 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.#1.........:   566.2 MH/s (355.15ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 10420 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #2

Speed.#1.........: 12483.1 MH/s (257.61ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 10500 - PDF 1.4 - 1.6 (Acrobat 5 - 8) (Iterations: 70)

Speed.#1.........: 25413.0 kH/s (114.15ms) @ Accel:1024 Loops:70 Thr:64 Vec:1

Hashmode: 10600 - PDF 1.7 Level 3 (Acrobat 9)

Speed.#1.........:  3982.7 MH/s (403.96ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 10700 - PDF 1.7 Level 8 (Acrobat 10 - 11) (Iterations: 64)

Speed.#1.........:     7833 H/s (391.75ms) @ Accel:4 Loops:1 Thr:1024 Vec:1

Hashmode: 10800 - SHA2-384

Speed.#1.........:  1619.9 MH/s (248.13ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 10900 - PBKDF2-HMAC-SHA256 (Iterations: 999)

Speed.#1.........:  2176.6 kH/s (355.73ms) @ Accel:16 Loops:999 Thr:1024 Vec:1

Hashmode: 10901 - RedHat 389-DS LDAP (PBKDF2-HMAC-SHA256) (Iterations: 8191)

Speed.#1.........:   267.2 kH/s (366.94ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 11000 - PrestaShop

Speed.#1.........:  9283.7 MH/s (346.54ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 11100 - PostgreSQL CRAM (MD5)

Speed.#1.........:  8987.2 MH/s (357.99ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 11200 - MySQL CRAM (SHA1)

Speed.#1.........:  3050.6 MH/s (263.55ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     8269 H/s (484.93ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 11400 - SIP digest authentication (MD5)

Speed.#1.........:  5484.1 MH/s (293.27ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11500 - CRC32

Speed.#1.........:  9780.5 MH/s (164.24ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   145.9 kH/s (668.95ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 11700 - GOST R 34.11-2012 (Streebog) 256-bit, big-endian

Speed.#1.........: 62653.5 kH/s (401.23ms) @ Accel:16 Loops:32 Thr:1024 Vec:1

Hashmode: 11750 - HMAC-Streebog-256 (key = $pass), big-endian

Speed.#1.........: 22638.7 kH/s (277.47ms) @ Accel:4 Loops:32 Thr:1024 Vec:1

Hashmode: 11760 - HMAC-Streebog-256 (key = $salt), big-endian

Speed.#1.........: 31504.7 kH/s (398.96ms) @ Accel:2 Loops:128 Thr:1024 Vec:1

Hashmode: 11800 - GOST R 34.11-2012 (Streebog) 512-bit, big-endian

Speed.#1.........: 61751.2 kH/s (407.10ms) @ Accel:4 Loops:128 Thr:1024 Vec:1

Hashmode: 11850 - HMAC-Streebog-512 (key = $pass), big-endian

Speed.#1.........: 19935.8 kH/s (315.15ms) @ Accel:8 Loops:16 Thr:1024 Vec:1

Hashmode: 11860 - HMAC-Streebog-512 (key = $salt), big-endian

Speed.#1.........: 26387.0 kH/s (476.45ms) @ Accel:4 Loops:64 Thr:1024 Vec:1

Hashmode: 11900 - PBKDF2-HMAC-MD5 (Iterations: 999)

Speed.#1.........: 13089.7 kH/s (223.00ms) @ Accel:64 Loops:999 Thr:1024 Vec:1

Hashmode: 12000 - PBKDF2-HMAC-SHA1 (Iterations: 999)

Speed.#1.........:  5282.8 kH/s (191.11ms) @ Accel:64 Loops:499 Thr:1024 Vec:1

Hashmode: 12001 - Atlassian (PBKDF2-HMAC-SHA1) (Iterations: 9999)

Speed.#1.........:   549.4 kH/s (291.38ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 12100 - PBKDF2-HMAC-SHA512 (Iterations: 999)

Speed.#1.........:   812.6 kH/s (476.76ms) @ Accel:8 Loops:999 Thr:1024 Vec:1

Hashmode: 12200 - eCryptfs (Iterations: 65536)

Speed.#1.........:    25527 H/s (480.47ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 12300 - Oracle T: Type (Oracle 12+) (Iterations: 4095)

Speed.#1.........:   200.1 kH/s (489.19ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 12400 - BSDi Crypt, Extended DES (Iterations: 2194)

Speed.#1.........:  2589.9 kH/s (397.94ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    61701 H/s (397.67ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 12600 - ColdFusion 10+

Speed.#1.........:  2815.5 MH/s (285.59ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 12700 - Blockchain, My Wallet (Iterations: 9)

Speed.#1.........: 95567.1 kH/s (12.54ms) @ Accel:64 Loops:9 Thr:1024 Vec:1

Hashmode: 12800 - MS-AzureSync PBKDF2-HMAC-SHA256 (Iterations: 99)

Speed.#1.........: 15545.3 kH/s (164.18ms) @ Accel:64 Loops:99 Thr:1024 Vec:1

Hashmode: 12900 - Android FDE (Samsung DEK) (Iterations: 4095)

Speed.#1.........:   469.4 kH/s (416.48ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    58886 H/s (415.83ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   469.7 MH/s (428.23ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 13200 - AxCrypt 1 (Iterations: 10467)

Speed.#1.........:   140.3 kH/s (1094.73ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 13300 - AxCrypt 1 in-memory SHA1

Speed.#1.........:  9015.5 MH/s (356.88ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    42740 H/s (765.94ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 13500 - PeopleSoft PS_TOKEN

Speed.#1.........:  8414.1 MH/s (382.40ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 13600 - WinZip (Iterations: 999)

Speed.#1.........:  5107.7 kH/s (291.00ms) @ Accel:32 Loops:999 Thr:1024 Vec:1

Hashmode: 13711 - VeraCrypt RIPEMD160 + XTS 512 bit (Iterations: 655330)

Speed.#1.........:     1645 H/s (180.36ms) @ Accel:32 Loops:250 Thr:1024 Vec:1

Hashmode: 13712 - VeraCrypt RIPEMD160 + XTS 1024 bit (Iterations: 655330)

Speed.#1.........:      940 H/s (157.16ms) @ Accel:32 Loops:125 Thr:1024 Vec:1

Hashmode: 13713 - VeraCrypt RIPEMD160 + XTS 1536 bit (Iterations: 655330)

Speed.#1.........:      641 H/s (223.36ms) @ Accel:64 Loops:62 Thr:1024 Vec:1

Hashmode: 13721 - VeraCrypt SHA512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:     1644 H/s (238.55ms) @ Accel:8 Loops:1000 Thr:1024 Vec:1

Hashmode: 13722 - VeraCrypt SHA512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      777 H/s (126.07ms) @ Accel:4 Loops:500 Thr:1024 Vec:1

Hashmode: 13723 - VeraCrypt SHA512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      519 H/s (188.75ms) @ Accel:4 Loops:500 Thr:1024 Vec:1

Hashmode: 13731 - VeraCrypt Whirlpool + XTS 512 bit (Iterations: 499999)

Speed.#1.........:      103 H/s (948.40ms) @ Accel:16 Loops:125 Thr:1024 Vec:1

Hashmode: 13732 - VeraCrypt Whirlpool + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:       52 H/s (945.56ms) @ Accel:4 Loops:250 Thr:1024 Vec:1

Hashmode: 13733 - VeraCrypt Whirlpool + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:       34 H/s (709.81ms) @ Accel:4 Loops:125 Thr:1024 Vec:1

Hashmode: 13741 - VeraCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 327660)

Speed.#1.........:     3319 H/s (183.08ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 13742 - VeraCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 327660)

Speed.#1.........:     1877 H/s (161.18ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 13743 - VeraCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 327660)

Speed.#1.........:     1305 H/s (230.83ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 13751 - VeraCrypt SHA256 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:     2114 H/s (184.07ms) @ Accel:32 Loops:250 Thr:1024 Vec:1

Hashmode: 13752 - VeraCrypt SHA256 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:     1124 H/s (168.66ms) @ Accel:64 Loops:62 Thr:1024 Vec:1

Hashmode: 13753 - VeraCrypt SHA256 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      734 H/s (127.93ms) @ Accel:64 Loops:31 Thr:1024 Vec:1

Hashmode: 13761 - VeraCrypt SHA256 + XTS 512 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     5303 H/s (187.85ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 13762 - VeraCrypt SHA256 + XTS 1024 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     2866 H/s (174.28ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 13763 - VeraCrypt SHA256 + XTS 1536 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     1893 H/s (131.48ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

Hashmode: 13771 - VeraCrypt Streebog-512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:       40 H/s (614.94ms) @ Accel:1 Loops:500 Thr:1024 Vec:1

Hashmode: 13772 - VeraCrypt Streebog-512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:       20 H/s (613.87ms) @ Accel:1 Loops:250 Thr:1024 Vec:1

Hashmode: 13773 - VeraCrypt Streebog-512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:       13 H/s (913.16ms) @ Accel:4 Loops:62 Thr:1024 Vec:1

Hashmode: 13800 - Windows Phone 8+ PIN/password

Speed.#1.........:  1276.7 MH/s (314.95ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 13900 - OpenCart

Speed.#1.........:  1848.9 MH/s (435.12ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 14000 - DES (PT = $salt, key = $pass)

Speed.#1.........: 36659.6 MH/s (87.31ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 14100 - 3DES (PT = $salt, key = $pass)

Speed.#1.........:  3652.0 MH/s (440.56ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 14400 - sha1(CX)

Speed.#1.........: 80384.5 kH/s (312.63ms) @ Accel:16 Loops:32 Thr:1024 Vec:1

Hashmode: 14600 - LUKS (Iterations: 163044)

Speed.#1.........:    16613 H/s (295.74ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 14700 - iTunes backup < 10.0 (Iterations: 9999)

Speed.#1.........:   269.2 kH/s (290.17ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 14800 - iTunes backup >= 10.0 (Iterations: 9999999)

Speed.#1.........:      219 H/s (365.46ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 14900 - Skip32 (PT = $salt, key = $pass)

Speed.#1.........:  5088.6 MH/s (12.74ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 15000 - FileZilla Server >= 0.9.55

Speed.#1.........:   540.6 MH/s (371.98ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 15100 - Juniper/NetBSD sha1crypt (Iterations: 19999)

Speed.#1.........:   272.0 kH/s (295.27ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 15200 - Blockchain, My Wallet, V2 (Iterations: 4999)

Speed.#1.........:   536.7 kH/s (291.65ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:   113.1 kH/s (294.21ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 15400 - ChaCha20

Speed.#1.........:  7834.5 MH/s (410.72ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 15500 - JKS Java Key Store Private Keys (SHA1)

Speed.#1.........:  8243.7 MH/s (390.31ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 15600 - Ethereum Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1023)

Speed.#1.........:  1840.6 kH/s (417.86ms) @ Accel:16 Loops:1023 Thr:1024 Vec:1

Hashmode: 15700 - Ethereum Wallet, SCRYPT (Iterations: 262144)

Speed.#1.........:        0 H/s (9.86ms) @ Accel:1 Loops:1024 Thr:4 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    63396 H/s (245.40ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 16000 - Tripcode

Speed.#1.........:   223.9 MH/s (449.09ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Hashmode: 16100 - TACACS+

Speed.#1.........: 13775.6 MH/s (233.40ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 16200 - Apple Secure Notes (Iterations: 19999)

Speed.#1.........:    95904 H/s (418.89ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 16300 - Ethereum Pre-Sale Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1999)

Speed.#1.........:   940.4 kH/s (407.93ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 16400 - CRAM-MD5 Dovecot

Speed.#1.........: 18397.7 MH/s (174.51ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 16500 - JWT (JSON Web Token)

Speed.#1.........:   966.4 MH/s (416.23ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 16600 - Electrum Wallet (Salt-Type 1-3)

Speed.#1.........:   649.4 MH/s (309.60ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 16700 - FileVault 2 (Iterations: 19999)

Speed.#1.........:    95870 H/s (419.03ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 16800 - WPA-PMKID-PBKDF2 (Iterations: 4095)

Speed.#1.........:   656.2 kH/s (298.34ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 16801 - WPA-PMKID-PMK (Iterations: 0)

Speed.#1.........:   230.5 MH/s (0.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 16900 - Ansible Vault (Iterations: 9999)

Speed.#1.........:   191.8 kH/s (408.96ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 17200 - PKZIP (Compressed)

Speed.#1.........:  5513.2 MH/s (145.64ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 17210 - PKZIP (Uncompressed)

Speed.#1.........:  2007.7 MH/s (200.12ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 17220 - PKZIP (Compressed Multi-File)

Speed.#1.........:  9328.9 MH/s (172.20ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 17225 - PKZIP (Mixed Multi-File)

Speed.#1.........: 11274.7 MH/s (285.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 17230 - PKZIP (Mixed Multi-File Checksum-Only)

Speed.#1.........: 11103.2 MH/s (289.24ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 17300 - SHA3-224

Speed.#1.........:  1267.2 MH/s (317.29ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 17400 - SHA3-256

Speed.#1.........:  1281.8 MH/s (313.70ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 17500 - SHA3-384

Speed.#1.........:  1281.4 MH/s (313.80ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 17600 - SHA3-512

Speed.#1.........:  1278.6 MH/s (314.47ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 17700 - Keccak-224

Speed.#1.........:  1285.1 MH/s (312.89ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 17800 - Keccak-256

Speed.#1.........:  1275.1 MH/s (315.34ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 17900 - Keccak-384

Speed.#1.........:  1288.6 MH/s (312.04ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 18000 - Keccak-512

Speed.#1.........:  1286.7 MH/s (312.50ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 18100 - TOTP (HMAC-SHA1)

Speed.#1.........:  2465.4 MH/s (326.20ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 18200 - Kerberos 5, etype 23, AS-REP

Speed.#1.........:   459.7 MH/s (437.47ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 18300 - Apple File System (APFS) (Iterations: 19999)

Speed.#1.........:    95828 H/s (419.22ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 18400 - Open Document Format (ODF) 1.2 (SHA-256, AES) (Iterations: 99999)

Speed.#1.........:    26836 H/s (299.44ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 18500 - sha1(md5(md5($pass)))

Speed.#1.........:  4895.5 MH/s (328.56ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 18600 - Open Document Format (ODF) 1.1 (SHA-1, Blowfish) (Iterations: 1023)

Speed.#1.........:   818.1 kH/s (290.88ms) @ Accel:1024 Loops:1023 Thr:12 Vec:1

Hashmode: 18700 - Java Object hashCode()

Speed.#1.........:   157.9 GH/s (19.95ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 18800 - Blockchain, My Wallet, Second Password (SHA256) (Iterations: 9999)

Speed.#1.........:   465.6 kH/s (336.98ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 18900 - Android Backup (Iterations: 9999)

Speed.#1.........:   268.1 kH/s (292.48ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 19000 - QNX /etc/shadow (MD5) (Iterations: 1000)

Speed.#1.........: 49346.3 kH/s (48.89ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 19100 - QNX /etc/shadow (SHA256) (Iterations: 1000)

Speed.#1.........: 23206.8 kH/s (116.53ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 19200 - QNX /etc/shadow (SHA512) (Iterations: 1000)

Speed.#1.........: 12637.6 kH/s (223.33ms) @ Accel:64 Loops:1000 Thr:1024 Vec:1

Hashmode: 19300 - sha1($salt1.$pass.$salt2)

Speed.#1.........:  1133.4 MH/s (354.84ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 19500 - Ruby on Rails Restful-Authentication

Speed.#1.........:   166.0 MH/s (302.75ms) @ Accel:16 Loops:64 Thr:1024 Vec:1

Hashmode: 19600 - Kerberos 5, etype 17, TGS-REP (Iterations: 4095)

Speed.#1.........:  1322.9 kH/s (294.03ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 19700 - Kerberos 5, etype 18, TGS-REP (Iterations: 4095)

Speed.#1.........:   663.7 kH/s (295.09ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 19800 - Kerberos 5, etype 17, Pre-Auth (Iterations: 4095)

Speed.#1.........:  1324.9 kH/s (293.96ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 19900 - Kerberos 5, etype 18, Pre-Auth (Iterations: 4095)

Speed.#1.........:   656.7 kH/s (297.19ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 20011 - DiskCryptor SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:   737.0 kH/s (470.54ms) @ Accel:8 Loops:999 Thr:1024 Vec:1

Hashmode: 20012 - DiskCryptor SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:   347.3 kH/s (475.83ms) @ Accel:4 Loops:999 Thr:1024 Vec:1

Hashmode: 20013 - DiskCryptor SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:   227.2 kH/s (238.40ms) @ Accel:4 Loops:499 Thr:1024 Vec:1

Hashmode: 20200 - Python passlib pbkdf2-sha512 (Iterations: 24999)

Speed.#1.........:    33243 H/s (483.45ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 20300 - Python passlib pbkdf2-sha256 (Iterations: 28999)

Speed.#1.........:    76614 H/s (361.70ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 20400 - Python passlib pbkdf2-sha1 (Iterations: 130999)

Speed.#1.........:    41645 H/s (293.40ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 20500 - PKZIP Master Key

Speed.#1.........:   136.6 GH/s (23.16ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 20510 - PKZIP Master Key (6 byte optimization)

Speed.#1.........: 25553.6 MH/s (125.62ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 20600 - Oracle Transportation Management (SHA256) (Iterations: 999)

Speed.#1.........:  4640.3 kH/s (222.51ms) @ Accel:64 Loops:499 Thr:1024 Vec:1

Hashmode: 20710 - sha256(sha256($pass).$salt)

Speed.#1.........:  1130.7 MH/s (355.71ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 20711 - AuthMe sha256

Speed.#1.........:  1124.0 MH/s (357.80ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 20800 - sha256(md5($pass))

Speed.#1.........:  3522.7 MH/s (456.78ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 20900 - md5(sha1($pass).md5($pass).sha1($pass))

Speed.#1.........:  3534.1 MH/s (455.30ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 21000 - BitShares v0.x - sha512(sha512_bin(pass))

Speed.#1.........:   552.8 MH/s (363.77ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 21100 - sha1(md5($pass.$salt))

Speed.#1.........:  4634.0 MH/s (347.13ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 21200 - md5(sha1($salt).md5($pass))

Speed.#1.........:  7007.0 MH/s (459.27ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 21300 - md5($salt.sha1($salt.$pass))

Speed.#1.........:  5180.7 MH/s (310.45ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 21400 - sha256(sha256_bin($pass))

Speed.#1.........:  2139.9 MH/s (375.89ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 21500 - SolarWinds Orion (Iterations: 999)

Speed.#1.........:    98819 H/s (479.20ms) @ Accel:16 Loops:62 Thr:1024 Vec:1

Hashmode: 21501 - SolarWinds Orion v2 (Iterations: 999)

Speed.#1.........:    94568 H/s (483.30ms) @ Accel:32 Loops:31 Thr:1024 Vec:1

Hashmode: 21600 - Web2py pbkdf2-sha512 (Iterations: 999)

Speed.#1.........:   800.3 kH/s (323.11ms) @ Accel:16 Loops:499 Thr:1024 Vec:1

Hashmode: 21700 - Electrum Wallet (Salt-Type 4) (Iterations: 1023)

Speed.#1.........:   541.5 kH/s (244.69ms) @ Accel:4 Loops:1023 Thr:1024 Vec:1

Hashmode: 21800 - Electrum Wallet (Salt-Type 5) (Iterations: 1023)

Speed.#1.........:   545.6 kH/s (489.05ms) @ Accel:8 Loops:1023 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   662.0 kH/s (295.76ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 22001 - WPA-PMK-PMKID+EAPOL (Iterations: 0)

Speed.#1.........:   229.6 MH/s (0.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 22100 - BitLocker (Iterations: 1048576)

Speed.#1.........:     2261 H/s (339.18ms) @ Accel:4 Loops:4096 Thr:1024 Vec:1

Hashmode: 22200 - Citrix NetScaler (SHA512)

Speed.#1.........:   604.0 MH/s (332.87ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 22300 - sha256($salt.$pass.$salt)

Speed.#1.........:  2991.6 MH/s (268.68ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 22301 - Telegram Mobile App Passcode (SHA256)

Speed.#1.........:  2977.0 MH/s (270.09ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 22400 - AES Crypt (SHA256) (Iterations: 8191)

Speed.#1.........:   515.0 kH/s (373.23ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 22500 - MultiBit Classic .key (MD5)

Speed.#1.........:   513.7 MH/s (391.52ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 22600 - Telegram Desktop < v2.1.14 (PBKDF2-HMAC-SHA1) (Iterations: 3999)

Speed.#1.........:   191.2 kH/s (255.10ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 22700 - MultiBit HD (scrypt) (Iterations: 16384)

Speed.#1.........:     2457 H/s (25.51ms) @ Accel:48 Loops:1024 Thr:32 Vec:1

Hashmode: 22911 - RSA/DSA/EC/OpenSSH Private Keys ($0$)

Speed.#1.........:   756.2 MH/s (265.80ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 22921 - RSA/DSA/EC/OpenSSH Private Keys ($6$)

Speed.#1.........:  2577.8 MH/s (311.97ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 22931 - RSA/DSA/EC/OpenSSH Private Keys ($1, $3$)

Speed.#1.........:   952.7 MH/s (422.22ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 22941 - RSA/DSA/EC/OpenSSH Private Keys ($4$)

Speed.#1.........:   793.8 MH/s (253.22ms) @ Accel:64 Loops:64 Thr:1024 Vec:1

Hashmode: 22951 - RSA/DSA/EC/OpenSSH Private Keys ($5$)

Speed.#1.........:   666.3 MH/s (301.71ms) @ Accel:64 Loops:64 Thr:1024 Vec:1

Hashmode: 23001 - SecureZIP AES-128

Speed.#1.........:   954.0 MH/s (421.61ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 23002 - SecureZIP AES-192

Speed.#1.........:   765.9 MH/s (262.44ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 23003 - SecureZIP AES-256

Speed.#1.........:   632.6 MH/s (317.81ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 23100 - Apple Keychain (Iterations: 999)

Speed.#1.........:  2649.8 kH/s (233.55ms) @ Accel:64 Loops:249 Thr:1024 Vec:1

Hashmode: 23200 - XMPP SCRAM PBKDF2-SHA1 (Iterations: 4095)

Speed.#1.........:  1317.0 kH/s (295.57ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 23300 - Apple iWork (Iterations: 3999)

Speed.#1.........:  1355.0 kH/s (287.64ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 23400 - Bitwarden (Iterations: 99999)

Speed.#1.........:    19446 H/s (413.15ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 23500 - AxCrypt 2 AES-128 (Iterations: 999)

Speed.#1.........:    65788 H/s (497.15ms) @ Accel:16 Loops:499 Thr:1024 Vec:1

Hashmode: 23600 - AxCrypt 2 AES-256 (Iterations: 999)

Speed.#1.........:    32808 H/s (1064.33ms) @ Accel:64 Loops:124 Thr:1024 Vec:1

Hashmode: 23700 - RAR3-p (Uncompressed) (Iterations: 262144)

Speed.#1.........:    61055 H/s (401.86ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 23800 - RAR3-p (Compressed) (Iterations: 262144)

Speed.#1.........:    61111 H/s (401.50ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 23900 - BestCrypt v3 Volume Encryption (Iterations: 1)

Speed.#1.........:  3561.8 kH/s (418.42ms) @ Accel:32 Loops:1 Thr:1024 Vec:1

Hashmode: 24100 - MongoDB ServerKey SCRAM-SHA-1 (Iterations: 9999)

Speed.#1.........:   536.0 kH/s (292.30ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 24200 - MongoDB ServerKey SCRAM-SHA-256 (Iterations: 14999)

Speed.#1.........:   127.4 kH/s (419.89ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 24300 - sha1($salt.sha1($pass.$salt))

Speed.#1.........:  3005.2 MH/s (267.53ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 24410 - PKCS#8 Private Keys (PBKDF2-HMAC-SHA1 + 3DES/AES) (Iterations: 2047)

Speed.#1.........:  1292.5 kH/s (300.37ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 24420 - PKCS#8 Private Keys (PBKDF2-HMAC-SHA256 + 3DES/AES) (Iterations: 2047)

Speed.#1.........:  1060.9 kH/s (366.66ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 24500 - Telegram Desktop >= v2.1.14 (PBKDF2-HMAC-SHA512) (Iterations: 99999)

Speed.#1.........:     2700 H/s (372.33ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Hashmode: 24600 - SQLCipher (Iterations: 63999)

Speed.#1.........:    42422 H/s (295.44ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 24700 - Stuffit5

Speed.#1.........: 11023.1 MH/s (291.79ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 24800 - Umbraco HMAC-SHA1

Speed.#1.........:   505.5 MH/s (397.83ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 24900 - Dahua Authentication MD5

Speed.#1.........: 21108.3 MH/s (152.17ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 25300 - MS Office 2016 - SheetProtection (Iterations: 100000)

Speed.#1.........:    16595 H/s (484.20ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 25400 - PDF 1.4 - 1.6 (Acrobat 5 - 8) - edit password (Iterations: 70)

Speed.#1.........: 25643.2 kH/s (113.39ms) @ Accel:1024 Loops:70 Thr:64 Vec:1

Hashmode: 25500 - Stargazer Stellar Wallet XLM (Iterations: 4095)

Speed.#1.........:   534.9 kH/s (365.44ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 25900 - KNX IP Secure - Device Authentication Code (Iterations: 65535)

Speed.#1.........:    29400 H/s (416.83ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 26000 - Mozilla key3.db

Speed.#1.........:   186.1 MH/s (270.07ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 26100 - Mozilla key4.db (Iterations: 9999)

Speed.#1.........:   219.9 kH/s (356.54ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 99999 - Plaintext

Speed.#1.........: 24078.0 MH/s (133.35ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Started: Wed Jun  9 09:58:38 2021

Stopped: Wed Jun  9 11:40:48 2021
```
