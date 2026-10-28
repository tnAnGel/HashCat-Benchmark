# NVIDIA Jetson Xavier NX (Xavier)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Jetson Xavier NX (Xavier)
- **Версия hashcat / Version:** v6.1.1-71-g57bef8ab
- **Источник / Source:** [brianhealey — gist](https://gist.github.com/brianhealey/19061f0b3cb791459b619b30bed5a3ca)

> Прогон с `--benchmark-all` (все режимы), питание `MODE_15W_6CORE`, hashcat собран с `-march=native`. Устройство определяется как `Xavier` (7763 MB, 6MCU).

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 2818.6 MH/s |
| 100 | SHA1 | 949.2 MH/s |
| 1400 | SHA2-256 | 415.0 MH/s |
| 1700 | SHA2-512 | 134.0 MH/s |
| 1000 | NTLM | 5103.3 MH/s |
| 3200 | bcrypt | 4290 H/s |
| 1800 | sha512crypt | 20710 H/s |
| 500 | md5crypt | 1363.9 kH/s |
| 2500 | WPA-EAPOL-PBKDF2 | 43858 H/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 48107 H/s |
| 7500 | Kerberos AS-REQ (23) | 61991.9 kH/s |
| 13100 | Kerberos TGS-REP (23) | 59783.8 kH/s |
| 11300 | Bitcoin wallet.dat | 576 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 37157 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat was built using CFLAGS&CFFLAGS = "-march=native"
Fresh install of sd card image for Jetson NX, apt upgrade ran. Stock hardware and power supply.

Power Settings:
sudo nvpmodel -q
NV Fan Mode:quiet
NV Power Mode: MODE_15W_6CORE
2

/etc/nv_tegra_release:
# R32 (release), REVISION: 4.3, GCID: 21589087, BOARD: t186ref, EABI: aarch64, DATE: Fri Jun 26 04:34:27 UTC 2020


hashcat (v6.1.1-71-g57bef8ab) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

CUDA API (CUDA 10.2)
====================
* Device #1: Xavier, 6103/7763 MB, 6MCU

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........:  2818.6 MH/s (71.09ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 10 - md5($pass.$salt)

Speed.#1.........:  2819.8 MH/s (71.07ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 11 - Joomla < 2.5.18

Speed.#1.........:  2877.0 MH/s (69.68ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 12 - PostgreSQL

Speed.#1.........:  2875.6 MH/s (69.69ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 20 - md5($salt.$pass)

Speed.#1.........:  1577.5 MH/s (63.52ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 21 - osCommerce, xt:Commerce

Speed.#1.........:  1580.6 MH/s (63.36ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 22 - Juniper NetScreen/SSG (ScreenOS)

Speed.#1.........:  1578.2 MH/s (63.48ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 23 - Skype

Speed.#1.........:  1576.5 MH/s (63.51ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 30 - md5(utf16le($pass).$salt)

Speed.#1.........:  2684.5 MH/s (74.69ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 40 - md5($salt.utf16le($pass))

Speed.#1.........:  1584.2 MH/s (63.25ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 50 - HMAC-MD5 (key = $pass)

Speed.#1.........:   478.1 MH/s (52.33ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 60 - HMAC-MD5 (key = $salt)

Speed.#1.........:  1038.1 MH/s (48.18ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........:   949.2 MH/s (52.72ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 101 - nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.#1.........:   949.4 MH/s (52.72ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 110 - sha1($pass.$salt)

Speed.#1.........:   965.7 MH/s (51.81ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 111 - nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.#1.........:   949.4 MH/s (52.72ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 112 - Oracle S: Type (Oracle 11+)

Speed.#1.........:   965.5 MH/s (51.83ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 120 - sha1($salt.$pass)

Speed.#1.........:   734.9 MH/s (68.19ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 121 - SMF (Simple Machines Forum) > v1.1

Speed.#1.........:   734.4 MH/s (68.24ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 122 - macOS v10.4, macOS v10.5, MacOS v10.6

Speed.#1.........:   733.1 MH/s (68.37ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 124 - Django (SHA-1)

Speed.#1.........:   732.8 MH/s (68.41ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 125 - ArubaOS

Speed.#1.........:   733.2 MH/s (68.35ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 130 - sha1(utf16le($pass).$salt)

Speed.#1.........:   965.2 MH/s (51.88ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 131 - MSSQL (2000)

Speed.#1.........:   964.9 MH/s (51.88ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 132 - MSSQL (2005)

Speed.#1.........:   964.7 MH/s (51.87ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 133 - PeopleSoft

Speed.#1.........:   949.0 MH/s (52.75ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 140 - sha1($salt.utf16le($pass))

Speed.#1.........:   733.3 MH/s (68.34ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 141 - Episerver 6.x < .NET 4

Speed.#1.........:   733.4 MH/s (68.34ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 150 - HMAC-SHA1 (key = $pass)

Speed.#1.........:   213.0 MH/s (58.80ms) @ Accel:32 Loops:64 Thr:1024 Vec:1

Hashmode: 160 - HMAC-SHA1 (key = $salt)

Speed.#1.........:   406.1 MH/s (61.71ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 200 - MySQL323

Speed.#1.........:  7351.6 MH/s (54.48ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 300 - MySQL4.1/MySQL5

Speed.#1.........:   415.5 MH/s (60.29ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 400 - phpass (Iterations: 2048)

Speed.#1.........:   820.7 kH/s (58.59ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........:  1363.9 kH/s (69.87ms) @ Accel:16 Loops:1000 Thr:1024 Vec:1

Hashmode: 501 - Juniper IVE (Iterations: 1000)

Speed.#1.........:  1363.2 kH/s (69.86ms) @ Accel:16 Loops:1000 Thr:1024 Vec:1

Hashmode: 600 - BLAKE2b-512

Speed.#1.........:   238.0 MH/s (52.57ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Hashmode: 900 - MD4

Speed.#1.........:  5100.5 MH/s (78.66ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........:  5103.3 MH/s (78.62ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 1100 - Domain Cached Credentials (DCC), MS Cache

Speed.#1.........:  1346.8 MH/s (74.45ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 1300 - SHA2-224

Speed.#1.........:   406.0 MH/s (61.72ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:   415.0 MH/s (60.35ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 1410 - sha256($pass.$salt)

Speed.#1.........:   415.7 MH/s (60.27ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 1411 - SSHA-256(Base64), LDAP {SSHA256}

Speed.#1.........:   415.0 MH/s (60.37ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 1420 - sha256($salt.$pass)

Speed.#1.........:   365.2 MH/s (68.62ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 1421 - hMailServer

Speed.#1.........:   365.4 MH/s (68.59ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 1430 - sha256(utf16le($pass).$salt)

Speed.#1.........:   415.3 MH/s (60.31ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 1440 - sha256($salt.utf16le($pass))

Speed.#1.........:   365.3 MH/s (68.61ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 1441 - Episerver 6.x >= .NET 4

Speed.#1.........:   365.2 MH/s (68.63ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 1450 - HMAC-SHA256 (key = $pass)

Speed.#1.........: 73729.0 kH/s (85.04ms) @ Accel:16 Loops:64 Thr:1024 Vec:1

Hashmode: 1460 - HMAC-SHA256 (key = $salt)

Speed.#1.........:   176.0 MH/s (71.23ms) @ Accel:4 Loops:512 Thr:1024 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:   100.8 MH/s (57.17ms) @ Accel:16 Loops:1024 Thr:64 Vec:1

Hashmode: 1600 - Apache $apr1$ MD5, md5apr1, MD5 (APR) (Iterations: 1000)

Speed.#1.........:  1361.1 kH/s (69.90ms) @ Accel:16 Loops:1000 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:   134.0 MH/s (93.62ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

Hashmode: 1710 - sha512($pass.$salt)

Speed.#1.........:   135.2 MH/s (92.76ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

Hashmode: 1711 - SSHA-512(Base64), LDAP {SSHA512}

Speed.#1.........:   135.3 MH/s (92.74ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

Hashmode: 1720 - sha512($salt.$pass)

Speed.#1.........:   126.9 MH/s (49.29ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 1722 - macOS v10.7

Speed.#1.........:   127.0 MH/s (49.28ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 1730 - sha512(utf16le($pass).$salt)

Speed.#1.........:   135.2 MH/s (92.77ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

Hashmode: 1731 - MSSQL (2012, 2014)

Speed.#1.........:   135.2 MH/s (92.76ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

Hashmode: 1740 - sha512($salt.utf16le($pass))

Speed.#1.........:   126.9 MH/s (49.29ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 1750 - HMAC-SHA512 (key = $pass)

Speed.#1.........: 27383.9 kH/s (57.16ms) @ Accel:2 Loops:128 Thr:1024 Vec:1

Hashmode: 1760 - HMAC-SHA512 (key = $salt)

Speed.#1.........: 57955.5 kH/s (54.00ms) @ Accel:2 Loops:256 Thr:1024 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:    20710 H/s (58.85ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 2000 - STDOUT

Speed.#1.........:  1975.8 GH/s (0.02ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2100 - Domain Cached Credentials 2 (DCC2), MS Cache 2 (Iterations: 10239)

Speed.#1.........:    38561 H/s (63.49ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 2400 - Cisco-PIX MD5

Speed.#1.........:  2018.3 MH/s (49.58ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 2410 - Cisco-ASA MD5

Speed.#1.........:  1825.4 MH/s (54.87ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#1.........:    43858 H/s (8.65ms) @ Accel:8 Loops:32 Thr:1024 Vec:1

Hashmode: 2501 - WPA-EAPOL-PMK (Iterations: 0)

Speed.#1.........: 41293.0 kH/s (0.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 2600 - md5(md5($pass))

Speed.#1.........:   867.9 MH/s (57.75ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 2611 - vBulletin < v3.8.5

Speed.#1.........:   867.8 MH/s (57.75ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 2612 - PHPS

Speed.#1.........:   867.1 MH/s (57.80ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 2711 - vBulletin >= v3.8.5

Speed.#1.........:   613.5 MH/s (81.74ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 2811 - MyBB 1.2+, IPB2+ (Invision Power Board)

Speed.#1.........:   664.3 MH/s (75.54ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 3000 - LM

Speed.#1.........:  2480.6 MH/s (75.25ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 3100 - Oracle H: Type (Oracle 7+)

Speed.#1.........: 69401.4 kH/s (90.43ms) @ Accel:16 Loops:64 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:     4290 H/s (32.39ms) @ Accel:4 Loops:16 Thr:12 Vec:1

Hashmode: 3710 - md5($salt.md5($pass))

Speed.#1.........:   794.2 MH/s (63.11ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 3711 - MediaWiki B type

Speed.#1.........:   795.8 MH/s (63.02ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 3800 - md5($salt.$pass.$salt)

Speed.#1.........:  1583.7 MH/s (63.33ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 3910 - md5(md5($pass).md5($salt))

Speed.#1.........:   617.4 MH/s (81.24ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 4010 - md5($salt.md5($salt.$pass))

Speed.#1.........:   711.1 MH/s (70.50ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 4110 - md5($salt.md5($pass.$salt))

Speed.#1.........:   757.8 MH/s (66.14ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 4300 - md5(strtoupper(md5($pass)))

Speed.#1.........:   867.6 MH/s (57.73ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 4400 - md5(sha1($pass))

Speed.#1.........:   519.0 MH/s (48.20ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 4500 - sha1(sha1($pass))

Speed.#1.........:   368.4 MH/s (68.02ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 4520 - sha1($salt.sha1($pass))

Speed.#1.........:   219.4 MH/s (57.12ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 4521 - Redmine

Speed.#1.........:   219.4 MH/s (57.14ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 4522 - PunBB

Speed.#1.........:   337.0 MH/s (74.43ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 4700 - sha1(md5($pass))

Speed.#1.........:   531.6 MH/s (94.41ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 4710 - sha1(md5($pass).$salt)

Speed.#1.........:   504.1 MH/s (49.69ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 4711 - Huawei sha1(md5($pass).$salt)

Speed.#1.........:   504.2 MH/s (49.69ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 4800 - iSCSI CHAP authentication, MD5(CHAP)

Speed.#1.........:  1803.4 MH/s (55.55ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 4900 - sha1($salt.$pass.$salt)

Speed.#1.........:   716.7 MH/s (69.95ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 5100 - Half MD5

Speed.#1.........:  1894.4 MH/s (52.91ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 5200 - Password Safe v3 (Iterations: 2049)

Speed.#1.........:   164.6 kH/s (49.35ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 5300 - IKE-PSK MD5

Speed.#1.........:   110.7 MH/s (56.58ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 5400 - IKE-PSK SHA1

Speed.#1.........: 45456.6 kH/s (68.98ms) @ Accel:2 Loops:256 Thr:1024 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........:  2964.0 MH/s (67.71ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:   211.8 MH/s (59.14ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Hashmode: 5700 - Cisco-IOS type 4 (SHA256)

Speed.#1.........:   415.2 MH/s (60.34ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 5800 - Samsung Android Password/PIN (Iterations: 1023)

Speed.#1.........:   661.6 kH/s (48.74ms) @ Accel:16 Loops:511 Thr:1024 Vec:1

Hashmode: 6000 - RIPEMD-160

Speed.#1.........:   650.9 MH/s (77.11ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 6100 - Whirlpool

Speed.#1.........: 59768.6 kH/s (52.43ms) @ Accel:16 Loops:32 Thr:1024 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:    37157 H/s (76.41ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 6212 - TrueCrypt RIPEMD160 + XTS 1024 bit (Iterations: 1999)

Speed.#1.........:    18338 H/s (10.12ms) @ Accel:16 Loops:4 Thr:1024 Vec:1

Hashmode: 6213 - TrueCrypt RIPEMD160 + XTS 1536 bit (Iterations: 1999)

Speed.#1.........:     7219 H/s (6.80ms) @ Accel:4 Loops:8 Thr:1024 Vec:1

Hashmode: 6221 - TrueCrypt SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:    50660 H/s (25.85ms) @ Accel:16 Loops:15 Thr:1024 Vec:1

Hashmode: 6222 - TrueCrypt SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:    24854 H/s (54.84ms) @ Accel:32 Loops:7 Thr:1024 Vec:1

Hashmode: 6223 - TrueCrypt SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:    18796 H/s (78.13ms) @ Accel:16 Loops:15 Thr:1024 Vec:1

Hashmode: 6231 - TrueCrypt Whirlpool + XTS 512 bit (Iterations: 999)

Speed.#1.........:     7134 H/s (153.64ms) @ Accel:12 Loops:15 Thr:1024 Vec:1

Hashmode: 6232 - TrueCrypt Whirlpool + XTS 1024 bit (Iterations: 999)

Speed.#1.........:     3385 H/s (108.16ms) @ Accel:4 Loops:15 Thr:1024 Vec:1

Hashmode: 6233 - TrueCrypt Whirlpool + XTS 1536 bit (Iterations: 999)

Speed.#1.........:     2298 H/s (148.09ms) @ Accel:8 Loops:7 Thr:1024 Vec:1

Hashmode: 6241 - TrueCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 999)

Speed.#1.........:    69064 H/s (67.99ms) @ Accel:8 Loops:124 Thr:1024 Vec:1

Hashmode: 6242 - TrueCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 999)

Speed.#1.........:    44840 H/s (65.48ms) @ Accel:32 Loops:15 Thr:1024 Vec:1

Hashmode: 6243 - TrueCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 999)

Speed.#1.........:    31587 H/s (92.88ms) @ Accel:32 Loops:15 Thr:1024 Vec:1

Hashmode: 6300 - AIX {smd5} (Iterations: 1000)

Speed.#1.........:  1363.0 kH/s (69.89ms) @ Accel:16 Loops:1000 Thr:1024 Vec:1

Hashmode: 6400 - AIX {ssha256} (Iterations: 63)

Speed.#1.........:  2263.8 kH/s (78.43ms) @ Accel:32 Loops:63 Thr:1024 Vec:1

Hashmode: 6500 - AIX {ssha512} (Iterations: 63)

Speed.#1.........:   805.8 kH/s (43.48ms) @ Accel:32 Loops:15 Thr:1024 Vec:1

Hashmode: 6600 - 1Password, agilekeychain (Iterations: 999)

Speed.#1.........:   355.5 kH/s (32.97ms) @ Accel:64 Loops:31 Thr:1024 Vec:1

Hashmode: 6700 - AIX {ssha1} (Iterations: 63)

Speed.#1.........:  4941.8 kH/s (68.70ms) @ Accel:64 Loops:63 Thr:1024 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:   310.0 kH/s (76.12ms) @ Accel:4 Loops:499 Thr:1024 Vec:1

Hashmode: 6900 - GOST R 34.11-94

Speed.#1.........: 43206.9 kH/s (72.57ms) @ Accel:4 Loops:128 Thr:1024 Vec:1

Hashmode: 7000 - FortiGate (FortiOS)

Speed.#1.........:   817.8 MH/s (61.31ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:    17823 H/s (12.21ms) @ Accel:8 Loops:7 Thr:1024 Vec:1

Hashmode: 7200 - GRUB 2 (Iterations: 1023)

Speed.#1.........:    55648 H/s (50.73ms) @ Accel:32 Loops:15 Thr:1024 Vec:1

Hashmode: 7300 - IPMI2 RAKP HMAC-SHA1

Speed.#1.........:   121.3 MH/s (51.65ms) @ Accel:4 Loops:256 Thr:1024 Vec:1

Hashmode: 7400 - sha256crypt $5$, SHA256 (Unix) (Iterations: 5000)

Speed.#1.........:    36217 H/s (67.66ms) @ Accel:64 Loops:32 Thr:1024 Vec:1

Hashmode: 7401 - MySQL $A$ (sha256crypt) (Iterations: 5000)

Speed.#1.........:    34025 H/s (71.64ms) @ Accel:64 Loops:32 Thr:1024 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........: 61991.9 kH/s (50.53ms) @ Accel:128 Loops:64 Thr:64 Vec:1

Hashmode: 7700 - SAP CODVN B (BCODE)

Speed.#1.........:   244.2 MH/s (51.23ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Hashmode: 7701 - SAP CODVN B (BCODE) from RFC_READ_TABLE

Speed.#1.........:   247.2 MH/s (101.58ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 7800 - SAP CODVN F/G (PASSCODE)

Speed.#1.........:   161.6 MH/s (77.63ms) @ Accel:32 Loops:64 Thr:1024 Vec:1

Hashmode: 7801 - SAP CODVN F/G (PASSCODE) from RFC_READ_TABLE

Speed.#1.........:   160.1 MH/s (78.36ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

Hashmode: 7900 - Drupal7 (Iterations: 16384)

Speed.#1.........:     7113 H/s (53.87ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 8000 - Sybase ASE

Speed.#1.........: 38240.2 kH/s (7.62ms) @ Accel:1 Loops:64 Thr:1024 Vec:1

Hashmode: 8100 - Citrix NetScaler (SHA1)

Speed.#1.........:   817.2 MH/s (61.36ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 8200 - 1Password, cloudkeychain (Iterations: 39999)

Speed.#1.........:     1461 H/s (53.73ms) @ Accel:2 Loops:256 Thr:1024 Vec:1

Hashmode: 8300 - DNSSEC (NSEC3)

Speed.#1.........:   353.3 MH/s (71.00ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 8400 - WBB3 (Woltlab Burning Board)

Speed.#1.........:   150.8 MH/s (83.21ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 8500 - RACF

Speed.#1.........:   338.6 MH/s (74.06ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 8600 - Lotus Notes/Domino 5

Speed.#1.........: 38893.3 kH/s (80.66ms) @ Accel:8 Loops:64 Thr:1024 Vec:1

Hashmode: 8700 - Lotus Notes/Domino 6

Speed.#1.........: 12807.7 kH/s (61.19ms) @ Accel:2 Loops:64 Thr:1024 Vec:1

Hashmode: 8800 - Android FDE <= 4.3 (Iterations: 1999)

Speed.#1.........:    97974 H/s (62.11ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 8900 - scrypt (Iterations: 1)

Speed.#1.........:    48009 H/s (31.22ms) @ Accel:16 Loops:1 Thr:16 Vec:1

Hashmode: 9000 - Password Safe v2 (Iterations: 1000)

Speed.#1.........:    88679 H/s (32.50ms) @ Accel:64 Loops:1000 Thr:12 Vec:1

Hashmode: 9100 - Lotus Notes/Domino 8 (Iterations: 4999)

Speed.#1.........:    76399 H/s (63.60ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 9200 - Cisco-IOS $8$ (PBKDF2-SHA256) (Iterations: 19999)

Speed.#1.........:     7880 H/s (39.38ms) @ Accel:4 Loops:256 Thr:1024 Vec:1

Hashmode: 9300 - Cisco-IOS $9$ (scrypt) (Iterations: 1)

Speed.#1.........:     1035 H/s (184.73ms) @ Accel:4 Loops:1 Thr:8 Vec:1

Hashmode: 9400 - MS Office 2007 (Iterations: 50000)

Speed.#1.........:    14594 H/s (34.26ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 9500 - MS Office 2010 (Iterations: 100000)

Speed.#1.........:     7955 H/s (63.17ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 9600 - MS Office 2013 (Iterations: 100000)

Speed.#1.........:     1137 H/s (55.23ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 9700 - MS Office <= 2003 $0/$1, MD5 + RC4

Speed.#1.........: 54800.9 kH/s (57.17ms) @ Accel:64 Loops:128 Thr:64 Vec:1

Hashmode: 9710 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.#1.........: 65935.3 kH/s (95.17ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 9720 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #2

Speed.#1.........:   243.6 MH/s (51.42ms) @ Accel:4 Loops:512 Thr:1024 Vec:1

Hashmode: 9800 - MS Office <= 2003 $3/$4, SHA1 + RC4

Speed.#1.........: 55590.1 kH/s (56.34ms) @ Accel:16 Loops:512 Thr:64 Vec:1

Hashmode: 9810 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.#1.........: 71600.8 kH/s (87.62ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Hashmode: 9820 - MS Office <= 2003 $3, SHA1 + RC4, collider #2

Speed.#1.........:   379.9 MH/s (66.03ms) @ Accel:64 Loops:64 Thr:1024 Vec:1

Hashmode: 9900 - Radmin2

Speed.#1.........:  1061.9 MH/s (94.54ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 10000 - Django (PBKDF2-SHA256) (Iterations: 9999)

Speed.#1.........:    15939 H/s (76.95ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 10100 - SipHash

Speed.#1.........:  3298.6 MH/s (60.76ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 10200 - CRAM-MD5

Speed.#1.........:   478.7 MH/s (52.30ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 10300 - SAP CODVN H (PWDSALTEDHASH) iSSHA-1 (Iterations: 1023)

Speed.#1.........:   647.8 kH/s (49.73ms) @ Accel:16 Loops:511 Thr:1024 Vec:1

Hashmode: 10400 - PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.#1.........: 75049.2 kH/s (83.60ms) @ Accel:128 Loops:128 Thr:64 Vec:1

Hashmode: 10410 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.#1.........:  7314.6 kH/s (53.38ms) @ Accel:4 Loops:256 Thr:64 Vec:1

Hashmode: 10420 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #2

Speed.#1.........:   914.5 MH/s (41.05ms) @ Accel:24 Loops:256 Thr:1024 Vec:1

Hashmode: 10500 - PDF 1.4 - 1.6 (Acrobat 5 - 8) (Iterations: 70)

Speed.#1.........:  3479.9 kH/s (105.16ms) @ Accel:1024 Loops:70 Thr:64 Vec:1

Hashmode: 10600 - PDF 1.7 Level 3 (Acrobat 9)

Speed.#1.........:   415.3 MH/s (60.33ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 10700 - PDF 1.7 Level 8 (Acrobat 10 - 11) (Iterations: 64)

Speed.#1.........:     8797 H/s (87.19ms) @ Accel:8 Loops:1 Thr:1024 Vec:1

Hashmode: 10800 - SHA2-384

Speed.#1.........:   132.2 MH/s (95.01ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

Hashmode: 10900 - PBKDF2-HMAC-SHA256 (Iterations: 999)

Speed.#1.........:   157.9 kH/s (61.67ms) @ Accel:8 Loops:249 Thr:1024 Vec:1

Hashmode: 10901 - RedHat 389-DS LDAP (PBKDF2-HMAC-SHA256) (Iterations: 8191)

Speed.#1.........:    19446 H/s (78.82ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 11000 - PrestaShop

Speed.#1.........:  1173.8 MH/s (85.47ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 11100 - PostgreSQL CRAM (MD5)

Speed.#1.........:   848.5 MH/s (59.04ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 11200 - MySQL CRAM (SHA1)

Speed.#1.........:   244.6 MH/s (51.21ms) @ Accel:64 Loops:32 Thr:1024 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:      576 H/s (54.36ms) @ Accel:1 Loops:1024 Thr:1024 Vec:1

Hashmode: 11400 - SIP digest authentication (MD5)

Speed.#1.........:   399.9 MH/s (62.72ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 11500 - CRC32

Speed.#1.........:   740.9 MH/s (33.71ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:    51636 H/s (56.19ms) @ Accel:2 Loops:4096 Thr:1024 Vec:1

Hashmode: 11700 - GOST R 34.11-2012 (Streebog) 256-bit, big-endian

Speed.#1.........:  8942.2 kH/s (65.75ms) @ Accel:24 Loops:4 Thr:1024 Vec:1

Hashmode: 11750 - HMAC-Streebog-256 (key = $pass), big-endian

Speed.#1.........:  3169.7 kH/s (61.82ms) @ Accel:4 Loops:8 Thr:1024 Vec:1

Hashmode: 11760 - HMAC-Streebog-256 (key = $salt), big-endian

Speed.#1.........:  4208.5 kH/s (93.21ms) @ Accel:4 Loops:16 Thr:1024 Vec:1

Hashmode: 11800 - GOST R 34.11-2012 (Streebog) 512-bit, big-endian

Speed.#1.........:  8221.8 kH/s (41.64ms) @ Accel:28 Loops:2 Thr:1024 Vec:1

Hashmode: 11850 - HMAC-Streebog-512 (key = $pass), big-endian

Speed.#1.........:  2644.4 kH/s (74.14ms) @ Accel:16 Loops:2 Thr:1024 Vec:1

Hashmode: 11860 - HMAC-Streebog-512 (key = $salt), big-endian

Speed.#1.........:  3251.6 kH/s (7.04ms) @ Accel:1 Loops:4 Thr:1024 Vec:1

Hashmode: 11900 - PBKDF2-HMAC-MD5 (Iterations: 999)

Speed.#1.........:   970.1 kH/s (32.54ms) @ Accel:16 Loops:499 Thr:1024 Vec:1

Hashmode: 12000 - PBKDF2-HMAC-SHA1 (Iterations: 999)

Speed.#1.........:   389.2 kH/s (49.75ms) @ Accel:16 Loops:249 Thr:1024 Vec:1

Hashmode: 12001 - Atlassian (PBKDF2-HMAC-SHA1) (Iterations: 9999)

Speed.#1.........:    39512 H/s (62.01ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 12100 - PBKDF2-HMAC-SHA512 (Iterations: 999)

Speed.#1.........:    57666 H/s (49.63ms) @ Accel:8 Loops:62 Thr:1024 Vec:1

Hashmode: 12200 - eCryptfs (Iterations: 65536)

Speed.#1.........:     1753 H/s (54.68ms) @ Accel:4 Loops:256 Thr:1024 Vec:1

Hashmode: 12300 - Oracle T: Type (Oracle 12+) (Iterations: 4095)

Speed.#1.........:    14223 H/s (53.75ms) @ Accel:2 Loops:256 Thr:1024 Vec:1

Hashmode: 12400 - BSDi Crypt, Extended DES (Iterations: 2194)

Speed.#1.........:   365.6 kH/s (52.78ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:     6522 H/s (58.72ms) @ Accel:1 Loops:16384 Thr:1024 Vec:1

Hashmode: 12600 - ColdFusion 10+

Speed.#1.........:   228.1 MH/s (54.96ms) @ Accel:64 Loops:32 Thr:1024 Vec:1

Hashmode: 12700 - Blockchain, My Wallet (Iterations: 9)

Speed.#1.........: 10245.8 kH/s (18.97ms) @ Accel:64 Loops:9 Thr:1024 Vec:1

Hashmode: 12800 - MS-AzureSync PBKDF2-HMAC-SHA256 (Iterations: 99)

Speed.#1.........:   151.9 kH/s (50.62ms) @ Accel:4 Loops:49 Thr:1024 Vec:1

Hashmode: 12900 - Android FDE (Samsung DEK) (Iterations: 4095)

Speed.#1.........:    36557 H/s (41.71ms) @ Accel:4 Loops:256 Thr:1024 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:     4886 H/s (78.28ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........: 59783.8 kH/s (52.42ms) @ Accel:128 Loops:64 Thr:64 Vec:1

Hashmode: 13200 - AxCrypt 1 (Iterations: 10467)

Speed.#1.........:    19649 H/s (122.15ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 13300 - AxCrypt 1 in-memory SHA1

Speed.#1.........:   884.2 MH/s (56.67ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:     6032 H/s (169.52ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 13500 - PeopleSoft PS_TOKEN

Speed.#1.........:   672.9 MH/s (74.54ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 13600 - WinZip (Iterations: 999)

Speed.#1.........:    40748 H/s (147.83ms) @ Accel:1 Loops:999 Thr:1024 Vec:1

Hashmode: 13711 - VeraCrypt RIPEMD160 + XTS 512 bit (Iterations: 655330)

Speed.#1.........:      119 H/s (38.95ms) @ Accel:32 Loops:31 Thr:1024 Vec:1

Hashmode: 13712 - VeraCrypt RIPEMD160 + XTS 1024 bit (Iterations: 655330)

Speed.#1.........:       68 H/s (34.05ms) @ Accel:8 Loops:62 Thr:1024 Vec:1

Hashmode: 13713 - VeraCrypt RIPEMD160 + XTS 1536 bit (Iterations: 655330)

Speed.#1.........:       47 H/s (46.97ms) @ Accel:32 Loops:15 Thr:1024 Vec:1

Hashmode: 13721 - VeraCrypt SHA512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:      116 H/s (26.36ms) @ Accel:2 Loops:250 Thr:1024 Vec:1

Hashmode: 13722 - VeraCrypt SHA512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:       56 H/s (27.28ms) @ Accel:4 Loops:62 Thr:1024 Vec:1

Hashmode: 13723 - VeraCrypt SHA512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:       37 H/s (39.35ms) @ Accel:16 Loops:15 Thr:1024 Vec:1

Hashmode: 13731 - VeraCrypt Whirlpool + XTS 512 bit (Iterations: 499999)

Speed.#1.........:       14 H/s (106.59ms) @ Accel:4 Loops:62 Thr:1024 Vec:1

Hashmode: 13732 - VeraCrypt Whirlpool + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:        7 H/s (108.80ms) @ Accel:4 Loops:31 Thr:1024 Vec:1

Hashmode: 13733 - VeraCrypt Whirlpool + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:        5 H/s (79.39ms) @ Accel:4 Loops:15 Thr:1024 Vec:1

Hashmode: 13741 - VeraCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 327660)

Speed.#1.........:      239 H/s (40.12ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 13742 - VeraCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 327660)

Speed.#1.........:      136 H/s (35.13ms) @ Accel:8 Loops:64 Thr:1024 Vec:1

Hashmode: 13743 - VeraCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 327660)

Speed.#1.........:       95 H/s (25.18ms) @ Accel:8 Loops:32 Thr:1024 Vec:1

Hashmode: 13751 - VeraCrypt SHA256 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:      153 H/s (39.43ms) @ Accel:32 Loops:31 Thr:1024 Vec:1

Hashmode: 13752 - VeraCrypt SHA256 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:       82 H/s (37.01ms) @ Accel:8 Loops:62 Thr:1024 Vec:1

Hashmode: 13753 - VeraCrypt SHA256 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:       53 H/s (27.57ms) @ Accel:16 Loops:15 Thr:1024 Vec:1

Hashmode: 13761 - VeraCrypt SHA256 + XTS 512 bit + boot-mode (Iterations: 199999)

Speed.#1.........:      385 H/s (40.64ms) @ Accel:32 Loops:32 Thr:1024 Vec:1

Hashmode: 13762 - VeraCrypt SHA256 + XTS 1024 bit + boot-mode (Iterations: 199999)

Speed.#1.........:      205 H/s (38.18ms) @ Accel:8 Loops:64 Thr:1024 Vec:1

Hashmode: 13763 - VeraCrypt SHA256 + XTS 1536 bit + boot-mode (Iterations: 199999)

Speed.#1.........:      136 H/s (28.80ms) @ Accel:8 Loops:32 Thr:1024 Vec:1

Hashmode: 13771 - VeraCrypt Streebog-512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:        5 H/s (137.57ms) @ Accel:2 Loops:62 Thr:1024 Vec:1

Hashmode: 13772 - VeraCrypt Streebog-512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:        3 H/s (121.89ms) @ Accel:8 Loops:7 Thr:1024 Vec:1

Hashmode: 13773 - VeraCrypt Streebog-512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:        2 H/s (78.97ms) @ Accel:8 Loops:3 Thr:1024 Vec:1

Hashmode: 13800 - Windows Phone 8+ PIN/password

Speed.#1.........: 97530.5 kH/s (64.28ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 13900 - OpenCart

Speed.#1.........:   231.8 MH/s (54.07ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 14000 - DES (PT = $salt, key = $pass)

Speed.#1.........:  2338.1 MH/s (80.94ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 14100 - 3DES (PT = $salt, key = $pass)

Speed.#1.........:   319.1 MH/s (78.64ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 14400 - sha1(CX)

Speed.#1.........: 45440.6 kH/s (69.03ms) @ Accel:32 Loops:16 Thr:1024 Vec:1

Hashmode: 14600 - LUKS (Iterations: 163044)

Speed.#1.........:     1204 H/s (63.96ms) @ Accel:256 Loops:128 Thr:64 Vec:1

Hashmode: 14700 - iTunes backup < 10.0 (Iterations: 9999)

Speed.#1.........:    19671 H/s (62.23ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 14800 - iTunes backup >= 10.0 (Iterations: 9999999)

Speed.#1.........:       16 H/s (78.82ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 14900 - Skip32 (PT = $salt, key = $pass)

Speed.#1.........:  1082.7 MH/s (61.74ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 15000 - FileZilla Server >= 0.9.55

Speed.#1.........:   121.9 MH/s (51.41ms) @ Accel:64 Loops:16 Thr:1024 Vec:1

Hashmode: 15100 - Juniper/NetBSD sha1crypt (Iterations: 19999)

Speed.#1.........:    19039 H/s (65.98ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 15200 - Blockchain, My Wallet, V2 (Iterations: 4999)

Speed.#1.........:    38504 H/s (63.62ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:     8218 H/s (63.66ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 15400 - ChaCha20

Speed.#1.........:   479.5 MH/s (839.39ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 15500 - JKS Java Key Store Private Keys (SHA1)

Speed.#1.........:   903.7 MH/s (55.46ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 15600 - Ethereum Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1023)

Speed.#1.........:   154.9 kH/s (62.42ms) @ Accel:8 Loops:255 Thr:1024 Vec:1

Hashmode: 15700 - Ethereum Wallet, SCRYPT (Iterations: 1)

Speed.#1.........:        0 H/s (29693.16ms) @ Accel:1 Loops:1 Thr:1 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:     4518 H/s (53.16ms) @ Accel:2 Loops:256 Thr:1024 Vec:1

Hashmode: 16000 - Tripcode

Speed.#1.........: 31454.4 kH/s (49.78ms) @ Accel:1 Loops:256 Thr:1024 Vec:1

Hashmode: 16100 - TACACS+

Speed.#1.........:  1627.6 MH/s (61.61ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1

Hashmode: 16200 - Apple Secure Notes (Iterations: 19999)

Speed.#1.........:     8032 H/s (78.18ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 16300 - Ethereum Pre-Sale Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1999)

Speed.#1.........:    79295 H/s (76.04ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 16400 - CRAM-MD5 Dovecot

Speed.#1.........:  2819.9 MH/s (71.15ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 16500 - JWT (JSON Web Token)

Speed.#1.........: 72791.6 kH/s (86.25ms) @ Accel:64 Loops:16 Thr:1024 Vec:1

Hashmode: 16600 - Electrum Wallet (Salt-Type 1-3)

Speed.#1.........: 80648.6 kH/s (77.79ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 16700 - FileVault 2 (Iterations: 19999)

Speed.#1.........:     8064 H/s (76.04ms) @ Accel:4 Loops:512 Thr:1024 Vec:1

Hashmode: 16800 - WPA-PMKID-PBKDF2 (Iterations: 4095)

Speed.#1.........:    48129 H/s (63.63ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 16801 - WPA-PMKID-PMK (Iterations: 0)

Speed.#1.........: 42754.1 kH/s (0.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 16900 - Ansible Vault (Iterations: 9999)

Speed.#1.........:    14917 H/s (20.73ms) @ Accel:4 Loops:128 Thr:1024 Vec:1

Hashmode: 17200 - PKZIP (Compressed)

Speed.#1.........:   210.1 MH/s (59.65ms) @ Accel:64 Loops:32 Thr:1024 Vec:1

Hashmode: 17210 - PKZIP (Uncompressed)

Speed.#1.........:   190.3 MH/s (32.83ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 17220 - PKZIP (Compressed Multi-File)

Speed.#1.........:   682.8 MH/s (36.62ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 17225 - PKZIP (Mixed Multi-File)

Speed.#1.........:   856.6 MH/s (27.26ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 17230 - PKZIP (Mixed Multi-File Checksum-Only)

Speed.#1.........:  1192.7 MH/s (84.18ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 17300 - SHA3-224

Speed.#1.........: 92376.8 kH/s (67.94ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 17400 - SHA3-256

Speed.#1.........: 92377.1 kH/s (67.94ms) @ Accel:16 Loops:64 Thr:1024 Vec:1

Hashmode: 17500 - SHA3-384

Speed.#1.........: 92293.6 kH/s (67.95ms) @ Accel:16 Loops:64 Thr:1024 Vec:1

Hashmode: 17600 - SHA3-512

Speed.#1.........: 92346.5 kH/s (67.92ms) @ Accel:16 Loops:64 Thr:1024 Vec:1

Hashmode: 17700 - Keccak-224

Speed.#1.........: 92275.2 kH/s (68.00ms) @ Accel:16 Loops:64 Thr:1024 Vec:1

Hashmode: 17800 - Keccak-256

Speed.#1.........: 92313.7 kH/s (67.94ms) @ Accel:16 Loops:64 Thr:1024 Vec:1

Hashmode: 17900 - Keccak-384

Speed.#1.........: 92392.1 kH/s (67.92ms) @ Accel:16 Loops:64 Thr:1024 Vec:1

Hashmode: 18000 - Keccak-512

Speed.#1.........: 92432.1 kH/s (67.87ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 18100 - TOTP (HMAC-SHA1)

Speed.#1.........:   179.5 MH/s (69.90ms) @ Accel:32 Loops:64 Thr:1024 Vec:1

Hashmode: 18200 - Kerberos 5, etype 23, AS-REP

Speed.#1.........: 47989.5 kH/s (14.92ms) @ Accel:4 Loops:512 Thr:64 Vec:1

Hashmode: 18300 - Apple File System (APFS) (Iterations: 19999)

Speed.#1.........:     8038 H/s (78.13ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 18400 - Open Document Format (ODF) 1.2 (SHA-256, AES) (Iterations: 99999)

Speed.#1.........:     1975 H/s (63.62ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 18500 - sha1(md5(md5($pass)))

Speed.#1.........:   364.8 MH/s (68.75ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 18600 - Open Document Format (ODF) 1.1 (SHA-1, Blowfish) (Iterations: 1023)

Speed.#1.........:   113.4 kH/s (51.92ms) @ Accel:512 Loops:511 Thr:12 Vec:1

Hashmode: 18700 - Java Object hashCode()

Speed.#1.........:  9713.2 MH/s (41.22ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 18800 - Blockchain, My Wallet, Second Password (SHA256) (Iterations: 9999)

Speed.#1.........:    33943 H/s (72.28ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 18900 - Android Backup (Iterations: 9999)

Speed.#1.........:    19728 H/s (62.16ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 19000 - QNX /etc/shadow (MD5) (Iterations: 1000)

Speed.#1.........:  3939.3 kH/s (43.58ms) @ Accel:64 Loops:500 Thr:1024 Vec:1

Hashmode: 19100 - QNX /etc/shadow (SHA256) (Iterations: 1000)

Speed.#1.........:  1749.7 kH/s (52.40ms) @ Accel:32 Loops:500 Thr:1024 Vec:1

Hashmode: 19200 - QNX /etc/shadow (SHA512) (Iterations: 1000)

Speed.#1.........:   804.4 kH/s (26.62ms) @ Accel:64 Loops:62 Thr:1024 Vec:1

Hashmode: 19300 - sha1($salt1.$pass.$salt2)

Speed.#1.........: 12055.6 kH/s (64.89ms) @ Accel:2 Loops:64 Thr:1024 Vec:1

Hashmode: 19500 - Ruby on Rails Restful-Authentication

Speed.#1.........: 12965.8 kH/s (60.46ms) @ Accel:16 Loops:8 Thr:1024 Vec:1

Hashmode: 19600 - Kerberos 5, etype 17, TGS-REP (Iterations: 4095)

Speed.#1.........:    95901 H/s (63.56ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 19700 - Kerberos 5, etype 18, TGS-REP (Iterations: 4095)

Speed.#1.........:    47987 H/s (63.65ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 19800 - Kerberos 5, etype 17, Pre-Auth (Iterations: 4095)

Speed.#1.........:    96205 H/s (63.45ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 19900 - Kerberos 5, etype 18, Pre-Auth (Iterations: 4095)

Speed.#1.........:    43813 H/s (34.80ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 20011 - DiskCryptor SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:    44088 H/s (56.10ms) @ Accel:4 Loops:124 Thr:1024 Vec:1

Hashmode: 20012 - DiskCryptor SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:    24183 H/s (51.86ms) @ Accel:16 Loops:15 Thr:1024 Vec:1

Hashmode: 20013 - DiskCryptor SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:    18756 H/s (78.13ms) @ Accel:16 Loops:15 Thr:1024 Vec:1

Hashmode: 20200 - Python passlib pbkdf2-sha512 (Iterations: 24999)

Speed.#1.........:     2336 H/s (53.78ms) @ Accel:2 Loops:256 Thr:1024 Vec:1

Hashmode: 20300 - Python passlib pbkdf2-sha256 (Iterations: 28999)

Speed.#1.........:     5499 H/s (78.79ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 20400 - Python passlib pbkdf2-sha1 (Iterations: 130999)

Speed.#1.........:     3021 H/s (63.49ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 20500 - PKZIP Master Key

Speed.#1.........:  9778.5 MH/s (40.93ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 20510 - PKZIP Master Key (6 byte optimization)

Speed.#1.........:  2147.6 MH/s (23.21ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 20600 - Oracle Transportation Management (SHA256) (Iterations: 999)

Speed.#1.........:   337.0 kH/s (64.28ms) @ Accel:32 Loops:124 Thr:1024 Vec:1

Hashmode: 20710 - sha256(sha256($pass).$salt)

Speed.#1.........:   110.8 MH/s (56.53ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 20711 - AuthMe sha256

Speed.#1.........:   110.8 MH/s (56.54ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 20800 - sha256(md5($pass))

Speed.#1.........:   314.0 MH/s (79.92ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 20900 - md5(sha1($pass).md5($pass).sha1($pass))

Speed.#1.........:   295.7 MH/s (84.88ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1

Hashmode: 21000 - BitShares v0.x - sha512(sha512_bin(pass))

Speed.#1.........: 61255.9 kH/s (51.16ms) @ Accel:8 Loops:64 Thr:1024 Vec:1

Hashmode: 21100 - sha1(md5($pass.$salt))

Speed.#1.........:   531.4 MH/s (94.49ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Hashmode: 21200 - md5(sha1($salt).md5($pass))

Speed.#1.........:   659.8 MH/s (76.06ms) @ Accel:64 Loops:128 Thr:1024 Vec:1

Hashmode: 21300 - md5($salt.sha1($salt.$pass))

Speed.#1.........:   375.3 MH/s (66.84ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 21400 - sha256(sha256_bin($pass))

Speed.#1.........:   178.0 MH/s (70.44ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Hashmode: 21500 - SolarWinds Orion (Iterations: 999)

Speed.#1.........:     7388 H/s (92.33ms) @ Accel:16 Loops:7 Thr:1024 Vec:1

Hashmode: 21600 - Web2py pbkdf2-sha512 (Iterations: 999)

Speed.#1.........:    57805 H/s (46.74ms) @ Accel:4 Loops:124 Thr:1024 Vec:1

Hashmode: 21700 - Electrum Wallet (Salt-Type 4) (Iterations: 1023)

Speed.#1.........:    41440 H/s (50.79ms) @ Accel:32 Loops:15 Thr:1024 Vec:1

Hashmode: 21800 - Electrum Wallet (Salt-Type 5) (Iterations: 1023)

Speed.#1.........:    41659 H/s (50.77ms) @ Accel:32 Loops:15 Thr:1024 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:    48107 H/s (63.65ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 22001 - WPA-PMK-PMKID+EAPOL (Iterations: 0)

Speed.#1.........: 42120.4 kH/s (0.00ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Hashmode: 22100 - BitLocker (Iterations: 1048576)

Speed.#1.........:      181 H/s (132.76ms) @ Accel:1 Loops:4096 Thr:1024 Vec:1

Hashmode: 22200 - Citrix NetScaler (SHA512)

Speed.#1.........:   134.4 MH/s (93.39ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Hashmode: 22300 - sha256($salt.$pass.$salt)

Speed.#1.........:   355.0 MH/s (70.68ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 22301 - Telegram Mobile App Passcode (SHA256)

Speed.#1.........:   356.0 MH/s (70.50ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 22400 - AES Crypt (SHA256) (Iterations: 8191)

Speed.#1.........:    37976 H/s (80.34ms) @ Accel:16 Loops:256 Thr:1024 Vec:1

Hashmode: 22500 - MultiBit Classic .key (MD5)

Speed.#1.........: 93546.8 kH/s (67.05ms) @ Accel:16 Loops:64 Thr:1024 Vec:1

Hashmode: 22600 - Telegram Desktop App Passcode (PBKDF2-HMAC-SHA1) (Iterations: 3999)

Speed.#1.........:    14049 H/s (55.34ms) @ Accel:8 Loops:64 Thr:1024 Vec:1

Hashmode: 22700 - MultiBit HD (scrypt) (Iterations: 1)

Speed.#1.........:       32 H/s (3027.55ms) @ Accel:1 Loops:1 Thr:16 Vec:1

Hashmode: 22911 - RSA/DSA/EC/OpenSSH Private Keys ($0$)

Speed.#1.........: 50857.8 kH/s (7.24ms) @ Accel:16 Loops:4 Thr:1024 Vec:1

Hashmode: 22921 - RSA/DSA/EC/OpenSSH Private Keys ($6$)

Speed.#1.........:   224.2 MH/s (55.90ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

Hashmode: 22931 - RSA/DSA/EC/OpenSSH Private Keys ($1, $3$)

Speed.#1.........:   131.1 MH/s (47.77ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 22941 - RSA/DSA/EC/OpenSSH Private Keys ($4$)

Speed.#1.........:   102.6 MH/s (61.08ms) @ Accel:8 Loops:128 Thr:1024 Vec:1

Hashmode: 22951 - RSA/DSA/EC/OpenSSH Private Keys ($5$)

Speed.#1.........: 85908.9 kH/s (73.01ms) @ Accel:4 Loops:256 Thr:1024 Vec:1

Hashmode: 23001 - SecureZIP AES-128

Speed.#1.........:   115.1 MH/s (54.44ms) @ Accel:4 Loops:256 Thr:1024 Vec:1

Hashmode: 23002 - SecureZIP AES-192

Speed.#1.........: 84419.1 kH/s (74.31ms) @ Accel:4 Loops:256 Thr:1024 Vec:1

Hashmode: 23003 - SecureZIP AES-256

Speed.#1.........: 76955.3 kH/s (81.52ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Hashmode: 23100 - Apple Keychain (Iterations: 999)

Speed.#1.........:   194.3 kH/s (58.89ms) @ Accel:32 Loops:62 Thr:1024 Vec:1

Hashmode: 23200 - XMPP SCRAM PBKDF2-SHA1 (Iterations: 4095)

Speed.#1.........:    96216 H/s (63.51ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 23300 - Apple iWork (Iterations: 3999)

Speed.#1.........:    98550 H/s (61.96ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 23400 - Bitwarden (Iterations: 99999)

Speed.#1.........:     1608 H/s (78.12ms) @ Accel:4 Loops:512 Thr:1024 Vec:1

Hashmode: 23500 - AxCrypt 2 AES-128 (Iterations: 999)

Speed.#1.........:     8675 H/s (31.36ms) @ Accel:4 Loops:124 Thr:1024 Vec:1

Hashmode: 23600 - AxCrypt 2 AES-256 (Iterations: 999)

Speed.#1.........:     4399 H/s (61.96ms) @ Accel:4 Loops:124 Thr:1024 Vec:1

Hashmode: 99999 - Plaintext

Speed.#1.........:  5102.1 MH/s (78.68ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

Started: Mon Sep  7 11:23:10 2020
[2K
Stopped: Mon Sep  7 13:29:09 2020
```
