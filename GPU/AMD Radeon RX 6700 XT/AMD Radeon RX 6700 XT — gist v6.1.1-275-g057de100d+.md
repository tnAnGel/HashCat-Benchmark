# AMD Radeon RX 6700 XT

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 6700 XT
- **Версия hashcat / Version:** v6.1.1-275-g057de100d+
- **Источник / Source:** [gist](https://gist.github.com/9500be7a04126a3c7182e4bc088c2b27)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 32145.1 MH/s |
| 100 | SHA1 | 12650.0 MH/s |
| 1400 | SHA2-256 | 5369.7 MH/s |
| 1700 | SHA2-512 | 1429.5 MH/s |
| 1000 | NTLM | 51847.3 MH/s |
| 3200 | bcrypt | 29618 H/s |
| 1800 | sha512crypt | 183.9 kH/s |
| 500 | md5crypt | 13206.7 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 647.1 kH/s |
| 2500 | WPA/WPA2 (legacy) | 646.5 kH/s |
| 7500 | Kerberos AS-REQ (23) | 514.2 MH/s |
| 13100 | Kerberos TGS-REP (23) | 505.8 MH/s |
| 11300 | Bitcoin wallet.dat | 6616 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 395.8 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.1.1-275-g057de100d+) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL API (OpenCL 2.1 AMD-APP (3180.7)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: gfx1031, 12160/12272 MB (10213 MB allocatable), 20MCU

Benchmark relevant options:
===========================
* --opencl-device-types=2
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........: 32145.1 MH/s (40.98ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........: 12650.0 MH/s (52.25ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  5369.7 MH/s (61.71ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1429.5 MH/s (57.80ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   647.1 kH/s (62.48ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 51847.3 MH/s (24.93ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 31896.8 MH/s (41.11ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 35034.1 MH/s (37.45ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  2163.3 MH/s (76.65ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1163.5 MH/s (71.09ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 13206.7 kH/s (92.61ms) @ Accel:1024 Loops:1000 Thr:64 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    29618 H/s (32.86ms) @ Accel:128 Loops:16 Thr:16 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   183.9 kH/s (87.94ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   514.2 MH/s (80.62ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   505.8 MH/s (82.03ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

* Device #1: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#1.........:   110.7 kH/s (62.52ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

* Device #1: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#1.........:    49093 H/s (65.61ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   614.0 kH/s (58.17ms) @ Accel:256 Loops:127 Thr:64 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   689.3 kH/s (57.47ms) @ Accel:128 Loops:4096 Thr:64 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    86139 H/s (58.77ms) @ Accel:64 Loops:16384 Thr:64 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    67962 H/s (74.62ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   395.8 kH/s (50.23ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    55227 H/s (246.50ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  4308.4 kH/s (48.24ms) @ Accel:512 Loops:249 Thr:64 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     6616 H/s (62.70ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Started: Wed Apr 28 17:46:17 2021
Stopped: Wed Apr 28 17:48:03 2021

## Full Benchmark

hashcat (v6.1.1-275-g057de100d+) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL API (OpenCL 2.1 AMD-APP (3180.7)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: gfx1031, 12160/12272 MB (10213 MB allocatable), 20MCU

Benchmark relevant options:
===========================
* --benchmark-all
* --opencl-device-types=2
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........: 32055.4 MH/s (40.90ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 10 - md5($pass.$salt)

Speed.#1.........: 32182.4 MH/s (40.92ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 11 - Joomla < 2.5.18

Speed.#1.........: 31888.0 MH/s (41.20ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 12 - PostgreSQL

Speed.#1.........: 31937.3 MH/s (41.22ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 20 - md5($salt.$pass)

Speed.#1.........: 16594.5 MH/s (79.94ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 21 - osCommerce, xt:Commerce

Speed.#1.........: 16574.7 MH/s (80.04ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 22 - Juniper NetScreen/SSG (ScreenOS)

Speed.#1.........: 16839.2 MH/s (78.80ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 23 - Skype

Speed.#1.........: 16691.2 MH/s (79.52ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 30 - md5(utf16le($pass).$salt)

Speed.#1.........: 32203.3 MH/s (40.89ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 40 - md5($salt.utf16le($pass))

Speed.#1.........: 16666.3 MH/s (79.61ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 50 - HMAC-MD5 (key = $pass)

Speed.#1.........:  4980.5 MH/s (66.50ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 60 - HMAC-MD5 (key = $salt)

Speed.#1.........:  9866.1 MH/s (67.13ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........: 12645.5 MH/s (52.15ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 101 - nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.#1.........: 12645.6 MH/s (52.17ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 110 - sha1($pass.$salt)

Speed.#1.........: 12731.3 MH/s (51.80ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 111 - nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.#1.........: 12641.9 MH/s (52.17ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 112 - Oracle S: Type (Oracle 11+)

Speed.#1.........: 12750.2 MH/s (51.79ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 120 - sha1($salt.$pass)

Speed.#1.........:  9911.3 MH/s (66.74ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 121 - SMF (Simple Machines Forum) > v1.1

Speed.#1.........:  9912.3 MH/s (66.72ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 122 - macOS v10.4, macOS v10.5, MacOS v10.6

Speed.#1.........:  9905.3 MH/s (66.79ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 124 - Django (SHA-1)

Speed.#1.........:  9905.0 MH/s (66.79ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 125 - ArubaOS

Speed.#1.........:  9910.5 MH/s (66.80ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 130 - sha1(utf16le($pass).$salt)

Speed.#1.........: 12746.6 MH/s (51.67ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 131 - MSSQL (2000)

Speed.#1.........: 12743.5 MH/s (51.34ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 132 - MSSQL (2005)

Speed.#1.........: 12763.5 MH/s (51.67ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 133 - PeopleSoft

Speed.#1.........: 12664.0 MH/s (52.09ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 140 - sha1($salt.utf16le($pass))

Speed.#1.........:  9910.2 MH/s (66.80ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 141 - Episerver 6.x < .NET 4

Speed.#1.........:  9918.3 MH/s (66.74ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 150 - HMAC-SHA1 (key = $pass)

Speed.#1.........:  2889.4 MH/s (57.14ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 160 - HMAC-SHA1 (key = $salt)

Speed.#1.........:  5424.5 MH/s (60.95ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 200 - MySQL323

Speed.#1.........: 78381.6 MH/s (16.33ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 300 - MySQL4.1/MySQL5

Speed.#1.........:  5631.8 MH/s (58.61ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 400 - phpass (Iterations: 2048)

Speed.#1.........:  9322.6 kH/s (66.91ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 13207.0 kH/s (92.39ms) @ Accel:1024 Loops:1000 Thr:64 Vec:1

Hashmode: 501 - Juniper IVE (Iterations: 1000)

Speed.#1.........: 13251.0 kH/s (92.49ms) @ Accel:1024 Loops:1000 Thr:64 Vec:1

Hashmode: 600 - BLAKE2b-512

Speed.#1.........:  2969.7 MH/s (55.57ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 900 - MD4

Speed.#1.........: 51888.1 MH/s (24.97ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........: 52244.7 MH/s (24.93ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 1100 - Domain Cached Credentials (DCC), MS Cache

Speed.#1.........: 17991.3 MH/s (73.68ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 1300 - SHA2-224

Speed.#1.........:  5255.0 MH/s (62.94ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  5367.9 MH/s (61.62ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 1410 - sha256($pass.$salt)

Speed.#1.........:  5377.0 MH/s (61.47ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 1411 - SSHA-256(Base64), LDAP {SSHA256}

Speed.#1.........:  5366.3 MH/s (61.61ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 1420 - sha256($salt.$pass)

Speed.#1.........:  4833.5 MH/s (68.49ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 1421 - hMailServer

Speed.#1.........:  4832.6 MH/s (68.50ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 1430 - sha256(utf16le($pass).$salt)

Speed.#1.........:  5380.2 MH/s (61.44ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 1440 - sha256($salt.utf16le($pass))

Speed.#1.........:  4838.1 MH/s (68.46ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 1441 - Episerver 6.x >= .NET 4

Speed.#1.........:  4839.8 MH/s (68.46ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 1450 - HMAC-SHA256 (key = $pass)

Speed.#1.........:  1059.9 MH/s (78.23ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 1460 - HMAC-SHA256 (key = $salt)

Speed.#1.........:  2310.9 MH/s (71.68ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1163.3 MH/s (71.02ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 1600 - Apache $apr1$ MD5, md5apr1, MD5 (APR) (Iterations: 1000)

Speed.#1.........: 13201.4 kH/s (92.56ms) @ Accel:1024 Loops:1000 Thr:64 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1430.4 MH/s (57.73ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 1710 - sha512($pass.$salt)

Speed.#1.........:  1270.8 MH/s (65.09ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 1711 - SSHA-512(Base64), LDAP {SSHA512}

Speed.#1.........:  1273.8 MH/s (64.95ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 1720 - sha512($salt.$pass)

Speed.#1.........:  1373.6 MH/s (60.14ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 1722 - macOS v10.7

Speed.#1.........:  1368.8 MH/s (60.40ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 1730 - sha512(utf16le($pass).$salt)

Speed.#1.........:  1272.6 MH/s (65.09ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 1731 - MSSQL (2012, 2014)

Speed.#1.........:  1274.3 MH/s (64.92ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 1740 - sha512($salt.utf16le($pass))

Speed.#1.........:  1262.1 MH/s (65.58ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 1750 - HMAC-SHA512 (key = $pass)

Speed.#1.........:   308.9 MH/s (67.02ms) @ Accel:128 Loops:128 Thr:64 Vec:1

Hashmode: 1760 - HMAC-SHA512 (key = $salt)

Speed.#1.........:   632.2 MH/s (65.47ms) @ Accel:128 Loops:256 Thr:64 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   184.3 kH/s (87.73ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 2000 - STDOUT

Speed.#1.........:  4702.8 GH/s (0.05ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 2100 - Domain Cached Credentials 2 (DCC2), MS Cache 2 (Iterations: 10239)

* Device #1: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#1.........:   516.9 kH/s (62.47ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 2400 - Cisco-PIX MD5

Speed.#1.........: 21484.0 MH/s (61.68ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 2410 - Cisco-ASA MD5

Speed.#1.........: 21391.0 MH/s (61.82ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#1.........:   646.5 kH/s (62.44ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 2501 - WPA-EAPOL-PMK (Iterations: 0)

Speed.#1.........:   294.4 MH/s (0.00ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 2600 - md5(md5($pass))

Speed.#1.........:  9562.3 MH/s (69.25ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 2611 - vBulletin < v3.8.5

Speed.#1.........:  9568.2 MH/s (69.23ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 2612 - PHPS

Speed.#1.........:  9567.3 MH/s (69.23ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 2711 - vBulletin >= v3.8.5

Speed.#1.........:  6473.7 MH/s (50.92ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 2811 - MyBB 1.2+, IPB2+ (Invision Power Board)

Speed.#1.........:  6764.1 MH/s (98.33ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 3000 - LM

Speed.#1.........: 31922.2 MH/s (41.06ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 3100 - Oracle H: Type (Oracle 7+)

Speed.#1.........:   777.6 MH/s (53.06ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    29540 H/s (32.86ms) @ Accel:128 Loops:16 Thr:16 Vec:1

Hashmode: 3710 - md5($salt.md5($pass))

Speed.#1.........:  8727.4 MH/s (75.96ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 3711 - MediaWiki B type

Speed.#1.........:  8721.0 MH/s (76.03ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 3800 - md5($salt.$pass.$salt)

Speed.#1.........: 16546.0 MH/s (80.16ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 3910 - md5(md5($pass).md5($salt))

Speed.#1.........:  6478.7 MH/s (50.87ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 4010 - md5($salt.md5($salt.$pass))

Speed.#1.........:  7745.1 MH/s (85.72ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 4110 - md5($salt.md5($pass.$salt))

Speed.#1.........:  8685.3 MH/s (76.35ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 4300 - md5(strtoupper(md5($pass)))

Speed.#1.........:  9567.1 MH/s (69.22ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 4400 - md5(sha1($pass))

Speed.#1.........:  6523.4 MH/s (50.53ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 4500 - sha1(sha1($pass))

Speed.#1.........:  5157.3 MH/s (64.14ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 4510 - sha1(sha1($pass).$salt)

Speed.#1.........:  4964.4 MH/s (66.66ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 4520 - sha1($salt.sha1($pass))

Speed.#1.........:  3143.3 MH/s (52.45ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 4521 - Redmine

Speed.#1.........:  3144.4 MH/s (52.45ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 4522 - PunBB

Speed.#1.........:  4802.3 MH/s (68.95ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 4700 - sha1(md5($pass))

Speed.#1.........:  6809.3 MH/s (97.66ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 4710 - sha1(md5($pass).$salt)

Speed.#1.........:  6379.1 MH/s (51.70ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 4711 - Huawei sha1(md5($pass).$salt)

Speed.#1.........:  6388.9 MH/s (51.70ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 4800 - iSCSI CHAP authentication, MD5(CHAP)

Speed.#1.........: 21149.6 MH/s (62.62ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 4900 - sha1($salt.$pass.$salt)

Speed.#1.........:  9749.2 MH/s (67.93ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 5100 - Half MD5

Speed.#1.........: 19632.7 MH/s (67.54ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5200 - Password Safe v3 (Iterations: 2049)

Speed.#1.........:  2159.4 kH/s (66.08ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 5300 - IKE-PSK MD5

Speed.#1.........:  1178.2 MH/s (70.28ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 5400 - IKE-PSK SHA1

Speed.#1.........:   627.0 MH/s (65.99ms) @ Accel:128 Loops:256 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 35162.3 MH/s (37.40ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  2167.1 MH/s (76.49ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 5700 - Cisco-IOS type 4 (SHA256)

Speed.#1.........:  5367.3 MH/s (61.61ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 5800 - Samsung Android Password/PIN (Iterations: 1023)

Speed.#1.........:  8957.7 kH/s (46.10ms) @ Accel:1024 Loops:511 Thr:64 Vec:1

Hashmode: 6000 - RIPEMD-160

Speed.#1.........:  6856.9 MH/s (96.99ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 6100 - Whirlpool

Speed.#1.........:   669.9 MH/s (61.69ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   396.2 kH/s (50.20ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 6212 - TrueCrypt RIPEMD160 + XTS 1024 bit (Iterations: 1999)

Speed.#1.........:   231.9 kH/s (86.74ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 6213 - TrueCrypt RIPEMD160 + XTS 1536 bit (Iterations: 1999)

Speed.#1.........:   160.7 kH/s (62.04ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 6221 - TrueCrypt SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:   623.7 kH/s (56.83ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 6222 - TrueCrypt SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:   310.7 kH/s (56.87ms) @ Accel:128 Loops:124 Thr:64 Vec:1

Hashmode: 6223 - TrueCrypt SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:   207.0 kH/s (85.45ms) @ Accel:128 Loops:124 Thr:64 Vec:1

Hashmode: 6231 - TrueCrypt Whirlpool + XTS 512 bit (Iterations: 999)

Speed.#1.........:    73746 H/s (64.49ms) @ Accel:64 Loops:62 Thr:64 Vec:1

Hashmode: 6232 - TrueCrypt Whirlpool + XTS 1024 bit (Iterations: 999)

Speed.#1.........:    36551 H/s (65.02ms) @ Accel:32 Loops:62 Thr:64 Vec:1

Hashmode: 6233 - TrueCrypt Whirlpool + XTS 1536 bit (Iterations: 999)

Speed.#1.........:    25710 H/s (95.55ms) @ Accel:64 Loops:31 Thr:64 Vec:1

Hashmode: 6241 - TrueCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 999)

Speed.#1.........:   784.4 kH/s (49.98ms) @ Accel:32 Loops:999 Thr:64 Vec:1

Hashmode: 6242 - TrueCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 999)

Speed.#1.........:   458.9 kH/s (77.10ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 6243 - TrueCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 999)

Speed.#1.........:   316.0 kH/s (55.14ms) @ Accel:128 Loops:124 Thr:64 Vec:1

Hashmode: 6300 - AIX {smd5} (Iterations: 1000)

Speed.#1.........: 13198.4 kH/s (92.50ms) @ Accel:1024 Loops:1000 Thr:64 Vec:1

Hashmode: 6400 - AIX {ssha256} (Iterations: 63)

Speed.#1.........: 28789.0 kH/s (37.78ms) @ Accel:1024 Loops:63 Thr:64 Vec:1

Hashmode: 6500 - AIX {ssha512} (Iterations: 63)

Speed.#1.........:  8861.1 kH/s (63.77ms) @ Accel:512 Loops:63 Thr:64 Vec:1

Hashmode: 6600 - 1Password, agilekeychain (Iterations: 999)

Speed.#1.........:  5141.8 kH/s (40.43ms) @ Accel:512 Loops:499 Thr:64 Vec:1

Hashmode: 6700 - AIX {ssha1} (Iterations: 63)

Speed.#1.........: 58854.2 kH/s (15.02ms) @ Accel:1024 Loops:63 Thr:64 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  4298.7 kH/s (48.25ms) @ Accel:512 Loops:249 Thr:64 Vec:1

Hashmode: 6900 - GOST R 34.11-94

Speed.#1.........:   398.4 MH/s (51.74ms) @ Accel:64 Loops:256 Thr:64 Vec:1

Hashmode: 7000 - FortiGate (FortiOS)

Speed.#1.........: 11456.9 MH/s (57.67ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   612.9 kH/s (58.24ms) @ Accel:256 Loops:127 Thr:64 Vec:1

Hashmode: 7200 - GRUB 2 (Iterations: 1023)

Speed.#1.........:   612.6 kH/s (58.25ms) @ Accel:256 Loops:127 Thr:64 Vec:1

Hashmode: 7300 - IPMI2 RAKP HMAC-SHA1

Speed.#1.........:  1630.3 MH/s (50.53ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 7400 - sha256crypt $5$, SHA256 (Unix) (Iterations: 5000)

Speed.#1.........:   508.7 kH/s (62.93ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 7401 - MySQL $A$ (sha256crypt) (Iterations: 5000)

Speed.#1.........:   481.0 kH/s (66.55ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   514.9 MH/s (80.64ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 7700 - SAP CODVN B (BCODE)

Speed.#1.........:  1382.5 MH/s (59.84ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 7701 - SAP CODVN B (BCODE) from RFC_READ_TABLE

Speed.#1.........:  1386.4 MH/s (59.66ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 7800 - SAP CODVN F/G (PASSCODE)

Speed.#1.........:  1286.9 MH/s (64.28ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 7801 - SAP CODVN F/G (PASSCODE) from RFC_READ_TABLE

Speed.#1.........:  1306.9 MH/s (63.26ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 7900 - Drupal7 (Iterations: 16384)

Speed.#1.........:    79873 H/s (63.43ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 8000 - Sybase ASE

Speed.#1.........:   655.8 MH/s (63.04ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 8100 - Citrix NetScaler (SHA1)

Speed.#1.........: 11217.0 MH/s (58.90ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 8200 - 1Password, cloudkeychain (Iterations: 39999)

Speed.#1.........:    15823 H/s (65.62ms) @ Accel:128 Loops:256 Thr:64 Vec:1

Hashmode: 8300 - DNSSEC (NSEC3)

Speed.#1.........:  4928.4 MH/s (67.15ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 8400 - WBB3 (Woltlab Burning Board)

Speed.#1.........:  2147.6 MH/s (77.17ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 8500 - RACF

Speed.#1.........:  4310.8 MH/s (76.92ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 8600 - Lotus Notes/Domino 5

Speed.#1.........:   328.1 MH/s (63.00ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 8700 - Lotus Notes/Domino 6

Speed.#1.........:   113.6 MH/s (91.36ms) @ Accel:256 Loops:32 Thr:64 Vec:1

Hashmode: 8800 - Android FDE <= 4.3 (Iterations: 1999)

Speed.#1.........:  1311.3 kH/s (60.93ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 8900 - scrypt (Iterations: 16384)

Speed.#1.........:     1346 H/s (41.60ms) @ Accel:20 Loops:1024 Thr:64 Vec:1

Hashmode: 9000 - Password Safe v2 (Iterations: 1000)

Speed.#1.........:   735.1 kH/s (34.68ms) @ Accel:128 Loops:1000 Thr:16 Vec:1

Hashmode: 9100 - Lotus Notes/Domino 8 (Iterations: 4999)

Speed.#1.........:  1049.0 kH/s (61.03ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 9200 - Cisco-IOS $8$ (PBKDF2-SHA256) (Iterations: 19999)

Speed.#1.........:   106.4 kH/s (76.29ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 9300 - Cisco-IOS $9$ (scrypt) (Iterations: 16384)

Speed.#1.........:    19428 H/s (1.01ms) @ Accel:20 Loops:1024 Thr:64 Vec:1

Hashmode: 9400 - MS Office 2007 (Iterations: 50000)

Speed.#1.........:   210.7 kH/s (62.93ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 9500 - MS Office 2010 (Iterations: 100000)

Speed.#1.........:   105.4 kH/s (62.92ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 9600 - MS Office 2013 (Iterations: 100000)

Speed.#1.........:    13148 H/s (63.12ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 9700 - MS Office <= 2003 $0/$1, MD5 + RC4

Speed.#1.........:   466.4 MH/s (89.04ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 9710 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.#1.........:   558.9 MH/s (74.35ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 9720 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #2

Speed.#1.........:  2408.6 MH/s (68.73ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 9800 - MS Office <= 2003 $3/$4, SHA1 + RC4

Speed.#1.........:   540.9 MH/s (76.63ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 9810 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.#1.........:   575.9 MH/s (71.96ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 9820 - MS Office <= 2003 $3, SHA1 + RC4, collider #2

Speed.#1.........:  4977.3 MH/s (66.48ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 9900 - Radmin2

Speed.#1.........: 10468.5 MH/s (63.17ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 10000 - Django (PBKDF2-SHA256) (Iterations: 9999)

Speed.#1.........:   212.7 kH/s (76.25ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 10100 - SipHash

Speed.#1.........: 42738.8 MH/s (30.61ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 10200 - CRAM-MD5

Speed.#1.........:  4976.8 MH/s (66.50ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 10300 - SAP CODVN H (PWDSALTEDHASH) iSSHA-1 (Iterations: 1023)

Speed.#1.........:  8433.6 kH/s (49.15ms) @ Accel:1024 Loops:511 Thr:64 Vec:1

Hashmode: 10400 - PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.#1.........:   595.0 MH/s (69.61ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 10410 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.#1.........:   631.7 MH/s (65.61ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 10420 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #2

Speed.#1.........: 10156.2 MH/s (65.24ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 10500 - PDF 1.4 - 1.6 (Acrobat 5 - 8) (Iterations: 70)

Speed.#1.........: 26291.5 kH/s (43.92ms) @ Accel:1024 Loops:70 Thr:64 Vec:1

Hashmode: 10600 - PDF 1.7 Level 3 (Acrobat 9)

Speed.#1.........:  5362.8 MH/s (61.65ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 10700 - PDF 1.7 Level 8 (Acrobat 10 - 11) (Iterations: 64)

Speed.#1.........:    78404 H/s (64.53ms) @ Accel:16 Loops:16 Thr:64 Vec:1

Hashmode: 10800 - SHA2-384

Speed.#1.........:  1410.3 MH/s (58.62ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 10900 - PBKDF2-HMAC-SHA256 (Iterations: 999)

Speed.#1.........:  2099.3 kH/s (60.84ms) @ Accel:512 Loops:249 Thr:64 Vec:1

Hashmode: 10901 - RedHat 389-DS LDAP (PBKDF2-HMAC-SHA256) (Iterations: 8191)

Speed.#1.........:   259.6 kH/s (78.09ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 11000 - PrestaShop

Speed.#1.........: 11069.7 MH/s (59.69ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 11100 - PostgreSQL CRAM (MD5)

Speed.#1.........:  9560.6 MH/s (69.27ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 11200 - MySQL CRAM (SHA1)

Speed.#1.........:  3530.8 MH/s (94.11ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     6613 H/s (62.64ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 11400 - SIP digest authentication (MD5)

Speed.#1.........:  4519.9 MH/s (73.32ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 11500 - CRC32

Speed.#1.........: 55555.9 MH/s (23.34ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   685.7 kH/s (57.46ms) @ Accel:128 Loops:4096 Thr:64 Vec:1

Hashmode: 11700 - GOST R 34.11-2012 (Streebog) 256-bit, big-endian

Speed.#1.........: 76618.8 kH/s (67.48ms) @ Accel:16 Loops:256 Thr:64 Vec:1

Hashmode: 11750 - HMAC-Streebog-256 (key = $pass), big-endian

Speed.#1.........: 27796.9 kH/s (93.41ms) @ Accel:64 Loops:32 Thr:64 Vec:1

Hashmode: 11760 - HMAC-Streebog-256 (key = $salt), big-endian

Speed.#1.........: 34750.5 kH/s (74.54ms) @ Accel:64 Loops:32 Thr:64 Vec:1

Hashmode: 11800 - GOST R 34.11-2012 (Streebog) 512-bit, big-endian

Speed.#1.........: 77688.9 kH/s (66.58ms) @ Accel:16 Loops:256 Thr:64 Vec:1

Hashmode: 11850 - HMAC-Streebog-512 (key = $pass), big-endian

Speed.#1.........: 21947.7 kH/s (58.80ms) @ Accel:16 Loops:64 Thr:64 Vec:1

Hashmode: 11860 - HMAC-Streebog-512 (key = $salt), big-endian

Speed.#1.........: 29471.2 kH/s (88.04ms) @ Accel:64 Loops:32 Thr:64 Vec:1

Hashmode: 11900 - PBKDF2-HMAC-MD5 (Iterations: 999)

Speed.#1.........:  9141.0 kH/s (44.33ms) @ Accel:1024 Loops:499 Thr:64 Vec:1

Hashmode: 12000 - PBKDF2-HMAC-SHA1 (Iterations: 999)

Speed.#1.........:  5076.6 kH/s (40.76ms) @ Accel:512 Loops:499 Thr:64 Vec:1

Hashmode: 12001 - Atlassian (PBKDF2-HMAC-SHA1) (Iterations: 9999)

Speed.#1.........:   528.3 kH/s (61.16ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 12100 - PBKDF2-HMAC-SHA512 (Iterations: 999)

Speed.#1.........:   627.7 kH/s (56.82ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 12200 - eCryptfs (Iterations: 65536)

Speed.#1.........:    20199 H/s (62.73ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 12300 - Oracle T: Type (Oracle 12+) (Iterations: 4095)

Speed.#1.........:   154.0 kH/s (65.57ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 12400 - BSDi Crypt, Extended DES (Iterations: 2194)

Speed.#1.........:  3272.4 kH/s (64.95ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    86019 H/s (58.82ms) @ Accel:64 Loops:16384 Thr:64 Vec:1

Hashmode: 12600 - ColdFusion 10+

Speed.#1.........:  3144.2 MH/s (52.45ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 12700 - Blockchain, My Wallet (Iterations: 9)

Speed.#1.........:   105.9 MH/s (4.33ms) @ Accel:1024 Loops:9 Thr:64 Vec:1

Hashmode: 12800 - MS-AzureSync PBKDF2-HMAC-SHA256 (Iterations: 99)

Speed.#1.........: 19872.4 kH/s (56.63ms) @ Accel:1024 Loops:99 Thr:64 Vec:1

Hashmode: 12900 - Android FDE (Samsung DEK) (Iterations: 4095)

Speed.#1.........:   541.3 kH/s (74.61ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    67937 H/s (74.62ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   505.8 MH/s (82.02ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 13200 - AxCrypt 1 (Iterations: 10467)

Speed.#1.........:   178.9 kH/s (178.26ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 13300 - AxCrypt 1 in-memory SHA1

Speed.#1.........: 11854.5 MH/s (55.69ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    54263 H/s (250.77ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 13500 - PeopleSoft PS_TOKEN

Speed.#1.........:  9133.4 MH/s (72.56ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 13600 - WinZip (Iterations: 999)

Speed.#1.........:  5043.9 kH/s (60.69ms) @ Accel:256 Loops:999 Thr:64 Vec:1

Hashmode: 13711 - VeraCrypt RIPEMD160 + XTS 512 bit (Iterations: 655330)

Speed.#1.........:     1211 H/s (25.39ms) @ Accel:32 Loops:1000 Thr:64 Vec:1

Hashmode: 13712 - VeraCrypt RIPEMD160 + XTS 1024 bit (Iterations: 655330)

Speed.#1.........:      708 H/s (43.70ms) @ Accel:256 Loops:125 Thr:64 Vec:1

Hashmode: 13713 - VeraCrypt RIPEMD160 + XTS 1536 bit (Iterations: 655330)

Speed.#1.........:      494 H/s (31.22ms) @ Accel:128 Loops:125 Thr:64 Vec:1

Hashmode: 13721 - VeraCrypt SHA512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:     1254 H/s (32.26ms) @ Accel:64 Loops:500 Thr:64 Vec:1

Hashmode: 13722 - VeraCrypt SHA512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      628 H/s (32.20ms) @ Accel:128 Loops:125 Thr:64 Vec:1

Hashmode: 13723 - VeraCrypt SHA512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      421 H/s (48.24ms) @ Accel:128 Loops:125 Thr:64 Vec:1

Hashmode: 13731 - VeraCrypt Whirlpool + XTS 512 bit (Iterations: 499999)

Speed.#1.........:      150 H/s (33.39ms) @ Accel:64 Loops:62 Thr:64 Vec:1

Hashmode: 13732 - VeraCrypt Whirlpool + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:       65 H/s (38.47ms) @ Accel:32 Loops:62 Thr:64 Vec:1

Hashmode: 13733 - VeraCrypt Whirlpool + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:       48 H/s (52.82ms) @ Accel:64 Loops:31 Thr:64 Vec:1

Hashmode: 13741 - VeraCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 327660)

Speed.#1.........:     2421 H/s (26.03ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

Hashmode: 13742 - VeraCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 327660)

Speed.#1.........:     1415 H/s (44.75ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 13743 - VeraCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 327660)

Speed.#1.........:      979 H/s (31.95ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 13751 - VeraCrypt SHA256 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:     2100 H/s (38.58ms) @ Accel:256 Loops:250 Thr:64 Vec:1

Hashmode: 13752 - VeraCrypt SHA256 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:     1053 H/s (38.48ms) @ Accel:128 Loops:250 Thr:64 Vec:1

Hashmode: 13753 - VeraCrypt SHA256 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      689 H/s (29.33ms) @ Accel:16 Loops:1000 Thr:64 Vec:1

Hashmode: 13761 - VeraCrypt SHA256 + XTS 512 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     5247 H/s (39.54ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 13762 - VeraCrypt SHA256 + XTS 1024 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     2633 H/s (39.42ms) @ Accel:128 Loops:256 Thr:64 Vec:1

Hashmode: 13763 - VeraCrypt SHA256 + XTS 1536 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     1731 H/s (29.54ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 13771 - VeraCrypt Streebog-512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:       47 H/s (53.62ms) @ Accel:32 Loops:62 Thr:64 Vec:1

Hashmode: 13772 - VeraCrypt Streebog-512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:       22 H/s (57.56ms) @ Accel:16 Loops:62 Thr:64 Vec:1

Hashmode: 13773 - VeraCrypt Streebog-512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:       14 H/s (86.28ms) @ Accel:16 Loops:62 Thr:64 Vec:1

Hashmode: 13800 - Windows Phone 8+ PIN/password

Speed.#1.........:  1358.9 MH/s (60.82ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 13900 - OpenCart

Speed.#1.........:  3377.4 MH/s (98.40ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 14000 - DES (PT = $salt, key = $pass)

Speed.#1.........: 31311.0 MH/s (41.68ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 14100 - 3DES (PT = $salt, key = $pass)

Speed.#1.........:  4525.5 MH/s (73.19ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 14400 - sha1(CX)

Speed.#1.........:   612.4 MH/s (67.56ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 14600 - LUKS (Iterations: 163044)

Speed.#1.........:    16264 H/s (62.60ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 14700 - iTunes backup < 10.0 (Iterations: 9999)

Speed.#1.........:   263.9 kH/s (61.12ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 14800 - iTunes backup >= 10.0 (Iterations: 9999999)

Speed.#1.........:      212 H/s (78.13ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 14900 - Skip32 (PT = $salt, key = $pass)

Speed.#1.........:  7148.2 MH/s (8.59ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 15000 - FileZilla Server >= 0.9.55

Speed.#1.........:  1425.7 MH/s (57.92ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 15100 - Juniper/NetBSD sha1crypt (Iterations: 19999)

Speed.#1.........:   266.3 kH/s (62.24ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 15200 - Blockchain, My Wallet, V2 (Iterations: 4999)

Speed.#1.........:   529.7 kH/s (61.00ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

* Device #1: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#1.........:   110.6 kH/s (62.48ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 15400 - ChaCha20

Speed.#1.........:  6446.5 MH/s (207.25ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 15500 - JKS Java Key Store Private Keys (SHA1)

Speed.#1.........: 12169.4 MH/s (54.24ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 15600 - Ethereum Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1023)

Speed.#1.........:  2138.4 kH/s (59.54ms) @ Accel:512 Loops:255 Thr:64 Vec:1

Hashmode: 15700 - Ethereum Wallet, SCRYPT (Iterations: 262144)

Speed.#1.........:        0 H/s (12.04ms) @ Accel:1 Loops:1024 Thr:4 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

* Device #1: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#1.........:    49090 H/s (65.59ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 16000 - Tripcode

Speed.#1.........:   292.6 MH/s (70.80ms) @ Accel:64 Loops:256 Thr:64 Vec:1

Hashmode: 16100 - TACACS+

Speed.#1.........: 19320.2 MH/s (68.64ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 16200 - Apple Secure Notes (Iterations: 19999)

Speed.#1.........:   111.6 kH/s (74.56ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 16300 - Ethereum Pre-Sale Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1999)

Speed.#1.........:  1094.7 kH/s (72.80ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 16400 - CRAM-MD5 Dovecot

Speed.#1.........: 32043.6 MH/s (41.11ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 16500 - JWT (JSON Web Token)

Speed.#1.........:  1050.2 MH/s (79.07ms) @ Accel:256 Loops:256 Thr:64 Vec:1

Hashmode: 16600 - Electrum Wallet (Salt-Type 1-3)

Speed.#1.........:   877.0 MH/s (94.67ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 16700 - FileVault 2 (Iterations: 19999)

Speed.#1.........:   111.6 kH/s (74.54ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 16800 - WPA-PMKID-PBKDF2 (Iterations: 4095)

Speed.#1.........:   647.5 kH/s (62.48ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 16801 - WPA-PMKID-PMK (Iterations: 0)

Speed.#1.........:   296.7 MH/s (0.00ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 16900 - Ansible Vault (Iterations: 9999)

Speed.#1.........:   222.7 kH/s (72.85ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 17200 - PKZIP (Compressed)

Speed.#1.........: 26613.7 kH/s (343.89ms) @ Accel:28 Loops:256 Thr:64 Vec:1

Hashmode: 17210 - PKZIP (Uncompressed)

Speed.#1.........:  2134.9 MH/s (77.75ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 17220 - PKZIP (Compressed Multi-File)

Speed.#1.........: 93892.1 kH/s (54.94ms) @ Accel:64 Loops:64 Thr:64 Vec:1

Hashmode: 17225 - PKZIP (Mixed Multi-File)

Speed.#1.........:   108.0 MH/s (47.60ms) @ Accel:128 Loops:32 Thr:64 Vec:1

Hashmode: 17230 - PKZIP (Mixed Multi-File Checksum-Only)

Speed.#1.........: 14578.3 MH/s (91.16ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 17300 - SHA3-224

Speed.#1.........:   826.5 MH/s (49.85ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 17400 - SHA3-256

Speed.#1.........:   843.5 MH/s (48.81ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 17500 - SHA3-384

Speed.#1.........:   844.0 MH/s (48.82ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 17600 - SHA3-512

Speed.#1.........:   843.6 MH/s (48.80ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 17700 - Keccak-224

Speed.#1.........:   827.5 MH/s (49.80ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 17800 - Keccak-256

Speed.#1.........:   844.5 MH/s (48.80ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 17900 - Keccak-384

Speed.#1.........:   844.2 MH/s (48.79ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 18000 - Keccak-512

Speed.#1.........:   843.5 MH/s (48.76ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 18100 - TOTP (HMAC-SHA1)

Speed.#1.........:  2683.1 MH/s (61.59ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 18200 - Kerberos 5, etype 23, AS-REP

Speed.#1.........:   503.7 MH/s (82.34ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 18300 - Apple File System (APFS) (Iterations: 19999)

Speed.#1.........:   111.4 kH/s (74.51ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 18400 - Open Document Format (ODF) 1.2 (SHA-256, AES) (Iterations: 99999)

Speed.#1.........:    26533 H/s (62.46ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 18500 - sha1(md5(md5($pass)))

Speed.#1.........:  4521.8 MH/s (73.25ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 18600 - Open Document Format (ODF) 1.1 (SHA-1, Blowfish) (Iterations: 1023)

Speed.#1.........:  1124.8 kH/s (39.95ms) @ Accel:1024 Loops:511 Thr:16 Vec:1

Hashmode: 18700 - Java Object hashCode()

Speed.#1.........: 72725.0 MH/s (17.56ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 18800 - Blockchain, My Wallet, Second Password (SHA256) (Iterations: 9999)

Speed.#1.........:   445.5 kH/s (72.71ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 18900 - Android Backup (Iterations: 9999)

Speed.#1.........:   265.0 kH/s (61.02ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 19000 - QNX /etc/shadow (MD5) (Iterations: 1000)

Speed.#1.........:  5845.8 kH/s (53.55ms) @ Accel:512 Loops:500 Thr:64 Vec:1

Hashmode: 19100 - QNX /etc/shadow (SHA256) (Iterations: 1000)

Speed.#1.........:  7501.2 kH/s (82.85ms) @ Accel:1024 Loops:500 Thr:64 Vec:1

Hashmode: 19200 - QNX /etc/shadow (SHA512) (Iterations: 1000)

Speed.#1.........:  6159.1 kH/s (48.92ms) @ Accel:512 Loops:500 Thr:64 Vec:1

Hashmode: 19300 - sha1($salt1.$pass.$salt2)

Speed.#1.........:  1690.8 MH/s (98.29ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 19500 - Ruby on Rails Restful-Authentication

Speed.#1.........:   332.0 MH/s (62.29ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 19600 - Kerberos 5, etype 17, TGS-REP (Iterations: 4095)

Speed.#1.........:  1282.1 kH/s (62.55ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 19700 - Kerberos 5, etype 18, TGS-REP (Iterations: 4095)

Speed.#1.........:   643.0 kH/s (62.52ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 19800 - Kerberos 5, etype 17, Pre-Auth (Iterations: 4095)

Speed.#1.........:  1282.6 kH/s (62.56ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 19900 - Kerberos 5, etype 18, Pre-Auth (Iterations: 4095)

Speed.#1.........:   643.4 kH/s (62.52ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 20011 - DiskCryptor SHA512 + XTS 512 bit (Iterations: 999)

* Device #1: Skipping hash-mode 20011 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

Hashmode: 20012 - DiskCryptor SHA512 + XTS 1024 bit (Iterations: 999)

* Device #1: Skipping hash-mode 20012 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

Hashmode: 20013 - DiskCryptor SHA512 + XTS 1536 bit (Iterations: 999)

* Device #1: Skipping hash-mode 20013 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

Hashmode: 20200 - Python passlib pbkdf2-sha512 (Iterations: 24999)

Speed.#1.........:    25296 H/s (65.59ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 20300 - Python passlib pbkdf2-sha256 (Iterations: 28999)

Speed.#1.........:    73310 H/s (78.19ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 20400 - Python passlib pbkdf2-sha1 (Iterations: 130999)

Speed.#1.........:    40439 H/s (62.59ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 20500 - PKZIP Master Key

Speed.#1.........:   123.2 GH/s (10.26ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 20510 - PKZIP Master Key (6 byte optimization)

Speed.#1.........: 20759.5 MH/s (63.89ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 20600 - Oracle Transportation Management (SHA256) (Iterations: 999)

Speed.#1.........:  4371.2 kH/s (48.31ms) @ Accel:512 Loops:499 Thr:64 Vec:1

Hashmode: 20710 - sha256(sha256($pass).$salt)

Speed.#1.........:  1436.0 MH/s (57.43ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 20711 - AuthMe sha256

Speed.#1.........:  1440.7 MH/s (57.44ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 20800 - sha256(md5($pass))

Speed.#1.........:  3998.9 MH/s (83.07ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 20900 - md5(sha1($pass).md5($pass).sha1($pass))

Speed.#1.........:  3585.8 MH/s (92.61ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 21000 - BitShares v0.x - sha512(sha512_bin(pass))

Speed.#1.........:   667.4 MH/s (62.04ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 21100 - sha1(md5($pass.$salt))

Speed.#1.........:  6805.5 MH/s (97.72ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 21200 - md5(sha1($salt).md5($pass))

Speed.#1.........:  6759.7 MH/s (98.30ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 21300 - md5($salt.sha1($salt.$pass))

Speed.#1.........:  4509.4 MH/s (73.61ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

Hashmode: 21400 - sha256(sha256_bin($pass))

Speed.#1.........:  2428.1 MH/s (68.19ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 21500 - SolarWinds Orion (Iterations: 999)

Speed.#1.........:    99724 H/s (47.46ms) @ Accel:64 Loops:62 Thr:64 Vec:1

Hashmode: 21600 - Web2py pbkdf2-sha512 (Iterations: 999)

Speed.#1.........:   628.6 kH/s (56.82ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 21700 - Electrum Wallet (Salt-Type 4) (Iterations: 1023)

Speed.#1.........:   406.8 kH/s (58.22ms) @ Accel:256 Loops:127 Thr:64 Vec:1

Hashmode: 21800 - Electrum Wallet (Salt-Type 5) (Iterations: 1023)

Speed.#1.........:   369.5 kH/s (58.23ms) @ Accel:256 Loops:127 Thr:64 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   647.5 kH/s (62.49ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 22001 - WPA-PMK-PMKID+EAPOL (Iterations: 0)

Speed.#1.........:   294.0 MH/s (0.00ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 22100 - BitLocker (Iterations: 1048576)

Speed.#1.........:     2405 H/s (65.88ms) @ Accel:32 Loops:4096 Thr:64 Vec:1

Hashmode: 22200 - Citrix NetScaler (SHA512)

Speed.#1.........:  1417.3 MH/s (58.31ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 22300 - sha256($salt.$pass.$salt)

Speed.#1.........:  4741.9 MH/s (69.92ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 22301 - Telegram Mobile App Passcode (SHA256)

Speed.#1.........:  4739.8 MH/s (69.83ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 22400 - AES Crypt (SHA256) (Iterations: 8191)

Speed.#1.........:   501.9 kH/s (80.18ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 22500 - MultiBit Classic .key (MD5)

Speed.#1.........:   957.9 MH/s (86.69ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 22600 - Telegram Desktop < v2.1.14 (PBKDF2-HMAC-SHA1) (Iterations: 3999)

Speed.#1.........:   188.4 kH/s (53.54ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 22700 - MultiBit HD (scrypt) (Iterations: 16384)

Speed.#1.........:     1341 H/s (41.66ms) @ Accel:20 Loops:1024 Thr:64 Vec:1

Hashmode: 22911 - RSA/DSA/EC/OpenSSH Private Keys ($0$)

Speed.#1.........:   780.6 MH/s (52.83ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 22921 - RSA/DSA/EC/OpenSSH Private Keys ($6$)

Speed.#1.........:  3066.3 MH/s (53.82ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 22931 - RSA/DSA/EC/OpenSSH Private Keys ($1, $3$)

Speed.#1.........:  1278.4 MH/s (64.82ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

Hashmode: 22941 - RSA/DSA/EC/OpenSSH Private Keys ($4$)

Speed.#1.........:  1111.9 MH/s (74.52ms) @ Accel:512 Loops:128 Thr:64 Vec:1

Hashmode: 22951 - RSA/DSA/EC/OpenSSH Private Keys ($5$)

Speed.#1.........:   906.4 MH/s (91.70ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 23001 - SecureZIP AES-128

Speed.#1.........:  1339.6 MH/s (124.33ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

Hashmode: 23002 - SecureZIP AES-192

Speed.#1.........:  1036.0 MH/s (80.08ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 23003 - SecureZIP AES-256

Speed.#1.........:   740.4 MH/s (55.75ms) @ Accel:128 Loops:256 Thr:64 Vec:1

Hashmode: 23100 - Apple Keychain (Iterations: 999)

Speed.#1.........:  2609.5 kH/s (48.67ms) @ Accel:512 Loops:249 Thr:64 Vec:1

Hashmode: 23200 - XMPP SCRAM PBKDF2-SHA1 (Iterations: 4095)

Speed.#1.........:  1284.3 kH/s (62.50ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 23300 - Apple iWork (Iterations: 3999)

Speed.#1.........:  1316.4 kH/s (60.95ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 23400 - Bitwarden (Iterations: 99999)

Speed.#1.........:    22274 H/s (74.55ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 23500 - AxCrypt 2 AES-128 (Iterations: 999)

Speed.#1.........:    80636 H/s (44.42ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 23600 - AxCrypt 2 AES-256 (Iterations: 999)

Speed.#1.........:    41468 H/s (87.12ms) @ Accel:256 Loops:124 Thr:64 Vec:1

Hashmode: 23700 - RAR3-p (Uncompressed) (Iterations: 262144)

Speed.#1.........:    86000 H/s (58.76ms) @ Accel:64 Loops:16384 Thr:64 Vec:1

Hashmode: 23800 - RAR3-p (Compressed) (Iterations: 262144)

Speed.#1.........:    84647 H/s (58.75ms) @ Accel:64 Loops:16384 Thr:64 Vec:1

Hashmode: 23900 - BestCrypt v3 Volume Encryption (Iterations: 1)

Speed.#1.........:  3649.1 kH/s (85.25ms) @ Accel:256 Loops:1 Thr:64 Vec:1

Hashmode: 24100 - MongoDB ServerKey SCRAM-SHA-1 (Iterations: 9999)

Speed.#1.........:   529.3 kH/s (61.03ms) @ Accel:512 Loops:512 Thr:64 Vec:1

Hashmode: 24200 - MongoDB ServerKey SCRAM-SHA-256 (Iterations: 14999)

Speed.#1.........:   148.4 kH/s (74.59ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 24300 - sha1($salt.sha1($pass.$salt))

Speed.#1.........:  4833.9 MH/s (68.58ms) @ Accel:1024 Loops:256 Thr:64 Vec:1

Hashmode: 24410 - PKCS#8 Private Keys (PBKDF2-HMAC-SHA1 + 3DES/AES) (Iterations: 2047)

Speed.#1.........:  1283.6 kH/s (62.51ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 24420 - PKCS#8 Private Keys (PBKDF2-HMAC-SHA256 + 3DES/AES) (Iterations: 2047)

Speed.#1.........:  1030.4 kH/s (78.03ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 24500 - Telegram Desktop >= v2.1.14 (PBKDF2-HMAC-SHA512) (Iterations: 99999)

Speed.#1.........:     2074 H/s (49.83ms) @ Accel:16 Loops:512 Thr:64 Vec:1

Hashmode: 24600 - SQLCipher (Iterations: 63999)

Speed.#1.........:    41452 H/s (62.51ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 24700 - Stuffit5

Speed.#1.........: 10376.8 MH/s (63.74ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

Hashmode: 24800 - Umbraco HMAC-SHA1

Speed.#1.........:  2716.4 MH/s (60.89ms) @ Accel:256 Loops:512 Thr:64 Vec:1

Hashmode: 24900 - Dahua Authentication MD5

Speed.#1.........: 20460.0 MH/s (64.65ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Hashmode: 25300 - MS Office 2016 - SheetProtection (Iterations: 100000)

Speed.#1.........:    13198 H/s (62.86ms) @ Accel:128 Loops:512 Thr:64 Vec:1

Hashmode: 25400 - PDF 1.4 - 1.6 (Acrobat 5 - 8) - edit password (Iterations: 70)

Speed.#1.........: 26267.1 kH/s (43.95ms) @ Accel:1024 Loops:70 Thr:64 Vec:1

Hashmode: 25500 - Stargazer Stellar Wallet XLM (Iterations: 4095)

Speed.#1.........:   541.8 kH/s (74.55ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 25900 - KNX IP Secure - Device Authentication Code (Iterations: 65535)

Speed.#1.........:    33974 H/s (74.60ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 26000 - Mozilla key3.db

Speed.#1.........:   360.9 MH/s (57.19ms) @ Accel:32 Loops:512 Thr:64 Vec:1

Hashmode: 26100 - Mozilla key4.db (Iterations: 9999)

Speed.#1.........:   213.0 kH/s (76.21ms) @ Accel:512 Loops:256 Thr:64 Vec:1

Hashmode: 99999 - Plaintext

Speed.#1.........: 51878.4 MH/s (25.01ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

Started: Wed Apr 28 17:48:50 2021
Stopped: Wed Apr 28 18:58:57 2021


## Tiny Sanity Test

root@gpu:/tmp/hashcat# rm hashcat.potfile; ./hashcat -a3 $(echo -n wat | md5sum | awk '{ print $1 }')
hashcat (v6.1.1-275-g057de100d+) starting...

OpenCL API (OpenCL 2.1 AMD-APP (3180.7)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: gfx1031, 12160/12272 MB (10213 MB allocatable), 20MCU

Minimum password length supported by kernel: 0
Maximum password length supported by kernel: 256

Hashes: 1 digests; 1 unique digests, 1 unique salts
Bitmaps: 16 bits, 65536 entries, 0x0000ffff mask, 262144 bytes, 5/13 rotates

Optimizers applied:
* Zero-Byte
* Early-Skip
* Not-Salted
* Not-Iterated
* Single-Hash
* Single-Salt
* Brute-Force
* Raw-Hash

ATTENTION! Pure (unoptimized) backend kernels selected.
Using pure kernels enables cracking longer passwords but for the price of drastically reduced performance.
If you want to switch to optimized backend kernels, append -O to your commandline.
See the above message to find out about the exact limits.

Watchdog: Temperature abort trigger set to 90c

Host memory required for this attack: 351 MB

The wordlist or mask that you are using is too small.
This means that hashcat cannot use the full parallel power of your device(s).
Unless you supply more work, your cracking speed will drop.
For tips on supplying more work, see: https://hashcat.net/faq/morework

Approaching final keyspace - workload adjusted.  

Session..........: hashcat                       
Status...........: Exhausted
Hash.Name........: MD5
Hash.Target......: 611c59af56268df5534fef5bc3c37b1d
Time.Started.....: Wed Apr 28 19:00:05 2021 (0 secs)
Time.Estimated...: Wed Apr 28 19:00:05 2021 (0 secs)
Guess.Mask.......: ?1 [1]
Guess.Charset....: -1 ?l?d?u, -2 ?l?d, -3 ?l?d*!$@_, -4 Undefined 
Guess.Queue......: 1/15 (6.67%)
Speed.#1.........:   152.2 kH/s (0.07ms) @ Accel:1024 Loops:62 Thr:64 Vec:1
Recovered........: 0/1 (0.00%) Digests
Progress.........: 62/62 (100.00%)
Rejected.........: 0/62 (0.00%)
Restore.Point....: 1/1 (100.00%)
Restore.Sub.#1...: Salt:0 Amplifier:0-62 Iteration:0-62
Candidates.#1....: s -> X
Hardware.Mon.#1..: Temp: 51c Fan: 20% Core:2615MHz Mem:1000MHz Bus:0

The wordlist or mask that you are using is too small.
This means that hashcat cannot use the full parallel power of your device(s).
Unless you supply more work, your cracking speed will drop.
For tips on supplying more work, see: https://hashcat.net/faq/morework

Approaching final keyspace - workload adjusted.  

Session..........: hashcat                       
Status...........: Exhausted
Hash.Name........: MD5
Hash.Target......: 611c59af56268df5534fef5bc3c37b1d
Time.Started.....: Wed Apr 28 19:00:05 2021 (0 secs)
Time.Estimated...: Wed Apr 28 19:00:05 2021 (0 secs)
Guess.Mask.......: ?1?2 [2]
Guess.Charset....: -1 ?l?d?u, -2 ?l?d, -3 ?l?d*!$@_, -4 Undefined 
Guess.Queue......: 2/15 (13.33%)
Speed.#1.........:  6963.7 kH/s (0.07ms) @ Accel:1024 Loops:62 Thr:64 Vec:1
Recovered........: 0/1 (0.00%) Digests
Progress.........: 2232/2232 (100.00%)
Rejected.........: 0/2232 (0.00%)
Restore.Point....: 36/36 (100.00%)
Restore.Sub.#1...: Salt:0 Amplifier:0-62 Iteration:0-62
Candidates.#1....: sa -> Xq
Hardware.Mon.#1..: Temp: 51c Fan: 20% Core:2615MHz Mem:1000MHz Bus:0

The wordlist or mask that you are using is too small.
This means that hashcat cannot use the full parallel power of your device(s).
Unless you supply more work, your cracking speed will drop.
For tips on supplying more work, see: https://hashcat.net/faq/morework

Approaching final keyspace - workload adjusted.  

611c59af56268df5534fef5bc3c37b1d:wat             
                                                 
Session..........: hashcat
Status...........: Cracked
Hash.Name........: MD5
Hash.Target......: 611c59af56268df5534fef5bc3c37b1d
Time.Started.....: Wed Apr 28 19:00:05 2021 (0 secs)
Time.Estimated...: Wed Apr 28 19:00:05 2021 (0 secs)
Guess.Mask.......: ?1?2?2 [3]
Guess.Charset....: -1 ?l?d?u, -2 ?l?d, -3 ?l?d*!$@_, -4 Undefined 
Guess.Queue......: 3/15 (20.00%)
Speed.#1.........:   270.0 MH/s (0.07ms) @ Accel:1024 Loops:62 Thr:64 Vec:1
Recovered........: 1/1 (100.00%) Digests
Progress.........: 80352/80352 (100.00%)
Rejected.........: 0/80352 (0.00%)
Restore.Point....: 0/1296 (0.00%)
Restore.Sub.#1...: Salt:0 Amplifier:0-62 Iteration:0-62
Candidates.#1....: sar -> Xqx
Hardware.Mon.#1..: Temp: 51c Fan: 20% Core:2615MHz Mem:1000MHz Bus:0

Started: Wed Apr 28 19:00:04 2021
Stopped: Wed Apr 28 19:00:06 2021
```
