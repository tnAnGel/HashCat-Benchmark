# NVIDIA Tesla V100 PCIe

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Tesla V100-PCIE-16GB
- **Версия hashcat / Version:** v5.1.0
- **Источник / Source:** [nobiinu-and](https://gist.github.com/nobiinu-and/48885061087ef732ebe5caecf7a6e61e)
- **Нестандартный прогон / Non-standard run:** прогон с `--benchmark-all` на 4× Tesla V100-PCIE-16GB (Azure NC24rs v3); в таблице ниже — показатели одной карты (Speed.#1)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 49964.8 MH/s |
| 100 | SHA1 | 15797.8 MH/s |
| 1400 | SHA2-256 | 6796.8 MH/s |
| 1700 | SHA2-512 | 2162.8 MH/s |
| 1000 | NTLM | 83431.6 MH/s |
| 3200 | bcrypt | 48940 H/s |
| 1800 | sha512crypt | 341.9 kH/s |
| 500 | md5crypt | 15622.8 kH/s |
| 7500 | Kerberos AS-REQ (23) | 936.8 MH/s |
| 13100 | Kerberos TGS-REP (23) | 908.4 MH/s |
| 11300 | Bitcoin wallet.dat | 10184 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 541.9 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.1.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL Platform #1: NVIDIA Corporation
======================================
* Device #1: Tesla V100-PCIE-16GB, 4064/16258 MB allocatable, 80MCU
* Device #2: Tesla V100-PCIE-16GB, 4064/16258 MB allocatable, 80MCU
* Device #3: Tesla V100-PCIE-16GB, 4064/16258 MB allocatable, 80MCU
* Device #4: Tesla V100-PCIE-16GB, 4064/16258 MB allocatable, 80MCU

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........: 49964.8 MH/s (26.49ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........: 49904.4 MH/s (26.53ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........: 49768.1 MH/s (26.57ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........: 49958.3 MH/s (26.55ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........:   199.6 GH/s

Hashmode: 10 - md5($pass.$salt)

Speed.#1.........: 50106.3 MH/s (26.48ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........: 50011.6 MH/s (26.53ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........: 50093.4 MH/s (26.50ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........: 50066.9 MH/s (26.51ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........:   200.3 GH/s

Hashmode: 11 - Joomla < 2.5.18

Speed.#1.........: 50030.9 MH/s (26.49ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........: 49942.8 MH/s (26.52ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........: 49986.6 MH/s (26.50ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........: 49968.7 MH/s (26.54ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........:   199.9 GH/s

Hashmode: 12 - PostgreSQL

Speed.#1.........: 50102.5 MH/s (26.49ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........: 50055.3 MH/s (26.51ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........: 50048.3 MH/s (26.53ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........: 49952.3 MH/s (26.52ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........:   200.2 GH/s

Hashmode: 20 - md5($salt.$pass)

Speed.#1.........: 26256.7 MH/s (50.67ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#2.........: 26236.2 MH/s (50.69ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#3.........: 26256.7 MH/s (50.68ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#4.........: 26179.6 MH/s (50.80ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#*.........:   104.9 GH/s

Hashmode: 21 - osCommerce, xt:Commerce

Speed.#1.........: 26239.2 MH/s (50.68ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#2.........: 26258.5 MH/s (50.67ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#3.........: 26262.5 MH/s (50.66ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#4.........: 26182.3 MH/s (50.82ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#*.........:   104.9 GH/s

Hashmode: 22 - Juniper NetScreen/SSG (ScreenOS)

Speed.#1.........: 26038.3 MH/s (51.07ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#2.........: 26044.4 MH/s (51.08ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#3.........: 26032.6 MH/s (51.09ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#4.........: 25968.6 MH/s (51.19ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#*.........:   104.1 GH/s

Hashmode: 23 - Skype

Speed.#1.........: 26253.1 MH/s (50.66ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#2.........: 26225.3 MH/s (50.68ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#3.........: 26232.6 MH/s (50.66ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#4.........: 26146.3 MH/s (50.78ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#*.........:   104.9 GH/s

Hashmode: 30 - md5(utf16le($pass).$salt)

Speed.#1.........: 48844.8 MH/s (26.74ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........: 48882.0 MH/s (26.76ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........: 48908.3 MH/s (26.74ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........: 48781.3 MH/s (26.76ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........:   195.4 GH/s

Hashmode: 40 - md5($salt.utf16le($pass))

Speed.#1.........: 26036.2 MH/s (50.66ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#2.........: 26058.6 MH/s (50.66ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#3.........: 26059.4 MH/s (50.65ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#4.........: 25993.7 MH/s (50.79ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#*.........:   104.1 GH/s

Hashmode: 50 - HMAC-MD5 (key = $pass)

Speed.#1.........:  7969.4 MH/s (83.48ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........:  7966.1 MH/s (83.55ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........:  7969.5 MH/s (83.52ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........:  7952.6 MH/s (83.64ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 31857.6 MH/s

Hashmode: 60 - HMAC-MD5 (key = $salt)

Speed.#1.........: 16793.7 MH/s (79.23ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 16698.9 MH/s (79.70ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#3.........: 16790.6 MH/s (79.29ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#4.........: 16764.1 MH/s (79.40ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#*.........: 67047.3 MH/s

Hashmode: 100 - SHA1

Speed.#1.........: 15797.8 MH/s (84.27ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#2.........: 15798.7 MH/s (84.26ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#3.........: 15798.8 MH/s (84.24ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#4.........: 15759.1 MH/s (84.43ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#*.........: 63154.4 MH/s

Hashmode: 101 - nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.#1.........: 15805.5 MH/s (84.26ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#2.........: 15748.9 MH/s (84.56ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#3.........: 15809.0 MH/s (84.25ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#4.........: 15747.8 MH/s (84.51ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#*.........: 63111.2 MH/s

Hashmode: 110 - sha1($pass.$salt)

Speed.#1.........: 15782.8 MH/s (84.26ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#2.........: 15752.6 MH/s (84.46ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#3.........: 15788.8 MH/s (84.24ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#4.........: 15745.6 MH/s (84.50ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#*.........: 63069.8 MH/s

Hashmode: 111 - nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.#1.........: 15780.8 MH/s (84.26ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#2.........: 15780.9 MH/s (84.27ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#3.........: 15789.3 MH/s (84.24ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#4.........: 15749.9 MH/s (84.44ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#*.........: 63100.9 MH/s

Hashmode: 112 - Oracle S: Type (Oracle 11+)

Speed.#1.........: 15778.1 MH/s (84.26ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#2.........: 15791.2 MH/s (84.27ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#3.........: 15791.6 MH/s (84.24ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#4.........: 15766.6 MH/s (84.39ms) @ Accel:32 Loops:1024 Thr:512 Vec:2
Speed.#*.........: 63127.5 MH/s

Hashmode: 120 - sha1($salt.$pass)

Speed.#1.........: 10784.5 MH/s (61.69ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#2.........: 10783.6 MH/s (61.68ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#3.........: 10816.8 MH/s (61.44ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#4.........: 10787.7 MH/s (61.65ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#*.........: 43172.4 MH/s

Hashmode: 121 - SMF (Simple Machines Forum) > v1.1

Speed.#1.........: 10790.5 MH/s (61.65ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#2.........: 10786.3 MH/s (61.68ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#3.........: 10819.4 MH/s (61.46ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#4.........: 10780.7 MH/s (61.68ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#*.........: 43176.9 MH/s

Hashmode: 122 - macOS v10.4, macOS v10.5, MacOS v10.6

Speed.#1.........: 10789.4 MH/s (61.66ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#2.........: 10788.1 MH/s (61.65ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#3.........: 10812.2 MH/s (61.45ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#4.........: 10791.2 MH/s (61.63ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#*.........: 43180.9 MH/s

Hashmode: 124 - Django (SHA-1)

Speed.#1.........: 10791.2 MH/s (61.68ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#2.........: 10790.6 MH/s (61.69ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#3.........: 10836.3 MH/s (61.43ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#4.........: 10764.0 MH/s (61.80ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#*.........: 43182.2 MH/s

Hashmode: 125 - ArubaOS

Speed.#1.........: 10788.4 MH/s (61.67ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#2.........: 10789.9 MH/s (61.66ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#3.........: 10820.4 MH/s (61.47ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#4.........: 10746.3 MH/s (61.84ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#*.........: 43145.0 MH/s

Hashmode: 130 - sha1(utf16le($pass).$salt)

Speed.#1.........: 17250.1 MH/s (77.01ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#2.........: 17206.5 MH/s (77.25ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#3.........: 17263.0 MH/s (77.04ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#4.........: 17252.9 MH/s (77.10ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#*.........: 68972.5 MH/s

Hashmode: 131 - MSSQL (2000)

Speed.#1.........: 17267.6 MH/s (76.51ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#2.........: 17216.4 MH/s (76.72ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#3.........: 17267.9 MH/s (76.54ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#4.........: 17230.0 MH/s (76.62ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#*.........: 68982.0 MH/s

Hashmode: 132 - MSSQL (2005)

Speed.#1.........: 17262.7 MH/s (77.01ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#2.........: 17249.4 MH/s (77.11ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#3.........: 17262.9 MH/s (77.06ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#4.........: 17234.8 MH/s (77.17ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#*.........: 69009.8 MH/s

Hashmode: 133 - PeopleSoft

Speed.#1.........: 17265.7 MH/s (77.02ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#2.........: 17246.6 MH/s (77.09ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#3.........: 17264.6 MH/s (77.05ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#4.........: 17222.7 MH/s (77.14ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#*.........: 68999.6 MH/s

Hashmode: 140 - sha1($salt.utf16le($pass))

Speed.#1.........: 10765.8 MH/s (61.67ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#2.........: 10772.7 MH/s (61.69ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#3.........: 10805.0 MH/s (61.48ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#4.........: 10719.1 MH/s (61.81ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#*.........: 43062.5 MH/s

Hashmode: 141 - Episerver 6.x < .NET 4

Speed.#1.........: 10780.8 MH/s (61.65ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#2.........: 10782.1 MH/s (61.65ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#3.........: 10811.1 MH/s (61.47ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#4.........: 10727.1 MH/s (61.79ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#*.........: 43101.3 MH/s

Hashmode: 150 - HMAC-SHA1 (key = $pass)

Speed.#1.........:  3115.3 MH/s (80.19ms) @ Accel:32 Loops:256 Thr:384 Vec:1
Speed.#2.........:  3113.9 MH/s (80.28ms) @ Accel:32 Loops:256 Thr:384 Vec:1
Speed.#3.........:  3057.9 MH/s (81.74ms) @ Accel:32 Loops:256 Thr:384 Vec:1
Speed.#4.........:  3115.5 MH/s (80.18ms) @ Accel:32 Loops:256 Thr:384 Vec:1
Speed.#*.........: 12402.6 MH/s

Hashmode: 160 - HMAC-SHA1 (key = $salt)

Speed.#1.........:  6570.7 MH/s (88.73ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#2.........:  6547.0 MH/s (89.03ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#3.........:  6567.2 MH/s (88.78ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#4.........:  6558.7 MH/s (88.82ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#*.........: 26243.6 MH/s

Hashmode: 200 - MySQL323

Speed.#1.........:   159.3 GH/s (8.26ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........:   159.1 GH/s (8.29ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........:   158.8 GH/s (8.25ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........:   158.7 GH/s (8.25ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........:   635.9 GH/s

Hashmode: 300 - MySQL4.1/MySQL5

Speed.#1.........:  7241.5 MH/s (91.97ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.#2.........:  7239.5 MH/s (91.99ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.#3.........:  7243.2 MH/s (91.95ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.#4.........:  7225.7 MH/s (92.17ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.#*.........: 28949.8 MH/s

Hashmode: 400 - phpass, WordPress (MD5), phpBB3 (MD5), Joomla (MD5) (Iterations: 2048)

Speed.#1.........: 10797.9 kH/s (46.86ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 10756.4 kH/s (46.86ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#3.........: 10780.3 kH/s (46.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#4.........: 10754.0 kH/s (46.94ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#*.........: 43088.6 kH/s

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 15622.8 kH/s (56.73ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#2.........: 15552.7 kH/s (56.55ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#3.........: 15450.6 kH/s (57.44ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#4.........: 15552.2 kH/s (56.48ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#*.........: 62178.2 kH/s

Hashmode: 501 - Juniper IVE (Iterations: 1000)

Speed.#1.........: 15544.7 kH/s (57.09ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#2.........: 15498.0 kH/s (57.44ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#3.........: 15538.5 kH/s (56.78ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#4.........: 15516.2 kH/s (56.71ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#*.........: 62097.4 kH/s

Hashmode: 600 - BLAKE2b

Speed.#1.........:  3729.9 MH/s (55.61ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#2.........:  3723.8 MH/s (55.71ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#3.........:  3729.0 MH/s (55.63ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#4.........:  3729.1 MH/s (55.64ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#*.........: 14911.8 MH/s

Hashmode: 900 - MD4

Speed.#1.........: 90506.3 MH/s (14.58ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........: 90423.5 MH/s (14.68ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........: 90656.4 MH/s (14.58ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........: 90524.3 MH/s (14.59ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........:   362.1 GH/s

Hashmode: 1000 - NTLM

Speed.#1.........: 83431.6 MH/s (15.47ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.#2.........: 83151.0 MH/s (15.53ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.#3.........: 83562.5 MH/s (15.46ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.#4.........: 83417.4 MH/s (15.47ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.#*.........:   333.6 GH/s

Hashmode: 1100 - Domain Cached Credentials (DCC), MS Cache

Speed.#1.........: 22521.4 MH/s (58.61ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........: 22434.9 MH/s (58.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........: 22522.4 MH/s (58.60ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........: 22496.4 MH/s (58.69ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........: 89975.2 MH/s

Hashmode: 1300 - SHA2-224

Speed.#1.........:  6685.6 MH/s (49.71ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  6643.2 MH/s (49.84ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  6683.7 MH/s (49.69ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  6676.8 MH/s (49.78ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 26689.3 MH/s

Hashmode: 1400 - SHA2-256

Speed.#1.........:  6796.8 MH/s (48.86ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  6788.2 MH/s (48.98ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  6804.3 MH/s (48.85ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  6796.0 MH/s (48.92ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 27185.3 MH/s

Hashmode: 1410 - sha256($pass.$salt)

Speed.#1.........:  6792.6 MH/s (48.87ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  6792.4 MH/s (48.89ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  6791.3 MH/s (48.84ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  6789.3 MH/s (48.93ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 27165.6 MH/s

Hashmode: 1411 - SSHA-256(Base64), LDAP {SSHA256}

Speed.#1.........:  6798.4 MH/s (48.86ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  6783.1 MH/s (48.96ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  6798.6 MH/s (48.87ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  6787.0 MH/s (48.95ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 27167.2 MH/s

Hashmode: 1420 - sha256($salt.$pass)

Speed.#1.........:  6142.7 MH/s (94.86ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#2.........:  6135.4 MH/s (95.02ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#3.........:  6141.2 MH/s (94.93ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#4.........:  6132.0 MH/s (95.06ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#*.........: 24551.3 MH/s

Hashmode: 1421 - hMailServer

Speed.#1.........:  6130.5 MH/s (94.87ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#2.........:  6130.2 MH/s (94.92ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#3.........:  6142.0 MH/s (94.92ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#4.........:  6137.0 MH/s (94.99ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#*.........: 24539.6 MH/s

Hashmode: 1430 - sha256(utf16le($pass).$salt)

Speed.#1.........:  6824.3 MH/s (48.63ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  6826.6 MH/s (48.65ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  6831.1 MH/s (48.61ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  6830.8 MH/s (48.65ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 27312.9 MH/s

Hashmode: 1440 - sha256($salt.utf16le($pass))

Speed.#1.........:  6142.9 MH/s (94.87ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#2.........:  6141.5 MH/s (94.91ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#3.........:  6141.1 MH/s (94.89ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#4.........:  6129.0 MH/s (95.09ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#*.........: 24554.4 MH/s

Hashmode: 1441 - Episerver 6.x >= .NET 4

Speed.#1.........:  6139.2 MH/s (94.87ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#2.........:  6139.3 MH/s (94.90ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#3.........:  6134.0 MH/s (94.97ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#4.........:  6129.1 MH/s (95.07ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#*.........: 24541.6 MH/s

Hashmode: 1450 - HMAC-SHA256 (key = $pass)

Speed.#1.........:  1240.4 MH/s (83.65ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  1240.4 MH/s (83.68ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  1239.8 MH/s (83.70ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  1238.4 MH/s (83.83ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  4959.1 MH/s

Hashmode: 1460 - HMAC-SHA256 (key = $salt)

Speed.#1.........:  2625.3 MH/s (55.43ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#2.........:  2616.6 MH/s (55.62ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#3.........:  2624.5 MH/s (55.46ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#4.........:  2621.6 MH/s (55.55ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#*.........: 10488.0 MH/s

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:  1696.3 MH/s (49.15ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  1699.8 MH/s (49.06ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  1697.7 MH/s (49.09ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  1697.2 MH/s (49.17ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  6791.0 MH/s

Hashmode: 1600 - Apache $apr1$ MD5, md5apr1, MD5 (APR) (Iterations: 1000)

Speed.#1.........: 15623.0 kH/s (56.71ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#2.........: 15531.1 kH/s (56.78ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#3.........: 15592.7 kH/s (56.54ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#4.........: 15566.7 kH/s (56.64ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#*.........: 62313.4 kH/s

Hashmode: 1700 - SHA2-512

Speed.#1.........:  2162.8 MH/s (47.91ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  2162.4 MH/s (47.91ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  2162.0 MH/s (47.96ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  2162.4 MH/s (47.92ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  8649.7 MH/s

Hashmode: 1710 - sha512($pass.$salt)

Speed.#1.........:  2170.3 MH/s (95.64ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#2.........:  2170.1 MH/s (95.64ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#3.........:  2169.9 MH/s (95.64ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#4.........:  2164.8 MH/s (95.84ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#*.........:  8675.1 MH/s

Hashmode: 1711 - SSHA-512(Base64), LDAP {SSHA512}

Speed.#1.........:  2160.9 MH/s (47.92ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  2160.7 MH/s (47.94ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  2159.3 MH/s (47.97ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  2159.8 MH/s (47.95ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  8640.7 MH/s

Hashmode: 1720 - sha512($salt.$pass)

Speed.#1.........:  1968.2 MH/s (52.65ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  1968.9 MH/s (52.67ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  1967.6 MH/s (52.66ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  1967.2 MH/s (52.71ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  7871.9 MH/s

Hashmode: 1722 - macOS v10.7

Speed.#1.........:  1969.2 MH/s (52.65ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  1969.2 MH/s (52.65ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  1968.9 MH/s (52.67ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  1965.9 MH/s (52.75ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  7873.2 MH/s

Hashmode: 1730 - sha512(utf16le($pass).$salt)

Speed.#1.........:  2169.0 MH/s (95.71ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#2.........:  2167.9 MH/s (95.73ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#3.........:  2165.0 MH/s (95.84ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#4.........:  2166.8 MH/s (95.82ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#*.........:  8668.6 MH/s

Hashmode: 1731 - MSSQL (2012, 2014)

Speed.#1.........:  2165.1 MH/s (95.70ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#2.........:  2167.1 MH/s (95.76ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#3.........:  2163.5 MH/s (95.77ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#4.........:  2166.6 MH/s (95.79ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#*.........:  8662.3 MH/s

Hashmode: 1740 - sha512($salt.utf16le($pass))

Speed.#1.........:  2061.4 MH/s (50.23ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  2061.4 MH/s (50.25ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  2060.9 MH/s (50.28ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  2059.4 MH/s (50.27ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  8243.1 MH/s

Hashmode: 1750 - HMAC-SHA512 (key = $pass)

Speed.#1.........:   434.2 MH/s (95.82ms) @ Accel:32 Loops:32 Thr:512 Vec:1
Speed.#2.........:   434.4 MH/s (95.80ms) @ Accel:32 Loops:32 Thr:512 Vec:1
Speed.#3.........:   434.6 MH/s (95.70ms) @ Accel:32 Loops:32 Thr:512 Vec:1
Speed.#4.........:   433.7 MH/s (95.91ms) @ Accel:32 Loops:32 Thr:512 Vec:1
Speed.#*.........:  1736.9 MH/s

Hashmode: 1760 - HMAC-SHA512 (key = $salt)

Speed.#1.........:   909.2 MH/s (91.54ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#2.........:   909.2 MH/s (91.55ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#3.........:   908.9 MH/s (91.58ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#4.........:   908.7 MH/s (91.59ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#*.........:  3635.9 MH/s

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   341.9 kH/s (47.05ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#2.........:   342.4 kH/s (47.05ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#3.........:   338.4 kH/s (47.58ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#4.........:   342.9 kH/s (46.97ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#*.........:  1365.6 kH/s

Hashmode: 2100 - Domain Cached Credentials 2 (DCC2), MS Cache 2 (Iterations: 10240)

Speed.#1.........:   629.7 kH/s (51.27ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:   626.2 kH/s (51.43ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:   630.2 kH/s (51.22ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:   630.1 kH/s (51.22ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........:  2516.2 kH/s

Hashmode: 2400 - Cisco-PIX MD5

Speed.#1.........: 35980.1 MH/s (36.94ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........: 35851.3 MH/s (37.04ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........: 35992.8 MH/s (36.93ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........: 35858.1 MH/s (36.95ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........:   143.7 GH/s

Hashmode: 2410 - Cisco-ASA MD5

Speed.#1.........: 37022.4 MH/s (44.73ms) @ Accel:32 Loops:1024 Thr:640 Vec:4
Speed.#2.........: 36896.9 MH/s (44.95ms) @ Accel:32 Loops:1024 Thr:640 Vec:4
Speed.#3.........: 37058.3 MH/s (44.75ms) @ Accel:32 Loops:1024 Thr:640 Vec:4
Speed.#4.........: 37010.2 MH/s (44.77ms) @ Accel:32 Loops:1024 Thr:640 Vec:4
Speed.#*.........:   148.0 GH/s

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4096)

Speed.#1.........:   773.6 kH/s (51.92ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#2.........:   773.8 kH/s (51.92ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#3.........:   774.1 kH/s (51.89ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#4.........:   774.1 kH/s (51.88ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#*.........:  3095.6 kH/s

Hashmode: 2501 - WPA-EAPOL-PMK (Iterations: 1)

Speed.#1.........: 43221.6 kH/s (0.01ms) @ Accel:16 Loops:1 Thr:1024 Vec:1
Speed.#2.........: 43679.3 kH/s (0.01ms) @ Accel:16 Loops:1 Thr:1024 Vec:1
Speed.#3.........: 41415.0 kH/s (0.01ms) @ Accel:16 Loops:1 Thr:1024 Vec:1
Speed.#4.........: 43574.6 kH/s (0.01ms) @ Accel:16 Loops:1 Thr:1024 Vec:1
Speed.#*.........:   171.9 MH/s

Hashmode: 2600 - md5(md5($pass))

Speed.#1.........: 14500.5 MH/s (91.66ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 14493.0 MH/s (91.86ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#3.........: 14515.2 MH/s (91.72ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#4.........: 14507.3 MH/s (91.78ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#*.........: 58016.0 MH/s

Hashmode: 2611 - vBulletin < v3.8.5

Speed.#1.........: 14463.4 MH/s (45.93ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........: 14418.8 MH/s (46.11ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........: 14486.5 MH/s (45.92ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 14459.5 MH/s (45.95ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 57828.1 MH/s

Hashmode: 2612 - PHPS

Speed.#1.........: 14526.0 MH/s (91.68ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 14491.4 MH/s (91.90ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#3.........: 14526.5 MH/s (91.69ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#4.........: 14519.6 MH/s (91.73ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#*.........: 58063.4 MH/s

Hashmode: 2711 - vBulletin >= v3.8.5

Speed.#1.........: 10117.9 MH/s (65.63ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........: 10113.9 MH/s (65.78ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........: 10124.5 MH/s (65.62ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 10119.4 MH/s (65.66ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 40475.7 MH/s

Hashmode: 2811 - IPB2+ (Invision Power Board), MyBB 1.2+

Speed.#1.........: 10683.1 MH/s (62.30ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........: 10619.5 MH/s (62.65ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........: 10677.0 MH/s (62.30ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 10677.5 MH/s (62.32ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 42657.2 MH/s

Hashmode: 3000 - LM

Speed.#1.........: 42326.7 MH/s (31.25ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#2.........: 42419.2 MH/s (31.19ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#3.........: 42393.0 MH/s (31.21ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#4.........: 42319.5 MH/s (31.29ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   169.5 GH/s

Hashmode: 3100 - Oracle H: Type (Oracle 7+)

Speed.#1.........:  2391.2 MH/s (60.91ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#2.........:  2391.6 MH/s (60.92ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#3.........:  2390.9 MH/s (60.95ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#4.........:  2385.9 MH/s (61.06ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#*.........:  9559.6 MH/s

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    48940 H/s (50.99ms) @ Accel:16 Loops:8 Thr:8 Vec:1
Speed.#2.........:    48982 H/s (50.96ms) @ Accel:16 Loops:8 Thr:8 Vec:1
Speed.#3.........:    48838 H/s (51.10ms) @ Accel:16 Loops:8 Thr:8 Vec:1
Speed.#4.........:    48830 H/s (51.12ms) @ Accel:16 Loops:8 Thr:8 Vec:1
Speed.#*.........:   195.6 kH/s

Hashmode: 3710 - md5($salt.md5($pass))

Speed.#1.........: 13342.9 MH/s (49.83ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........: 13334.4 MH/s (49.88ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........: 13351.2 MH/s (49.83ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 13346.6 MH/s (49.84ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 53375.1 MH/s

Hashmode: 3711 - MediaWiki B type

Speed.#1.........: 13346.7 MH/s (49.82ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........: 13306.6 MH/s (49.95ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........: 13345.6 MH/s (49.85ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 13324.3 MH/s (49.88ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 53323.2 MH/s

Hashmode: 3800 - md5($salt.$pass.$salt)

Speed.#1.........: 26273.2 MH/s (50.59ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#2.........: 26251.1 MH/s (50.63ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#3.........: 26272.2 MH/s (50.60ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#4.........: 26230.5 MH/s (50.69ms) @ Accel:32 Loops:1024 Thr:512 Vec:4
Speed.#*.........:   105.0 GH/s

Hashmode: 3910 - md5(md5($pass).md5($salt))

Speed.#1.........: 10242.2 MH/s (64.98ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........: 10186.3 MH/s (65.34ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........: 10237.8 MH/s (65.00ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 10230.6 MH/s (65.03ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 40896.8 MH/s

Hashmode: 4010 - md5($salt.md5($salt.$pass))

Speed.#1.........: 10654.1 MH/s (62.39ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#2.........: 10656.4 MH/s (62.39ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#3.........: 10674.5 MH/s (62.28ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#4.........: 10626.1 MH/s (62.54ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#*.........: 42611.2 MH/s

Hashmode: 4110 - md5($salt.md5($pass.$salt))

Speed.#1.........: 11274.3 MH/s (59.03ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#2.........: 11272.7 MH/s (59.01ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#3.........: 11290.6 MH/s (58.94ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#4.........: 11256.7 MH/s (59.12ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#*.........: 45094.4 MH/s

Hashmode: 4300 - md5(strtoupper(md5($pass)))

Speed.#1.........: 14516.6 MH/s (91.66ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 14449.7 MH/s (92.07ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#3.........: 14518.4 MH/s (91.68ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#4.........: 14515.1 MH/s (91.73ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#*.........: 57999.8 MH/s

Hashmode: 4400 - md5(sha1($pass))

Speed.#1.........:  8910.2 MH/s (74.72ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........:  8860.4 MH/s (75.14ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........:  8912.5 MH/s (74.71ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........:  8899.9 MH/s (74.81ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 35583.0 MH/s

Hashmode: 4500 - sha1(sha1($pass))

Speed.#1.........:  6473.8 MH/s (51.34ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  6460.6 MH/s (51.48ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  6474.5 MH/s (51.33ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  6462.5 MH/s (51.41ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 25871.4 MH/s

Hashmode: 4520 - sha1($salt.sha1($pass))

Speed.#1.........:  5067.4 MH/s (65.64ms) @ Accel:32 Loops:256 Thr:512 Vec:2
Speed.#2.........:  5068.2 MH/s (65.62ms) @ Accel:32 Loops:256 Thr:512 Vec:2
Speed.#3.........:  5082.5 MH/s (65.31ms) @ Accel:32 Loops:256 Thr:512 Vec:2
Speed.#4.........:  5059.0 MH/s (65.75ms) @ Accel:32 Loops:256 Thr:512 Vec:2
Speed.#*.........: 20277.1 MH/s

Hashmode: 4521 - Redmine

Speed.#1.........:  5067.0 MH/s (65.58ms) @ Accel:32 Loops:256 Thr:512 Vec:2
Speed.#2.........:  5069.5 MH/s (65.57ms) @ Accel:32 Loops:256 Thr:512 Vec:2
Speed.#3.........:  5093.7 MH/s (65.27ms) @ Accel:32 Loops:256 Thr:512 Vec:2
Speed.#4.........:  5074.0 MH/s (65.56ms) @ Accel:32 Loops:256 Thr:512 Vec:2
Speed.#*.........: 20304.2 MH/s

Hashmode: 4522 - PunBB

Speed.#1.........:  5073.9 MH/s (65.56ms) @ Accel:32 Loops:256 Thr:512 Vec:2
Speed.#2.........:  5072.9 MH/s (65.58ms) @ Accel:32 Loops:256 Thr:512 Vec:2
Speed.#3.........:  5094.0 MH/s (65.26ms) @ Accel:32 Loops:256 Thr:512 Vec:2
Speed.#4.........:  5068.4 MH/s (65.60ms) @ Accel:32 Loops:256 Thr:512 Vec:2
Speed.#*.........: 20309.3 MH/s

Hashmode: 4700 - sha1(md5($pass))

Speed.#1.........:  9177.8 MH/s (72.44ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........:  9176.5 MH/s (72.51ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........:  9178.0 MH/s (72.46ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........:  9172.1 MH/s (72.55ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 36704.3 MH/s

Hashmode: 4800 - iSCSI CHAP authentication, MD5(CHAP)

Speed.#1.........: 29185.1 MH/s (45.52ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........: 29170.1 MH/s (45.55ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........: 29196.8 MH/s (45.50ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........: 29196.1 MH/s (45.54ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........:   116.7 GH/s

Hashmode: 4900 - sha1($salt.$pass.$salt)

Speed.#1.........: 10541.2 MH/s (63.14ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#2.........: 10538.3 MH/s (63.14ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#3.........: 10576.5 MH/s (62.89ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#4.........: 10523.4 MH/s (63.24ms) @ Accel:32 Loops:512 Thr:512 Vec:4
Speed.#*.........: 42179.3 MH/s

Hashmode: 5100 - Half MD5

Speed.#1.........: 31327.9 MH/s (42.45ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........: 31299.0 MH/s (42.49ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........: 31284.3 MH/s (42.47ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........: 31288.5 MH/s (42.50ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........:   125.2 GH/s

Hashmode: 5200 - Password Safe v3 (Iterations: 2048)

Speed.#1.........:  2628.7 kH/s (58.84ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  2624.1 kH/s (58.91ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  2629.7 kH/s (58.78ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  2621.1 kH/s (58.92ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 10503.6 kH/s

Hashmode: 5300 - IKE-PSK MD5

Speed.#1.........:  3877.3 MH/s (85.83ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  3869.4 MH/s (86.02ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  3877.5 MH/s (85.82ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  3874.7 MH/s (85.90ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 15498.9 MH/s

Hashmode: 5400 - IKE-PSK SHA1

Speed.#1.........:  1517.9 MH/s (82.33ms) @ Accel:16 Loops:128 Thr:768 Vec:1
Speed.#2.........:  1517.4 MH/s (82.33ms) @ Accel:16 Loops:128 Thr:768 Vec:1
Speed.#3.........:  1517.8 MH/s (82.33ms) @ Accel:16 Loops:128 Thr:768 Vec:1
Speed.#4.........:  1514.5 MH/s (82.54ms) @ Accel:16 Loops:128 Thr:768 Vec:1
Speed.#*.........:  6067.6 MH/s

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 47615.9 MH/s (27.40ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 47741.7 MH/s (27.42ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#3.........: 47752.6 MH/s (27.40ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#4.........: 47712.6 MH/s (27.40ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:   190.8 GH/s

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  3549.4 MH/s (93.77ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  3547.2 MH/s (93.83ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  3549.9 MH/s (93.77ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  3545.1 MH/s (93.89ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 14191.6 MH/s

Hashmode: 5700 - Cisco-IOS type 4 (SHA256)

Speed.#1.........:  6799.7 MH/s (48.88ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  6799.7 MH/s (48.88ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  6798.3 MH/s (48.84ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  6789.7 MH/s (48.92ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 27187.5 MH/s

Hashmode: 5800 - Samsung Android Password/PIN (Iterations: 1023)

Speed.#1.........:  9480.6 kH/s (36.96ms) @ Accel:16 Loops:511 Thr:1024 Vec:1
Speed.#2.........:  9448.9 kH/s (36.96ms) @ Accel:16 Loops:511 Thr:1024 Vec:1
Speed.#3.........:  9472.0 kH/s (36.98ms) @ Accel:16 Loops:511 Thr:1024 Vec:1
Speed.#4.........:  9447.2 kH/s (36.99ms) @ Accel:16 Loops:511 Thr:1024 Vec:1
Speed.#*.........: 37848.6 kH/s

Hashmode: 6000 - RIPEMD-160

Speed.#1.........: 10936.9 MH/s (60.79ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........: 10934.9 MH/s (60.82ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........: 10935.3 MH/s (60.79ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 10937.2 MH/s (60.80ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 43744.2 MH/s

Hashmode: 6100 - Whirlpool

Speed.#1.........:   727.6 MH/s (85.91ms) @ Accel:16 Loops:64 Thr:768 Vec:1
Speed.#2.........:   727.6 MH/s (85.88ms) @ Accel:16 Loops:64 Thr:768 Vec:1
Speed.#3.........:   727.5 MH/s (85.88ms) @ Accel:16 Loops:64 Thr:768 Vec:1
Speed.#4.........:   727.0 MH/s (85.98ms) @ Accel:16 Loops:64 Thr:768 Vec:1
Speed.#*.........:  2909.7 MH/s

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 2000)

Speed.#1.........:   541.9 kH/s (61.89ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#2.........:   543.7 kH/s (61.88ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#3.........:   541.9 kH/s (61.91ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#4.........:   542.8 kH/s (61.89ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#*.........:  2170.2 kH/s

Hashmode: 6212 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1024 bit (Iterations: 2000)

Speed.#1.........:   214.2 kH/s (48.22ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#2.........:   213.3 kH/s (48.25ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#3.........:   212.1 kH/s (48.20ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#4.........:   214.2 kH/s (48.22ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#*.........:   853.8 kH/s

Hashmode: 6213 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1536 bit (Iterations: 2000)

Speed.#1.........:   260.3 kH/s (69.17ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#2.........:   260.3 kH/s (69.18ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#3.........:   260.0 kH/s (69.26ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#4.........:   259.6 kH/s (69.32ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#*.........:  1040.3 kH/s

Hashmode: 6221 - TrueCrypt PBKDF2-HMAC-SHA512 + XTS 512 bit (Iterations: 1000)

Speed.#1.........:   708.8 kH/s (83.97ms) @ Accel:32 Loops:62 Thr:512 Vec:1
Speed.#2.........:   712.4 kH/s (84.08ms) @ Accel:32 Loops:62 Thr:512 Vec:1
Speed.#3.........:   710.8 kH/s (84.07ms) @ Accel:32 Loops:62 Thr:512 Vec:1
Speed.#4.........:   711.9 kH/s (84.09ms) @ Accel:32 Loops:62 Thr:512 Vec:1
Speed.#*.........:  2843.9 kH/s

Hashmode: 6222 - TrueCrypt PBKDF2-HMAC-SHA512 + XTS 1024 bit (Iterations: 1000)

Speed.#1.........:   236.5 kH/s (65.84ms) @ Accel:32 Loops:31 Thr:384 Vec:1
Speed.#2.........:   236.8 kH/s (65.88ms) @ Accel:32 Loops:31 Thr:384 Vec:1
Speed.#3.........:   235.9 kH/s (65.91ms) @ Accel:32 Loops:31 Thr:384 Vec:1
Speed.#4.........:   238.0 kH/s (65.99ms) @ Accel:32 Loops:31 Thr:384 Vec:1
Speed.#*.........:   947.2 kH/s

Hashmode: 6223 - TrueCrypt PBKDF2-HMAC-SHA512 + XTS 1536 bit (Iterations: 1000)

Speed.#1.........:   169.5 kH/s (49.33ms) @ Accel:32 Loops:15 Thr:384 Vec:1
Speed.#2.........:   169.1 kH/s (49.32ms) @ Accel:32 Loops:15 Thr:384 Vec:1
Speed.#3.........:   169.2 kH/s (49.33ms) @ Accel:32 Loops:15 Thr:384 Vec:1
Speed.#4.........:   168.6 kH/s (49.42ms) @ Accel:32 Loops:15 Thr:384 Vec:1
Speed.#*.........:   676.3 kH/s

Hashmode: 6231 - TrueCrypt PBKDF2-HMAC-Whirlpool + XTS 512 bit (Iterations: 1000)

Speed.#1.........:   106.9 kH/s (136.74ms) @ Accel:32 Loops:15 Thr:384 Vec:1
Speed.#2.........:   107.0 kH/s (136.67ms) @ Accel:32 Loops:15 Thr:384 Vec:1
Speed.#3.........:   106.8 kH/s (136.82ms) @ Accel:32 Loops:15 Thr:384 Vec:1
Speed.#4.........:   106.7 kH/s (136.97ms) @ Accel:32 Loops:15 Thr:384 Vec:1
Speed.#*.........:   427.4 kH/s

Hashmode: 6232 - TrueCrypt PBKDF2-HMAC-Whirlpool + XTS 1024 bit (Iterations: 1000)

Speed.#1.........:    53609 H/s (136.79ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.#2.........:    53601 H/s (136.81ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.#3.........:    53474 H/s (137.14ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.#4.........:    53630 H/s (136.69ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.#*.........:   214.3 kH/s

Hashmode: 6233 - TrueCrypt PBKDF2-HMAC-Whirlpool + XTS 1536 bit (Iterations: 1000)

Speed.#1.........:    35704 H/s (205.26ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.#2.........:    35703 H/s (205.26ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.#3.........:    35564 H/s (206.07ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.#4.........:    35719 H/s (205.13ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.#*.........:   142.7 kH/s

Hashmode: 6241 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 1000)

Speed.#1.........:   920.7 kH/s (58.32ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.#2.........:   920.8 kH/s (58.34ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.#3.........:   920.1 kH/s (58.32ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.#4.........:   919.7 kH/s (58.35ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.#*.........:  3681.4 kH/s

Hashmode: 6242 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 1000)

Speed.#1.........:   299.2 kH/s (46.06ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.#2.........:   297.2 kH/s (46.06ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.#3.........:   296.5 kH/s (46.09ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.#4.........:   298.1 kH/s (46.12ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.#*.........:  1191.0 kH/s

Hashmode: 6243 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 1000)

Speed.#1.........:   226.2 kH/s (65.54ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.#2.........:   224.9 kH/s (65.60ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.#3.........:   223.7 kH/s (65.59ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.#4.........:   224.4 kH/s (65.71ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.#*.........:   899.3 kH/s

Hashmode: 6300 - AIX {smd5} (Iterations: 1000)

Speed.#1.........: 15555.5 kH/s (57.07ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#2.........: 15086.7 kH/s (56.50ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#3.........: 15597.8 kH/s (56.67ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#4.........: 15544.1 kH/s (56.74ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.#*.........: 61784.2 kH/s

Hashmode: 6400 - AIX {ssha256} (Iterations: 64)

Speed.#1.........: 21259.8 kH/s (28.11ms) @ Accel:16 Loops:64 Thr:896 Vec:1
Speed.#2.........: 21164.6 kH/s (28.12ms) @ Accel:16 Loops:64 Thr:896 Vec:1
Speed.#3.........: 21317.9 kH/s (28.17ms) @ Accel:16 Loops:64 Thr:896 Vec:1
Speed.#4.........: 21111.1 kH/s (28.07ms) @ Accel:16 Loops:64 Thr:896 Vec:1
Speed.#*.........: 84853.4 kH/s

Hashmode: 6500 - AIX {ssha512} (Iterations: 64)

Speed.#1.........: 10492.4 kH/s (91.35ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#2.........: 10521.8 kH/s (91.32ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#3.........: 10533.8 kH/s (91.17ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#4.........: 10526.5 kH/s (91.14ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#*.........: 42074.4 kH/s

Hashmode: 6600 - 1Password, agilekeychain (Iterations: 1000)

Speed.#1.........:  5679.3 kH/s (50.04ms) @ Accel:16 Loops:250 Thr:1024 Vec:1
Speed.#2.........:  5644.6 kH/s (50.26ms) @ Accel:16 Loops:250 Thr:1024 Vec:1
Speed.#3.........:  5684.0 kH/s (49.95ms) @ Accel:16 Loops:250 Thr:1024 Vec:1
Speed.#4.........:  5678.2 kH/s (49.95ms) @ Accel:16 Loops:250 Thr:1024 Vec:1
Speed.#*.........: 22686.1 kH/s

Hashmode: 6700 - AIX {ssha1} (Iterations: 64)

Speed.#1.........: 31599.1 kH/s (12.99ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#2.........: 31414.0 kH/s (12.99ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#3.........: 31441.0 kH/s (12.98ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#4.........: 31311.0 kH/s (12.99ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#*.........:   125.8 MH/s

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 500)

Speed.#1.........:  4842.5 kH/s (51.79ms) @ Accel:16 Loops:125 Thr:896 Vec:1
Speed.#2.........:  4834.8 kH/s (51.77ms) @ Accel:16 Loops:125 Thr:896 Vec:1
Speed.#3.........:  4845.1 kH/s (51.75ms) @ Accel:16 Loops:125 Thr:896 Vec:1
Speed.#4.........:  4821.9 kH/s (51.75ms) @ Accel:16 Loops:125 Thr:896 Vec:1
Speed.#*.........: 19344.3 kH/s

Hashmode: 6900 - GOST R 34.11-94

Speed.#1.........:   690.3 MH/s (75.15ms) @ Accel:32 Loops:32 Thr:640 Vec:1
Speed.#2.........:   690.4 MH/s (75.15ms) @ Accel:32 Loops:32 Thr:640 Vec:1
Speed.#3.........:   691.3 MH/s (75.04ms) @ Accel:32 Loops:32 Thr:640 Vec:1
Speed.#4.........:   689.7 MH/s (75.21ms) @ Accel:32 Loops:32 Thr:640 Vec:1
Speed.#*.........:  2761.7 MH/s

Hashmode: 7000 - FortiGate (FortiOS)

Speed.#1.........: 13349.3 MH/s (49.83ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........: 13317.5 MH/s (49.87ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........: 13332.0 MH/s (49.89ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 13333.6 MH/s (49.89ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 53332.3 MH/s

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 35000)

Speed.#1.........:    26009 H/s (91.28ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#2.........:    25993 H/s (91.25ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#3.........:    26020 H/s (91.26ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#4.........:    25948 H/s (91.52ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#*.........:   104.0 kH/s

Hashmode: 7200 - GRUB 2 (Iterations: 10000)

Speed.#1.........:    91055 H/s (91.27ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#2.........:    91059 H/s (91.27ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#3.........:    91057 H/s (91.25ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#4.........:    90799 H/s (91.53ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#*.........:   364.0 kH/s

Hashmode: 7300 - IPMI2 RAKP HMAC-SHA1

Speed.#1.........:  3134.8 MH/s (79.71ms) @ Accel:16 Loops:256 Thr:768 Vec:1
Speed.#2.........:  3134.9 MH/s (79.71ms) @ Accel:16 Loops:256 Thr:768 Vec:1
Speed.#3.........:  3131.5 MH/s (79.80ms) @ Accel:16 Loops:256 Thr:768 Vec:1
Speed.#4.........:  3126.8 MH/s (79.92ms) @ Accel:16 Loops:256 Thr:768 Vec:1
Speed.#*.........: 12528.1 MH/s

Hashmode: 7400 - sha256crypt $5$, SHA256 (Unix) (Iterations: 5000)

Speed.#1.........:   934.8 kH/s (68.07ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:   934.8 kH/s (68.06ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:   934.6 kH/s (68.11ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:   932.4 kH/s (68.26ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........:  3736.5 kH/s

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.#1.........:   936.8 MH/s (88.72ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#2.........:   935.9 MH/s (88.85ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#3.........:   929.1 MH/s (89.57ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#4.........:   930.4 MH/s (89.43ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#*.........:  3732.2 MH/s

Hashmode: 7700 - SAP CODVN B (BCODE)

Speed.#1.........:  4399.5 MH/s (75.64ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  4397.2 MH/s (75.65ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  4357.7 MH/s (76.36ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  4403.8 MH/s (75.49ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 17558.1 MH/s

Hashmode: 7701 - SAP CODVN B (BCODE) mangled from RFC_READ_TABLE

Speed.#1.........:  4458.5 MH/s (74.59ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  4456.9 MH/s (74.64ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  4424.0 MH/s (75.20ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  4470.7 MH/s (74.38ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 17810.2 MH/s

Hashmode: 7800 - SAP CODVN F/G (PASSCODE)

Speed.#1.........:  2492.8 MH/s (83.22ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#2.........:  2494.5 MH/s (83.24ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#3.........:  2494.7 MH/s (83.23ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#4.........:  2494.5 MH/s (83.20ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#*.........:  9976.5 MH/s

Hashmode: 7801 - SAP CODVN F/G (PASSCODE) mangled from RFC_READ_TABLE

Speed.#1.........:  3326.3 MH/s (62.43ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#2.........:  3327.0 MH/s (62.35ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#3.........:  3321.9 MH/s (62.51ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#4.........:  3318.7 MH/s (62.57ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.#*.........: 13293.9 MH/s

Hashmode: 7900 - Drupal7 (Iterations: 16384)

Speed.#1.........:   117.0 kH/s (86.80ms) @ Accel:32 Loops:128 Thr:512 Vec:1
Speed.#2.........:   117.0 kH/s (86.80ms) @ Accel:32 Loops:128 Thr:512 Vec:1
Speed.#3.........:   116.6 kH/s (87.12ms) @ Accel:32 Loops:128 Thr:512 Vec:1
Speed.#4.........:   117.0 kH/s (86.83ms) @ Accel:32 Loops:128 Thr:512 Vec:1
Speed.#*.........:   467.4 kH/s

Hashmode: 8000 - Sybase ASE

Speed.#1.........:   834.5 MH/s (49.76ms) @ Accel:32 Loops:32 Thr:512 Vec:1
Speed.#2.........:   833.9 MH/s (49.78ms) @ Accel:32 Loops:32 Thr:512 Vec:1
Speed.#3.........:   833.1 MH/s (49.78ms) @ Accel:32 Loops:32 Thr:512 Vec:1
Speed.#4.........:   834.1 MH/s (49.79ms) @ Accel:32 Loops:32 Thr:512 Vec:1
Speed.#*.........:  3335.6 MH/s

Hashmode: 8100 - Citrix NetScaler

Speed.#1.........: 14132.0 MH/s (47.03ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........: 14129.6 MH/s (47.03ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........: 14132.4 MH/s (47.03ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 14120.4 MH/s (47.08ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 56514.3 MH/s

Hashmode: 8200 - 1Password, cloudkeychain (Iterations: 40000)

Speed.#1.........:    23591 H/s (87.85ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#2.........:    23563 H/s (87.91ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#3.........:    23662 H/s (87.53ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#4.........:    23600 H/s (87.82ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#*.........:    94417 H/s

Hashmode: 8300 - DNSSEC (NSEC3)

Speed.#1.........:  6223.6 MH/s (93.67ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#2.........:  6225.1 MH/s (93.61ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#3.........:  6220.4 MH/s (93.73ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#4.........:  6212.3 MH/s (93.84ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.#*.........: 24881.4 MH/s

Hashmode: 8400 - WBB3 (Woltlab Burning Board)

Speed.#1.........:  2467.1 MH/s (50.63ms) @ Accel:16 Loops:128 Thr:768 Vec:1
Speed.#2.........:  2468.2 MH/s (50.63ms) @ Accel:16 Loops:128 Thr:768 Vec:1
Speed.#3.........:  2464.7 MH/s (50.69ms) @ Accel:16 Loops:128 Thr:768 Vec:1
Speed.#4.........:  2460.8 MH/s (50.78ms) @ Accel:16 Loops:128 Thr:768 Vec:1
Speed.#*.........:  9860.8 MH/s

Hashmode: 8500 - RACF

Speed.#1.........:  5814.2 MH/s (57.19ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  5817.4 MH/s (57.19ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  5812.8 MH/s (57.24ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  5796.7 MH/s (57.35ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 23241.0 MH/s

Hashmode: 8600 - Lotus Notes/Domino 5

Speed.#1.........:   643.4 MH/s (64.59ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.#2.........:   643.4 MH/s (64.63ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.#3.........:   643.3 MH/s (64.62ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.#4.........:   641.9 MH/s (64.73ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.#*.........:  2572.1 MH/s

Hashmode: 8700 - Lotus Notes/Domino 6

Speed.#1.........:   210.9 MH/s (49.14ms) @ Accel:16 Loops:8 Thr:1024 Vec:1
Speed.#2.........:   211.3 MH/s (49.15ms) @ Accel:16 Loops:8 Thr:1024 Vec:1
Speed.#3.........:   211.3 MH/s (49.15ms) @ Accel:16 Loops:8 Thr:1024 Vec:1
Speed.#4.........:   211.1 MH/s (49.20ms) @ Accel:16 Loops:8 Thr:1024 Vec:1
Speed.#*.........:   844.5 MH/s

Hashmode: 8800 - Android FDE <= 4.3 (Iterations: 2000)

Speed.#1.........:  1549.3 kH/s (50.74ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#2.........:  1549.0 kH/s (50.74ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#3.........:  1550.9 kH/s (50.70ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#4.........:  1549.4 kH/s (50.72ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#*.........:  6198.6 kH/s

Hashmode: 8900 - scrypt (Iterations: 1)

Speed.#1.........:  1035.0 kH/s (15.19ms) @ Accel:16 Loops:1 Thr:16 Vec:1
Speed.#2.........:  1045.4 kH/s (15.03ms) @ Accel:16 Loops:1 Thr:16 Vec:1
Speed.#3.........:  1090.9 kH/s (14.47ms) @ Accel:16 Loops:1 Thr:16 Vec:1
Speed.#4.........:  1085.8 kH/s (14.83ms) @ Accel:16 Loops:1 Thr:16 Vec:1
Speed.#*.........:  4257.1 kH/s

Hashmode: 9000 - Password Safe v2 (Iterations: 1000)

Speed.#1.........:  1009.4 kH/s (50.91ms) @ Accel:512 Loops:250 Thr:8 Vec:1
Speed.#2.........:  1009.3 kH/s (50.88ms) @ Accel:512 Loops:250 Thr:8 Vec:1
Speed.#3.........:  1010.3 kH/s (50.90ms) @ Accel:512 Loops:250 Thr:8 Vec:1
Speed.#4.........:  1009.2 kH/s (50.91ms) @ Accel:512 Loops:250 Thr:8 Vec:1
Speed.#*.........:  4038.3 kH/s

Hashmode: 9100 - Lotus Notes/Domino 8 (Iterations: 5000)

Speed.#1.........:  1263.6 kH/s (50.08ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  1262.8 kH/s (50.14ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  1266.3 kH/s (49.96ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  1267.5 kH/s (49.95ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........:  5060.1 kH/s

Hashmode: 9200 - Cisco-IOS $8$ (PBKDF2-SHA256) (Iterations: 20000)

Speed.#1.........:   137.2 kH/s (53.03ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#2.........:   137.2 kH/s (53.03ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#3.........:   137.0 kH/s (53.12ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#4.........:   137.0 kH/s (53.12ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#*.........:   548.5 kH/s

Hashmode: 9300 - Cisco-IOS $9$ (scrypt) (Iterations: 1)

Speed.#1.........:    53720 H/s (134.16ms) @ Accel:16 Loops:1 Thr:8 Vec:1
Speed.#2.........:    50671 H/s (146.35ms) @ Accel:16 Loops:1 Thr:8 Vec:1
Speed.#3.........:    53054 H/s (133.52ms) @ Accel:16 Loops:1 Thr:8 Vec:1
Speed.#4.........:    51367 H/s (142.60ms) @ Accel:16 Loops:1 Thr:8 Vec:1
Speed.#*.........:   208.8 kH/s

Hashmode: 9400 - MS Office 2007 (Iterations: 50000)

Speed.#1.........:   259.6 kH/s (51.27ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........:   259.3 kH/s (51.31ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........:   259.5 kH/s (51.26ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........:   259.5 kH/s (51.30ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........:  1038.0 kH/s

Hashmode: 9500 - MS Office 2010 (Iterations: 100000)

Speed.#1.........:   129.8 kH/s (51.27ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........:   129.3 kH/s (51.31ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........:   129.7 kH/s (51.31ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........:   129.7 kH/s (51.31ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........:   518.5 kH/s

Hashmode: 9600 - MS Office 2013 (Iterations: 100000)

Speed.#1.........:    20267 H/s (81.91ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#2.........:    20289 H/s (81.98ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#3.........:    20305 H/s (81.95ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#4.........:    20328 H/s (81.83ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#*.........:    81188 H/s

Hashmode: 9700 - MS Office <= 2003 $0/$1, MD5 + RC4

Speed.#1.........:   793.4 MH/s (52.54ms) @ Accel:128 Loops:64 Thr:64 Vec:1
Speed.#2.........:   795.0 MH/s (52.45ms) @ Accel:128 Loops:64 Thr:64 Vec:1
Speed.#3.........:   793.0 MH/s (52.58ms) @ Accel:128 Loops:64 Thr:64 Vec:1
Speed.#4.........:   795.2 MH/s (52.42ms) @ Accel:128 Loops:64 Thr:64 Vec:1
Speed.#*.........:  3176.6 MH/s

Hashmode: 9710 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.#1.........:  1021.8 MH/s (75.01ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#2.........:  1022.0 MH/s (75.02ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#3.........:  1020.3 MH/s (75.02ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#4.........:  1021.7 MH/s (75.05ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#*.........:  4085.8 MH/s

Hashmode: 9720 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #2

Speed.#1.........:  4072.6 MH/s (81.71ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  4071.4 MH/s (81.74ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  4071.6 MH/s (81.74ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  4060.4 MH/s (81.89ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 16276.0 MH/s

Hashmode: 9800 - MS Office <= 2003 $3/$4, SHA1 + RC4

Speed.#1.........:   962.9 MH/s (86.36ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#2.........:   960.9 MH/s (86.52ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#3.........:   963.9 MH/s (86.24ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#4.........:   957.6 MH/s (86.84ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#*.........:  3845.3 MH/s

Hashmode: 9810 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.#1.........:  1086.0 MH/s (70.56ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#2.........:  1086.1 MH/s (70.56ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#3.........:  1086.1 MH/s (70.58ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#4.........:  1085.6 MH/s (70.59ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#*.........:  4343.7 MH/s

Hashmode: 9820 - MS Office <= 2003 $3, SHA1 + RC4, collider #2

Speed.#1.........:  6599.8 MH/s (50.36ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  6602.2 MH/s (50.36ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  6600.2 MH/s (50.38ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  6588.2 MH/s (50.47ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 26390.5 MH/s

Hashmode: 9900 - Radmin2

Speed.#1.........: 17742.2 MH/s (75.03ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........: 17722.6 MH/s (75.05ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........: 17736.4 MH/s (75.05ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........: 17724.6 MH/s (75.11ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........: 70925.7 MH/s

Hashmode: 10000 - Django (PBKDF2-SHA256) (Iterations: 20000)

Speed.#1.........:   137.3 kH/s (53.03ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#2.........:   137.3 kH/s (53.03ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#3.........:   136.8 kH/s (53.13ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#4.........:   136.9 kH/s (53.17ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#*.........:   548.4 kH/s

Hashmode: 10100 - SipHash

Speed.#1.........: 55017.1 MH/s (24.08ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 55005.8 MH/s (24.10ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#3.........: 55059.1 MH/s (24.09ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#4.........: 55038.6 MH/s (24.11ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:   220.1 GH/s

Hashmode: 10200 - CRAM-MD5

Speed.#1.........:  7959.8 MH/s (83.46ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........:  7964.2 MH/s (83.51ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........:  7963.8 MH/s (83.56ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........:  7951.5 MH/s (83.60ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 31839.2 MH/s

Hashmode: 10300 - SAP CODVN H (PWDSALTEDHASH) iSSHA-1 (Iterations: 1023)

Speed.#1.........:  9322.1 kH/s (84.91ms) @ Accel:16 Loops:1023 Thr:768 Vec:1
Speed.#2.........:  9291.2 kH/s (84.99ms) @ Accel:16 Loops:1023 Thr:768 Vec:1
Speed.#3.........:  9286.7 kH/s (85.10ms) @ Accel:16 Loops:1023 Thr:768 Vec:1
Speed.#4.........:  9181.8 kH/s (85.13ms) @ Accel:16 Loops:1023 Thr:768 Vec:1
Speed.#*.........: 37081.8 kH/s

Hashmode: 10400 - PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.#1.........:  1183.6 MH/s (70.27ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#2.........:  1184.1 MH/s (70.20ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#3.........:  1182.8 MH/s (70.33ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#4.........:  1183.3 MH/s (70.28ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#*.........:  4733.8 MH/s

Hashmode: 10410 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.#1.........:  1173.6 MH/s (64.44ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#2.........:  1173.2 MH/s (64.46ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#3.........:  1171.8 MH/s (64.48ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#4.........:  1171.3 MH/s (64.41ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#*.........:  4690.0 MH/s

Hashmode: 10420 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #2

Speed.#1.........: 15277.7 MH/s (87.17ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 15265.1 MH/s (87.24ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#3.........: 15249.5 MH/s (87.27ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#4.........: 15259.2 MH/s (87.27ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#*.........: 61051.5 MH/s

Hashmode: 10500 - PDF 1.4 - 1.6 (Acrobat 5 - 8) (Iterations: 70)

Speed.#1.........: 25559.8 kH/s (23.27ms) @ Accel:256 Loops:70 Thr:64 Vec:1
Speed.#2.........: 24507.3 kH/s (25.70ms) @ Accel:256 Loops:70 Thr:64 Vec:1
Speed.#3.........: 25512.1 kH/s (23.44ms) @ Accel:256 Loops:70 Thr:64 Vec:1
Speed.#4.........: 25514.8 kH/s (23.21ms) @ Accel:256 Loops:70 Thr:64 Vec:1
Speed.#*.........:   101.1 MH/s

Hashmode: 10600 - PDF 1.7 Level 3 (Acrobat 9)

Speed.#1.........:  6800.7 MH/s (48.84ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:  6799.5 MH/s (48.87ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  6796.5 MH/s (48.88ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:  6791.7 MH/s (48.90ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........: 27188.3 MH/s

Hashmode: 10700 - PDF 1.7 Level 8 (Acrobat 10 - 11) (Iterations: 64)

Speed.#1.........:    81926 H/s (155.90ms) @ Accel:8 Loops:2 Thr:640 Vec:1
Speed.#2.........:    82192 H/s (155.38ms) @ Accel:8 Loops:2 Thr:640 Vec:1
Speed.#3.........:    83100 H/s (153.65ms) @ Accel:8 Loops:2 Thr:640 Vec:1
Speed.#4.........:    81787 H/s (156.17ms) @ Accel:8 Loops:2 Thr:640 Vec:1
Speed.#*.........:   329.0 kH/s

Hashmode: 10800 - SHA2-384

Speed.#1.........:  2131.3 MH/s (48.68ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  2131.2 MH/s (48.67ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  2129.5 MH/s (48.74ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  2126.7 MH/s (48.78ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  8518.8 MH/s

Hashmode: 10900 - PBKDF2-HMAC-SHA256 (Iterations: 999)

Speed.#1.........:  2569.5 kH/s (46.55ms) @ Accel:16 Loops:124 Thr:896 Vec:1
Speed.#2.........:  2575.5 kH/s (46.37ms) @ Accel:16 Loops:124 Thr:896 Vec:1
Speed.#3.........:  2576.1 kH/s (46.39ms) @ Accel:16 Loops:124 Thr:896 Vec:1
Speed.#4.........:  2577.7 kH/s (46.35ms) @ Accel:16 Loops:124 Thr:896 Vec:1
Speed.#*.........: 10298.8 kH/s

Hashmode: 11000 - PrestaShop

Speed.#1.........: 17763.9 MH/s (74.95ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 17730.4 MH/s (74.98ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#3.........: 17749.3 MH/s (74.97ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#4.........: 17748.5 MH/s (75.01ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#*.........: 70992.1 MH/s

Hashmode: 11100 - PostgreSQL CRAM (MD5)

Speed.#1.........: 14110.3 MH/s (94.29ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 14086.3 MH/s (94.33ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#3.........: 14112.1 MH/s (94.30ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#4.........: 14100.5 MH/s (94.42ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#*.........: 56409.3 MH/s

Hashmode: 11200 - MySQL CRAM (SHA1)

Speed.#1.........:  4344.1 MH/s (67.04ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.#2.........:  4344.1 MH/s (67.03ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.#3.........:  4342.7 MH/s (67.08ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.#4.........:  4331.6 MH/s (67.22ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.#*.........: 17362.6 MH/s

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 199999)

Speed.#1.........:    10184 H/s (81.68ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#2.........:    10176 H/s (81.71ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#3.........:    10177 H/s (81.76ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#4.........:    10188 H/s (81.63ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#*.........:    40724 H/s

Hashmode: 11400 - SIP digest authentication (MD5)

Speed.#1.........:  6888.6 MH/s (60.29ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.#2.........:  6886.0 MH/s (60.28ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.#3.........:  6875.8 MH/s (60.38ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.#4.........:  6863.8 MH/s (60.42ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.#*.........: 27514.2 MH/s

Hashmode: 11500 - CRC32

Speed.#1.........: 12883.6 MH/s (51.63ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........: 12858.1 MH/s (51.72ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........: 12863.3 MH/s (51.73ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 12881.3 MH/s (51.64ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 51486.4 MH/s

Hashmode: 11600 - 7-Zip (Iterations: 524288)

Speed.#1.........:    19575 H/s (48.67ms) @ Accel:16 Loops:512 Thr:768 Vec:1
Speed.#2.........:    19561 H/s (48.65ms) @ Accel:16 Loops:512 Thr:768 Vec:1
Speed.#3.........:    19597 H/s (48.57ms) @ Accel:16 Loops:512 Thr:768 Vec:1
Speed.#4.........:    19588 H/s (48.65ms) @ Accel:16 Loops:512 Thr:768 Vec:1
Speed.#*.........:    78321 H/s

Hashmode: 11700 - GOST R 34.11-2012 (Streebog) 256-bit, big-endian

Speed.#1.........:   149.5 MH/s (69.49ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.#2.........:   149.6 MH/s (69.50ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.#3.........:   149.4 MH/s (69.58ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.#4.........:   149.6 MH/s (69.43ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.#*.........:   598.0 MH/s

Hashmode: 11750 - HMAC-Streebog-256 (key = $pass), big-endian

Speed.#1.........: 50867.5 kH/s (51.30ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#2.........: 50855.2 kH/s (51.30ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#3.........: 50706.8 kH/s (51.41ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#4.........: 50733.6 kH/s (51.39ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#*.........:   203.2 MH/s

Hashmode: 11760 - HMAC-Streebog-256 (key = $salt), big-endian

Speed.#1.........: 70928.2 kH/s (73.53ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#2.........: 70947.4 kH/s (73.42ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#3.........: 70928.7 kH/s (73.53ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#4.........: 70806.3 kH/s (73.66ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#*.........:   283.6 MH/s

Hashmode: 11800 - GOST R 34.11-2012 (Streebog) 512-bit, big-endian

Speed.#1.........:   149.5 MH/s (69.55ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.#2.........:   149.4 MH/s (69.56ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.#3.........:   149.7 MH/s (69.44ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.#4.........:   149.7 MH/s (69.43ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.#*.........:   598.2 MH/s

Hashmode: 11850 - HMAC-Streebog-512 (key = $pass), big-endian

Speed.#1.........: 43572.2 kH/s (59.93ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#2.........: 43600.8 kH/s (59.89ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#3.........: 43851.6 kH/s (59.52ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#4.........: 43555.1 kH/s (59.92ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#*.........:   174.6 MH/s

Hashmode: 11860 - HMAC-Streebog-512 (key = $salt), big-endian

Speed.#1.........: 58561.4 kH/s (89.07ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#2.........: 58546.0 kH/s (89.10ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#3.........: 58475.8 kH/s (89.24ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#4.........: 58534.8 kH/s (89.10ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#*.........:   234.1 MH/s

Hashmode: 11900 - PBKDF2-HMAC-MD5 (Iterations: 999)

Speed.#1.........: 11885.6 kH/s (15.88ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.#2.........: 11822.4 kH/s (15.87ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.#3.........: 11826.5 kH/s (15.85ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.#4.........: 11787.0 kH/s (15.87ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.#*.........: 47321.4 kH/s

Hashmode: 12000 - PBKDF2-HMAC-SHA1 (Iterations: 999)

Speed.#1.........:  5461.8 kH/s (41.13ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.#2.........:  5487.1 kH/s (40.81ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.#3.........:  5500.9 kH/s (40.74ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.#4.........:  5481.2 kH/s (40.79ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.#*.........: 21930.9 kH/s

Hashmode: 12001 - Atlassian (PBKDF2-HMAC-SHA1) (Iterations: 9999)

Speed.#1.........:   637.6 kH/s (50.43ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:   636.5 kH/s (50.48ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:   636.9 kH/s (50.42ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:   637.7 kH/s (50.43ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........:  2548.8 kH/s

Hashmode: 12100 - PBKDF2-HMAC-SHA512 (Iterations: 999)

Speed.#1.........:   892.0 kH/s (43.43ms) @ Accel:32 Loops:31 Thr:512 Vec:1
Speed.#2.........:   891.5 kH/s (43.45ms) @ Accel:32 Loops:31 Thr:512 Vec:1
Speed.#3.........:   889.3 kH/s (43.40ms) @ Accel:32 Loops:31 Thr:512 Vec:1
Speed.#4.........:   890.1 kH/s (43.52ms) @ Accel:32 Loops:31 Thr:512 Vec:1
Speed.#*.........:  3562.9 kH/s

Hashmode: 12200 - eCryptfs (Iterations: 65535)

Speed.#1.........:    31078 H/s (81.68ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#2.........:    31033 H/s (81.77ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#3.........:    31000 H/s (81.80ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#4.........:    31080 H/s (81.63ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#*.........:   124.2 kH/s

Hashmode: 12300 - Oracle T: Type (Oracle 12+) (Iterations: 4095)

Speed.#1.........:   230.3 kH/s (87.77ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#2.........:   230.0 kH/s (87.88ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#3.........:   231.1 kH/s (87.53ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#4.........:   230.3 kH/s (87.85ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#*.........:   921.7 kH/s

Hashmode: 12400 - BSDi Crypt, Extended DES (Iterations: 2899)

Speed.#1.........:  3458.7 kH/s (14.85ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#2.........:  3454.3 kH/s (14.85ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#3.........:  3455.4 kH/s (14.87ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#4.........:  3457.5 kH/s (14.84ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#*.........: 13825.9 kH/s

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:   104.3 kH/s (73.28ms) @ Accel:4 Loops:16384 Thr:384 Vec:1
Speed.#2.........:   104.4 kH/s (73.30ms) @ Accel:4 Loops:16384 Thr:384 Vec:1
Speed.#3.........:   104.4 kH/s (73.29ms) @ Accel:4 Loops:16384 Thr:384 Vec:1
Speed.#4.........:   104.4 kH/s (73.33ms) @ Accel:4 Loops:16384 Thr:384 Vec:1
Speed.#*.........:   417.5 kH/s

Hashmode: 12600 - ColdFusion 10+

Speed.#1.........:  3914.2 MH/s (74.45ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.#2.........:  3909.1 MH/s (74.44ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.#3.........:  3912.0 MH/s (74.49ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.#4.........:  3899.5 MH/s (74.73ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.#*.........: 15634.8 MH/s

Hashmode: 12700 - Blockchain, My Wallet (Iterations: 10)

Speed.#1.........: 32738.9 kH/s (4.42ms) @ Accel:16 Loops:10 Thr:1024 Vec:1
Speed.#2.........: 33464.4 kH/s (4.42ms) @ Accel:16 Loops:10 Thr:1024 Vec:1
Speed.#3.........: 29537.8 kH/s (4.43ms) @ Accel:16 Loops:10 Thr:1024 Vec:1
Speed.#4.........: 33607.4 kH/s (4.41ms) @ Accel:16 Loops:10 Thr:1024 Vec:1
Speed.#*.........:   129.3 MH/s

Hashmode: 12800 - MS-AzureSync PBKDF2-HMAC-SHA256 (Iterations: 99)

Speed.#1.........: 16211.1 kH/s (41.14ms) @ Accel:16 Loops:99 Thr:896 Vec:1
Speed.#2.........: 16141.0 kH/s (41.15ms) @ Accel:16 Loops:99 Thr:896 Vec:1
Speed.#3.........: 16275.4 kH/s (41.24ms) @ Accel:16 Loops:99 Thr:896 Vec:1
Speed.#4.........: 16123.0 kH/s (41.11ms) @ Accel:16 Loops:99 Thr:896 Vec:1
Speed.#*.........: 64750.6 kH/s

Hashmode: 12900 - Android FDE (Samsung DEK) (Iterations: 4095)

Speed.#1.........:   663.3 kH/s (53.05ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#2.........:   661.6 kH/s (53.18ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#3.........:   662.8 kH/s (53.02ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#4.........:   662.2 kH/s (53.12ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#*.........:  2649.9 kH/s

Hashmode: 13000 - RAR5 (Iterations: 32767)

Speed.#1.........:    83670 H/s (53.03ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#2.........:    83789 H/s (53.04ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#3.........:    83776 H/s (53.05ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#4.........:    83508 H/s (53.23ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#*.........:   334.7 kH/s

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23

Speed.#1.........:   908.4 MH/s (91.57ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#2.........:   906.9 MH/s (91.76ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#3.........:   898.8 MH/s (92.58ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#4.........:   906.6 MH/s (91.78ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#*.........:  3620.6 MH/s

Hashmode: 13200 - AxCrypt (Iterations: 10000)

Speed.#1.........:   320.5 kH/s (103.87ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:   320.5 kH/s (103.88ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:   320.4 kH/s (103.86ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:   320.0 kH/s (103.94ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........:  1281.5 kH/s

Hashmode: 13300 - AxCrypt in-memory SHA1

Speed.#1.........: 13316.8 MH/s (75.07ms) @ Accel:32 Loops:1024 Thr:384 Vec:4
Speed.#2.........: 13322.6 MH/s (75.03ms) @ Accel:32 Loops:1024 Thr:384 Vec:4
Speed.#3.........: 13243.6 MH/s (75.51ms) @ Accel:32 Loops:1024 Thr:384 Vec:4
Speed.#4.........: 13318.0 MH/s (75.02ms) @ Accel:32 Loops:1024 Thr:384 Vec:4
Speed.#*.........: 53201.0 MH/s

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 6000)

Speed.#1.........:   328.4 kH/s (84.07ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#2.........:   328.5 kH/s (84.06ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#3.........:   328.4 kH/s (84.05ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#4.........:   328.5 kH/s (84.08ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#*.........:  1313.9 kH/s

Hashmode: 13500 - PeopleSoft PS_TOKEN

Speed.#1.........:  6061.0 MH/s (82.46ms) @ Accel:16 Loops:512 Thr:768 Vec:1
Speed.#2.........:  6057.7 MH/s (82.46ms) @ Accel:16 Loops:512 Thr:768 Vec:1
Speed.#3.........:  6048.7 MH/s (82.57ms) @ Accel:16 Loops:512 Thr:768 Vec:1
Speed.#4.........:  6038.7 MH/s (82.65ms) @ Accel:16 Loops:512 Thr:768 Vec:1
Speed.#*.........: 24206.1 MH/s

Hashmode: 13600 - WinZip (Iterations: 1000)

Speed.#1.........:  2025.1 kH/s (35.71ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.#2.........:  2023.2 kH/s (35.72ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.#3.........:  2025.5 kH/s (35.70ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.#4.........:  2024.3 kH/s (35.70ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.#*.........:  8098.2 kH/s

Hashmode: 13711 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 655331)

Speed.#1.........:     1991 H/s (63.35ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#2.........:     1987 H/s (63.40ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#3.........:     1991 H/s (63.35ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#4.........:     1991 H/s (63.36ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#*.........:     7960 H/s

Hashmode: 13712 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1024 bit (Iterations: 655331)

Speed.#1.........:     1135 H/s (48.59ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#2.........:     1132 H/s (48.67ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#3.........:     1135 H/s (48.60ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#4.........:     1133 H/s (48.65ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#*.........:     4534 H/s

Hashmode: 13713 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1536 bit (Iterations: 655331)

Speed.#1.........:      794 H/s (69.15ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#2.........:      794 H/s (69.21ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#3.........:      793 H/s (69.26ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#4.........:      791 H/s (69.34ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#*.........:     3172 H/s

Hashmode: 13721 - VeraCrypt PBKDF2-HMAC-SHA512 + XTS 512 bit (Iterations: 500000)

Speed.#1.........:     1820 H/s (91.27ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#2.........:     1817 H/s (91.33ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#3.........:     1816 H/s (91.45ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#4.........:     1813 H/s (91.59ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#*.........:     7265 H/s

Hashmode: 13722 - VeraCrypt PBKDF2-HMAC-SHA512 + XTS 1024 bit (Iterations: 500000)

Speed.#1.........:      897 H/s (69.48ms) @ Accel:32 Loops:32 Thr:384 Vec:1
Speed.#2.........:      897 H/s (69.49ms) @ Accel:32 Loops:32 Thr:384 Vec:1
Speed.#3.........:      895 H/s (69.59ms) @ Accel:32 Loops:32 Thr:384 Vec:1
Speed.#4.........:      894 H/s (69.74ms) @ Accel:32 Loops:32 Thr:384 Vec:1
Speed.#*.........:     3584 H/s

Hashmode: 13723 - VeraCrypt PBKDF2-HMAC-SHA512 + XTS 1536 bit (Iterations: 500000)

Speed.#1.........:      589 H/s (52.79ms) @ Accel:32 Loops:16 Thr:384 Vec:1
Speed.#2.........:      589 H/s (52.82ms) @ Accel:32 Loops:16 Thr:384 Vec:1
Speed.#3.........:      590 H/s (52.80ms) @ Accel:32 Loops:16 Thr:384 Vec:1
Speed.#4.........:      588 H/s (52.91ms) @ Accel:32 Loops:16 Thr:384 Vec:1
Speed.#*.........:     2356 H/s

Hashmode: 13731 - VeraCrypt PBKDF2-HMAC-Whirlpool + XTS 512 bit (Iterations: 500000)

Speed.#1.........:      214 H/s (145.78ms) @ Accel:32 Loops:16 Thr:384 Vec:1
Speed.#2.........:      214 H/s (145.82ms) @ Accel:32 Loops:16 Thr:384 Vec:1
Speed.#3.........:      213 H/s (145.94ms) @ Accel:32 Loops:16 Thr:384 Vec:1
Speed.#4.........:      213 H/s (145.99ms) @ Accel:32 Loops:16 Thr:384 Vec:1
Speed.#*.........:      854 H/s

Hashmode: 13732 - VeraCrypt PBKDF2-HMAC-Whirlpool + XTS 1024 bit (Iterations: 500000)

Speed.#1.........:      106 H/s (146.44ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.#2.........:      106 H/s (146.44ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.#3.........:      106 H/s (146.55ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.#4.........:      106 H/s (146.59ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.#*.........:      424 H/s

Hashmode: 13733 - VeraCrypt PBKDF2-HMAC-Whirlpool + XTS 1536 bit (Iterations: 500000)

Speed.#1.........:       71 H/s (219.96ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.#2.........:       71 H/s (219.91ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.#3.........:       71 H/s (220.12ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.#4.........:       71 H/s (220.06ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.#*.........:      282 H/s

Hashmode: 13741 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 327661)

Speed.#1.........:     3981 H/s (63.36ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#2.........:     3980 H/s (63.38ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#3.........:     3982 H/s (63.35ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#4.........:     3978 H/s (63.41ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.#*.........:    15921 H/s

Hashmode: 13742 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 327661)

Speed.#1.........:     2269 H/s (48.60ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#2.........:     2266 H/s (48.66ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#3.........:     2268 H/s (48.62ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#4.........:     2263 H/s (48.66ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#*.........:     9066 H/s

Hashmode: 13743 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 327661)

Speed.#1.........:     1589 H/s (69.16ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#2.........:     1589 H/s (69.20ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#3.........:     1587 H/s (69.23ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#4.........:     1584 H/s (69.38ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.#*.........:     6350 H/s

Hashmode: 13751 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 512 bit (Iterations: 500000)

Speed.#1.........:     2580 H/s (48.34ms) @ Accel:16 Loops:64 Thr:768 Vec:1
Speed.#2.........:     2579 H/s (48.35ms) @ Accel:16 Loops:64 Thr:768 Vec:1
Speed.#3.........:     2577 H/s (48.40ms) @ Accel:16 Loops:64 Thr:768 Vec:1
Speed.#4.........:     2569 H/s (48.47ms) @ Accel:16 Loops:64 Thr:768 Vec:1
Speed.#*.........:    10305 H/s

Hashmode: 13752 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 1024 bit (Iterations: 500000)

Speed.#1.........:     1264 H/s (49.22ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#2.........:     1263 H/s (49.26ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#3.........:     1259 H/s (49.30ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#4.........:     1260 H/s (49.36ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#*.........:     5045 H/s

Hashmode: 13753 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 1536 bit (Iterations: 500000)

Speed.#1.........:      842 H/s (73.61ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#2.........:      842 H/s (73.63ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#3.........:      842 H/s (73.72ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#4.........:      840 H/s (73.87ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#*.........:     3365 H/s

Hashmode: 13761 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 512 bit + boot-mode (Iterations: 200000)

Speed.#1.........:     6449 H/s (48.34ms) @ Accel:16 Loops:64 Thr:768 Vec:1
Speed.#2.........:     6443 H/s (48.35ms) @ Accel:16 Loops:64 Thr:768 Vec:1
Speed.#3.........:     6445 H/s (48.39ms) @ Accel:16 Loops:64 Thr:768 Vec:1
Speed.#4.........:     6437 H/s (48.47ms) @ Accel:16 Loops:64 Thr:768 Vec:1
Speed.#*.........:    25775 H/s

Hashmode: 13762 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 1024 bit + boot-mode (Iterations: 200000)

Speed.#1.........:     3155 H/s (49.23ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#2.........:     3156 H/s (49.25ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#3.........:     3150 H/s (49.32ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#4.........:     3145 H/s (49.41ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#*.........:    12606 H/s

Hashmode: 13763 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 1536 bit + boot-mode (Iterations: 200000)

Speed.#1.........:     2107 H/s (73.62ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#2.........:     2106 H/s (73.65ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#3.........:     2103 H/s (73.71ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#4.........:     2099 H/s (73.89ms) @ Accel:16 Loops:32 Thr:768 Vec:1
Speed.#*.........:     8416 H/s

Hashmode: 13771 - VeraCrypt PBKDF2-HMAC-Streebog-512 + XTS 512 bit (Iterations: 500000)

Speed.#1.........:       94 H/s (222.05ms) @ Accel:32 Loops:16 Thr:256 Vec:1
Speed.#2.........:       94 H/s (222.07ms) @ Accel:32 Loops:16 Thr:256 Vec:1
Speed.#3.........:       94 H/s (221.55ms) @ Accel:32 Loops:16 Thr:256 Vec:1
Speed.#4.........:       94 H/s (221.56ms) @ Accel:32 Loops:16 Thr:256 Vec:1
Speed.#*.........:      375 H/s

Hashmode: 13772 - VeraCrypt PBKDF2-HMAC-Streebog-512 + XTS 1024 bit (Iterations: 500000)

Speed.#1.........:       44 H/s (234.69ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#2.........:       44 H/s (234.75ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#3.........:       44 H/s (234.29ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#4.........:       44 H/s (234.78ms) @ Accel:32 Loops:8 Thr:256 Vec:1
Speed.#*.........:      176 H/s

Hashmode: 13773 - VeraCrypt PBKDF2-HMAC-Streebog-512 + XTS 1536 bit (Iterations: 500000)

Speed.#1.........:       29 H/s (177.43ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#2.........:       29 H/s (177.42ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#3.........:       29 H/s (177.45ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#4.........:       29 H/s (177.46ms) @ Accel:16 Loops:8 Thr:256 Vec:1
Speed.#*.........:      117 H/s

Hashmode: 13800 - Windows Phone 8+ PIN/password

Speed.#1.........:  1571.4 MH/s (79.47ms) @ Accel:32 Loops:128 Thr:384 Vec:2
Speed.#2.........:  1571.5 MH/s (79.49ms) @ Accel:32 Loops:128 Thr:384 Vec:2
Speed.#3.........:  1564.6 MH/s (79.84ms) @ Accel:32 Loops:128 Thr:384 Vec:2
Speed.#4.........:  1568.8 MH/s (79.63ms) @ Accel:32 Loops:128 Thr:384 Vec:2
Speed.#*.........:  6276.4 MH/s

Hashmode: 13900 - OpenCart

Speed.#1.........:  3995.5 MH/s (72.96ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.#2.........:  3984.8 MH/s (73.14ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.#3.........:  3980.1 MH/s (73.09ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.#4.........:  3980.9 MH/s (73.22ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.#*.........: 15941.3 MH/s

Hashmode: 14000 - DES (PT = $salt, key = $pass)

Speed.#1.........: 40309.0 MH/s (32.87ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#2.........: 40415.3 MH/s (32.78ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#3.........: 40341.9 MH/s (32.84ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#4.........: 40257.4 MH/s (32.90ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   161.3 GH/s

Hashmode: 14100 - 3DES (PT = $salt, key = $pass)

Speed.#1.........:  1993.9 MH/s (83.90ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  1996.0 MH/s (83.86ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  1995.0 MH/s (83.90ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  1995.7 MH/s (83.86ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  7980.7 MH/s

Hashmode: 14400 - sha1(CX)

Speed.#1.........:   678.2 MH/s (92.07ms) @ Accel:32 Loops:64 Thr:384 Vec:1
Speed.#2.........:   679.5 MH/s (92.03ms) @ Accel:32 Loops:64 Thr:384 Vec:1
Speed.#3.........:   680.3 MH/s (91.93ms) @ Accel:32 Loops:64 Thr:384 Vec:1
Speed.#4.........:   676.5 MH/s (92.44ms) @ Accel:32 Loops:64 Thr:384 Vec:1
Speed.#*.........:  2714.5 MH/s

Hashmode: 14600 - LUKS (Iterations: 163044)

Speed.#1.........:    19926 H/s (51.79ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1
Speed.#2.........:    19835 H/s (51.95ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1
Speed.#3.........:    19925 H/s (51.55ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1
Speed.#4.........:    19899 H/s (51.61ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:    79586 H/s

Hashmode: 14700 - iTunes backup < 10.0 (Iterations: 9999)

Speed.#1.........:   319.2 kH/s (52.08ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#2.........:   319.3 kH/s (52.10ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#3.........:   319.5 kH/s (52.08ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#4.........:   319.1 kH/s (52.13ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#*.........:  1277.0 kH/s

Hashmode: 14800 - iTunes backup >= 10.0 (Iterations: 9999999)

Speed.#1.........:      276 H/s (12.93ms) @ Accel:2 Loops:250 Thr:896 Vec:1
Speed.#2.........:      275 H/s (12.93ms) @ Accel:2 Loops:250 Thr:896 Vec:1
Speed.#3.........:      276 H/s (12.93ms) @ Accel:2 Loops:250 Thr:896 Vec:1
Speed.#4.........:      275 H/s (12.97ms) @ Accel:2 Loops:250 Thr:896 Vec:1
Speed.#*.........:     1101 H/s

Hashmode: 14900 - Skip32 (PT = $salt, key = $pass)

Speed.#1.........: 14329.8 MH/s (4.58ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#2.........:        0 H/s (0.00ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#3.........:        0 H/s (0.00ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#4.........:        0 H/s (0.00ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#*.........: 14329.8 MH/s

Hashmode: 15000 - FileZilla Server >= 0.9.55

Speed.#1.........:  1983.7 MH/s (62.92ms) @ Accel:32 Loops:128 Thr:384 Vec:1
Speed.#2.........:  1986.3 MH/s (62.93ms) @ Accel:32 Loops:128 Thr:384 Vec:1
Speed.#3.........:  1927.0 MH/s (64.85ms) @ Accel:32 Loops:128 Thr:384 Vec:1
Speed.#4.........:  1982.2 MH/s (63.06ms) @ Accel:32 Loops:128 Thr:384 Vec:1
Speed.#*.........:  7879.2 MH/s

Hashmode: 15100 - Juniper/NetBSD sha1crypt (Iterations: 19999)

Speed.#1.........:   328.1 kH/s (50.17ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#2.........:   327.7 kH/s (50.22ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#3.........:   328.2 kH/s (50.16ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#4.........:   327.5 kH/s (50.26ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.#*.........:  1311.4 kH/s

Hashmode: 15200 - Blockchain, My Wallet, V2 (Iterations: 5000)

Speed.#1.........:   635.0 kH/s (50.70ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#2.........:   634.7 kH/s (50.71ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#3.........:   634.8 kH/s (50.68ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#4.........:   634.1 kH/s (50.76ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#*.........:  2538.6 kH/s

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:   133.8 kH/s (51.78ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#2.........:   133.7 kH/s (51.84ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#3.........:   133.8 kH/s (51.79ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#4.........:   133.7 kH/s (51.83ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#*.........:   535.0 kH/s

Hashmode: 15400 - ChaCha20

Speed.#1.........: 10183.5 MH/s (65.36ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........: 10042.5 MH/s (66.26ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........: 10184.6 MH/s (65.36ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 10142.1 MH/s (65.62ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 40552.7 MH/s

Hashmode: 15500 - JKS Java Key Store Private Keys (SHA1)

Speed.#1.........: 16015.1 MH/s (51.82ms) @ Accel:32 Loops:512 Thr:640 Vec:1
Speed.#2.........: 16006.5 MH/s (51.85ms) @ Accel:32 Loops:512 Thr:640 Vec:1
Speed.#3.........: 16004.1 MH/s (51.86ms) @ Accel:32 Loops:512 Thr:640 Vec:1
Speed.#4.........: 15962.7 MH/s (51.99ms) @ Accel:32 Loops:512 Thr:640 Vec:1
Speed.#*.........: 63988.4 MH/s

Hashmode: 15600 - Ethereum Wallet, PBKDF2-HMAC-SHA256 (Iterations: 262143)

Speed.#1.........:    10477 H/s (53.04ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#2.........:    10453 H/s (53.14ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#3.........:    10459 H/s (53.11ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#4.........:    10445 H/s (53.14ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#*.........:    41835 H/s

Hashmode: 15700 - Ethereum Wallet, SCRYPT (Iterations: 1)

Speed.#1.........:        5 H/s (9036.45ms) @ Accel:1 Loops:1 Thr:1 Vec:1
Speed.#2.........:        5 H/s (9034.88ms) @ Accel:1 Loops:1 Thr:1 Vec:1
Speed.#3.........:        5 H/s (9023.63ms) @ Accel:1 Loops:1 Thr:1 Vec:1
Speed.#4.........:        5 H/s (9018.09ms) @ Accel:1 Loops:1 Thr:1 Vec:1
Speed.#*.........:       21 H/s

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 7999)

Speed.#1.........:   108.4 kH/s (96.09ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#2.........:   108.2 kH/s (96.17ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#3.........:   108.4 kH/s (96.11ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#4.........:   108.2 kH/s (96.22ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#*.........:   433.1 kH/s

Hashmode: 16000 - Tripcode

Speed.#1.........:   527.4 MH/s (78.90ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.#2.........:   526.5 MH/s (79.00ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.#3.........:   527.1 MH/s (78.95ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.#4.........:   526.2 MH/s (79.08ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.#*.........:  2107.3 MH/s

Hashmode: 16100 - TACACS+

Speed.#1.........: 28277.1 MH/s (47.04ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 28121.6 MH/s (47.29ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#3.........: 28262.8 MH/s (47.05ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#4.........: 28251.4 MH/s (47.08ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:   112.9 GH/s

Hashmode: 16200 - Apple Secure Notes (Iterations: 19999)

Speed.#1.........:   137.5 kH/s (53.01ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#2.........:   137.5 kH/s (53.00ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#3.........:   137.2 kH/s (53.10ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#4.........:   137.0 kH/s (53.16ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#*.........:   549.2 kH/s

Hashmode: 16300 - Ethereum Pre-Sale Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1999)

Speed.#1.........:  1325.6 kH/s (51.77ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#2.........:  1324.7 kH/s (51.77ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#3.........:  1325.1 kH/s (51.78ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#4.........:  1325.3 kH/s (51.76ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#*.........:  5300.6 kH/s

Hashmode: 16400 - CRAM-MD5 Dovecot

Speed.#1.........: 50357.8 MH/s (26.36ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#2.........: 50317.9 MH/s (26.39ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#3.........: 50355.2 MH/s (26.36ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#4.........: 50298.9 MH/s (26.40ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.#*.........:   201.3 GH/s

Hashmode: 16500 - JWT (JSON Web Token)

Speed.#1.........:  1192.7 MH/s (69.69ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#2.........:  1192.3 MH/s (69.75ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#3.........:  1191.4 MH/s (69.81ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#4.........:  1192.4 MH/s (69.71ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.#*.........:  4768.9 MH/s

Hashmode: 16600 - Electrum Wallet (Salt-Type 1-3)

Speed.#1.........:   777.4 MH/s (53.49ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.#2.........:   777.3 MH/s (53.51ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.#3.........:   776.5 MH/s (53.56ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.#4.........:   776.6 MH/s (53.53ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.#*.........:  3107.8 MH/s

Hashmode: 16700 - FileVault 2 (Iterations: 19999)

Speed.#1.........:   137.4 kH/s (53.00ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#2.........:   137.0 kH/s (53.08ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#3.........:   137.2 kH/s (53.09ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#4.........:   137.1 kH/s (53.10ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#*.........:   548.6 kH/s

Hashmode: 16800 - WPA-PMKID-PBKDF2 (Iterations: 4096)

Speed.#1.........:   773.0 kH/s (51.93ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#2.........:   771.6 kH/s (52.04ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#3.........:   773.3 kH/s (51.92ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#4.........:   772.8 kH/s (51.95ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#*.........:  3090.6 kH/s

Hashmode: 16801 - WPA-PMKID-PMK (Iterations: 1)

Speed.#1.........: 42367.4 kH/s (0.01ms) @ Accel:16 Loops:1 Thr:1024 Vec:1
Speed.#2.........: 42836.1 kH/s (0.01ms) @ Accel:16 Loops:1 Thr:1024 Vec:1
Speed.#3.........: 43561.3 kH/s (0.01ms) @ Accel:16 Loops:1 Thr:1024 Vec:1
Speed.#4.........: 43432.1 kH/s (0.01ms) @ Accel:16 Loops:1 Thr:1024 Vec:1
Speed.#*.........:   172.2 MH/s

Hashmode: 16900 - Ansible Vault (Iterations: 9999)

Speed.#1.........:   274.7 kH/s (53.03ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#2.........:   274.4 kH/s (53.09ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#3.........:   274.6 kH/s (53.05ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#4.........:   274.1 kH/s (53.14ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#*.........:  1097.9 kH/s

Hashmode: 17300 - SHA3-224

Speed.#1.........:  1550.4 MH/s (66.89ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  1550.6 MH/s (66.93ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  1551.4 MH/s (66.88ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  1549.7 MH/s (66.96ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  6202.1 MH/s

Hashmode: 17400 - SHA3-256

Speed.#1.........:  1545.9 MH/s (67.09ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  1543.3 MH/s (67.25ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  1546.0 MH/s (67.10ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  1543.7 MH/s (67.18ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  6178.8 MH/s

Hashmode: 17500 - SHA3-384

Speed.#1.........:  1550.2 MH/s (66.92ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  1543.3 MH/s (67.25ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  1549.8 MH/s (66.97ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  1547.1 MH/s (67.01ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  6190.5 MH/s

Hashmode: 17600 - SHA3-512

Speed.#1.........:  1550.1 MH/s (66.93ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  1545.6 MH/s (66.94ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  1550.1 MH/s (66.97ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  1547.7 MH/s (67.06ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  6193.6 MH/s

Hashmode: 17700 - Keccak-224

Speed.#1.........:  1551.5 MH/s (66.86ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  1551.5 MH/s (66.88ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  1550.5 MH/s (66.89ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  1550.0 MH/s (66.97ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  6203.6 MH/s

Hashmode: 17800 - Keccak-256

Speed.#1.........:  1547.0 MH/s (67.06ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  1547.1 MH/s (67.07ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  1547.1 MH/s (67.09ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  1545.1 MH/s (67.17ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  6186.2 MH/s

Hashmode: 17900 - Keccak-384

Speed.#1.........:  1550.4 MH/s (66.91ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  1550.4 MH/s (66.92ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  1550.4 MH/s (66.93ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  1548.2 MH/s (67.03ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  6199.4 MH/s

Hashmode: 18000 - Keccak-512

Speed.#1.........:  1549.9 MH/s (66.93ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#2.........:  1549.8 MH/s (66.95ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#3.........:  1549.9 MH/s (66.96ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#4.........:  1548.2 MH/s (67.03ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.#*.........:  6197.7 MH/s

Hashmode: 18100 - TOTP (HMAC-SHA1)

Speed.#1.........:  2852.4 MH/s (58.32ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#2.........:  2852.9 MH/s (58.32ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#3.........:  2839.2 MH/s (58.55ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#4.........:  2854.9 MH/s (58.28ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#*.........: 11399.5 MH/s

Hashmode: 18200 - Kerberos 5 AS-REP etype 23

Speed.#1.........:   899.2 MH/s (92.54ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#2.........:   901.9 MH/s (92.20ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#3.........:   899.2 MH/s (92.54ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#4.........:   896.5 MH/s (92.82ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#*.........:  3596.7 MH/s

Hashmode: 18300 - Apple File System (APFS) (Iterations: 19999)

Speed.#1.........:   137.4 kH/s (53.00ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#2.........:   137.2 kH/s (53.01ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#3.........:   137.4 kH/s (53.04ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#4.........:   137.2 kH/s (53.11ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.#*.........:   549.1 kH/s
```
