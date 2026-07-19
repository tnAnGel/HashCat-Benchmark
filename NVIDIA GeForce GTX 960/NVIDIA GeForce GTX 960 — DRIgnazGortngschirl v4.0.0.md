# NVIDIA GeForce GTX 960

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 960
- **Версия hashcat / Version:** v4.0.0
- **Источник / Source:** [DRIgnazGortngschirl](https://github.com/DRIgnazGortngschirl/Benchmark-Scores-of-HashCAT)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 6483.8 MH/s |
| 100 | SHA1 | 2236.1 MH/s |
| 1400 | SHA2-256 | 862.2 MH/s |
| 1700 | SHA2-512 | 255.4 MH/s |
| 1000 | NTLM | 11924.1 MH/s |
| 3200 | bcrypt | 3755 H/s |
| 1800 | sha512crypt | 44884 H/s |
| 500 | md5crypt | 2540.9 kH/s |
| 2500 | WPA/WPA2 (legacy) | 111.5 kH/s |
| 7500 | Kerberos AS-REQ (23) | 84044.5 kH/s |
| 13100 | Kerberos TGS-REP (23) | 72264.9 kH/s |
| 11300 | Bitcoin wallet.dat | 1180 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 79266 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v4.0.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #1: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
OpenCL Platform #1: NVIDIA Corporation
======================================
* Device #1: GeForce GTX 960, 1008/4035 MB allocatable, 8MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 900 - MD4

Speed.Dev.#1.....: 11778.7 MH/s (23.46ms)

Hashmode: 0 - MD5

Speed.Dev.#1.....:  6483.8 MH/s (41.72ms)

Hashmode: 5100 - Half MD5

Speed.Dev.#1.....:  4124.4 MH/s (62.74ms)

Hashmode: 100 - SHA1

Speed.Dev.#1.....:  2236.1 MH/s (58.26ms)

Hashmode: 1400 - SHA-256

Speed.Dev.#1.....:   862.2 MH/s (82.76ms)

Hashmode: 10800 - SHA-384

Speed.Dev.#1.....:   251.3 MH/s (65.13ms)

Hashmode: 1700 - SHA-512

Speed.Dev.#1.....:   255.4 MH/s (63.98ms)

Hashmode: 5000 - SHA-3 (Keccak)

Speed.Dev.#1.....:   231.9 MH/s (72.90ms)

Hashmode: 10100 - SipHash

Speed.Dev.#1.....:  8445.9 MH/s (32.16ms)

Hashmode: 14900 - Skip32 (PT = $salt, key = $pass)

Speed.Dev.#1.....:  1747.7 MH/s (37.65ms)

Hashmode: 6000 - RIPEMD-160

Speed.Dev.#1.....:  1339.8 MH/s (50.73ms)

Hashmode: 6100 - Whirlpool

Speed.Dev.#1.....: 60049.9 kH/s (70.28ms)

Hashmode: 6900 - GOST R 34.11-94

Speed.Dev.#1.....: 67393.5 kH/s (62.22ms)

Hashmode: 11700 - GOST R 34.11-2012 (Streebog) 256-bit

Speed.Dev.#1.....: 11841.9 kH/s (81.34ms)

Hashmode: 11800 - GOST R 34.11-2012 (Streebog) 512-bit

Speed.Dev.#1.....: 10516.0 kH/s (48.88ms)

Hashmode: 14000 - DES (PT = $salt, key = $pass)

Speed.Dev.#1.....:  5255.0 MH/s (98.08ms)

Hashmode: 14100 - 3DES (PT = $salt, key = $pass)

Speed.Dev.#1.....:   308.0 MH/s (55.96ms)

Hashmode: 400 - phpass, WordPress (MD5), phpBB3 (MD5), Joomla (MD5)

Speed.Dev.#1.....:  1786.4 kH/s (68.43ms)

Hashmode: 8900 - scrypt

Speed.Dev.#1.....:   185.1 kH/s (10.05ms)

Hashmode: 11900 - PBKDF2-HMAC-MD5

Speed.Dev.#1.....:  1933.4 kH/s (61.97ms)

Hashmode: 12000 - PBKDF2-HMAC-SHA1

Speed.Dev.#1.....:   918.6 kH/s (73.09ms)

Hashmode: 10900 - PBKDF2-HMAC-SHA256

Speed.Dev.#1.....:   312.5 kH/s (51.83ms)

Hashmode: 12100 - PBKDF2-HMAC-SHA512

Speed.Dev.#1.....:    99393 H/s (74.25ms)

Hashmode: 23 - Skype

Speed.Dev.#1.....:  3495.1 MH/s (76.30ms)

Hashmode: 2500 - WPA/WPA2

Speed.Dev.#1.....:   111.5 kH/s (73.90ms)

Hashmode: 2501 - WPA/WPA2 PMK

Speed.Dev.#1.....: 42064.2 kH/s (0.03ms)

Hashmode: 5300 - IKE-PSK MD5

Speed.Dev.#1.....:   498.5 MH/s (64.67ms)

Hashmode: 5400 - IKE-PSK SHA1

Speed.Dev.#1.....:   188.4 MH/s (88.09ms)

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.Dev.#1.....:  5233.8 MH/s (48.57ms)

Hashmode: 5600 - NetNTLMv2

Speed.Dev.#1.....:   482.7 MH/s (70.35ms)

Hashmode: 7300 - IPMI2 RAKP HMAC-SHA1

Speed.Dev.#1.....:   425.4 MH/s (80.54ms)

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.Dev.#1.....: 84044.5 kH/s (50.39ms)

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23

Speed.Dev.#1.....: 72264.9 kH/s (56.10ms)

Hashmode: 8300 - DNSSEC (NSEC3)

Speed.Dev.#1.....:   821.6 MH/s (77.48ms)

Hashmode: 11100 - PostgreSQL CRAM (MD5)

Speed.Dev.#1.....:  1818.0 MH/s (76.71ms)

Hashmode: 11200 - MySQL CRAM (SHA1)

Speed.Dev.#1.....:   610.1 MH/s (53.37ms)

Hashmode: 11400 - SIP digest authentication (MD5)

Speed.Dev.#1.....:   949.9 MH/s (75.69ms)

Hashmode: 121 - SMF (Simple Machines Forum) > v1.1

Speed.Dev.#1.....:  1869.2 MH/s (72.30ms)

Hashmode: 2611 - vBulletin < v3.8.5

Speed.Dev.#1.....:  1972.9 MH/s (68.62ms)

Hashmode: 2711 - vBulletin >= v3.8.5

Speed.Dev.#1.....:  1332.7 MH/s (50.58ms)

Hashmode: 2811 - IPB2+ (Invision Power Board), MyBB 1.2+

Speed.Dev.#1.....:  1391.4 MH/s (94.66ms)

Hashmode: 8400 - WBB3 (Woltlab Burning Board)

Speed.Dev.#1.....:   332.3 MH/s (49.57ms)

Hashmode: 13900 - OpenCart

Speed.Dev.#1.....:   573.9 MH/s (59.03ms)

Hashmode: 11 - Joomla < 2.5.18

Speed.Dev.#1.....:  6615.9 MH/s (41.00ms)

Hashmode: 2612 - PHPS

Speed.Dev.#1.....:  1923.3 MH/s (68.75ms)

Hashmode: 7900 - Drupal7

Speed.Dev.#1.....:    14569 H/s (70.24ms)

Hashmode: 21 - osCommerce, xt:Commerce

Speed.Dev.#1.....:  3741.4 MH/s (71.99ms)

Hashmode: 11000 - PrestaShop

Speed.Dev.#1.....:  2383.4 MH/s (56.58ms)

Hashmode: 124 - Django (SHA-1)

Speed.Dev.#1.....:  1848.7 MH/s (72.38ms)

Hashmode: 10000 - Django (PBKDF2-SHA256)

Speed.Dev.#1.....:    15744 H/s (53.17ms)

Hashmode: 3711 - MediaWiki B type

Speed.Dev.#1.....:  1825.3 MH/s (74.16ms)

Hashmode: 4521 - Redmine

Speed.Dev.#1.....:   847.0 MH/s (79.97ms)

Hashmode: 4522 - PunBB

Speed.Dev.#1.....:   804.8 MH/s (80.03ms)

Hashmode: 12 - PostgreSQL

Speed.Dev.#1.....:  6629.0 MH/s (40.65ms)

Hashmode: 131 - MSSQL (2000)

Speed.Dev.#1.....:  2366.0 MH/s (57.32ms)

Hashmode: 132 - MSSQL (2005)

Speed.Dev.#1.....:  2357.4 MH/s (57.30ms)

Hashmode: 1731 - MSSQL (2012, 2014)

Speed.Dev.#1.....:   249.0 MH/s (65.55ms)

Hashmode: 200 - MySQL323

Speed.Dev.#1.....: 14617.5 MH/s (4.58ms)

Hashmode: 300 - MySQL4.1/MySQL5

Speed.Dev.#1.....:   968.0 MH/s (65.33ms)

Hashmode: 3100 - Oracle H: Type (Oracle 7+)

Speed.Dev.#1.....:   237.6 MH/s (34.06ms)

Hashmode: 112 - Oracle S: Type (Oracle 11+)

Speed.Dev.#1.....:  2323.2 MH/s (58.30ms)

Hashmode: 12300 - Oracle T: Type (Oracle 12+)

Speed.Dev.#1.....:    24851 H/s (79.64ms)

Hashmode: 8000 - Sybase ASE

Speed.Dev.#1.....: 96901.9 kH/s (87.03ms)

Hashmode: 141 - Episerver 6.x < .NET 4

Speed.Dev.#1.....:  1863.7 MH/s (72.29ms)

Hashmode: 1441 - Episerver 6.x >= .NET 4

Speed.Dev.#1.....:   741.1 MH/s (91.08ms)

Hashmode: 1600 - Apache $apr1$ MD5, md5apr1, MD5 (APR)

Speed.Dev.#1.....:  2920.6 kH/s (43.83ms)

Hashmode: 12600 - ColdFusion 10+

Speed.Dev.#1.....:   491.5 MH/s (68.43ms)

Hashmode: 1421 - hMailServer

Speed.Dev.#1.....:   745.6 MH/s (90.77ms)

Hashmode: 101 - nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.Dev.#1.....:  2316.8 MH/s (58.51ms)

Hashmode: 111 - nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.Dev.#1.....:  2319.7 MH/s (58.40ms)

Hashmode: 1411 - SSHA-256(Base64), LDAP {SSHA256}

Speed.Dev.#1.....:   863.1 MH/s (78.52ms)

Hashmode: 1711 - SSHA-512(Base64), LDAP {SSHA512}

Speed.Dev.#1.....:   262.5 MH/s (63.90ms)

Hashmode: 3000 - LM

Speed.Dev.#1.....:  5693.5 MH/s (94.77ms)

Hashmode: 1000 - NTLM

Speed.Dev.#1.....: 11924.1 MH/s (22.89ms)

Hashmode: 1100 - Domain Cached Credentials (DCC), MS Cache

Speed.Dev.#1.....:  3118.7 MH/s (88.38ms)

Hashmode: 2100 - Domain Cached Credentials 2 (DCC2), MS Cache 2

Speed.Dev.#1.....:    92159 H/s (70.95ms)

Hashmode: 15300 - DPAPI masterkey file v1

Speed.Dev.#1.....:    19213 H/s (72.46ms)

Hashmode: 15900 - DPAPI masterkey file v2

Speed.Dev.#1.....:    12344 H/s (83.38ms)

Hashmode: 12800 - MS-AzureSync PBKDF2-HMAC-SHA256

Speed.Dev.#1.....:  2514.0 kH/s (41.85ms)

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.Dev.#1.....:   275.3 MH/s (62.92ms)

Hashmode: 12400 - BSDi Crypt, Extended DES

Speed.Dev.#1.....:   437.1 kH/s (102.48ms)

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)

Speed.Dev.#1.....:  2540.9 kH/s (48.07ms)

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix)

Speed.Dev.#1.....:     3755 H/s (31.89ms)

Hashmode: 7400 - sha256crypt $5$, SHA256 (Unix)

Speed.Dev.#1.....:    97883 H/s (33.77ms)

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix)

Speed.Dev.#1.....:    44884 H/s (73.20ms)

Hashmode: 122 - macOS v10.4, macOS v10.5, MacOS v10.6

Speed.Dev.#1.....:  1864.5 MH/s (72.50ms)

Hashmode: 1722 - macOS v10.7

Speed.Dev.#1.....:   249.0 MH/s (67.50ms)

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512)

Speed.Dev.#1.....:     3032 H/s (77.97ms)

Hashmode: 6300 - AIX {smd5}

Speed.Dev.#1.....:  2923.3 kH/s (46.01ms)

Hashmode: 6700 - AIX {ssha1}

Speed.Dev.#1.....:  9643.0 kH/s (10.00ms)

Hashmode: 6400 - AIX {ssha256}

Speed.Dev.#1.....:  4045.7 kH/s (27.05ms)

Hashmode: 6500 - AIX {ssha512}

Speed.Dev.#1.....:  1378.0 kH/s (80.00ms)

Hashmode: 2400 - Cisco-PIX MD5

Speed.Dev.#1.....:  4633.6 MH/s (58.63ms)

Hashmode: 2410 - Cisco-ASA MD5

Speed.Dev.#1.....:  4616.9 MH/s (58.04ms)

Hashmode: 5700 - Cisco-IOS type 4 (SHA256)

Speed.Dev.#1.....:   844.4 MH/s (78.78ms)

Hashmode: 9200 - Cisco-IOS $8$ (PBKDF2-SHA256)

Speed.Dev.#1.....:    15701 H/s (53.26ms)

Hashmode: 9300 - Cisco-IOS $9$ (scrypt)

Speed.Dev.#1.....:     4774 H/s (233.14ms)

Hashmode: 22 - Juniper NetScreen/SSG (ScreenOS)

Speed.Dev.#1.....:  3447.0 MH/s (74.04ms)

Hashmode: 501 - Juniper IVE

Speed.Dev.#1.....:  2848.2 kH/s (43.99ms)

Hashmode: 5800 - Samsung Android Password/PIN

Speed.Dev.#1.....:  1582.4 kH/s (82.54ms)

Hashmode: 8100 - Citrix NetScaler

Speed.Dev.#1.....:  1882.7 MH/s (68.89ms)

Hashmode: 8500 - RACF

Speed.Dev.#1.....:   743.0 MH/s (93.83ms)

Hashmode: 7200 - GRUB 2

Speed.Dev.#1.....:    10721 H/s (76.98ms)

Hashmode: 9900 - Radmin2

Speed.Dev.#1.....:  2152.9 MH/s (58.56ms)

Hashmode: 7700 - SAP CODVN B (BCODE)

Speed.Dev.#1.....:   512.6 MH/s (66.29ms)

Hashmode: 7800 - SAP CODVN F/G (PASSCODE)

Speed.Dev.#1.....:   327.7 MH/s (51.33ms)

Hashmode: 10300 - SAP CODVN H (PWDSALTEDHASH) iSSHA-1

Speed.Dev.#1.....:  1570.7 kH/s (81.75ms)

Hashmode: 8600 - Lotus Notes/Domino 5

Speed.Dev.#1.....: 62983.2 kH/s (66.94ms)

Hashmode: 8700 - Lotus Notes/Domino 6

Speed.Dev.#1.....: 20717.9 kH/s (50.93ms)

Hashmode: 9100 - Lotus Notes/Domino 8

Speed.Dev.#1.....:   165.8 kH/s (76.70ms)

Hashmode: 133 - PeopleSoft

Speed.Dev.#1.....:  2368.5 MH/s (61.56ms)

Hashmode: 13500 - PeopleSoft PS_TOKEN

Speed.Dev.#1.....:   861.1 MH/s (79.08ms)

Hashmode: 11600 - 7-Zip

Speed.Dev.#1.....:     2186 H/s (14.51ms)

Hashmode: 13600 - WinZip

Speed.Dev.#1.....:   300.8 kH/s (51.20ms)

Hashmode: 12500 - RAR3-hp

Speed.Dev.#1.....:    10103 H/s (24.45ms)

Hashmode: 13000 - RAR5

Speed.Dev.#1.....:     9634 H/s (53.07ms)

Hashmode: 13200 - AxCrypt

Speed.Dev.#1.....:    27520 H/s (112.28ms)

Hashmode: 13300 - AxCrypt in-memory SHA1

Speed.Dev.#1.....:  1860.6 MH/s (70.68ms)

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit

Speed.Dev.#1.....:    79266 H/s (49.54ms)

Hashmode: 6221 - TrueCrypt PBKDF2-HMAC-SHA512 + XTS 512 bit

Speed.Dev.#1.....:    93846 H/s (81.16ms)

Hashmode: 6231 - TrueCrypt PBKDF2-HMAC-Whirlpool + XTS 512 bit

Speed.Dev.#1.....:     8824 H/s (111.41ms)

Hashmode: 6241 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit + boot-mode

Speed.Dev.#1.....:   143.1 kH/s (50.42ms)

Hashmode: 13711 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit

Speed.Dev.#1.....:      249 H/s (50.54ms)

Hashmode: 13721 - VeraCrypt PBKDF2-HMAC-SHA512 + XTS 512 bit

Speed.Dev.#1.....:      186 H/s (80.50ms)

Hashmode: 13731 - VeraCrypt PBKDF2-HMAC-Whirlpool + XTS 512 bit

Speed.Dev.#1.....:        0 H/s (111.86ms)

Hashmode: 13741 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit + boot-mode

Speed.Dev.#1.....:      497 H/s (50.15ms)

Hashmode: 13751 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 512 bit

Speed.Dev.#1.....:      248 H/s (60.58ms)

Hashmode: 13761 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 512 bit + boot-mode

Speed.Dev.#1.....:      683 H/s (59.71ms)

Hashmode: 8800 - Android FDE <= 4.3

Speed.Dev.#1.....:   227.2 kH/s (72.92ms)

Hashmode: 12900 - Android FDE (Samsung DEK)

Speed.Dev.#1.....:    76496 H/s (53.45ms)

Hashmode: 12200 - eCryptfs

Speed.Dev.#1.....:     3655 H/s (69.90ms)

Hashmode: 9700 - MS Office <= 2003 $0/$1, MD5 + RC4

Speed.Dev.#1.....: 69585.1 kH/s (62.65ms)

Hashmode: 9710 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.Dev.#1.....: 92200.7 kH/s (98.48ms)

Hashmode: 9800 - MS Office <= 2003 $3/$4, SHA1 + RC4

Speed.Dev.#1.....: 77663.3 kH/s (98.86ms)

Hashmode: 9810 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.Dev.#1.....: 77352.1 kH/s (101.86ms)

Hashmode: 9400 - MS Office 2007

Speed.Dev.#1.....:    35906 H/s (74.57ms)

Hashmode: 9500 - MS Office 2010

Speed.Dev.#1.....:    18577 H/s (72.67ms)

Hashmode: 9600 - MS Office 2013

Speed.Dev.#1.....:     2418 H/s (68.93ms)

Hashmode: 10400 - PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.Dev.#1.....: 96757.0 kH/s (83.62ms)

Hashmode: 10410 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.Dev.#1.....:   106.3 MH/s (76.70ms)

Hashmode: 10500 - PDF 1.4 - 1.6 (Acrobat 5 - 8)

Speed.Dev.#1.....:  4712.8 kH/s (48.64ms)

Hashmode: 10600 - PDF 1.7 Level 3 (Acrobat 9)

Speed.Dev.#1.....:   841.7 MH/s (79.19ms)

Hashmode: 10700 - PDF 1.7 Level 8 (Acrobat 10 - 11)

Speed.Dev.#1.....:     8226 H/s (50.79ms)

Hashmode: 9000 - Password Safe v2

Speed.Dev.#1.....:    93631 H/s (56.20ms)

Hashmode: 5200 - Password Safe v3

Speed.Dev.#1.....:   328.7 kH/s (49.18ms)

Hashmode: 6800 - LastPass + LastPass sniffed

Speed.Dev.#1.....:   610.6 kH/s (52.36ms)

Hashmode: 6600 - 1Password, agilekeychain

Speed.Dev.#1.....:   875.9 kH/s (72.63ms)

Hashmode: 8200 - 1Password, cloudkeychain

Speed.Dev.#1.....:     2530 H/s (81.80ms)

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat

Speed.Dev.#1.....:     1180 H/s (69.70ms)

Hashmode: 12700 - Blockchain, My Wallet

Speed.Dev.#1.....: 17465.8 kH/s (2.85ms)

Hashmode: 15200 - Blockchain, My Wallet, V2

Speed.Dev.#1.....:    89283 H/s (72.57ms)

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES)

Speed.Dev.#1.....:    38723 H/s (142.47ms)

Hashmode: 15500 - JKS Java Key Store Private Keys (SHA1)

Speed.Dev.#1.....:  2214.4 MH/s (61.51ms)

Hashmode: 15600 - Ethereum Wallet, PBKDF2-HMAC-SHA256

Speed.Dev.#1.....:     1175 H/s (53.68ms)

Hashmode: 125 - ArubaOS

Speed.Dev.#1.....:  1797.0 MH/s (72.30ms)

Hashmode: 15400 - ChaCha20

Speed.Dev.#1.....:  1158.6 MH/s (58.21ms)

Started: Fri Nov 10 22:06:16 2017
Stopped: Fri Nov 10 22:25:59 2017
```
