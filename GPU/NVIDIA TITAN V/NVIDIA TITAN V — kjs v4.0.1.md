# NVIDIA TITAN V

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA TITAN V
- **Версия hashcat / Version:** v4.0.1
- **Источник / Source:** [kjs](https://hashcat.net/forum/thread-7182.html)
- **Особенности прогона / Run options:** `hashcat64.exe --benchmark --opencl-devices 1` (Windows 10 64-bit, драйвер NVIDIA 390.65, частоты и power limit стоковые); вторая карта (GTX 1080 Ti) и CPU исключены, результаты — `Speed.Dev.#1`
- **Примечание / Note:** формат вывода hashcat v4.x (`Hashmode:` / `Speed.Dev.#1`); режима 22000 в этой версии ещё нет — WPA представлен режимом 2500

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 45493.6 MH/s |
| 100 | SHA1 | 14689.0 MH/s |
| 1400 | SHA2-256 | 6491.5 MH/s |
| 1700 | SHA2-512 | 1881.0 MH/s |
| 1000 | NTLM | 67541.2 MH/s |
| 3200 | bcrypt | 47247 H/s |
| 1800 | sha512crypt | 333.2 kH/s |
| 500 | md5crypt | 21398.1 kH/s |
| 2500 | WPA/WPA2 | 684.8 kH/s |
| 7500 | Kerberos AS-REQ (23) | 879.3 MH/s |
| 13100 | Kerberos TGS-REP (23) | 880.9 MH/s |
| 11300 | Bitcoin wallet.dat | 8938 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 478.1 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
PS D:\hashcat> .\hashcat64.exe --benchmark --opencl-devices 1 | Tee-Object -file .\hashcat-benchmark-titanv.log

hashcat (v4.0.1) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #1: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
* Device #3: Not a native Intel OpenCL runtime. Expect massive speed loss.
             You can use --force to override, but do not report related errors.
OpenCL Platform #1: NVIDIA Corporation
======================================
* Device #1: TITAN V, 3072/12288 MB allocatable, 80MCU
* Device #2: GeForce GTX 1080 Ti, skipped.

OpenCL Platform #2: Advanced Micro Devices, Inc.
================================================
* Device #3: Intel(R) Core(TM) i7-6850K CPU @ 3.60GHz, skipped.

Benchmark relevant options:
===========================
* --opencl-devices=1
* --optimized-kernel-enable

Hashmode: 900 - MD4

Speed.Dev.#1.....: 67276.3 MH/s (39.80ms)

Hashmode: 0 - MD5

Speed.Dev.#1.....: 45493.6 MH/s (58.90ms)

Hashmode: 5100 - Half MD5

Speed.Dev.#1.....: 30191.4 MH/s (88.78ms)

Hashmode: 100 - SHA1

Speed.Dev.#1.....: 14689.0 MH/s (91.27ms)

Hashmode: 1400 - SHA-256

Speed.Dev.#1.....:  6491.5 MH/s (51.67ms)

Hashmode: 10800 - SHA-384

Speed.Dev.#1.....:  1864.4 MH/s (89.44ms)

Hashmode: 1700 - SHA-512

Speed.Dev.#1.....:  1881.0 MH/s (88.98ms)

Hashmode: 5000 - SHA-3 (Keccak)

Speed.Dev.#1.....:  1482.4 MH/s (56.23ms)

Hashmode: 10100 - SipHash

Speed.Dev.#1.....: 52731.2 MH/s (50.80ms)

Hashmode: 14900 - Skip32 (PT = $salt, key = $pass)

Speed.Dev.#1.....: 16868.4 MH/s (3.86ms)

Hashmode: 6000 - RIPEMD-160

Speed.Dev.#1.....:  8712.0 MH/s (77.06ms)

Hashmode: 6100 - Whirlpool

Speed.Dev.#1.....:   587.3 MH/s (71.26ms)

Hashmode: 6900 - GOST R 34.11-94

Speed.Dev.#1.....:   589.2 MH/s (70.84ms)

Hashmode: 11700 - GOST R 34.11-2012 (Streebog) 256-bit

Speed.Dev.#1.....:   116.2 MH/s (89.08ms)

Hashmode: 11800 - GOST R 34.11-2012 (Streebog) 512-bit

Speed.Dev.#1.....:   117.3 MH/s (89.07ms)

Hashmode: 14000 - DES (PT = $salt, key = $pass)

Speed.Dev.#1.....: 40014.2 MH/s (67.02ms)

Hashmode: 14100 - 3DES (PT = $salt, key = $pass)

Speed.Dev.#1.....:  2422.1 MH/s (69.04ms)

Hashmode: 400 - phpass, WordPress (MD5), phpBB3 (MD5), Joomla (MD5)

Speed.Dev.#1.....: 13075.6 kH/s (48.86ms)

Hashmode: 8900 - scrypt

Speed.Dev.#1.....:  1378.7 kH/s (13.60ms)

Hashmode: 11900 - PBKDF2-HMAC-MD5

Speed.Dev.#1.....: 15654.3 kH/s (79.79ms)

Hashmode: 12000 - PBKDF2-HMAC-SHA1

Speed.Dev.#1.....:  5590.6 kH/s (53.85ms)

Hashmode: 10900 - PBKDF2-HMAC-SHA256

Speed.Dev.#1.....:  2314.8 kH/s (69.77ms)

Hashmode: 12100 - PBKDF2-HMAC-SHA512

Speed.Dev.#1.....:   721.2 kH/s (53.69ms)

Hashmode: 23 - Skype

Speed.Dev.#1.....: 24560.0 MH/s (54.49ms)

Hashmode: 2500 - WPA/WPA2

Speed.Dev.#1.....:   684.8 kH/s (59.44ms)

Hashmode: 2501 - WPA/WPA2 PMK

Speed.Dev.#1.....:   317.0 MH/s (0.14ms)

Hashmode: 5300 - IKE-PSK MD5

Speed.Dev.#1.....:  3531.5 MH/s (94.13ms)

Hashmode: 5400 - IKE-PSK SHA1

Speed.Dev.#1.....:  1194.7 MH/s (69.94ms)

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.Dev.#1.....: 38502.4 MH/s (69.67ms)

Hashmode: 5600 - NetNTLMv2

Speed.Dev.#1.....:  3188.3 MH/s (52.66ms)

Hashmode: 7300 - IPMI2 RAKP HMAC-SHA1

Speed.Dev.#1.....:  2493.4 MH/s (66.85ms)

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.Dev.#1.....:   879.3 MH/s (95.15ms)

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23

Speed.Dev.#1.....:   880.9 MH/s (94.93ms)

Hashmode: 8300 - DNSSEC (NSEC3)

Speed.Dev.#1.....:  5448.1 MH/s (61.33ms)

Hashmode: 11100 - PostgreSQL CRAM (MD5)

Speed.Dev.#1.....: 13523.0 MH/s (49.59ms)

Hashmode: 11200 - MySQL CRAM (SHA1)

Speed.Dev.#1.....:  3681.6 MH/s (91.08ms)

Hashmode: 11400 - SIP digest authentication (MD5)

Speed.Dev.#1.....:  6534.9 MH/s (51.14ms)

Hashmode: 121 - SMF (Simple Machines Forum) > v1.1

Speed.Dev.#1.....: 11389.0 MH/s (58.60ms)

Hashmode: 2611 - vBulletin < v3.8.5

Speed.Dev.#1.....: 13916.3 MH/s (48.11ms)

Hashmode: 2711 - vBulletin >= v3.8.5

Speed.Dev.#1.....:  9788.9 MH/s (68.57ms)

Hashmode: 2811 - IPB2+ (Invision Power Board), MyBB 1.2+

Speed.Dev.#1.....: 10203.2 MH/s (65.43ms)

Hashmode: 8400 - WBB3 (Woltlab Burning Board)

Speed.Dev.#1.....:  1969.6 MH/s (85.08ms)

Hashmode: 13900 - OpenCart

Speed.Dev.#1.....:  3346.0 MH/s (49.92ms)

Hashmode: 11 - Joomla < 2.5.18

Speed.Dev.#1.....: 45511.4 MH/s (58.92ms)

Hashmode: 2612 - PHPS

Speed.Dev.#1.....: 13948.6 MH/s (96.10ms)

Hashmode: 7900 - Drupal7

Speed.Dev.#1.....:    99217 H/s (51.21ms)

Hashmode: 21 - osCommerce, xt:Commerce

Speed.Dev.#1.....: 24530.5 MH/s (54.40ms)

Hashmode: 11000 - PrestaShop

Speed.Dev.#1.....: 17072.8 MH/s (78.49ms)

Hashmode: 124 - Django (SHA-1)

Speed.Dev.#1.....: 11368.1 MH/s (58.70ms)

Hashmode: 10000 - Django (PBKDF2-SHA256)

Speed.Dev.#1.....:   117.3 kH/s (71.31ms)

Hashmode: 3711 - MediaWiki B type

Speed.Dev.#1.....: 12873.0 MH/s (52.05ms)

Hashmode: 4521 - Redmine

Speed.Dev.#1.....:  5015.7 MH/s (66.88ms)

Hashmode: 4522 - PunBB

Speed.Dev.#1.....:  5016.6 MH/s (66.86ms)

Hashmode: 12 - PostgreSQL

Speed.Dev.#1.....: 45467.3 MH/s (58.91ms)

Hashmode: 131 - MSSQL (2000)

Speed.Dev.#1.....: 15025.5 MH/s (89.13ms)

Hashmode: 132 - MSSQL (2005)

Speed.Dev.#1.....: 15043.4 MH/s (89.16ms)

Hashmode: 1731 - MSSQL (2012, 2014)

Speed.Dev.#1.....:  1889.0 MH/s (88.81ms)

Hashmode: 200 - MySQL323

Speed.Dev.#1.....:   128.3 GH/s (5.08ms)

Hashmode: 300 - MySQL4.1/MySQL5

Speed.Dev.#1.....:  6380.3 MH/s (52.53ms)

Hashmode: 3100 - Oracle H: Type (Oracle 7+)

Speed.Dev.#1.....:  2029.9 MH/s (41.08ms)

Hashmode: 112 - Oracle S: Type (Oracle 11+)

Speed.Dev.#1.....: 14690.6 MH/s (91.18ms)

Hashmode: 12300 - Oracle T: Type (Oracle 12+)

Speed.Dev.#1.....:   205.0 kH/s (96.53ms)

Hashmode: 8000 - Sybase ASE

Speed.Dev.#1.....:   724.2 MH/s (57.93ms)

Hashmode: 141 - Episerver 6.x < .NET 4

Speed.Dev.#1.....: 11383.7 MH/s (58.67ms)

Hashmode: 1441 - Episerver 6.x >= .NET 4

Speed.Dev.#1.....:  5703.0 MH/s (59.02ms)

Hashmode: 1600 - Apache $apr1$ MD5, md5apr1, MD5 (APR)

Speed.Dev.#1.....: 21380.1 kH/s (58.81ms)

Hashmode: 12600 - ColdFusion 10+

Speed.Dev.#1.....:  3436.0 MH/s (48.47ms)

Hashmode: 1421 - hMailServer

Speed.Dev.#1.....:  5694.8 MH/s (59.01ms)

Hashmode: 101 - nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.Dev.#1.....: 14706.6 MH/s (91.25ms)

Hashmode: 111 - nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.Dev.#1.....: 14701.1 MH/s (91.16ms)

Hashmode: 1411 - SSHA-256(Base64), LDAP {SSHA256}

Speed.Dev.#1.....:  6495.9 MH/s (51.70ms)

Hashmode: 1711 - SSHA-512(Base64), LDAP {SSHA512}

Speed.Dev.#1.....:  1883.0 MH/s (88.96ms)

Hashmode: 3000 - LM

Speed.Dev.#1.....: 40545.9 MH/s (66.21ms)

Hashmode: 1000 - NTLM

Speed.Dev.#1.....: 67541.2 MH/s (39.65ms)

Hashmode: 1100 - Domain Cached Credentials (DCC), MS Cache

Speed.Dev.#1.....: 19603.8 MH/s (68.54ms)

Hashmode: 2100 - Domain Cached Credentials 2 (DCC2), MS Cache 2

Speed.Dev.#1.....:   555.4 kH/s (58.74ms)

Hashmode: 15300 - DPAPI masterkey file v1

Speed.Dev.#1.....:   118.6 kH/s (58.76ms)

Hashmode: 15900 - DPAPI masterkey file v2

Speed.Dev.#1.....:   104.5 kH/s (97.90ms)

Hashmode: 12800 - MS-AzureSync PBKDF2-HMAC-SHA256

Speed.Dev.#1.....: 21486.1 kH/s (51.44ms)

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.Dev.#1.....:  1717.9 MH/s (48.42ms)

Hashmode: 12400 - BSDi Crypt, Extended DES

Speed.Dev.#1.....:  4207.9 kH/s (53.18ms)

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)

Speed.Dev.#1.....: 21398.1 kH/s (58.81ms)

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix)

Speed.Dev.#1.....:    47247 H/s (52.55ms)

Hashmode: 7400 - sha256crypt $5$, SHA256 (Unix)

Speed.Dev.#1.....:   873.1 kH/s (37.34ms)

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix)

Speed.Dev.#1.....:   333.2 kH/s (48.91ms)

Hashmode: 122 - macOS v10.4, macOS v10.5, MacOS v10.6

Speed.Dev.#1.....: 11450.2 MH/s (58.59ms)

Hashmode: 1722 - macOS v10.7

Speed.Dev.#1.....:  1825.6 MH/s (91.49ms)

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512)

Speed.Dev.#1.....:    20704 H/s (57.64ms)

Hashmode: 6300 - AIX {smd5}

Speed.Dev.#1.....: 21409.6 kH/s (58.76ms)

Hashmode: 6700 - AIX {ssha1}

Speed.Dev.#1.....: 74099.6 kH/s (14.42ms)

Hashmode: 6400 - AIX {ssha256}

Speed.Dev.#1.....: 34843.1 kH/s (33.30ms)

Hashmode: 6500 - AIX {ssha512}

Speed.Dev.#1.....: 10393.0 kH/s (56.71ms)

Hashmode: 2400 - Cisco-PIX MD5

Speed.Dev.#1.....: 34525.7 MH/s (77.63ms)

Hashmode: 2410 - Cisco-ASA MD5

Speed.Dev.#1.....: 35133.6 MH/s (76.15ms)

Hashmode: 5700 - Cisco-IOS type 4 (SHA256)

Speed.Dev.#1.....:  6503.4 MH/s (51.96ms)

Hashmode: 9200 - Cisco-IOS $8$ (PBKDF2-SHA256)

Speed.Dev.#1.....:   117.3 kH/s (71.29ms)

Hashmode: 9300 - Cisco-IOS $9$ (scrypt)

Speed.Dev.#1.....:        0 H/s (0.00ms)

Hashmode: 22 - Juniper NetScreen/SSG (ScreenOS)

Speed.Dev.#1.....: 24653.7 MH/s (54.42ms)

Hashmode: 501 - Juniper IVE

Speed.Dev.#1.....: 21414.1 kH/s (58.79ms)

Hashmode: 5800 - Samsung Android Password/PIN

Speed.Dev.#1.....: 10086.4 kH/s (63.57ms)

Hashmode: 8100 - Citrix NetScaler

Speed.Dev.#1.....: 12689.5 MH/s (52.76ms)

Hashmode: 8500 - RACF

Speed.Dev.#1.....:  5167.9 MH/s (64.76ms)

Hashmode: 7200 - GRUB 2

Speed.Dev.#1.....:    72519 H/s (57.64ms)

Hashmode: 9900 - Radmin2

Speed.Dev.#1.....: 17257.1 MH/s (77.61ms)

Hashmode: 7700 - SAP CODVN B (BCODE)

Speed.Dev.#1.....:  2866.9 MH/s (58.52ms)

Hashmode: 7800 - SAP CODVN F/G (PASSCODE)

Speed.Dev.#1.....:  2221.9 MH/s (37.42ms)

Hashmode: 10300 - SAP CODVN H (PWDSALTEDHASH) iSSHA-1

Speed.Dev.#1.....:  9967.9 kH/s (64.37ms)

Hashmode: 8600 - Lotus Notes/Domino 5

Speed.Dev.#1.....:   627.6 MH/s (66.71ms)

Hashmode: 8700 - Lotus Notes/Domino 6

Speed.Dev.#1.....:   200.1 MH/s (52.32ms)

Hashmode: 9100 - Lotus Notes/Domino 8

Speed.Dev.#1.....:  1137.7 kH/s (57.75ms)

Hashmode: 133 - PeopleSoft

Speed.Dev.#1.....: 15025.4 MH/s (89.13ms)

Hashmode: 13500 - PeopleSoft PS_TOKEN

Speed.Dev.#1.....:  5198.8 MH/s (64.53ms)

Hashmode: 11600 - 7-Zip

Speed.Dev.#1.....:    16532 H/s (19.23ms)

Hashmode: 13600 - WinZip

Speed.Dev.#1.....:  1816.8 kH/s (83.24ms)

Hashmode: 12500 - RAR3-hp

Speed.Dev.#1.....:    70494 H/s (36.15ms)

Hashmode: 13000 - RAR5

Speed.Dev.#1.....:    71608 H/s (71.27ms)

Hashmode: 13200 - AxCrypt

Speed.Dev.#1.....:   310.6 kH/s (106.37ms)

Hashmode: 13300 - AxCrypt in-memory SHA1

Speed.Dev.#1.....: 13617.8 MH/s (48.95ms)

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit

Speed.Dev.#1.....:   478.1 kH/s (79.99ms)

Hashmode: 6221 - TrueCrypt PBKDF2-HMAC-SHA512 + XTS 512 bit

Speed.Dev.#1.....:   652.8 kH/s (53.70ms)

Hashmode: 6231 - TrueCrypt PBKDF2-HMAC-Whirlpool + XTS 512 bit

Speed.Dev.#1.....:    83326 H/s (116.60ms)

Hashmode: 6241 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit + boot-mode

Speed.Dev.#1.....:   895.7 kH/s (78.83ms)

Hashmode: 13711 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit

Speed.Dev.#1.....:     1550 H/s (80.61ms)

Hashmode: 13721 - VeraCrypt PBKDF2-HMAC-SHA512 + XTS 512 bit

Speed.Dev.#1.....:     1434 H/s (57.63ms)

Hashmode: 13731 - VeraCrypt PBKDF2-HMAC-Whirlpool + XTS 512 bit

Speed.Dev.#1.....:      152 H/s (123.47ms)

Hashmode: 13741 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit + boot-mode

Speed.Dev.#1.....:     3133 H/s (80.61ms)

Hashmode: 13751 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 512 bit

Speed.Dev.#1.....:     2288 H/s (72.38ms)

Hashmode: 13761 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 512 bit + boot-mode

Speed.Dev.#1.....:     5752 H/s (72.37ms)

Hashmode: 8800 - Android FDE <= 4.3

Speed.Dev.#1.....:  1398.9 kH/s (58.52ms)

Hashmode: 12900 - Android FDE (Samsung DEK)

Speed.Dev.#1.....:   572.0 kH/s (71.26ms)

Hashmode: 12200 - eCryptfs

Speed.Dev.#1.....:    27299 H/s (93.51ms)

Hashmode: 9700 - MS Office <= 2003 $0/$1, MD5 + RC4

Speed.Dev.#1.....:   747.7 MH/s (55.90ms)

Hashmode: 9710 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.Dev.#1.....:  1063.8 MH/s (78.72ms)

Hashmode: 9800 - MS Office <= 2003 $3/$4, SHA1 + RC4

Speed.Dev.#1.....:   912.0 MH/s (91.75ms)

Hashmode: 9810 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.Dev.#1.....:  1131.7 MH/s (73.95ms)

Hashmode: 9400 - MS Office 2007

Speed.Dev.#1.....:   232.3 kH/s (57.60ms)

Hashmode: 9500 - MS Office 2010

Speed.Dev.#1.....:   116.2 kH/s (57.56ms)

Hashmode: 9600 - MS Office 2013

Speed.Dev.#1.....:    17812 H/s (93.84ms)

Hashmode: 10400 - PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.Dev.#1.....:  1121.5 MH/s (74.64ms)

Hashmode: 10410 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.Dev.#1.....:  1241.5 MH/s (67.38ms)

Hashmode: 10500 - PDF 1.4 - 1.6 (Acrobat 5 - 8)

Speed.Dev.#1.....: 49478.3 kH/s (10.68ms)

Hashmode: 10600 - PDF 1.7 Level 3 (Acrobat 9)

Speed.Dev.#1.....:  6419.6 MH/s (51.84ms)

Hashmode: 10700 - PDF 1.7 Level 8 (Acrobat 10 - 11)

Speed.Dev.#1.....:    58825 H/s (72.04ms)

Hashmode: 9000 - Password Safe v2

Speed.Dev.#1.....:  1005.2 kH/s (51.14ms)

Hashmode: 5200 - Password Safe v3

Speed.Dev.#1.....:  2584.2 kH/s (62.90ms)

Hashmode: 6800 - LastPass + LastPass sniffed

Speed.Dev.#1.....:  4618.9 kH/s (68.15ms)

Hashmode: 6600 - 1Password, agilekeychain

Speed.Dev.#1.....:  5556.7 kH/s (56.96ms)

Hashmode: 8200 - 1Password, cloudkeychain

Speed.Dev.#1.....:    21004 H/s (99.02ms)

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat

Speed.Dev.#1.....:     8938 H/s (93.49ms)

Hashmode: 12700 - Blockchain, My Wallet

Speed.Dev.#1.....:   112.8 MH/s (4.68ms)

Hashmode: 15200 - Blockchain, My Wallet, V2

Speed.Dev.#1.....:   565.0 kH/s (58.20ms)

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES)

Speed.Dev.#1.....:   241.8 kH/s (56.61ms)

Hashmode: 15500 - JKS Java Key Store Private Keys (SHA1)

Speed.Dev.#1.....: 14181.1 MH/s (47.23ms)

Hashmode: 15600 - Ethereum Wallet, PBKDF2-HMAC-SHA256

Speed.Dev.#1.....:     8949 H/s (71.30ms)

Hashmode: 125 - ArubaOS

Speed.Dev.#1.....: 11388.2 MH/s (58.72ms)

Hashmode: 15400 - ChaCha20

Speed.Dev.#1.....:  7209.8 MH/s (92.97ms)

Started: Wed Jan 17 22:01:09 2018

Stopped: Wed Jan 17 22:29:56 2018
```
