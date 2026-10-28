# AMD Radeon RX 6800 XT

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 6800 XT
- **Версия hashcat / Version:** v6.1.1-120-g15bf8b730
- **Источник / Source:** [epixoip](https://gist.github.com/epixoip/99085955a1145ff61ec83512a50421a7)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 52380.4 MH/s |
| 100 | SHA1 | 20640.2 MH/s |
| 1400 | SHA2-256 | 8743.5 MH/s |
| 1700 | SHA2-512 | 2344.2 MH/s |
| 1000 | NTLM | 85356.1 MH/s |
| 3200 | bcrypt | 58177 H/s |
| 1800 | sha512crypt | 288.0 kH/s |
| 500 | md5crypt | 21741.1 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 1061.3 kH/s |
| 2500 | WPA/WPA2 (legacy) | 1071.0 kH/s |
| 7500 | Kerberos AS-REQ (23) | 893.0 MH/s |
| 13100 | Kerberos TGS-REP (23) | 881.9 MH/s |
| 11300 | Bitcoin wallet.dat | 10945 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 669.9 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.1.1-120-g15bf8b730) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL API (OpenCL 2.0 AMD-APP (3212.0)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: gfx1030, 16256/16368 MB (13912 MB allocatable), 36MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........: 52380.4 MH/s (45.25ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........: 20640.2 MH/s (57.57ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  8743.5 MH/s (68.19ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  2344.2 MH/s (63.63ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:  1061.3 kH/s (68.60ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 85356.1 MH/s (27.38ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 52545.8 MH/s (44.81ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 57356.8 MH/s (41.17ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  3534.2 MH/s (84.52ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1872.7 MH/s (79.44ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 21741.1 kH/s (100.86ms) @ Accel:1024 Loops:1000 Thr:64 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    58177 H/s (37.79ms) @ Accel:16 Loops:8 Thr:16 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   288.0 kH/s (101.10ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   893.0 MH/s (83.61ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   881.9 MH/s (84.72ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:   182.2 kH/s (68.14ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    81195 H/s (70.47ms) @ Accel:128 Loops:256 Thr:64 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:  1017.8 kH/s (63.17ms) @ Accel:256 Loops:127 Thr:64 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   954.0 kH/s (63.28ms) @ Accel:128 Loops:4096 Thr:64 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:   139.1 kH/s (64.67ms) @ Accel:64 Loops:16384 Thr:64 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:   112.5 kH/s (81.16ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   669.9 kH/s (53.90ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    92956 H/s (263.61ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  7099.9 kH/s (52.22ms) @ Accel:512 Loops:249 Thr:64 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:    10945 H/s (68.24ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Started: Fri Dec 18 22:46:28 2020
Stopped: Fri Dec 18 22:51:06 2020

## Full Benchmark
[epixoip@precision hashcat]$ ./hashcat -b --benchmark-all
hashcat (v6.1.1-120-g15bf8b730) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL API (OpenCL 2.0 AMD-APP (3212.0)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: gfx1030, 16256/16368 MB (13912 MB allocatable), 36MCU

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........: 52473.8 MH/s (45.31ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 10 - md5($pass.$salt)

Speed.#1.........: 52311.2 MH/s (45.28ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 11 - Joomla < 2.5.18

Speed.#1.........: 51809.1 MH/s (45.73ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 12 - PostgreSQL

Speed.#1.........: 52040.6 MH/s (45.86ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 20 - md5($salt.$pass)

Speed.#1.........: 27012.4 MH/s (88.51ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 21 - osCommerce, xt:Commerce

Speed.#1.........: 26939.0 MH/s (88.68ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 22 - Juniper NetScreen/SSG (ScreenOS)

Speed.#1.........: 27422.5 MH/s (87.31ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 23 - Skype

Speed.#1.........: 27157.5 MH/s (88.04ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 30 - md5(utf16le($pass).$salt)

Speed.#1.........: 52399.7 MH/s (45.23ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 40 - md5($salt.utf16le($pass))

Speed.#1.........: 27154.6 MH/s (88.09ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 50 - HMAC-MD5 (key = $pass)

Speed.#1.........:  8127.0 MH/s (73.56ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 60 - HMAC-MD5 (key = $salt)

Speed.#1.........: 16142.3 MH/s (74.08ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........: 20675.2 MH/s (57.78ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 101 - nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.#1.........: 20715.6 MH/s (57.56ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 110 - sha1($pass.$salt)

Speed.#1.........: 20862.8 MH/s (57.12ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 111 - nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.#1.........: 20689.3 MH/s (57.62ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 112 - Oracle S: Type (Oracle 11+)

Speed.#1.........: 20791.7 MH/s (57.21ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 120 - sha1($salt.$pass)

Speed.#1.........: 16248.7 MH/s (73.56ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 121 - SMF (Simple Machines Forum) > v1.1

Speed.#1.........: 16228.6 MH/s (73.72ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 122 - macOS v10.4, macOS v10.5, MacOS v10.6

Speed.#1.........: 16185.2 MH/s (73.90ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 124 - Django (SHA-1)

Speed.#1.........: 16222.9 MH/s (73.73ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 125 - ArubaOS

Speed.#1.........: 16196.0 MH/s (73.81ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 130 - sha1(utf16le($pass).$salt)

Speed.#1.........: 20877.7 MH/s (57.01ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 131 - MSSQL (2000)

Speed.#1.........: 20863.3 MH/s (56.66ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 132 - MSSQL (2005)

Speed.#1.........: 20870.4 MH/s (57.04ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 133 - PeopleSoft

Speed.#1.........: 20748.8 MH/s (57.32ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 140 - sha1($salt.utf16le($pass))

Speed.#1.........: 16181.0 MH/s (73.83ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 141 - Episerver 6.x < .NET 4

Speed.#1.........: 16180.6 MH/s (73.78ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 150 - HMAC-SHA1 (key = $pass)

Speed.#1.........:  4745.6 MH/s (62.79ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 160 - HMAC-SHA1 (key = $salt)

Speed.#1.........:  8910.7 MH/s (66.88ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 200 - MySQL323

Speed.#1.........:   133.1 GH/s (17.45ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 300 - MySQL4.1/MySQL5

Speed.#1.........:  9257.7 MH/s (64.43ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 400 - phpass (Iterations: 2048)

Speed.#1.........: 15183.7 kH/s (73.96ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 21811.9 kH/s (100.84ms) @ Accel:1024 Loops:1000 Thr:64 Vec:1

Hashmode: 501 - Juniper IVE (Iterations: 1000)

Speed.#1.........: 21787.3 kH/s (100.83ms) @ Accel:1024 Loops:1000 Thr:64 Vec:1

Hashmode: 600 - BLAKE2b-512

Speed.#1.........:  4879.4 MH/s (60.88ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 900 - MD4

Speed.#1.........: 85730.5 MH/s (27.42ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 86703.5 MH/s (27.35ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 1100 - Domain Cached Credentials (DCC), MS Cache

Speed.#1.........: 29466.6 MH/s (81.08ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 1300 - SHA2-224

Speed.#1.........:  8646.6 MH/s (68.92ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  8837.3 MH/s (67.54ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 1410 - sha256($pass.$salt)

Speed.#1.........:  8856.6 MH/s (67.26ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 1411 - SSHA-256(Base64), LDAP {SSHA256}

Speed.#1.........:  8826.5 MH/s (67.50ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 1420 - sha256($salt.$pass)

Speed.#1.........:  7990.3 MH/s (74.70ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 1421 - hMailServer

Speed.#1.........:  7977.6 MH/s (74.78ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 1430 - sha256(utf16le($pass).$salt)

Speed.#1.........:  8867.2 MH/s (67.13ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 1440 - sha256($salt.utf16le($pass))

Speed.#1.........:  7990.8 MH/s (74.69ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 1441 - Episerver 6.x >= .NET 4

Speed.#1.........:  7978.8 MH/s (74.86ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 1450 - HMAC-SHA256 (key = $pass)

Speed.#1.........:  1748.0 MH/s (85.47ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 1460 - HMAC-SHA256 (key = $salt)

Speed.#1.........:  3820.7 MH/s (78.15ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1934.7 MH/s (76.82ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 1600 - Apache $apr1$ MD5, md5apr1, MD5 (APR) (Iterations: 1000)

Speed.#1.........: 21821.1 kH/s (100.58ms) @ Accel:1024 Loops:1000 Thr:64 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  2363.4 MH/s (63.05ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 1710 - sha512($pass.$salt)

Speed.#1.........:  2075.1 MH/s (71.92ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 1711 - SSHA-512(Base64), LDAP {SSHA512}

Speed.#1.........:  2037.6 MH/s (73.37ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 1720 - sha512($salt.$pass)

Speed.#1.........:  2259.0 MH/s (66.10ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 1722 - macOS v10.7

Speed.#1.........:  2246.8 MH/s (66.70ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 1730 - sha512(utf16le($pass).$salt)

Speed.#1.........:  2081.1 MH/s (71.79ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 1731 - MSSQL (2012, 2014)

Speed.#1.........:  2075.2 MH/s (71.91ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 1740 - sha512($salt.utf16le($pass))

Speed.#1.........:  2059.5 MH/s (72.42ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 1750 - HMAC-SHA512 (key = $pass)

Speed.#1.........:   512.1 MH/s (72.85ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 1760 - HMAC-SHA512 (key = $salt)

Speed.#1.........:  1040.0 MH/s (71.79ms) @ Accel:64 Loops:512 Thr:64 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   286.8 kH/s (101.68ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 2000 - STDOUT

Speed.#1.........: 21533.0 GH/s (0.03ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 2100 - Domain Cached Credentials 2 (DCC2), MS Cache 2 (Iterations: 10239)

Speed.#1.........:   854.2 kH/s (68.17ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 2400 - Cisco-PIX MD5

Speed.#1.........: 35337.9 MH/s (67.55ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 2410 - Cisco-ASA MD5

Speed.#1.........: 35141.4 MH/s (67.84ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#1.........:  1071.0 kH/s (68.04ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 2501 - WPA-EAPOL-PMK (Iterations: 0)

Speed.#1.........:   380.8 MH/s (0.00ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 2600 - md5(md5($pass))

Speed.#1.........: 15751.9 MH/s (75.87ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 2611 - vBulletin < v3.8.5

Speed.#1.........: 15716.9 MH/s (75.98ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 2612 - PHPS

Speed.#1.........: 15667.6 MH/s (76.20ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 2711 - vBulletin >= v3.8.5

Speed.#1.........: 10594.7 MH/s (56.12ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 2811 - MyBB 1.2+, IPB2+ (Invision Power Board)

Speed.#1.........: 10896.7 MH/s (54.45ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 52534.7 MH/s (44.86ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 3100 - Oracle H: Type (Oracle 7+)

Speed.#1.........:  1227.7 MH/s (60.68ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    58134 H/s (37.88ms) @ Accel:16 Loops:8 Thr:16 Vec:1

Hashmode: 3710 - md5($salt.md5($pass))

Speed.#1.........: 14302.7 MH/s (84.09ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 3711 - MediaWiki B type

Speed.#1.........: 14255.4 MH/s (83.98ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 3800 - md5($salt.$pass.$salt)

Speed.#1.........: 27062.4 MH/s (88.60ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 3910 - md5(md5($pass).md5($salt))

Speed.#1.........: 10564.2 MH/s (56.33ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 4010 - md5($salt.md5($salt.$pass))

Speed.#1.........: 12685.4 MH/s (94.55ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 4110 - md5($salt.md5($pass.$salt))

Speed.#1.........: 14245.8 MH/s (84.12ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 4300 - md5(strtoupper(md5($pass)))

Speed.#1.........: 15659.2 MH/s (76.47ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 4400 - md5(sha1($pass))

Speed.#1.........: 10613.1 MH/s (56.16ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 4500 - sha1(sha1($pass))

Speed.#1.........:  8381.1 MH/s (71.35ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 4510 - sha1(sha1($pass).$salt)

Speed.#1.........:  8151.5 MH/s (73.40ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 4520 - sha1($salt.sha1($pass))

Speed.#1.........:  5188.9 MH/s (57.37ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 4521 - Redmine

Speed.#1.........:  5151.9 MH/s (57.80ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 4522 - PunBB

Speed.#1.........:  7819.0 MH/s (76.47ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 4700 - sha1(md5($pass))

Speed.#1.........: 11068.7 MH/s (53.71ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 4710 - sha1(md5($pass).$salt)

Speed.#1.........: 10513.3 MH/s (56.60ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 4711 - Huawei sha1(md5($pass).$salt)

Speed.#1.........: 10506.4 MH/s (56.64ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 4800 - iSCSI CHAP authentication, MD5(CHAP)

Speed.#1.........: 34590.9 MH/s (68.99ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 4900 - sha1($salt.$pass.$salt)

Speed.#1.........: 16007.0 MH/s (74.61ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 5100 - Half MD5

Speed.#1.........: 32192.1 MH/s (74.21ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5200 - Password Safe v3 (Iterations: 2049)

Speed.#1.........:  3558.2 kH/s (54.10ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 5300 - IKE-PSK MD5

Speed.#1.........:  1954.5 MH/s (76.40ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 5400 - IKE-PSK SHA1

Speed.#1.........:  1076.8 MH/s (69.24ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 57946.5 MH/s (40.96ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  3558.5 MH/s (84.05ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 5700 - Cisco-IOS type 4 (SHA256)

Speed.#1.........:  8843.3 MH/s (67.41ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 5800 - Samsung Android Password/PIN (Iterations: 1023)

Speed.#1.........: 14769.3 kH/s (50.49ms) @ Accel:1024 Loops:511 Thr:64 Vec:1

Hashmode: 6000 - RIPEMD-160

Speed.#1.........: 11185.7 MH/s (53.22ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 6100 - Whirlpool

Speed.#1.........:  1099.7 MH/s (67.77ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   669.0 kH/s (54.03ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 6212 - TrueCrypt RIPEMD160 + XTS 1024 bit (Iterations: 1999)

Speed.#1.........:   382.1 kH/s (94.60ms) @ Accel:128 Loops:256 Thr:64 Vec:1

Hashmode: 6213 - TrueCrypt RIPEMD160 + XTS 1536 bit (Iterations: 1999)

Speed.#1.........:   264.6 kH/s (67.81ms) @ Accel:128 Loops:128 Thr:64 Vec:1

Hashmode: 6221 - TrueCrypt SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:  1033.3 kH/s (62.06ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 6222 - TrueCrypt SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:   507.7 kH/s (70.58ms) @ Accel:16 Loops:999 Thr:64 Vec:1

Hashmode: 6223 - TrueCrypt SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:   326.3 kH/s (43.48ms) @ Accel:32 Loops:249 Thr:64 Vec:1

Hashmode: 6231 - TrueCrypt Whirlpool + XTS 512 bit (Iterations: 999)

Speed.#1.........:   123.3 kH/s (64.50ms) @ Accel:32 Loops:124 Thr:64 Vec:1

Hashmode: 6232 - TrueCrypt Whirlpool + XTS 1024 bit (Iterations: 999)

Speed.#1.........:    63828 H/s (66.53ms) @ Accel:32 Loops:62 Thr:64 Vec:1

Hashmode: 6233 - TrueCrypt Whirlpool + XTS 1536 bit (Iterations: 999)

Speed.#1.........:    43606 H/s (100.65ms) @ Accel:64 Loops:31 Thr:64 Vec:1

Hashmode: 6241 - TrueCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 999)

Speed.#1.........:  1322.3 kH/s (48.01ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 6242 - TrueCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 999)

Speed.#1.........:   753.5 kH/s (84.32ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 6243 - TrueCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 999)

Speed.#1.........:   517.9 kH/s (60.31ms) @ Accel:128 Loops:124 Thr:64 Vec:1

Hashmode: 6300 - AIX {smd5} (Iterations: 1000)

Speed.#1.........: 21769.7 kH/s (100.81ms) @ Accel:1024 Loops:1000 Thr:64 Vec:1

Hashmode: 6400 - AIX {ssha256} (Iterations: 63)

Speed.#1.........: 49308.4 kH/s (38.17ms) @ Accel:1024 Loops:63 Thr:64 Vec:1

Hashmode: 6500 - AIX {ssha512} (Iterations: 63)

Speed.#1.........: 14718.5 kH/s (69.37ms) @ Accel:512 Loops:63 Thr:64 Vec:1

Hashmode: 6600 - 1Password, agilekeychain (Iterations: 999)

Speed.#1.........:  8471.8 kH/s (43.96ms) @ Accel:512 Loops:499 Thr:64 Vec:1

Hashmode: 6700 - AIX {ssha1} (Iterations: 63)

Speed.#1.........: 96440.4 kH/s (15.06ms) @ Accel:1024 Loops:63 Thr:64 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  7093.0 kH/s (52.32ms) @ Accel:512 Loops:249 Thr:64 Vec:1

Hashmode: 6900 - GOST R 34.11-94

Speed.#1.........:   658.7 MH/s (56.44ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 7000 - FortiGate (FortiOS)

Speed.#1.........: 18849.8 MH/s (63.19ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:  1011.4 kH/s (63.58ms) @ Accel:256 Loops:127 Thr:64 Vec:1

Hashmode: 7200 - GRUB 2 (Iterations: 1023)

Speed.#1.........:  1011.2 kH/s (63.64ms) @ Accel:256 Loops:127 Thr:64 Vec:1

Hashmode: 7300 - IPMI2 RAKP HMAC-SHA1

Speed.#1.........:  2699.7 MH/s (55.10ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 7400 - sha256crypt $5$, SHA256 (Unix) (Iterations: 5000)

Speed.#1.........:   842.2 kH/s (68.60ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 7401 - MySQL $A$ (sha256crypt) (Iterations: 5000)

Speed.#1.........:   796.3 kH/s (72.51ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   892.2 MH/s (83.69ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 7700 - SAP CODVN B (BCODE)

Speed.#1.........:  2392.6 MH/s (62.20ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 7701 - SAP CODVN B (BCODE) from RFC_READ_TABLE

Speed.#1.........:  2333.8 MH/s (63.79ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 7800 - SAP CODVN F/G (PASSCODE)

Speed.#1.........:  2037.0 MH/s (73.11ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 7801 - SAP CODVN F/G (PASSCODE) from RFC_READ_TABLE

Speed.#1.........:  2080.4 MH/s (71.65ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 7900 - Drupal7 (Iterations: 16384)

Speed.#1.........:   132.1 kH/s (69.03ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 8000 - Sybase ASE

Speed.#1.........:  1091.4 MH/s (68.28ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 8100 - Citrix NetScaler (SHA1)

Speed.#1.........: 18473.3 MH/s (64.45ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 8200 - 1Password, cloudkeychain (Iterations: 39999)

Speed.#1.........:    26171 H/s (71.58ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 8300 - DNSSEC (NSEC3)

Speed.#1.........:  8120.9 MH/s (73.50ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 8400 - WBB3 (Woltlab Burning Board)

Speed.#1.........:  3522.5 MH/s (84.94ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 8500 - RACF

Speed.#1.........:  6969.8 MH/s (85.76ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 8600 - Lotus Notes/Domino 5

Speed.#1.........:   553.4 MH/s (67.46ms) @ Accel:128 Loops:128 Thr:64 Vec:1

Hashmode: 8700 - Lotus Notes/Domino 6

Speed.#1.........:   168.6 MH/s (55.06ms) @ Accel:32 Loops:128 Thr:64 Vec:1

Hashmode: 8800 - Android FDE <= 4.3 (Iterations: 1999)

Speed.#1.........:  2161.9 kH/s (66.63ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 8900 - scrypt (Iterations: 1)

Speed.#1.........:  1076.4 kH/s (8.11ms) @ Accel:16 Loops:1 Thr:16 Vec:1

Hashmode: 9000 - Password Safe v2 (Iterations: 1000)

Speed.#1.........:  1300.8 kH/s (35.46ms) @ Accel:128 Loops:1000 Thr:16 Vec:1

Hashmode: 9100 - Lotus Notes/Domino 8 (Iterations: 4999)

Speed.#1.........:  1728.3 kH/s (66.72ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 9200 - Cisco-IOS $8$ (PBKDF2-SHA256) (Iterations: 19999)

Speed.#1.........:   175.8 kH/s (85.21ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 9300 - Cisco-IOS $9$ (scrypt) (Iterations: 1)

Speed.#1.........:    49851 H/s (90.56ms) @ Accel:16 Loops:1 Thr:8 Vec:1

Hashmode: 9400 - MS Office 2007 (Iterations: 50000)

Speed.#1.........:   345.8 kH/s (69.07ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 9500 - MS Office 2010 (Iterations: 100000)

Speed.#1.........:   174.0 kH/s (68.85ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 9600 - MS Office 2013 (Iterations: 100000)

Speed.#1.........:    21721 H/s (69.00ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 9700 - MS Office <= 2003 $0/$1, MD5 + RC4

Speed.#1.........:   814.8 MH/s (91.81ms) @ Accel:512 Loops:64 Thr:64 Vec:1

Hashmode: 9710 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.#1.........:   972.2 MH/s (76.74ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 9720 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #2

Speed.#1.........:  4028.7 MH/s (74.05ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 9800 - MS Office <= 2003 $3/$4, SHA1 + RC4

Speed.#1.........:   945.4 MH/s (78.97ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 9810 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.#1.........:  1007.7 MH/s (74.28ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 9820 - MS Office <= 2003 $3, SHA1 + RC4, collider #2

Speed.#1.........:  8174.2 MH/s (72.99ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 9900 - Radmin2

Speed.#1.........: 17249.7 MH/s (69.25ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 10000 - Django (PBKDF2-SHA256) (Iterations: 9999)

Speed.#1.........:   350.0 kH/s (83.54ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 10100 - SipHash

Speed.#1.........: 70724.3 MH/s (33.47ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 10200 - CRAM-MD5

Speed.#1.........:  8197.7 MH/s (72.81ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 10300 - SAP CODVN H (PWDSALTEDHASH) iSSHA-1 (Iterations: 1023)

Speed.#1.........: 13933.2 kH/s (79.53ms) @ Accel:512 Loops:1023 Thr:64 Vec:1

Hashmode: 10400 - PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.#1.........:  1035.4 MH/s (72.03ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 10410 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.#1.........:  1102.5 MH/s (67.79ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 10420 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #2

Speed.#1.........: 16694.9 MH/s (71.62ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 10500 - PDF 1.4 - 1.6 (Acrobat 5 - 8) (Iterations: 70)

Speed.#1.........: 44480.7 kH/s (45.23ms) @ Accel:1024 Loops:70 Thr:64 Vec:1

Hashmode: 10600 - PDF 1.7 Level 3 (Acrobat 9)

Speed.#1.........:  8837.0 MH/s (67.46ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 10700 - PDF 1.7 Level 8 (Acrobat 10 - 11) (Iterations: 64)

Speed.#1.........:   131.7 kH/s (69.10ms) @ Accel:16 Loops:16 Thr:64 Vec:1

Hashmode: 10800 - SHA2-384

Speed.#1.........:  2334.1 MH/s (63.81ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 10900 - PBKDF2-HMAC-SHA256 (Iterations: 999)

Speed.#1.........:  3457.9 kH/s (66.32ms) @ Accel:512 Loops:249 Thr:64 Vec:1

Hashmode: 10901 - RedHat 389-DS LDAP (PBKDF2-HMAC-SHA256) (Iterations: 8191)

Speed.#1.........:   427.9 kH/s (85.26ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 11000 - PrestaShop

Speed.#1.........: 18144.9 MH/s (65.68ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 11100 - PostgreSQL CRAM (MD5)

Speed.#1.........: 15667.1 MH/s (76.27ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 11200 - MySQL CRAM (SHA1)

Speed.#1.........:  5755.5 MH/s (51.57ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:    10862 H/s (68.69ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 11400 - SIP digest authentication (MD5)

Speed.#1.........:  7042.1 MH/s (84.88ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 11500 - CRC32

Speed.#1.........:   108.4 GH/s (21.57ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:  1053.9 kH/s (63.48ms) @ Accel:128 Loops:4096 Thr:64 Vec:1

Hashmode: 11700 - GOST R 34.11-2012 (Streebog) 256-bit, big-endian

Speed.#1.........:   131.2 MH/s (70.99ms) @ Accel:32 Loops:128 Thr:64 Vec:1

Hashmode: 11750 - HMAC-Streebog-256 (key = $pass), big-endian

Speed.#1.........: 45656.9 kH/s (102.38ms) @ Accel:128 Loops:16 Thr:64 Vec:1

Hashmode: 11760 - HMAC-Streebog-256 (key = $salt), big-endian

Speed.#1.........: 62503.2 kH/s (74.68ms) @ Accel:32 Loops:64 Thr:64 Vec:1

Hashmode: 11800 - GOST R 34.11-2012 (Streebog) 512-bit, big-endian

Speed.#1.........:   133.2 MH/s (69.93ms) @ Accel:32 Loops:128 Thr:64 Vec:1

Hashmode: 11850 - HMAC-Streebog-512 (key = $pass), big-endian

Speed.#1.........: 38901.6 kH/s (59.83ms) @ Accel:32 Loops:32 Thr:64 Vec:1

Hashmode: 11860 - HMAC-Streebog-512 (key = $salt), big-endian

Speed.#1.........: 52705.3 kH/s (88.57ms) @ Accel:32 Loops:64 Thr:64 Vec:1

Hashmode: 11900 - PBKDF2-HMAC-MD5 (Iterations: 999)

Speed.#1.........: 15060.3 kH/s (48.62ms) @ Accel:1024 Loops:499 Thr:64 Vec:1

Hashmode: 12000 - PBKDF2-HMAC-SHA1 (Iterations: 999)

Speed.#1.........:  8499.0 kH/s (66.30ms) @ Accel:256 Loops:999 Thr:64 Vec:1

Hashmode: 12001 - Atlassian (PBKDF2-HMAC-SHA1) (Iterations: 9999)

Speed.#1.........:   872.3 kH/s (66.64ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 12100 - PBKDF2-HMAC-SHA512 (Iterations: 999)

Speed.#1.........:  1030.7 kH/s (55.90ms) @ Accel:128 Loops:249 Thr:64 Vec:1

Hashmode: 12200 - eCryptfs (Iterations: 65536)

Speed.#1.........:    33302 H/s (68.59ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 12300 - Oracle T: Type (Oracle 12+) (Iterations: 4095)

Speed.#1.........:   254.8 kH/s (71.54ms) @ Accel:128 Loops:256 Thr:64 Vec:1

Hashmode: 12400 - BSDi Crypt, Extended DES (Iterations: 2194)

Speed.#1.........:  5437.3 kH/s (84.55ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:   138.7 kH/s (64.93ms) @ Accel:64 Loops:16384 Thr:64 Vec:1

Hashmode: 12600 - ColdFusion 10+

Speed.#1.........:  5185.6 MH/s (57.40ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 12700 - Blockchain, My Wallet (Iterations: 9)

Speed.#1.........:   159.8 MH/s (4.35ms) @ Accel:1024 Loops:9 Thr:64 Vec:1

Hashmode: 12800 - MS-AzureSync PBKDF2-HMAC-SHA256 (Iterations: 99)

Speed.#1.........: 32611.1 kH/s (60.71ms) @ Accel:1024 Loops:99 Thr:64 Vec:1

Hashmode: 12900 - Android FDE (Samsung DEK) (Iterations: 4095)

Speed.#1.........:   897.8 kH/s (81.21ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:   112.2 kH/s (81.43ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   880.9 MH/s (84.78ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 13200 - AxCrypt 1 (Iterations: 10467)

Speed.#1.........:   314.1 kH/s (169.81ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 13300 - AxCrypt 1 in-memory SHA1

Speed.#1.........: 19550.2 MH/s (61.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    92590 H/s (264.72ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 13500 - PeopleSoft PS_TOKEN

Speed.#1.........: 15034.6 MH/s (79.60ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 13600 - WinZip (Iterations: 999)

Speed.#1.........:  8203.1 kH/s (67.59ms) @ Accel:256 Loops:999 Thr:64 Vec:1

Hashmode: 13711 - VeraCrypt RIPEMD160 + XTS 512 bit (Iterations: 655330)

Speed.#1.........:     2024 H/s (27.27ms) @ Accel:256 Loops:125 Thr:64 Vec:1

Hashmode: 13712 - VeraCrypt RIPEMD160 + XTS 1024 bit (Iterations: 655330)

Speed.#1.........:     1131 H/s (48.78ms) @ Accel:64 Loops:500 Thr:64 Vec:1

Hashmode: 13713 - VeraCrypt RIPEMD160 + XTS 1536 bit (Iterations: 655330)

Speed.#1.........:      800 H/s (34.24ms) @ Accel:128 Loops:125 Thr:64 Vec:1

Hashmode: 13721 - VeraCrypt SHA512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:     2071 H/s (35.17ms) @ Accel:128 Loops:250 Thr:64 Vec:1

Hashmode: 13722 - VeraCrypt SHA512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:     1017 H/s (35.44ms) @ Accel:32 Loops:500 Thr:64 Vec:1

Hashmode: 13723 - VeraCrypt SHA512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      674 H/s (26.19ms) @ Accel:128 Loops:62 Thr:64 Vec:1

Hashmode: 13731 - VeraCrypt Whirlpool + XTS 512 bit (Iterations: 499999)

Speed.#1.........:      244 H/s (36.59ms) @ Accel:32 Loops:125 Thr:64 Vec:1

Hashmode: 13732 - VeraCrypt Whirlpool + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      113 H/s (39.41ms) @ Accel:32 Loops:62 Thr:64 Vec:1

Hashmode: 13733 - VeraCrypt Whirlpool + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:       81 H/s (55.28ms) @ Accel:64 Loops:31 Thr:64 Vec:1

Hashmode: 13741 - VeraCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 327660)

Speed.#1.........:     4013 H/s (28.14ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 13742 - VeraCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 327660)

Speed.#1.........:     2279 H/s (49.70ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 13743 - VeraCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 327660)

Speed.#1.........:     1588 H/s (35.56ms) @ Accel:32 Loops:512 Thr:64 Vec:1

Hashmode: 13751 - VeraCrypt SHA256 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:     3431 H/s (42.61ms) @ Accel:128 Loops:500 Thr:64 Vec:1

Hashmode: 13752 - VeraCrypt SHA256 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:     1723 H/s (41.87ms) @ Accel:128 Loops:250 Thr:64 Vec:1

Hashmode: 13753 - VeraCrypt SHA256 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:     1137 H/s (31.50ms) @ Accel:64 Loops:250 Thr:64 Vec:1

Hashmode: 13761 - VeraCrypt SHA256 + XTS 512 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     8623 H/s (43.36ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 13762 - VeraCrypt SHA256 + XTS 1024 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     4196 H/s (44.14ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 13763 - VeraCrypt SHA256 + XTS 1536 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     2835 H/s (32.30ms) @ Accel:128 Loops:128 Thr:64 Vec:1

Hashmode: 13771 - VeraCrypt Streebog-512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:       82 H/s (55.43ms) @ Accel:64 Loops:31 Thr:64 Vec:1

Hashmode: 13772 - VeraCrypt Streebog-512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:       39 H/s (56.90ms) @ Accel:32 Loops:31 Thr:64 Vec:1

Hashmode: 13773 - VeraCrypt Streebog-512 + XTS 1536 bit (Iterations: 499999)


Speed.#1.........:       27 H/s (78.89ms) @ Accel:64 Loops:15 Thr:64 Vec:1

Hashmode: 13800 - Windows Phone 8+ PIN/password

Speed.#1.........:  2256.0 MH/s (66.05ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 13900 - OpenCart

Speed.#1.........:  5489.4 MH/s (54.24ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 14000 - DES (PT = $salt, key = $pass)

Speed.#1.........: 51533.0 MH/s (45.75ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 14100 - 3DES (PT = $salt, key = $pass)

Speed.#1.........:  7124.6 MH/s (83.97ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 14400 - sha1(CX)

Speed.#1.........:   999.5 MH/s (74.66ms) @ Accel:128 Loops:256 Thr:64 Vec:1

Hashmode: 14600 - LUKS (Iterations: 163044)

Speed.#1.........:    26790 H/s (68.64ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 14700 - iTunes backup < 10.0 (Iterations: 9999)

Speed.#1.........:   435.4 kH/s (66.83ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 14800 - iTunes backup >= 10.0 (Iterations: 9999999)

Speed.#1.........:      351 H/s (85.31ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 14900 - Skip32 (PT = $salt, key = $pass)

Speed.#1.........: 12829.8 MH/s (4.44ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 15000 - FileZilla Server >= 0.9.55

Speed.#1.........:  2361.9 MH/s (63.14ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 15100 - Juniper/NetBSD sha1crypt (Iterations: 19999)

Speed.#1.........:   435.1 kH/s (67.05ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 15200 - Blockchain, My Wallet, V2 (Iterations: 4999)

Speed.#1.........:   862.7 kH/s (67.38ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:   180.4 kH/s (67.42ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 15400 - ChaCha20

Speed.#1.........: 10502.1 MH/s (229.42ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 15500 - JKS Java Key Store Private Keys (SHA1)

Speed.#1.........: 20030.1 MH/s (59.51ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 15600 - Ethereum Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1023)

Speed.#1.........:  3520.6 kH/s (64.96ms) @ Accel:512 Loops:255 Thr:64 Vec:1

Hashmode: 15700 - Ethereum Wallet, SCRYPT (Iterations: 1)

Speed.#1.........:        2 H/s (14849.87ms) @ Accel:1 Loops:1 Thr:1 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    81158 H/s (69.21ms) @ Accel:64 Loops:512 Thr:64 Vec:1

Hashmode: 16000 - Tripcode

Speed.#1.........:   471.6 MH/s (79.22ms) @ Accel:32 Loops:512 Thr:64 Vec:1

Hashmode: 16100 - TACACS+

Speed.#1.........: 31790.3 MH/s (75.25ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 16200 - Apple Secure Notes (Iterations: 19999)

Speed.#1.........:   184.2 kH/s (79.38ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 16300 - Ethereum Pre-Sale Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1999)

Speed.#1.........:  1807.0 kH/s (79.26ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 16400 - CRAM-MD5 Dovecot

Speed.#1.........: 52810.8 MH/s (45.07ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 16500 - JWT (JSON Web Token)

Speed.#1.........:  1703.6 MH/s (87.83ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 16600 - Electrum Wallet (Salt-Type 1-3)

Speed.#1.........:  1429.0 MH/s (51.95ms) @ Accel:64 Loops:512 Thr:64 Vec:1

Hashmode: 16700 - FileVault 2 (Iterations: 19999)

Speed.#1.........:   183.5 kH/s (79.76ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 16800 - WPA-PMKID-PBKDF2 (Iterations: 4095)

Speed.#1.........:  1065.1 kH/s (68.25ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 16801 - WPA-PMKID-PMK (Iterations: 0)

Speed.#1.........:   356.9 MH/s (0.00ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 16900 - Ansible Vault (Iterations: 9999)

Speed.#1.........:   366.4 kH/s (79.76ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 17200 - PKZIP (Compressed)

* Device #1: Skipping hash-mode 17200 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

Hashmode: 17210 - PKZIP (Uncompressed)

Speed.#1.........:  3658.1 MH/s (40.61ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 17220 - PKZIP (Compressed Multi-File)

* Device #1: Skipping hash-mode 17220 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

Hashmode: 17225 - PKZIP (Mixed Multi-File)

* Device #1: Skipping hash-mode 17225 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

Hashmode: 17230 - PKZIP (Mixed Multi-File Checksum-Only)

Speed.#1.........: 23672.8 MH/s (50.25ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 17300 - SHA3-224

Speed.#1.........:  1415.3 MH/s (52.57ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 17400 - SHA3-256

Speed.#1.........:  1427.0 MH/s (52.12ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 17500 - SHA3-384

Speed.#1.........:  1425.5 MH/s (52.12ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 17600 - SHA3-512

Speed.#1.........:  1427.3 MH/s (52.03ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 17700 - Keccak-224

Speed.#1.........:  1425.1 MH/s (52.09ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 17800 - Keccak-256

Speed.#1.........:  1427.4 MH/s (52.12ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 17900 - Keccak-384

Speed.#1.........:  1425.1 MH/s (52.14ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 18000 - Keccak-512

Speed.#1.........:  1427.0 MH/s (52.04ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 18100 - TOTP (HMAC-SHA1)

Speed.#1.........:  4404.4 MH/s (67.74ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 18200 - Kerberos 5, etype 23, AS-REP

Speed.#1.........:   876.6 MH/s (85.24ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 18300 - Apple File System (APFS) (Iterations: 19999)

Speed.#1.........:   184.1 kH/s (79.38ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 18400 - Open Document Format (ODF) 1.2 (SHA-256, AES) (Iterations: 99999)

Speed.#1.........:    43861 H/s (68.25ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 18500 - sha1(md5(md5($pass)))

Speed.#1.........:  7214.2 MH/s (82.91ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 18600 - Open Document Format (ODF) 1.1 (SHA-1, Blowfish) (Iterations: 1023)

Speed.#1.........:  1955.4 kH/s (62.83ms) @ Accel:512 Loops:1023 Thr:16 Vec:1

Hashmode: 18700 - Java Object hashCode()

Speed.#1.........:   130.7 GH/s (17.71ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 18800 - Blockchain, My Wallet, Second Password (SHA256) (Iterations: 9999)

Speed.#1.........:   737.4 kH/s (79.11ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 18900 - Android Backup (Iterations: 9999)

Speed.#1.........:   438.2 kH/s (66.59ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 19000 - QNX /etc/shadow (MD5) (Iterations: 1000)

Speed.#1.........:  7173.1 kH/s (79.22ms) @ Accel:512 Loops:500 Thr:64 Vec:1

Hashmode: 19100 - QNX /etc/shadow (SHA256) (Iterations: 1000)

Speed.#1.........: 11975.3 kH/s (92.99ms) @ Accel:512 Loops:1000 Thr:64 Vec:1

Hashmode: 19200 - QNX /etc/shadow (SHA512) (Iterations: 1000)

Speed.#1.........:  7838.0 kH/s (70.65ms) @ Accel:256 Loops:1000 Thr:64 Vec:1

Hashmode: 19300 - sha1($salt1.$pass.$salt2)

Speed.#1.........:  2720.1 MH/s (54.66ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 19500 - Ruby on Rails Restful-Authentication

Speed.#1.........:   548.8 MH/s (67.89ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 19600 - Kerberos 5, etype 17, TGS-REP (Iterations: 4095)

Speed.#1.........:  2118.4 kH/s (68.06ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 19700 - Kerberos 5, etype 18, TGS-REP (Iterations: 4095)

Speed.#1.........:  1062.6 kH/s (68.10ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 19800 - Kerberos 5, etype 17, Pre-Auth (Iterations: 4095)

Speed.#1.........:  2122.1 kH/s (67.90ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 19900 - Kerberos 5, etype 18, Pre-Auth (Iterations: 4095)

Speed.#1.........:  1061.1 kH/s (68.10ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 20011 - DiskCryptor SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:  1035.4 kH/s (61.86ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 20012 - DiskCryptor SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:   513.9 kH/s (62.00ms) @ Accel:128 Loops:124 Thr:64 Vec:1

Hashmode: 20013 - DiskCryptor SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:   341.5 kH/s (49.18ms) @ Accel:128 Loops:62 Thr:64 Vec:1

Hashmode: 20200 - Python passlib pbkdf2-sha512 (Iterations: 24999)

Speed.#1.........:    41836 H/s (71.58ms) @ Accel:128 Loops:256 Thr:64 Vec:1

Hashmode: 20300 - Python passlib pbkdf2-sha256 (Iterations: 28999)

Speed.#1.........:   120.1 kH/s (84.06ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 20400 - Python passlib pbkdf2-sha1 (Iterations: 130999)

Speed.#1.........:    66456 H/s (68.71ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 20500 - PKZIP Master Key

Speed.#1.........:   201.1 GH/s (11.30ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 20510 - PKZIP Master Key (6 byte optimization)

Speed.#1.........: 34861.8 MH/s (68.38ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 20600 - Oracle Transportation Management (SHA256) (Iterations: 999)

Speed.#1.........:  7238.5 kH/s (78.29ms) @ Accel:256 Loops:999 Thr:64 Vec:1

Hashmode: 20710 - sha256(sha256($pass).$salt)

Speed.#1.........:  2414.8 MH/s (61.72ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 20711 - AuthMe sha256

Speed.#1.........:  2405.6 MH/s (61.91ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 20800 - sha256(md5($pass))

Speed.#1.........:  6582.8 MH/s (90.84ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 20900 - md5(sha1($pass).md5($pass).sha1($pass))

Speed.#1.........:  5854.2 MH/s (50.82ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 21000 - BitShares v0.x - sha512(sha512_bin(pass))

Speed.#1.........:  1104.6 MH/s (67.67ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 21100 - sha1(md5($pass.$salt))

Speed.#1.........: 11056.4 MH/s (53.80ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 21200 - md5(sha1($salt).md5($pass))

Speed.#1.........: 11071.8 MH/s (53.70ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 21300 - md5($salt.sha1($salt.$pass))

Speed.#1.........:  7729.8 MH/s (77.34ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 21400 - sha256(sha256_bin($pass))

Speed.#1.........:  4015.3 MH/s (74.32ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 21500 - SolarWinds Orion (Iterations: 999)

Speed.#1.........:   165.0 kH/s (51.61ms) @ Accel:64 Loops:62 Thr:64 Vec:1

Hashmode: 21600 - Web2py pbkdf2-sha512 (Iterations: 999)

Speed.#1.........:  1039.1 kH/s (61.87ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 21700 - Electrum Wallet (Salt-Type 4) (Iterations: 1023)

* Device #1: Skipping hash-mode 21700 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

Hashmode: 21800 - Electrum Wallet (Salt-Type 5) (Iterations: 1023)

* Device #1: Skipping hash-mode 21800 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:  1072.0 kH/s (67.94ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 22001 - WPA-PMK-PMKID+EAPOL (Iterations: 0)

Speed.#1.........:   375.1 MH/s (0.00ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 22100 - BitLocker (Iterations: 1048576)

Speed.#1.........:     3984 H/s (71.73ms) @ Accel:32 Loops:4096 Thr:64 Vec:1

Hashmode: 22200 - Citrix NetScaler (SHA512)

Speed.#1.........:  2336.2 MH/s (63.75ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 22300 - sha256($salt.$pass.$salt)

Speed.#1.........:  7809.4 MH/s (76.55ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 22301 - Telegram Mobile App Passcode (SHA256)

Speed.#1.........:  7784.2 MH/s (76.73ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 22400 - AES Crypt (SHA256) (Iterations: 8191)

Speed.#1.........:   807.8 kH/s (89.64ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 22500 - MultiBit Classic .key (MD5)

Speed.#1.........:  1428.8 MH/s (51.97ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 22600 - Telegram Desktop App Passcode (PBKDF2-HMAC-SHA1) (Iterations: 3999)

Speed.#1.........:   310.5 kH/s (58.56ms) @ Accel:128 Loops:256 Thr:64 Vec:1

Hashmode: 22700 - MultiBit HD (scrypt) (Iterations: 1)

Speed.#1.........:      366 H/s (1569.74ms) @ Accel:1 Loops:1 Thr:16 Vec:1

Hashmode: 22911 - RSA/DSA/EC/OpenSSH Private Keys ($0$)

Speed.#1.........:  1365.4 MH/s (54.41ms) @ Accel:128 Loops:256 Thr:64 Vec:1

Hashmode: 22921 - RSA/DSA/EC/OpenSSH Private Keys ($6$)

Speed.#1.........:  5096.7 MH/s (58.39ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 22931 - RSA/DSA/EC/OpenSSH Private Keys ($1, $3$)

Speed.#1.........:  2082.3 MH/s (71.68ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 22941 - RSA/DSA/EC/OpenSSH Private Keys ($4$)

Speed.#1.........:  1749.9 MH/s (85.45ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 22951 - RSA/DSA/EC/OpenSSH Private Keys ($5$)

Speed.#1.........:  1517.9 MH/s (98.67ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 23001 - SecureZIP AES-128

Speed.#1.........:  2100.6 MH/s (71.11ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 23002 - SecureZIP AES-192

Speed.#1.........:  1663.8 MH/s (89.90ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 23003 - SecureZIP AES-256

Speed.#1.........:  1136.3 MH/s (65.54ms) @ Accel:64 Loops:512 Thr:64 Vec:1

Hashmode: 23100 - Apple Keychain (Iterations: 999)

Speed.#1.........:  4298.5 kH/s (44.02ms) @ Accel:256 Loops:499 Thr:64 Vec:1

Hashmode: 23200 - XMPP SCRAM PBKDF2-SHA1 (Iterations: 4095)

Speed.#1.........:  2127.9 kH/s (67.94ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 23300 - Apple iWork (Iterations: 3999)

Speed.#1.........:  2185.7 kH/s (66.13ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 23400 - Bitwarden (Iterations: 99999)

Speed.#1.........:    36900 H/s (81.19ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 23500 - AxCrypt 2 AES-128 (Iterations: 999)

Speed.#1.........:   141.0 kH/s (45.86ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 23600 - AxCrypt 2 AES-256 (Iterations: 999)

Speed.#1.........:    72172 H/s (90.19ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 23700 - RAR3-p (Uncompressed) (Iterations: 262144)

Speed.#1.........:   138.2 kH/s (65.06ms) @ Accel:64 Loops:16384 Thr:64 Vec:1

Hashmode: 23800 - RAR3-p (Compressed) (Iterations: 262144)

Speed.#1.........:   130.2 kH/s (65.08ms) @ Accel:64 Loops:16384 Thr:64 Vec:1

Hashmode: 23900 - BestCrypt v3 Volume Encryption (Iterations: 1)

Speed.#1.........:  5827.3 kH/s (93.96ms) @ Accel:256 Loops:1 Thr:64 Vec:1

Hashmode: 24410 - PKCS#8 Private Keys (PBKDF2-HMAC-SHA1 + 3DES/AES) (Iterations: 2047)

Speed.#1.........:  2118.5 kH/s (67.96ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 24420 - PKCS#8 Private Keys (PBKDF2-HMAC-SHA256 + 3DES/AES) (Iterations: 2047)

Speed.#1.........:  1706.2 kH/s (84.82ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 99999 - Plaintext

Speed.#1.........: 85875.3 MH/s (27.41ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Started: Fri Dec 18 22:56:59 2020
Stopped: Sat Dec 19 00:20:44 2020
```
