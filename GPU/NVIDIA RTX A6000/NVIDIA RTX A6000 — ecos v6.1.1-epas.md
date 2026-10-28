# NVIDIA RTX A6000

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA RTX A6000
- **Версия hashcat / Version:** v6.1.1-epas
- **Источник / Source:** [ecos](https://hashcat.net/forum/thread-10061.html)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 68198.7 MH/s |
| 100 | SHA1 | 22982.9 MH/s |
| 1400 | SHA2-256 | 9794.7 MH/s |
| 1700 | SHA2-512 | 2900.7 MH/s |
| 1000 | NTLM | 121.5 GH/s |
| 3200 | bcrypt | 90570 H/s |
| 1800 | sha512crypt | 411.9 kH/s |
| 500 | md5crypt | 32638.5 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 1148.9 kH/s |
| 7500 | Kerberos AS-REQ (23) | 1579.3 MH/s |
| 13100 | Kerberos TGS-REP (23) | 1579.6 MH/s |
| 11300 | Bitcoin wallet.dat | 15105 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 858.6 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.1.1-epas) starting in benchmark mode...

OpenCL API (OpenCL 3.0 CUDA 11.3.55) - Platform #1 [NVIDIA Corporation]
=======================================================================
* Device #1: NVIDIA RTX A6000, 48384/48685 MB (12171 MB allocatable), 84MCU

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 68198.7 MH/s (41.28ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 10 - md5($pass.$salt)

Speed.#1.........: 67929.8 MH/s (41.44ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11 - Joomla < 2.5.18

Speed.#1.........: 60547.0 MH/s (46.50ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 12 - PostgreSQL

Speed.#1.........: 60461.4 MH/s (46.57ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 20 - md5($salt.$pass)

Speed.#1.........: 38129.9 MH/s (73.87ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 21 - osCommerce, xt:Commerce

Speed.#1.........: 38303.0 MH/s (73.53ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 22 - Juniper NetScreen/SSG (ScreenOS)

Speed.#1.........: 38123.7 MH/s (73.88ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 23 - Skype

Speed.#1.........: 38018.8 MH/s (74.08ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 30 - md5(utf16le($pass).$salt)

Speed.#1.........: 64561.4 MH/s (43.60ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 40 - md5($salt.utf16le($pass))

Speed.#1.........: 38262.3 MH/s (73.61ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 50 - HMAC-MD5 (key = $pass)

Speed.#1.........: 11337.0 MH/s (248.56ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 60 - HMAC-MD5 (key = $salt)

Speed.#1.........: 23888.3 MH/s (117.94ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........: 22982.9 MH/s (122.59ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 101 - nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.#1.........: 22961.5 MH/s (122.70ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 110 - sha1($pass.$salt)

Speed.#1.........: 23069.5 MH/s (122.13ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 111 - nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.#1.........: 22946.3 MH/s (122.78ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 112 - Oracle S: Type (Oracle 11+)

Speed.#1.........: 23046.9 MH/s (122.25ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 120 - sha1($salt.$pass)

Speed.#1.........: 17575.6 MH/s (160.32ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 121 - SMF (Simple Machines Forum) > v1.1

Speed.#1.........: 17550.0 MH/s (160.55ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 122 - macOS v10.4, macOS v10.5, MacOS v10.6

Speed.#1.........: 17589.2 MH/s (160.19ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 124 - Django (SHA-1)

Speed.#1.........: 17565.8 MH/s (160.41ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 125 - ArubaOS

Speed.#1.........: 17560.8 MH/s (160.45ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 130 - sha1(utf16le($pass).$salt)

Speed.#1.........: 23094.5 MH/s (121.99ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 131 - MSSQL (2000)

Speed.#1.........: 23090.8 MH/s (122.01ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 132 - MSSQL (2005)

Speed.#1.........: 23099.1 MH/s (121.97ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 133 - PeopleSoft

Speed.#1.........: 22969.7 MH/s (122.66ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 140 - sha1($salt.utf16le($pass))

Speed.#1.........: 17608.9 MH/s (160.01ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 141 - Episerver 6.x < .NET 4

Speed.#1.........: 17601.7 MH/s (160.08ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 150 - HMAC-SHA1 (key = $pass)

Speed.#1.........:  5212.0 MH/s (270.34ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 160 - HMAC-SHA1 (key = $salt)

Speed.#1.........:  9559.1 MH/s (294.81ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 200 - MySQL323

Speed.#1.........:  179.3 GH/s (15.69ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 300 - MySQL4.1/MySQL5

Speed.#1.........:  9950.2 MH/s (283.22ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 400 - phpass (Iterations: 2048)

Speed.#1.........: 19525.9 kH/s (68.85ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 32638.5 kH/s (81.22ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1

Hashmode: 501 - Juniper IVE (Iterations: 1000)

Speed.#1.........: 32636.2 kH/s (81.25ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1

Hashmode: 600 - BLAKE2b-512

Speed.#1.........:  5739.3 MH/s (245.50ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 900 - MD4

Speed.#1.........:  121.2 GH/s (23.20ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........:  121.5 GH/s (23.15ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1100 - Domain Cached Credentials (DCC), MS Cache

Speed.#1.........: 32129.1 MH/s (87.67ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1300 - SHA2-224

Speed.#1.........:  9560.7 MH/s (294.76ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  9794.7 MH/s (287.71ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1410 - sha256($pass.$salt)

Speed.#1.........:  9810.8 MH/s (287.24ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1411 - SSHA-256(Base64), LDAP {SSHA256}

Speed.#1.........:  9788.6 MH/s (287.89ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1420 - sha256($salt.$pass)

Speed.#1.........:  8815.6 MH/s (319.67ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1421 - hMailServer

Speed.#1.........:  8806.5 MH/s (320.00ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1430 - sha256(utf16le($pass).$salt)

Speed.#1.........:  9809.2 MH/s (287.29ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1440 - sha256($salt.utf16le($pass))

Speed.#1.........:  8811.4 MH/s (319.83ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1441 - Episerver 6.x >= .NET 4

Speed.#1.........:  8813.2 MH/s (319.76ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 1450 - HMAC-SHA256 (key = $pass)

Speed.#1.........:  1900.8 MH/s (370.65ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 1460 - HMAC-SHA256 (key = $salt)

Speed.#1.........:  4156.7 MH/s (338.99ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  2815.3 MH/s (250.21ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 1600 - Apache $apr1$ MD5, md5apr1, MD5 (APR) (Iterations: 1000)

Speed.#1.........: 32501.4 kH/s (81.57ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  2900.7 MH/s (242.87ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 1710 - sha512($pass.$salt)

Speed.#1.........:  2876.3 MH/s (244.93ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 1711 - SSHA-512(Base64), LDAP {SSHA512}

Speed.#1.........:  2875.6 MH/s (244.99ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 1720 - sha512($salt.$pass)

Speed.#1.........:  2846.6 MH/s (247.49ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 1722 - macOS v10.7

Speed.#1.........:  2845.0 MH/s (247.63ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 1730 - sha512(utf16le($pass).$salt)

Speed.#1.........:  2875.8 MH/s (244.97ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 1731 - MSSQL (2012, 2014)

Speed.#1.........:  2876.4 MH/s (244.92ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 1740 - sha512($salt.utf16le($pass))

Speed.#1.........:  2844.1 MH/s (247.71ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 1750 - HMAC-SHA512 (key = $pass)

Speed.#1.........:  715.0 MH/s (246.31ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

Hashmode: 1760 - HMAC-SHA512 (key = $salt)

Speed.#1.........:  1418.5 MH/s (248.33ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:  411.9 kH/s (332.49ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 2000 - STDOUT

Speed.#1.........: 46486.8 GH/s (0.01ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2100 - Domain Cached Credentials 2 (DCC2), MS Cache 2 (Iterations: 10239)

Speed.#1.........:  913.8 kH/s (300.72ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2400 - Cisco-PIX MD5

Speed.#1.........: 47707.2 MH/s (59.03ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2410 - Cisco-ASA MD5

Speed.#1.........: 43248.4 MH/s (65.12ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#1.........:  1132.0 kH/s (303.31ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 2501 - WPA-EAPOL-PMK (Iterations: 0)

Speed.#1.........:  832.4 MH/s (0.00ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2600 - md5(md5($pass))

Speed.#1.........: 20233.8 MH/s (139.25ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2611 - vBulletin < v3.8.5

Speed.#1.........: 20227.4 MH/s (139.29ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2612 - PHPS

Speed.#1.........: 20230.2 MH/s (139.27ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2711 - vBulletin >= v3.8.5

Speed.#1.........: 14200.6 MH/s (198.43ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 2811 - MyBB 1.2+, IPB2+ (Invision Power Board)

Speed.#1.........: 14998.0 MH/s (187.87ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 69250.7 MH/s (40.62ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 3100 - Oracle H: Type (Oracle 7+)

Speed.#1.........:  1608.6 MH/s (437.99ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    90570 H/s (121.40ms) @ Accel:1024 Loops:32 Thr:11 Vec:1

Hashmode: 3710 - md5($salt.md5($pass))

Speed.#1.........: 18760.9 MH/s (150.18ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 3711 - MediaWiki B type

Speed.#1.........: 18807.7 MH/s (149.81ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 3800 - md5($salt.$pass.$salt)

Speed.#1.........: 37730.8 MH/s (74.65ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 3910 - md5(md5($pass).md5($salt))

Speed.#1.........: 14282.6 MH/s (197.29ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4010 - md5($salt.md5($salt.$pass))

Speed.#1.........: 16715.9 MH/s (168.56ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4110 - md5($salt.md5($pass.$salt))

Speed.#1.........: 17901.6 MH/s (157.39ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4300 - md5(strtoupper(md5($pass)))

Speed.#1.........: 20235.7 MH/s (139.23ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4400 - md5(sha1($pass))

Speed.#1.........: 12129.3 MH/s (232.32ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4500 - sha1(sha1($pass))

Speed.#1.........:  8774.8 MH/s (321.16ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4510 - sha1(sha1($pass).$salt)

Speed.#1.........:  8504.6 MH/s (331.36ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4520 - sha1($salt.sha1($pass))

Speed.#1.........:  5377.4 MH/s (262.02ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 4521 - Redmine

Speed.#1.........:  5377.2 MH/s (262.03ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 4522 - PunBB

Speed.#1.........:  8147.2 MH/s (345.90ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4700 - sha1(md5($pass))

Speed.#1.........: 12510.0 MH/s (225.25ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4710 - sha1(md5($pass).$salt)

Speed.#1.........: 11764.2 MH/s (239.53ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4711 - Huawei sha1(md5($pass).$salt)

Speed.#1.........: 11760.4 MH/s (239.61ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4800 - iSCSI CHAP authentication, MD5(CHAP)

Speed.#1.........: 42766.2 MH/s (65.85ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 4900 - sha1($salt.$pass.$salt)

Speed.#1.........: 17080.9 MH/s (164.96ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 5100 - Half MD5

Speed.#1.........: 44568.2 MH/s (63.19ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 5200 - Password Safe v3 (Iterations: 2049)

Speed.#1.........:  3920.9 kH/s (232.88ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 5300 - IKE-PSK MD5

Speed.#1.........:  2684.8 MH/s (262.40ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 5400 - IKE-PSK SHA1

Speed.#1.........:  1167.8 MH/s (301.65ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 68324.4 MH/s (41.20ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  5080.7 MH/s (277.33ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 5700 - Cisco-IOS type 4 (SHA256)

Speed.#1.........:  9777.6 MH/s (288.21ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 5800 - Samsung Android Password/PIN (Iterations: 1023)

Speed.#1.........: 16001.8 kH/s (168.93ms) @ Accel:32 Loops:1023 Thr:1024 Vec:1

Hashmode: 6000 - RIPEMD-160

Speed.#1.........: 15238.3 MH/s (184.91ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 6100 - Whirlpool

Speed.#1.........:  1547.9 MH/s (455.16ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:  858.6 kH/s (368.12ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 6212 - TrueCrypt RIPEMD160 + XTS 1024 bit (Iterations: 1999)

Speed.#1.........:  464.2 kH/s (322.17ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 6213 - TrueCrypt RIPEMD160 + XTS 1536 bit (Iterations: 1999)

Speed.#1.........:  320.2 kH/s (460.66ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 6221 - TrueCrypt SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:  1267.4 kH/s (319.29ms) @ Accel:16 Loops:499 Thr:1024 Vec:1

Hashmode: 6222 - TrueCrypt SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:  600.3 kH/s (319.15ms) @ Accel:8 Loops:499 Thr:1024 Vec:1

Hashmode: 6223 - TrueCrypt SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:  389.4 kH/s (359.01ms) @ Accel:2 Loops:999 Thr:1024 Vec:1

Hashmode: 6231 - TrueCrypt Whirlpool + XTS 512 bit (Iterations: 999)

Speed.#1.........:  187.6 kH/s (905.75ms) @ Accel:16 Loops:124 Thr:1024 Vec:1

Hashmode: 6232 - TrueCrypt Whirlpool + XTS 1024 bit (Iterations: 999)

Speed.#1.........:    94554 H/s (895.99ms) @ Accel:16 Loops:62 Thr:1024 Vec:1

Hashmode: 6233 - TrueCrypt Whirlpool + XTS 1536 bit (Iterations: 999)

Speed.#1.........:    63247 H/s (671.15ms) @ Accel:8 Loops:62 Thr:1024 Vec:1

Hashmode: 6241 - TrueCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 999)

Speed.#1.........:  1624.8 kH/s (359.82ms) @ Accel:8 Loops:999 Thr:1024 Vec:1

Hashmode: 6242 - TrueCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 999)

Speed.#1.........:  840.2 kH/s (211.48ms) @ Accel:8 Loops:499 Thr:1024 Vec:1

Hashmode: 6243 - TrueCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 999)

Speed.#1.........:  566.0 kH/s (405.44ms) @ Accel:32 Loops:124 Thr:1024 Vec:1

Hashmode: 6300 - AIX {smd5} (Iterations: 1000)

Speed.#1.........: 32904.7 kH/s (80.58ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1

Hashmode: 6400 - AIX {ssha256} (Iterations: 63)

Speed.#1.........: 52758.6 kH/s (46.55ms) @ Accel:32 Loops:63 Thr:1024 Vec:1

Hashmode: 6500 - AIX {ssha512} (Iterations: 63)

Speed.#1.........: 21067.1 kH/s (117.98ms) @ Accel:32 Loops:63 Thr:1024 Vec:1

Hashmode: 6600 - 1Password, agilekeychain (Iterations: 999)

Speed.#1.........:  9328.2 kH/s (290.45ms) @ Accel:32 Loops:999 Thr:1024 Vec:1

Hashmode: 6700 - AIX {ssha1} (Iterations: 63)

Speed.#1.........:  131.4 MH/s (17.27ms) @ Accel:32 Loops:63 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  8127.3 kH/s (330.93ms) @ Accel:32 Loops:499 Thr:1024 Vec:1

Hashmode: 6900 - GOST R 34.11-94

Speed.#1.........:  1125.7 MH/s (312.93ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 7000 - FortiGate (FortiOS)

Speed.#1.........: 20111.8 MH/s (140.09ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:  1413.9 kH/s (321.78ms) @ Accel:16 Loops:511 Thr:1024 Vec:1

Hashmode: 7200 - GRUB 2 (Iterations: 1023)

Speed.#1.........:  1411.2 kH/s (322.39ms) @ Accel:16 Loops:511 Thr:1024 Vec:1

Hashmode: 7300 - IPMI2 RAKP HMAC-SHA1

Speed.#1.........:  3028.7 MH/s (465.26ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 7400 - sha256crypt $5$, SHA256 (Unix) (Iterations: 5000)

Speed.#1.........:  922.4 kH/s (295.44ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 7401 - MySQL $A$ (sha256crypt) (Iterations: 5000)

Speed.#1.........:  865.5 kH/s (314.46ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:  1579.3 MH/s (446.12ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 7700 - SAP CODVN B (BCODE)

Speed.#1.........:  3845.4 MH/s (366.43ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 7701 - SAP CODVN B (BCODE) from RFC_READ_TABLE

Speed.#1.........:  4180.4 MH/s (337.07ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 7800 - SAP CODVN F/G (PASSCODE)

Speed.#1.........:  3901.1 MH/s (361.20ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 7801 - SAP CODVN F/G (PASSCODE) from RFC_READ_TABLE

Speed.#1.........:  3894.3 MH/s (361.84ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 7900 - Drupal7 (Iterations: 16384)

Speed.#1.........:  173.5 kH/s (247.51ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 8000 - Sybase ASE

Speed.#1.........:  1322.3 MH/s (266.40ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 8100 - Citrix NetScaler (SHA1)

Speed.#1.........: 19503.7 MH/s (144.46ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 8200 - 1Password, cloudkeychain (Iterations: 39999)

Speed.#1.........:    36344 H/s (483.81ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 8300 - DNSSEC (NSEC3)

Speed.#1.........:  8531.9 MH/s (330.30ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 8400 - WBB3 (Woltlab Burning Board)

Speed.#1.........:  3677.9 MH/s (383.13ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 8500 - RACF

Speed.#1.........:  7817.5 MH/s (360.49ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 8501 - RACF KDFAES

Speed.#1.........:    83679 H/s (1027.88ms) @ Accel:1 Loops:1 Thr:1024 Vec:1

Hashmode: 8600 - Lotus Notes/Domino 5

Speed.#1.........:  907.6 MH/s (388.13ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 8700 - Lotus Notes/Domino 6

Speed.#1.........:  305.9 MH/s (287.87ms) @ Accel:1 Loops:1024 Thr:1024 Vec:1

Hashmode: 8800 - Android FDE <= 4.3 (Iterations: 1999)

Speed.#1.........:  2338.7 kH/s (291.95ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 8900 - scrypt (Iterations: 16384)

Speed.#1.........:    5534 H/s (14.15ms) @ Accel:84 Loops:1024 Thr:32 Vec:1

Hashmode: 9000 - Password Safe v2 (Iterations: 1000)

Speed.#1.........:  2217.8 kH/s (136.23ms) @ Accel:512 Loops:1000 Thr:11 Vec:1

Hashmode: 9100 - Lotus Notes/Domino 8 (Iterations: 4999)

Speed.#1.........:  1874.3 kH/s (291.07ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 9200 - Cisco-IOS $8$ (PBKDF2-SHA256) (Iterations: 19999)

Speed.#1.........:  191.2 kH/s (368.22ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 9300 - Cisco-IOS $9$ (scrypt) (Iterations: 16384)

Speed.#1.........:    41306 H/s (2.06ms) @ Accel:84 Loops:1024 Thr:32 Vec:1

Hashmode: 9400 - MS Office 2007 (Iterations: 50000)

Speed.#1.........:  383.3 kH/s (146.94ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 9500 - MS Office 2010 (Iterations: 100000)

Speed.#1.........:  191.5 kH/s (147.02ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 9600 - MS Office 2013 (Iterations: 100000)

Speed.#1.........:    30285 H/s (464.50ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 9700 - MS Office <= 2003 $0/$1, MD5 + RC4

Speed.#1.........:  1439.6 MH/s (244.68ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 9710 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.#1.........:  1761.1 MH/s (400.08ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 9720 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #2

Speed.#1.........:  5829.6 MH/s (483.44ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 9800 - MS Office <= 2003 $3/$4, SHA1 + RC4

Speed.#1.........:  1578.0 MH/s (446.48ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 9810 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.#1.........:  1740.9 MH/s (404.72ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 9820 - MS Office <= 2003 $3, SHA1 + RC4, collider #2

Speed.#1.........:  9237.9 MH/s (305.06ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 9900 - Radmin2

Speed.#1.........: 25087.3 MH/s (112.30ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 10000 - Django (PBKDF2-SHA256) (Iterations: 9999)

Speed.#1.........:  380.9 kH/s (361.04ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 10100 - SipHash

Speed.#1.........: 80141.3 MH/s (35.12ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 10200 - CRAM-MD5

Speed.#1.........: 11341.6 MH/s (248.46ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 10300 - SAP CODVN H (PWDSALTEDHASH) iSSHA-1 (Iterations: 1023)

Speed.#1.........: 15492.8 kH/s (174.41ms) @ Accel:32 Loops:1023 Thr:1024 Vec:1

Hashmode: 10400 - PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.#1.........:  1850.1 MH/s (380.81ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 10410 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.#1.........:  1960.0 MH/s (359.47ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 10420 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #2

Speed.#1.........: 21861.6 MH/s (128.88ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 10500 - PDF 1.4 - 1.6 (Acrobat 5 - 8) (Iterations: 70)

Speed.#1.........: 80899.7 kH/s (30.56ms) @ Accel:512 Loops:70 Thr:64 Vec:1

Hashmode: 10600 - PDF 1.7 Level 3 (Acrobat 9)

Speed.#1.........:  9899.2 MH/s (284.67ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 10700 - PDF 1.7 Level 8 (Acrobat 10 - 11) (Iterations: 64)

Speed.#1.........:  254.0 kH/s (338.51ms) @ Accel:16 Loops:4 Thr:1024 Vec:1

Hashmode: 10800 - SHA2-384

Speed.#1.........:  2939.1 MH/s (479.45ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 10900 - PBKDF2-HMAC-SHA256 (Iterations: 999)

Speed.#1.........:  3786.3 kH/s (360.71ms) @ Accel:16 Loops:999 Thr:1024 Vec:1

Hashmode: 10901 - RedHat 389-DS LDAP (PBKDF2-HMAC-SHA256) (Iterations: 8191)

Speed.#1.........:  463.7 kH/s (370.61ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 11000 - PrestaShop

Speed.#1.........: 25363.1 MH/s (111.07ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11100 - PostgreSQL CRAM (MD5)

Speed.#1.........: 19750.7 MH/s (142.65ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11200 - MySQL CRAM (SHA1)

Speed.#1.........:  6045.5 MH/s (466.17ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:    15105 H/s (465.03ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 11400 - SIP digest authentication (MD5)

Speed.#1.........: 10019.5 MH/s (281.25ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11500 - CRC32

Speed.#1.........: 17399.6 MH/s (161.94ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:  1120.2 kH/s (294.71ms) @ Accel:16 Loops:4096 Thr:1024 Vec:1

Hashmode: 11700 - GOST R 34.11-2012 (Streebog) 256-bit, big-endian

Speed.#1.........:  233.9 MH/s (376.53ms) @ Accel:4 Loops:256 Thr:1024 Vec:1

Hashmode: 11750 - HMAC-Streebog-256 (key = $pass), big-endian

Speed.#1.........: 83587.6 kH/s (263.38ms) @ Accel:1 Loops:256 Thr:1024 Vec:1

Hashmode: 11760 - HMAC-Streebog-256 (key = $salt), big-endian

Speed.#1.........:  115.8 MH/s (380.10ms) @ Accel:2 Loops:256 Thr:1024 Vec:1

Hashmode: 11800 - GOST R 34.11-2012 (Streebog) 512-bit, big-endian

Speed.#1.........:  234.7 MH/s (375.28ms) @ Accel:1 Loops:1024 Thr:1024 Vec:1

Hashmode: 11850 - HMAC-Streebog-512 (key = $pass), big-endian

Speed.#1.........: 73385.9 kH/s (300.00ms) @ Accel:1 Loops:256 Thr:1024 Vec:1

Hashmode: 11860 - HMAC-Streebog-512 (key = $salt), big-endian

Speed.#1.........: 96665.2 kH/s (455.54ms) @ Accel:2 Loops:256 Thr:1024 Vec:1

Hashmode: 11900 - PBKDF2-HMAC-MD5 (Iterations: 999)

Speed.#1.........: 23665.6 kH/s (111.72ms) @ Accel:32 Loops:999 Thr:1024 Vec:1

Hashmode: 12000 - PBKDF2-HMAC-SHA1 (Iterations: 999)

Speed.#1.........:  9360.5 kH/s (289.57ms) @ Accel:32 Loops:999 Thr:1024 Vec:1

Hashmode: 12001 - Atlassian (PBKDF2-HMAC-SHA1) (Iterations: 9999)

Speed.#1.........:  944.7 kH/s (290.90ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 12100 - PBKDF2-HMAC-SHA512 (Iterations: 999)

Speed.#1.........:  1448.8 kH/s (313.93ms) @ Accel:16 Loops:499 Thr:1024 Vec:1

Hashmode: 12200 - eCryptfs (Iterations: 65536)

Speed.#1.........:    46278 H/s (463.92ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 12300 - Oracle T: Type (Oracle 12+) (Iterations: 4095)

Speed.#1.........:  355.8 kH/s (482.31ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 12400 - BSDi Crypt, Extended DES (Iterations: 2194)

Speed.#1.........:  7931.5 kH/s (113.66ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:  126.2 kH/s (340.57ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 12600 - ColdFusion 10+

Speed.#1.........:  5659.7 MH/s (248.95ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 12700 - Blockchain, My Wallet (Iterations: 9)

Speed.#1.........:  218.9 MH/s (5.54ms) @ Accel:32 Loops:9 Thr:1024 Vec:1

Hashmode: 12800 - MS-AzureSync PBKDF2-HMAC-SHA256 (Iterations: 99)

Speed.#1.........: 38418.9 kH/s (65.28ms) @ Accel:32 Loops:99 Thr:1024 Vec:1

Hashmode: 12900 - Android FDE (Samsung DEK) (Iterations: 4095)

Speed.#1.........:  1004.5 kH/s (341.54ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:  125.4 kH/s (342.35ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:  1579.6 MH/s (446.03ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 13200 - AxCrypt 1 (Iterations: 10467)

Speed.#1.........:  507.3 kH/s (530.37ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 13300 - AxCrypt 1 in-memory SHA1

Speed.#1.........: 21479.3 MH/s (131.17ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:  154.5 kH/s (370.87ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 13500 - PeopleSoft PS_TOKEN

Speed.#1.........: 16416.8 MH/s (171.64ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 13600 - WinZip (Iterations: 999)

Speed.#1.........:  9185.1 kH/s (293.92ms) @ Accel:32 Loops:999 Thr:1024 Vec:1

Hashmode: 13711 - VeraCrypt RIPEMD160 + XTS 512 bit (Iterations: 655330)

Speed.#1.........:    2884 H/s (181.79ms) @ Accel:16 Loops:500 Thr:1024 Vec:1

Hashmode: 13712 - VeraCrypt RIPEMD160 + XTS 1024 bit (Iterations: 655330)

Speed.#1.........:    1650 H/s (158.88ms) @ Accel:16 Loops:250 Thr:1024 Vec:1

Hashmode: 13713 - VeraCrypt RIPEMD160 + XTS 1536 bit (Iterations: 655330)

Speed.#1.........:    1157 H/s (226.37ms) @ Accel:16 Loops:250 Thr:1024 Vec:1

Hashmode: 13721 - VeraCrypt SHA512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:    2908 H/s (236.32ms) @ Accel:16 Loops:500 Thr:1024 Vec:1

Hashmode: 13722 - VeraCrypt SHA512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:    1466 H/s (234.55ms) @ Accel:4 Loops:1000 Thr:1024 Vec:1

Hashmode: 13723 - VeraCrypt SHA512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      979 H/s (175.67ms) @ Accel:4 Loops:500 Thr:1024 Vec:1

Hashmode: 13731 - VeraCrypt Whirlpool + XTS 512 bit (Iterations: 499999)

Speed.#1.........:      378 H/s (446.20ms) @ Accel:32 Loops:62 Thr:1024 Vec:1

Hashmode: 13732 - VeraCrypt Whirlpool + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      189 H/s (447.53ms) @ Accel:16 Loops:62 Thr:1024 Vec:1

Hashmode: 13733 - VeraCrypt Whirlpool + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      126 H/s (335.87ms) @ Accel:8 Loops:62 Thr:1024 Vec:1

Hashmode: 13741 - VeraCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 327660)

Speed.#1.........:    5782 H/s (185.74ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 13742 - VeraCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 327660)

Speed.#1.........:    3288 H/s (163.23ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 13743 - VeraCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 327660)

Speed.#1.........:    2302 H/s (233.08ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 13751 - VeraCrypt SHA256 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:    4049 H/s (169.58ms) @ Accel:32 Loops:250 Thr:1024 Vec:1

Hashmode: 13752 - VeraCrypt SHA256 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:    2048 H/s (167.72ms) @ Accel:16 Loops:250 Thr:1024 Vec:1

Hashmode: 13753 - VeraCrypt SHA256 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:    1370 H/s (125.44ms) @ Accel:4 Loops:500 Thr:1024 Vec:1

Hashmode: 13761 - VeraCrypt SHA256 + XTS 512 bit + boot-mode (Iterations: 199999)

Speed.#1.........:    10257 H/s (171.63ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 13762 - VeraCrypt SHA256 + XTS 1024 bit + boot-mode (Iterations: 199999)

Speed.#1.........:    5096 H/s (172.69ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 13763 - VeraCrypt SHA256 + XTS 1536 bit + boot-mode (Iterations: 199999)

Speed.#1.........:    3386 H/s (129.91ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 13771 - VeraCrypt Streebog-512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:      147 H/s (583.79ms) @ Accel:4 Loops:250 Thr:1024 Vec:1

Hashmode: 13772 - VeraCrypt Streebog-512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      72 H/s (560.67ms) @ Accel:32 Loops:15 Thr:1024 Vec:1

Hashmode: 13773 - VeraCrypt Streebog-512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      48 H/s (420.25ms) @ Accel:16 Loops:15 Thr:1024 Vec:1

Hashmode: 13800 - Windows Phone 8+ PIN/password

Speed.#1.........:  2533.7 MH/s (278.05ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 13900 - OpenCart

Speed.#1.........:  5692.5 MH/s (247.51ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 14000 - DES (PT = $salt, key = $pass)

Speed.#1.........: 69036.8 MH/s (40.74ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 14100 - 3DES (PT = $salt, key = $pass)

Speed.#1.........:  7947.1 MH/s (354.61ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 14400 - sha1(CX)

Speed.#1.........:  1089.2 MH/s (323.39ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 14600 - LUKS (Iterations: 163044)

Speed.#1.........:    28801 H/s (299.75ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 14700 - iTunes backup < 10.0 (Iterations: 9999)

Speed.#1.........:  469.7 kH/s (292.22ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 14800 - iTunes backup >= 10.0 (Iterations: 9999999)

Speed.#1.........:      382 H/s (368.73ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 14900 - Skip32 (PT = $salt, key = $pass)

Speed.#1.........: 20853.2 MH/s (3.16ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 15000 - FileZilla Server >= 0.9.55

Speed.#1.........:  2920.1 MH/s (482.56ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 15100 - Juniper/NetBSD sha1crypt (Iterations: 19999)

Speed.#1.........:  476.5 kH/s (295.49ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 15200 - Blockchain, My Wallet, V2 (Iterations: 4999)

Speed.#1.........:  938.1 kH/s (292.71ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:  195.5 kH/s (299.68ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 15400 - ChaCha20

Speed.#1.........: 13555.1 MH/s (207.88ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 15500 - JKS Java Key Store Private Keys (SHA1)

Speed.#1.........: 22039.0 MH/s (127.84ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 15600 - Ethereum Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1023)

Speed.#1.........:  3973.0 kH/s (228.46ms) @ Accel:32 Loops:511 Thr:1024 Vec:1

Hashmode: 15700 - Ethereum Wallet, SCRYPT (Iterations: 262144)

Speed.#1.........:        1 H/s (9.94ms) @ Accel:1 Loops:1024 Thr:4 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:  112.7 kH/s (483.69ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 16000 - Tripcode

Speed.#1.........:  669.6 MH/s (263.04ms) @ Accel:32 Loops:64 Thr:1024 Vec:1

Hashmode: 16100 - TACACS+

Speed.#1.........: 40880.6 MH/s (68.89ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 16200 - Apple Secure Notes (Iterations: 19999)

Speed.#1.........:  205.0 kH/s (343.25ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 16300 - Ethereum Pre-Sale Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1999)

Speed.#1.........:  2023.4 kH/s (335.45ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 16400 - CRAM-MD5 Dovecot

Speed.#1.........: 67660.0 MH/s (41.60ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 16500 - JWT (JSON Web Token)

Speed.#1.........:  1883.2 MH/s (374.12ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 16600 - Electrum Wallet (Salt-Type 1-3)

Speed.#1.........:  2240.7 MH/s (314.42ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 16700 - FileVault 2 (Iterations: 19999)

Speed.#1.........:  205.0 kH/s (343.56ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 16800 - WPA-PMKID-PBKDF2 (Iterations: 4095)

Speed.#1.........:  1147.1 kH/s (299.30ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 16801 - WPA-PMKID-PMK (Iterations: 0)

Speed.#1.........:  830.9 MH/s (0.00ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 16900 - Ansible Vault (Iterations: 9999)

Speed.#1.........:  409.7 kH/s (343.53ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 17200 - PKZIP (Compressed)

Speed.#1.........: 16650.1 MH/s (169.23ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 17210 - PKZIP (Uncompressed)

Speed.#1.........:  4046.2 MH/s (348.25ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 17220 - PKZIP (Compressed Multi-File)

Speed.#1.........: 23852.3 MH/s (118.11ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 17225 - PKZIP (Mixed Multi-File)

Speed.#1.........: 27017.7 MH/s (104.27ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 17230 - PKZIP (Mixed Multi-File Checksum-Only)

Speed.#1.........: 27065.2 MH/s (104.09ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 17300 - SHA3-224

Speed.#1.........:  2280.2 MH/s (308.97ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 17400 - SHA3-256

Speed.#1.........:  2283.4 MH/s (308.55ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 17500 - SHA3-384

Speed.#1.........:  2277.0 MH/s (309.41ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 17600 - SHA3-512

Speed.#1.........:  2279.6 MH/s (309.05ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 17700 - Keccak-224

Speed.#1.........:  2274.6 MH/s (309.73ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 17800 - Keccak-256

Speed.#1.........:  2273.1 MH/s (309.93ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 17900 - Keccak-384

Speed.#1.........:  2269.8 MH/s (310.39ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 18000 - Keccak-512

Speed.#1.........:  2269.3 MH/s (310.46ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 18100 - TOTP (HMAC-SHA1)

Speed.#1.........:  4591.4 MH/s (306.89ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 18200 - Kerberos 5, etype 23, AS-REP

Speed.#1.........:  1559.0 MH/s (451.93ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 18300 - Apple File System (APFS) (Iterations: 19999)

Speed.#1.........:  204.9 kH/s (343.62ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 18400 - Open Document Format (ODF) 1.2 (SHA-256, AES) (Iterations: 99999)

Speed.#1.........:    46954 H/s (299.94ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 18500 - sha1(md5(md5($pass)))

Speed.#1.........:  8631.0 MH/s (326.51ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 18600 - Open Document Format (ODF) 1.1 (SHA-1, Blowfish) (Iterations: 1023)

Speed.#1.........:  2142.9 kH/s (273.91ms) @ Accel:1024 Loops:1023 Thr:11 Vec:1

Hashmode: 18700 - Java Object hashCode()

Speed.#1.........:  322.5 GH/s (8.69ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 18800 - Blockchain, My Wallet, Second Password (SHA256) (Iterations: 9999)

Speed.#1.........:  814.4 kH/s (337.61ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 18900 - Android Backup (Iterations: 9999)

Speed.#1.........:  469.7 kH/s (292.68ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 19000 - QNX /etc/shadow (MD5) (Iterations: 1000)

Speed.#1.........: 97105.1 kH/s (23.84ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1

Hashmode: 19100 - QNX /etc/shadow (SHA256) (Iterations: 1000)

Speed.#1.........: 45738.9 kH/s (55.26ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1

Hashmode: 19200 - QNX /etc/shadow (SHA512) (Iterations: 1000)

Speed.#1.........: 27835.2 kH/s (89.28ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1

Hashmode: 19300 - sha1($salt1.$pass.$salt2)

Speed.#1.........:  1382.6 MH/s (254.76ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 19500 - Ruby on Rails Restful-Authentication

Speed.#1.........:  193.9 MH/s (454.29ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 19600 - Kerberos 5, etype 17, TGS-REP (Iterations: 4095)

Speed.#1.........:  2287.9 kH/s (298.99ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 19700 - Kerberos 5, etype 18, TGS-REP (Iterations: 4095)

Speed.#1.........:  1141.8 kH/s (299.52ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 19800 - Kerberos 5, etype 17, Pre-Auth (Iterations: 4095)

Speed.#1.........:  2292.2 kH/s (298.72ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 19900 - Kerberos 5, etype 18, Pre-Auth (Iterations: 4095)

Speed.#1.........:  1144.8 kH/s (299.52ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 20011 - DiskCryptor SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:  1288.6 kH/s (312.13ms) @ Accel:16 Loops:499 Thr:1024 Vec:1

Hashmode: 20012 - DiskCryptor SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:  612.2 kH/s (311.31ms) @ Accel:8 Loops:499 Thr:1024 Vec:1

Hashmode: 20013 - DiskCryptor SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:  401.9 kH/s (311.59ms) @ Accel:16 Loops:124 Thr:1024 Vec:1

Hashmode: 20200 - Python passlib pbkdf2-sha512 (Iterations: 24999)

Speed.#1.........:    58654 H/s (480.10ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 20300 - Python passlib pbkdf2-sha256 (Iterations: 28999)

Speed.#1.........:  131.9 kH/s (368.09ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 20400 - Python passlib pbkdf2-sha1 (Iterations: 130999)

Speed.#1.........:    71924 H/s (298.83ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 20500 - PKZIP Master Key

Speed.#1.........:  239.5 GH/s (11.72ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 20510 - PKZIP Master Key (6 byte optimization)

Speed.#1.........: 56050.0 MH/s (50.23ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 20600 - Oracle Transportation Management (SHA256) (Iterations: 999)

Speed.#1.........:  8121.3 kH/s (335.57ms) @ Accel:32 Loops:999 Thr:1024 Vec:1

Hashmode: 20710 - sha256(sha256($pass).$salt)

Speed.#1.........:  3053.8 MH/s (461.43ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 20711 - AuthMe sha256

Speed.#1.........:  3053.5 MH/s (461.47ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 20800 - sha256(md5($pass))

Speed.#1.........:  7509.5 MH/s (375.28ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 20900 - md5(sha1($pass).md5($pass).sha1($pass))

Speed.#1.........:  7081.1 MH/s (397.98ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 21000 - BitShares v0.x - sha512(sha512_bin(pass))

Speed.#1.........:  1454.8 MH/s (242.12ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 21100 - sha1(md5($pass.$salt))

Speed.#1.........: 12656.2 MH/s (222.65ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 21200 - md5(sha1($salt).md5($pass))

Speed.#1.........: 15096.2 MH/s (186.65ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 21300 - md5($salt.sha1($salt.$pass))

Speed.#1.........:  8857.9 MH/s (318.14ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 21400 - sha256(sha256_bin($pass))

Speed.#1.........:  4473.3 MH/s (314.99ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 21500 - SolarWinds Orion (Iterations: 999)

Speed.#1.........:  176.0 kH/s (481.39ms) @ Accel:16 Loops:62 Thr:1024 Vec:1

Hashmode: 21600 - Web2py pbkdf2-sha512 (Iterations: 999)

Speed.#1.........:  1441.2 kH/s (473.32ms) @ Accel:8 Loops:999 Thr:1024 Vec:1

Hashmode: 21700 - Electrum Wallet (Salt-Type 4) (Iterations: 1023)

Speed.#1.........:  1086.6 kH/s (322.04ms) @ Accel:16 Loops:511 Thr:1024 Vec:1

Hashmode: 21800 - Electrum Wallet (Salt-Type 5) (Iterations: 1023)

Speed.#1.........:  1091.2 kH/s (386.34ms) @ Accel:32 Loops:255 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:  1148.9 kH/s (298.83ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 22001 - WPA-PMK-PMKID+EAPOL (Iterations: 0)

Speed.#1.........:  840.2 MH/s (0.00ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 22100 - BitLocker (Iterations: 1048576)

Speed.#1.........:    4445 H/s (302.29ms) @ Accel:4 Loops:4096 Thr:1024 Vec:1

Hashmode: 22200 - Citrix NetScaler (SHA512)

Speed.#1.........:  2937.1 MH/s (479.76ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 22300 - sha256($salt.$pass.$salt)

Speed.#1.........:  8758.9 MH/s (321.74ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 22301 - Telegram Mobile App Passcode (SHA256)

Speed.#1.........:  8787.1 MH/s (320.71ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 22400 - AES Crypt (SHA256) (Iterations: 8191)

Speed.#1.........:  942.4 kH/s (362.01ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 22500 - MultiBit Classic .key (MD5)

Speed.#1.........:  2461.4 MH/s (286.23ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 22600 - Telegram Desktop < v2.1.14 (PBKDF2-HMAC-SHA1) (Iterations: 3999)

Speed.#1.........:  336.2 kH/s (255.19ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 22700 - MultiBit HD (scrypt) (Iterations: 16384)

Speed.#1.........:    5497 H/s (14.27ms) @ Accel:84 Loops:1024 Thr:32 Vec:1

Hashmode: 22911 - RSA/DSA/EC/OpenSSH Private Keys ($0$)

Speed.#1.........:  1755.4 MH/s (401.36ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 22921 - RSA/DSA/EC/OpenSSH Private Keys ($6$)

Speed.#1.........:  5900.9 MH/s (238.77ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 22931 - RSA/DSA/EC/OpenSSH Private Keys ($1, $3$)

Speed.#1.........:  3442.8 MH/s (409.29ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 22941 - RSA/DSA/EC/OpenSSH Private Keys ($4$)

Speed.#1.........:  2815.8 MH/s (250.19ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 22951 - RSA/DSA/EC/OpenSSH Private Keys ($5$)

Speed.#1.........:  2374.0 MH/s (296.76ms) @ Accel:32 Loops:256 Thr:1024 Vec:1

Hashmode: 23001 - SecureZIP AES-128

Speed.#1.........:  3250.4 MH/s (433.52ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 23002 - SecureZIP AES-192

Speed.#1.........:  2410.2 MH/s (292.30ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 23003 - SecureZIP AES-256

Speed.#1.........:  2113.5 MH/s (333.34ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 23100 - Apple Keychain (Iterations: 999)

Speed.#1.........:  4663.8 kH/s (194.69ms) @ Accel:32 Loops:499 Thr:1024 Vec:1

Hashmode: 23200 - XMPP SCRAM PBKDF2-SHA1 (Iterations: 4095)

Speed.#1.........:  2294.7 kH/s (298.60ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 23300 - Apple iWork (Iterations: 3999)

Speed.#1.........:  2350.4 kH/s (291.47ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 23400 - Bitwarden (Iterations: 99999)

Speed.#1.........:    41054 H/s (343.01ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 23500 - AxCrypt 2 AES-128 (Iterations: 999)

Speed.#1.........:  219.3 kH/s (272.43ms) @ Accel:32 Loops:249 Thr:1024 Vec:1

Hashmode: 23600 - AxCrypt 2 AES-256 (Iterations: 999)

Speed.#1.........:  114.8 kH/s (499.12ms) @ Accel:8 Loops:999 Thr:1024 Vec:1

Hashmode: 23700 - RAR3-p (Uncompressed) (Iterations: 262144)

Speed.#1.........:  126.2 kH/s (340.57ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 23800 - RAR3-p (Compressed) (Iterations: 262144)

Speed.#1.........:  125.6 kH/s (342.24ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

Hashmode: 23900 - BestCrypt v3 Volume Encryption (Iterations: 1)

Speed.#1.........:  6326.1 kH/s (423.57ms) @ Accel:32 Loops:1 Thr:1024 Vec:1

Hashmode: 24100 - MongoDB ServerKey SCRAM-SHA-1 (Iterations: 9999)

Speed.#1.........:  941.1 kH/s (292.05ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 24200 - MongoDB ServerKey SCRAM-SHA-256 (Iterations: 14999)

Speed.#1.........:  273.1 kH/s (343.50ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 24300 - sha1($salt.sha1($pass.$salt))

Speed.#1.........:  8322.1 MH/s (338.63ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 24410 - PKCS#8 Private Keys (PBKDF2-HMAC-SHA1 + 3DES/AES) (Iterations: 2047)

Speed.#1.........:  2290.8 kH/s (298.76ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 24420 - PKCS#8 Private Keys (PBKDF2-HMAC-SHA256 + 3DES/AES) (Iterations: 2047)

Speed.#1.........:  1859.4 kH/s (368.42ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 24500 - Telegram Desktop >= v2.1.14 (PBKDF2-HMAC-SHA512) (Iterations: 99999)

Speed.#1.........:    4861 H/s (362.27ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Hashmode: 24600 - SQLCipher (Iterations: 63999)

Speed.#1.........:    73597 H/s (299.01ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 24700 - Stuffit5

Speed.#1.........: 24710.9 MH/s (114.01ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 24800 - Umbraco HMAC-SHA1

Speed.#1.........:  4764.8 MH/s (295.71ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 24900 - Dahua Authentication MD5

Speed.#1.........: 37083.3 MH/s (75.95ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 25300 - MS Office 2016 - SheetProtection (Iterations: 100000)

Speed.#1.........:    30284 H/s (464.92ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 25400 - PDF 1.4 - 1.6 (Acrobat 5 - 8) - edit password (Iterations: 70)

Speed.#1.........: 81455.7 kH/s (30.49ms) @ Accel:512 Loops:70 Thr:64 Vec:1

Hashmode: 25500 - Stargazer Stellar Wallet XLM (Iterations: 4095)

Speed.#1.........:  923.3 kH/s (369.19ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 25900 - KNX IP Secure - Device Authentication Code (Iterations: 65535)

Speed.#1.........:    62613 H/s (343.17ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 26000 - Mozilla key3.db

Speed.#1.........:  274.3 MH/s (321.04ms) @ Accel:1 Loops:1024 Thr:1024 Vec:1

Hashmode: 26100 - Mozilla key4.db (Iterations: 9999)

Speed.#1.........:  381.5 kH/s (368.91ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 99999 - Plaintext

Speed.#1.........:  122.6 GH/s (22.95ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Started: Mon May  3 12:50:49 2021
Stopped: Mon May  3 13:59:51 2021
```
