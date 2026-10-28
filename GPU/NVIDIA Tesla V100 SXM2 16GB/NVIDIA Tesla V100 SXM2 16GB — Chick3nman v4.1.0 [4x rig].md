# NVIDIA Tesla V100 SXM2 16GB (4x rig)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Tesla V100 SXM2 16GB
- **Конфигурация / Setup:** 4x rig
- **Версия hashcat / Version:** v4.1.0
- **Источник / Source:** [Chick3nman](https://gist.github.com/Chick3nman/4d3c5fd44f33610ddbbf026d46d9e0aa)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 56166.6 MH/s |
| 100 | SHA1 | 17064.3 MH/s |
| 1400 | SHA2-256 | 7601.4 MH/s |
| 1700 | SHA2-512 | 2410.3 MH/s |
| 1000 | NTLM | 79394.7 MH/s |
| 3200 | bcrypt | 54262 H/s |
| 1800 | sha512crypt | 377.1 kH/s |
| 500 | md5crypt | 24742.7 kH/s |
| 2500 | WPA/WPA2 (legacy) | 813.8 kH/s |
| 7500 | Kerberos AS-REQ (23) | 996.2 MH/s |
| 13100 | Kerberos TGS-REP (23) | 997.1 MH/s |
| 11300 | Bitcoin wallet.dat | 11238 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 577.9 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v4.1.0) starting in benchmark mode...

OpenCL Platform #1: NVIDIA Corporation
======================================
* Device #1: Tesla V100-SXM2-16GB, 4040/16160 MB allocatable, 80MCU
* Device #2: Tesla V100-SXM2-16GB, 4040/16160 MB allocatable, 80MCU
* Device #3: Tesla V100-SXM2-16GB, 4040/16160 MB allocatable, 80MCU
* Device #4: Tesla V100-SXM2-16GB, 4040/16160 MB allocatable, 80MCU

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.Dev.#1.....: 56166.6 MH/s (23.80ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#2.....: 56168.1 MH/s (23.80ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#3.....: 56046.7 MH/s (23.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#4.....: 56107.9 MH/s (23.82ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#*.....:   224.5 GH/s

Hashmode: 10 - md5($pass.$salt)

Speed.Dev.#1.....: 56163.2 MH/s (23.80ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#2.....: 56170.2 MH/s (23.80ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#3.....: 56045.5 MH/s (23.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#4.....: 56104.8 MH/s (23.82ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#*.....:   224.5 GH/s

Hashmode: 11 - Joomla < 2.5.18

Speed.Dev.#1.....: 56172.4 MH/s (23.80ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#2.....: 56172.0 MH/s (23.80ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#3.....: 56054.2 MH/s (23.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#4.....: 56119.5 MH/s (23.82ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#*.....:   224.5 GH/s

Hashmode: 12 - PostgreSQL

Speed.Dev.#1.....: 56165.8 MH/s (23.80ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#2.....: 56166.0 MH/s (23.80ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#3.....: 56053.7 MH/s (23.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#4.....: 56125.8 MH/s (23.82ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#*.....:   224.5 GH/s

Hashmode: 20 - md5($salt.$pass)

Speed.Dev.#1.....: 28900.7 MH/s (46.34ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 28899.1 MH/s (46.35ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 28832.0 MH/s (46.48ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 28836.8 MH/s (46.44ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....:   115.5 GH/s

Hashmode: 21 - osCommerce, xt:Commerce

Speed.Dev.#1.....: 28903.1 MH/s (46.43ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 28901.1 MH/s (46.36ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 28905.1 MH/s (46.43ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 28843.4 MH/s (46.45ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....:   115.6 GH/s

Hashmode: 22 - Juniper NetScreen/SSG (ScreenOS)

Speed.Dev.#1.....: 28908.8 MH/s (46.33ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 28904.9 MH/s (46.34ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 28910.6 MH/s (46.34ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 28851.6 MH/s (46.43ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....:   115.6 GH/s

Hashmode: 23 - Skype

Speed.Dev.#1.....: 28903.2 MH/s (46.36ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 28901.7 MH/s (46.35ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 28903.3 MH/s (46.34ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 28840.5 MH/s (46.45ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....:   115.5 GH/s

Hashmode: 30 - md5(utf16le($pass).$salt)

Speed.Dev.#1.....: 55149.6 MH/s (24.24ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#2.....: 55148.8 MH/s (24.25ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#3.....: 55023.0 MH/s (24.30ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#4.....: 55057.2 MH/s (24.28ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#*.....:   220.4 GH/s

Hashmode: 40 - md5($salt.utf16le($pass))

Speed.Dev.#1.....: 28898.1 MH/s (46.38ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 28897.6 MH/s (46.43ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 28826.1 MH/s (46.48ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 28831.8 MH/s (46.45ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....:   115.5 GH/s

Hashmode: 50 - HMAC-MD5 (key = $pass)

Speed.Dev.#1.....:  8895.9 MH/s (75.32ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:  8895.2 MH/s (75.33ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:  8868.5 MH/s (75.57ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:  8875.5 MH/s (75.51ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 35535.0 MH/s

Hashmode: 60 - HMAC-MD5 (key = $salt)

Speed.Dev.#1.....: 18658.7 MH/s (71.84ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 18658.2 MH/s (71.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 18613.3 MH/s (72.07ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 18609.6 MH/s (72.01ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....: 74539.7 MH/s

Hashmode: 100 - SHA1

Speed.Dev.#1.....: 17064.3 MH/s (78.53ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#2.....: 17070.2 MH/s (78.54ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#3.....: 17013.4 MH/s (78.79ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#4.....: 17036.1 MH/s (78.71ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#*.....: 68184.1 MH/s

Hashmode: 101 - nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.Dev.#1.....: 17070.3 MH/s (78.54ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#2.....: 17071.2 MH/s (78.59ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#3.....: 17022.9 MH/s (78.73ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#4.....: 17035.4 MH/s (78.73ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#*.....: 68199.8 MH/s

Hashmode: 110 - sha1($pass.$salt)

Speed.Dev.#1.....: 17071.6 MH/s (78.53ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#2.....: 17071.3 MH/s (78.54ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#3.....: 17026.1 MH/s (78.76ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#4.....: 17035.6 MH/s (78.69ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#*.....: 68204.5 MH/s

Hashmode: 111 - nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.Dev.#1.....: 16992.3 MH/s (78.64ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#2.....: 17061.9 MH/s (78.54ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#3.....: 17029.9 MH/s (78.76ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#4.....: 17039.5 MH/s (78.70ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#*.....: 68123.6 MH/s

Hashmode: 112 - Oracle S: Type (Oracle 11+)

Speed.Dev.#1.....: 16999.1 MH/s (78.74ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#2.....: 17062.1 MH/s (78.54ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#3.....: 17022.4 MH/s (78.73ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#4.....: 17034.7 MH/s (78.71ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#*.....: 68118.3 MH/s

Hashmode: 120 - sha1($salt.$pass)

Speed.Dev.#1.....: 13198.4 MH/s (50.74ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 13244.4 MH/s (50.57ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 13199.5 MH/s (50.73ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 13247.6 MH/s (50.64ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 52889.9 MH/s

Hashmode: 121 - SMF (Simple Machines Forum) > v1.1

Speed.Dev.#1.....: 13200.6 MH/s (50.73ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 13246.9 MH/s (50.57ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 13202.5 MH/s (50.74ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 13248.3 MH/s (50.59ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 52898.3 MH/s

Hashmode: 122 - macOS v10.4, macOS v10.5, MacOS v10.6

Speed.Dev.#1.....: 13198.8 MH/s (50.72ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 13246.5 MH/s (50.57ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 13203.0 MH/s (50.74ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 13248.7 MH/s (50.60ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 52897.0 MH/s

Hashmode: 124 - Django (SHA-1)

Speed.Dev.#1.....: 13197.6 MH/s (50.71ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 13246.5 MH/s (50.57ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 13200.0 MH/s (50.74ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 13248.4 MH/s (50.60ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 52892.5 MH/s

Hashmode: 125 - ArubaOS

Speed.Dev.#1.....: 13193.8 MH/s (50.70ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 13245.1 MH/s (50.58ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 13201.7 MH/s (50.71ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 13248.5 MH/s (50.61ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 52889.1 MH/s

Hashmode: 130 - sha1(utf16le($pass).$salt)

Speed.Dev.#1.....: 17522.0 MH/s (76.43ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#2.....: 17576.6 MH/s (76.26ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#3.....: 17533.4 MH/s (76.48ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#4.....: 17577.3 MH/s (76.28ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#*.....: 70209.3 MH/s

Hashmode: 131 - MSSQL (2000)

Speed.Dev.#1.....: 16320.9 MH/s (75.94ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#2.....: 16368.2 MH/s (75.78ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#3.....: 16331.4 MH/s (75.98ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#4.....: 16367.9 MH/s (75.85ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#*.....: 65388.4 MH/s

Hashmode: 132 - MSSQL (2005)

Speed.Dev.#1.....: 17515.1 MH/s (76.44ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#2.....: 17576.7 MH/s (76.26ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#3.....: 17530.0 MH/s (76.48ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#4.....: 17578.4 MH/s (76.33ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#*.....: 70200.3 MH/s

Hashmode: 133 - PeopleSoft

Speed.Dev.#1.....: 17515.1 MH/s (76.45ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#2.....: 17577.5 MH/s (76.27ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#3.....: 17531.5 MH/s (76.43ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#4.....: 17578.7 MH/s (76.33ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#*.....: 70202.8 MH/s

Hashmode: 140 - sha1($salt.utf16le($pass))

Speed.Dev.#1.....: 13194.3 MH/s (50.68ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 13245.2 MH/s (50.58ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 13203.7 MH/s (50.74ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 13245.5 MH/s (50.58ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 52888.7 MH/s

Hashmode: 141 - Episerver 6.x < .NET 4

Speed.Dev.#1.....: 13195.9 MH/s (50.68ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 13246.0 MH/s (50.57ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 13204.9 MH/s (50.73ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 13248.3 MH/s (50.62ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 52895.2 MH/s

Hashmode: 150 - HMAC-SHA1 (key = $pass)

Speed.Dev.#1.....:  3191.8 MH/s (78.80ms) @ Accel:64 Loops:128 Thr:384 Vec:1
Speed.Dev.#2.....:  3190.7 MH/s (78.80ms) @ Accel:64 Loops:128 Thr:384 Vec:1
Speed.Dev.#3.....:  3187.7 MH/s (78.88ms) @ Accel:64 Loops:128 Thr:384 Vec:1
Speed.Dev.#4.....:  3187.2 MH/s (78.90ms) @ Accel:64 Loops:128 Thr:384 Vec:1
Speed.Dev.#*.....: 12757.5 MH/s

Hashmode: 160 - HMAC-SHA1 (key = $salt)

Speed.Dev.#1.....:  6737.7 MH/s (86.83ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.Dev.#2.....:  6765.8 MH/s (86.71ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.Dev.#3.....:  6745.5 MH/s (86.95ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.Dev.#4.....:  6765.5 MH/s (86.81ms) @ Accel:16 Loops:512 Thr:896 Vec:1
Speed.Dev.#*.....: 27014.5 MH/s

Hashmode: 200 - MySQL323

Speed.Dev.#1.....:   168.2 GH/s (7.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#2.....:   169.2 GH/s (7.84ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#3.....:   168.5 GH/s (7.84ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#4.....:   169.0 GH/s (7.84ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#*.....:   674.9 GH/s

Hashmode: 300 - MySQL4.1/MySQL5

Speed.Dev.#1.....:  7497.0 MH/s (89.43ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.Dev.#2.....:  7495.9 MH/s (89.43ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.Dev.#3.....:  7474.2 MH/s (89.57ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.Dev.#4.....:  7487.2 MH/s (89.55ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.Dev.#*.....: 29954.2 MH/s

Hashmode: 400 - phpass, WordPress (MD5), phpBB3 (MD5), Joomla (MD5) (Iterations: 2048)

Speed.Dev.#1.....: 15172.8 kH/s (42.12ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 15168.7 kH/s (42.12ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 15125.1 kH/s (42.22ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 15143.7 kH/s (42.24ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....: 60610.4 kH/s

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.Dev.#1.....: 24742.7 kH/s (51.25ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#2.....: 24737.3 kH/s (51.30ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#3.....: 24718.0 kH/s (51.35ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#4.....: 24743.6 kH/s (51.34ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#*.....: 98941.6 kH/s

Hashmode: 501 - Juniper IVE (Iterations: 1000)

Speed.Dev.#1.....: 24750.1 kH/s (51.25ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#2.....: 24728.6 kH/s (51.27ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#3.....: 24677.9 kH/s (51.35ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#4.....: 24704.1 kH/s (51.33ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#*.....: 98860.7 kH/s

Hashmode: 600 - BLAKE2b

Speed.Dev.#1.....:  3990.1 MH/s (52.48ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:  3989.8 MH/s (52.48ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:  3989.9 MH/s (52.47ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:  3982.6 MH/s (52.56ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....: 15952.4 MH/s

Hashmode: 900 - MD4

Speed.Dev.#1.....: 81683.8 MH/s (16.33ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#2.....: 81668.4 MH/s (16.33ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#3.....: 81440.7 MH/s (16.38ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#4.....: 81661.7 MH/s (16.33ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#*.....:   326.5 GH/s

Hashmode: 1000 - NTLM

Speed.Dev.#1.....: 79394.7 MH/s (16.81ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#2.....: 79403.1 MH/s (16.81ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#3.....: 79180.2 MH/s (16.86ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#4.....: 79253.5 MH/s (16.84ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#*.....:   317.2 GH/s

Hashmode: 1100 - Domain Cached Credentials (DCC), MS Cache

Speed.Dev.#1.....: 22435.4 MH/s (52.26ms) @ Accel:16 Loops:1024 Thr:896 Vec:4
Speed.Dev.#2.....: 22433.3 MH/s (52.27ms) @ Accel:16 Loops:1024 Thr:896 Vec:4
Speed.Dev.#3.....: 22381.7 MH/s (52.40ms) @ Accel:16 Loops:1024 Thr:896 Vec:4
Speed.Dev.#4.....: 22385.5 MH/s (52.39ms) @ Accel:16 Loops:1024 Thr:896 Vec:4
Speed.Dev.#*.....: 89635.9 MH/s

Hashmode: 1300 - SHA-224

Speed.Dev.#1.....:  7405.7 MH/s (45.21ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  7404.9 MH/s (45.22ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  7379.9 MH/s (45.34ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  7390.7 MH/s (45.32ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 29581.3 MH/s

Hashmode: 1400 - SHA-256

Speed.Dev.#1.....:  7601.4 MH/s (88.21ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:  7600.2 MH/s (88.21ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:  7574.4 MH/s (88.52ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:  7584.4 MH/s (88.34ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 30360.3 MH/s

Hashmode: 1410 - sha256($pass.$salt)

Speed.Dev.#1.....:  7600.8 MH/s (88.19ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:  7600.3 MH/s (88.21ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:  7573.9 MH/s (88.52ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:  7583.4 MH/s (88.41ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 30358.3 MH/s

Hashmode: 1411 - SSHA-256(Base64), LDAP {SSHA256}

Speed.Dev.#1.....:  7601.3 MH/s (88.19ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:  7600.9 MH/s (88.21ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:  7574.1 MH/s (88.44ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:  7580.5 MH/s (88.43ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 30356.9 MH/s

Hashmode: 1420 - sha256($salt.$pass)

Speed.Dev.#1.....:  6812.3 MH/s (49.16ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  6812.2 MH/s (49.16ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  6787.2 MH/s (49.36ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  6793.9 MH/s (49.31ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 27205.6 MH/s

Hashmode: 1421 - hMailServer

Speed.Dev.#1.....:  6812.3 MH/s (49.16ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  6811.7 MH/s (49.17ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  6789.6 MH/s (49.35ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  6793.5 MH/s (49.31ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 27206.9 MH/s

Hashmode: 1430 - sha256(utf16le($pass).$salt)

Speed.Dev.#1.....:  7577.2 MH/s (88.47ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:  7576.7 MH/s (88.48ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:  7550.2 MH/s (88.79ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:  7558.6 MH/s (88.70ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 30262.7 MH/s

Hashmode: 1440 - sha256($salt.utf16le($pass))

Speed.Dev.#1.....:  6812.6 MH/s (49.16ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  6812.0 MH/s (49.16ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  6813.0 MH/s (49.16ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  6797.0 MH/s (49.29ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 27234.6 MH/s

Hashmode: 1441 - Episerver 6.x >= .NET 4

Speed.Dev.#1.....:  6809.1 MH/s (49.16ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  6808.4 MH/s (49.16ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  6783.2 MH/s (49.35ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  6793.1 MH/s (49.27ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 27193.7 MH/s

Hashmode: 1450 - HMAC-SHA256 (key = $pass)

Speed.Dev.#1.....:  1334.2 MH/s (47.06ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#2.....:  1333.9 MH/s (47.07ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#3.....:  1330.9 MH/s (47.18ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#4.....:  1331.7 MH/s (47.15ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#*.....:  5330.7 MH/s

Hashmode: 1460 - HMAC-SHA256 (key = $salt)

Speed.Dev.#1.....:  2793.8 MH/s (52.46ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.Dev.#2.....:  2793.7 MH/s (52.46ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.Dev.#3.....:  2793.7 MH/s (52.46ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.Dev.#4.....:  2787.6 MH/s (52.57ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.Dev.#*.....: 11168.8 MH/s

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.Dev.#1.....:  1855.3 MH/s (90.14ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.Dev.#2.....:  1861.4 MH/s (90.19ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.Dev.#3.....:  1856.9 MH/s (90.31ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.Dev.#4.....:  1853.8 MH/s (90.22ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.Dev.#*.....:  7427.4 MH/s

Hashmode: 1600 - Apache $apr1$ MD5, md5apr1, MD5 (APR) (Iterations: 1000)

Speed.Dev.#1.....: 24709.4 kH/s (51.35ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#2.....: 24767.3 kH/s (51.26ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#3.....: 24792.5 kH/s (51.22ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#4.....: 24720.0 kH/s (51.35ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#*.....: 98989.3 kH/s

Hashmode: 1700 - SHA-512

Speed.Dev.#1.....:  2410.3 MH/s (86.87ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:  2411.3 MH/s (86.88ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:  2404.4 MH/s (87.14ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:  2405.0 MH/s (87.11ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:  9630.9 MH/s

Hashmode: 1710 - sha512($pass.$salt)

Speed.Dev.#1.....:  2411.1 MH/s (86.88ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:  2411.6 MH/s (86.88ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:  2406.6 MH/s (87.08ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:  2405.7 MH/s (87.10ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:  9635.0 MH/s

Hashmode: 1711 - SSHA-512(Base64), LDAP {SSHA512}

Speed.Dev.#1.....:  2404.3 MH/s (43.74ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#2.....:  2404.2 MH/s (43.53ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#3.....:  2398.4 MH/s (43.63ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#4.....:  2399.5 MH/s (43.63ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#*.....:  9606.4 MH/s

Hashmode: 1720 - sha512($salt.$pass)

Speed.Dev.#1.....:  2189.7 MH/s (95.75ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:  2189.6 MH/s (95.68ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:  2183.9 MH/s (95.84ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:  2184.9 MH/s (95.93ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:  8748.0 MH/s

Hashmode: 1722 - macOS v10.7

Speed.Dev.#1.....:  2188.8 MH/s (95.68ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:  2188.9 MH/s (95.69ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:  2184.3 MH/s (95.92ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:  2184.4 MH/s (95.92ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:  8746.4 MH/s

Hashmode: 1730 - sha512(utf16le($pass).$salt)

Speed.Dev.#1.....:  2409.8 MH/s (86.90ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:  2409.6 MH/s (86.91ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:  2404.8 MH/s (87.11ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:  2404.8 MH/s (87.13ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:  9628.9 MH/s

Hashmode: 1731 - MSSQL (2012, 2014)

Speed.Dev.#1.....:  2410.8 MH/s (86.90ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:  2410.7 MH/s (86.91ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:  2405.0 MH/s (87.04ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:  2404.8 MH/s (87.14ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:  9631.2 MH/s

Hashmode: 1740 - sha512($salt.utf16le($pass))

Speed.Dev.#1.....:  2272.0 MH/s (45.87ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#2.....:  2281.7 MH/s (45.86ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#3.....:  2276.9 MH/s (45.96ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#4.....:  2276.8 MH/s (45.93ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#*.....:  9107.4 MH/s

Hashmode: 1750 - HMAC-SHA512 (key = $pass)

Speed.Dev.#1.....:   481.9 MH/s (86.88ms) @ Accel:32 Loops:32 Thr:512 Vec:1
Speed.Dev.#2.....:   482.5 MH/s (86.89ms) @ Accel:32 Loops:32 Thr:512 Vec:1
Speed.Dev.#3.....:   480.9 MH/s (86.92ms) @ Accel:32 Loops:32 Thr:512 Vec:1
Speed.Dev.#4.....:   480.2 MH/s (87.06ms) @ Accel:32 Loops:32 Thr:512 Vec:1
Speed.Dev.#*.....:  1925.5 MH/s

Hashmode: 1760 - HMAC-SHA512 (key = $salt)

Speed.Dev.#1.....:  1001.9 MH/s (83.65ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#2.....:  1001.1 MH/s (83.66ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#3.....:  1000.1 MH/s (83.84ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#4.....:   999.5 MH/s (83.83ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#*.....:  4002.5 MH/s

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.Dev.#1.....:   377.1 kH/s (85.84ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.Dev.#2.....:   380.4 kH/s (85.10ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.Dev.#3.....:   378.7 kH/s (85.38ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.Dev.#4.....:   377.6 kH/s (85.74ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.Dev.#*.....:  1513.8 kH/s

Hashmode: 2100 - Domain Cached Credentials 2 (DCC2), MS Cache 2 (Iterations: 10240)

Speed.Dev.#1.....:   657.9 kH/s (49.72ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:   657.9 kH/s (49.71ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:   655.9 kH/s (49.86ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:   656.2 kH/s (49.84ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....:  2627.9 kH/s

Hashmode: 2400 - Cisco-PIX MD5

Speed.Dev.#1.....: 38395.6 MH/s (34.93ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#2.....: 38398.1 MH/s (35.00ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#3.....: 38292.4 MH/s (34.97ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#4.....: 38325.4 MH/s (35.04ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#*.....:   153.4 GH/s

Hashmode: 2410 - Cisco-ASA MD5

Speed.Dev.#1.....: 41486.1 MH/s (40.35ms) @ Accel:32 Loops:1024 Thr:640 Vec:4
Speed.Dev.#2.....: 41487.0 MH/s (40.35ms) @ Accel:32 Loops:1024 Thr:640 Vec:4
Speed.Dev.#3.....: 41388.5 MH/s (40.46ms) @ Accel:32 Loops:1024 Thr:640 Vec:4
Speed.Dev.#4.....: 41426.8 MH/s (40.41ms) @ Accel:32 Loops:1024 Thr:640 Vec:4
Speed.Dev.#*.....:   165.8 GH/s

Hashmode: 2500 - WPA/WPA2 (Iterations: 4096)

Speed.Dev.#1.....:   813.8 kH/s (50.20ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#2.....:   813.9 kH/s (50.21ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#3.....:   813.8 kH/s (50.21ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#4.....:   812.2 kH/s (50.32ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#*.....:  3253.7 kH/s

Hashmode: 2501 - WPA/WPA2 PMK (Iterations: 1)

Speed.Dev.#1.....:   423.1 MH/s (0.01ms) @ Accel:16 Loops:1 Thr:1024 Vec:1
Speed.Dev.#2.....:   423.2 MH/s (0.01ms) @ Accel:16 Loops:1 Thr:1024 Vec:1
Speed.Dev.#3.....:   423.0 MH/s (0.01ms) @ Accel:16 Loops:1 Thr:1024 Vec:1
Speed.Dev.#4.....:   423.1 MH/s (0.01ms) @ Accel:16 Loops:1 Thr:1024 Vec:1
Speed.Dev.#*.....:  1692.4 MH/s

Hashmode: 2600 - md5(md5($pass))

Speed.Dev.#1.....: 16125.8 MH/s (83.06ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 16145.4 MH/s (83.05ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 16115.0 MH/s (83.24ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 16112.7 MH/s (83.22ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....: 64499.0 MH/s

Hashmode: 2611 - vBulletin < v3.8.5

Speed.Dev.#1.....: 16145.4 MH/s (83.05ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 16145.6 MH/s (83.05ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 16144.9 MH/s (83.05ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 16111.7 MH/s (83.20ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....: 64547.5 MH/s

Hashmode: 2612 - PHPS

Speed.Dev.#1.....: 16142.9 MH/s (83.08ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 16143.3 MH/s (83.10ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 16142.4 MH/s (83.05ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 16112.9 MH/s (83.26ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....: 64541.5 MH/s

Hashmode: 2711 - vBulletin >= v3.8.5

Speed.Dev.#1.....: 11175.6 MH/s (59.97ms) @ Accel:16 Loops:512 Thr:1024 Vec:2
Speed.Dev.#2.....: 11176.8 MH/s (59.96ms) @ Accel:16 Loops:512 Thr:1024 Vec:2
Speed.Dev.#3.....: 11141.5 MH/s (60.12ms) @ Accel:16 Loops:512 Thr:1024 Vec:2
Speed.Dev.#4.....: 11146.0 MH/s (60.12ms) @ Accel:16 Loops:512 Thr:1024 Vec:2
Speed.Dev.#*.....: 44639.9 MH/s

Hashmode: 2811 - IPB2+ (Invision Power Board), MyBB 1.2+

Speed.Dev.#1.....: 11927.4 MH/s (56.18ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 11926.6 MH/s (56.18ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 11925.3 MH/s (56.18ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 11915.9 MH/s (56.26ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 47695.2 MH/s

Hashmode: 3000 - LM

Speed.Dev.#1.....: 47826.7 MH/s (27.90ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.Dev.#2.....: 47825.3 MH/s (27.89ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.Dev.#3.....: 47831.8 MH/s (27.89ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.Dev.#4.....: 47775.1 MH/s (27.93ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.Dev.#*.....:   191.3 GH/s

Hashmode: 3100 - Oracle H: Type (Oracle 7+)

Speed.Dev.#1.....:  2624.2 MH/s (55.82ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.Dev.#2.....:  2627.6 MH/s (55.73ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.Dev.#3.....:  2619.8 MH/s (55.87ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.Dev.#4.....:  2620.4 MH/s (55.88ms) @ Accel:16 Loops:128 Thr:896 Vec:1
Speed.Dev.#*.....: 10492.0 MH/s

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.Dev.#1.....:    54262 H/s (46.06ms) @ Accel:16 Loops:8 Thr:8 Vec:1
Speed.Dev.#2.....:    54197 H/s (46.11ms) @ Accel:16 Loops:8 Thr:8 Vec:1
Speed.Dev.#3.....:    54112 H/s (46.18ms) @ Accel:16 Loops:8 Thr:8 Vec:1
Speed.Dev.#4.....:    54133 H/s (46.16ms) @ Accel:16 Loops:8 Thr:8 Vec:1
Speed.Dev.#*.....:   216.7 kH/s

Hashmode: 3710 - md5($salt.md5($pass))

Speed.Dev.#1.....: 15053.4 MH/s (89.08ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 15052.2 MH/s (89.08ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 15052.9 MH/s (89.08ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 15029.7 MH/s (89.25ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....: 60188.2 MH/s

Hashmode: 3711 - MediaWiki B type

Speed.Dev.#1.....: 14836.9 MH/s (79.07ms) @ Accel:16 Loops:1024 Thr:896 Vec:2
Speed.Dev.#2.....: 14838.3 MH/s (79.08ms) @ Accel:16 Loops:1024 Thr:896 Vec:2
Speed.Dev.#3.....: 14836.6 MH/s (79.08ms) @ Accel:16 Loops:1024 Thr:896 Vec:2
Speed.Dev.#4.....: 14811.8 MH/s (79.24ms) @ Accel:16 Loops:1024 Thr:896 Vec:2
Speed.Dev.#*.....: 59323.6 MH/s

Hashmode: 3800 - md5($salt.$pass.$salt)

Speed.Dev.#1.....: 28941.1 MH/s (46.27ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 28939.0 MH/s (46.27ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 28940.9 MH/s (46.28ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 28883.9 MH/s (46.44ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....:   115.7 GH/s

Hashmode: 3910 - md5(md5($pass).md5($salt))

Speed.Dev.#1.....: 11361.7 MH/s (58.97ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 11363.1 MH/s (58.97ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 11362.8 MH/s (58.97ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 11349.9 MH/s (59.05ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 45437.4 MH/s

Hashmode: 4010 - md5($salt.md5($salt.$pass))

Speed.Dev.#1.....: 13278.7 MH/s (50.42ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 13279.0 MH/s (50.43ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 13288.4 MH/s (50.42ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 13262.8 MH/s (50.52ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 53108.9 MH/s

Hashmode: 4110 - md5($salt.md5($pass.$salt))

Speed.Dev.#1.....: 14211.1 MH/s (47.12ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 14213.3 MH/s (47.14ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 14182.4 MH/s (47.22ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 14193.7 MH/s (47.18ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 56800.5 MH/s

Hashmode: 4300 - md5(strtoupper(md5($pass)))

Speed.Dev.#1.....: 16145.1 MH/s (83.05ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 16143.3 MH/s (83.05ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 16103.8 MH/s (83.27ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 16142.7 MH/s (83.07ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....: 64534.9 MH/s

Hashmode: 4400 - md5(sha1($pass))

Speed.Dev.#1.....:  9479.1 MH/s (70.70ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:  9478.8 MH/s (70.71ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:  9446.4 MH/s (70.92ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:  9458.3 MH/s (70.88ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 37862.5 MH/s

Hashmode: 4500 - sha1(sha1($pass))

Speed.Dev.#1.....:  6742.3 MH/s (49.67ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  6742.1 MH/s (49.67ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  6721.0 MH/s (49.85ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  6728.6 MH/s (49.80ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 26934.0 MH/s

Hashmode: 4520 - sha1($salt.sha1($pass))

Speed.Dev.#1.....:  6150.9 MH/s (68.10ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#2.....:  6150.4 MH/s (68.10ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#3.....:  6137.2 MH/s (68.27ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#4.....:  6133.8 MH/s (68.29ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#*.....: 24572.2 MH/s

Hashmode: 4521 - Redmine

Speed.Dev.#1.....:  6151.1 MH/s (68.10ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#2.....:  6150.5 MH/s (68.10ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#3.....:  6150.1 MH/s (68.10ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#4.....:  6136.3 MH/s (68.28ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#*.....: 24588.0 MH/s

Hashmode: 4522 - PunBB

Speed.Dev.#1.....:  6150.5 MH/s (68.10ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#2.....:  6150.6 MH/s (68.10ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#3.....:  6149.4 MH/s (68.10ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#4.....:  6134.4 MH/s (68.29ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#*.....: 24585.0 MH/s

Hashmode: 4700 - sha1(md5($pass))

Speed.Dev.#1.....:  9857.4 MH/s (67.98ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:  9854.0 MH/s (67.98ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:  9853.9 MH/s (67.99ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:  9857.2 MH/s (67.98ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 39422.6 MH/s

Hashmode: 4800 - iSCSI CHAP authentication, MD5(CHAP)

Speed.Dev.#1.....: 33368.1 MH/s (40.13ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 33366.8 MH/s (40.13ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 33380.6 MH/s (40.16ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 33333.1 MH/s (40.17ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....:   133.4 GH/s

Hashmode: 4900 - sha1($salt.$pass.$salt)

Speed.Dev.#1.....: 12959.2 MH/s (51.69ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 12958.9 MH/s (51.70ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 12922.8 MH/s (51.86ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 12931.7 MH/s (51.81ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 51772.6 MH/s

Hashmode: 5000 - SHA-3 (Keccak)

Speed.Dev.#1.....:  1740.9 MH/s (60.14ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#2.....:  1740.9 MH/s (60.15ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#3.....:  1736.0 MH/s (60.32ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#4.....:  1737.1 MH/s (60.30ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#*.....:  6955.0 MH/s

Hashmode: 5100 - Half MD5

Speed.Dev.#1.....: 35462.3 MH/s (37.78ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#2.....: 35462.0 MH/s (37.82ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#3.....: 35359.5 MH/s (37.87ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#4.....: 35462.6 MH/s (37.83ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#*.....:   141.7 GH/s

Hashmode: 5200 - Password Safe v3 (Iterations: 2048)

Speed.Dev.#1.....:  3052.2 kH/s (53.39ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  3051.9 kH/s (53.40ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  3041.6 kH/s (53.53ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  3044.6 kH/s (53.54ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 12190.3 kH/s

Hashmode: 5300 - IKE-PSK MD5

Speed.Dev.#1.....:  4325.4 MH/s (77.49ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  4324.9 MH/s (77.49ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  4310.5 MH/s (77.76ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  4316.0 MH/s (77.68ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 17276.8 MH/s

Hashmode: 5400 - IKE-PSK SHA1

Speed.Dev.#1.....:  1545.0 MH/s (67.78ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#2.....:  1545.8 MH/s (67.82ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#3.....:  1541.1 MH/s (67.95ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#4.....:  1541.9 MH/s (67.89ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#*.....:  6173.9 MH/s

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.Dev.#1.....: 41776.0 MH/s (29.96ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 41799.1 MH/s (29.97ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 41645.1 MH/s (30.04ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 41723.6 MH/s (30.03ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....:   166.9 GH/s

Hashmode: 5600 - NetNTLMv2

Speed.Dev.#1.....:  3912.0 MH/s (85.68ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  3912.2 MH/s (85.68ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  3901.0 MH/s (85.92ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  3905.5 MH/s (85.86ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 15630.7 MH/s

Hashmode: 5700 - Cisco-IOS type 4 (SHA256)

Speed.Dev.#1.....:  7586.5 MH/s (44.14ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  7585.1 MH/s (44.14ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  7561.7 MH/s (44.30ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  7563.1 MH/s (44.25ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 30296.4 MH/s

Hashmode: 5800 - Samsung Android Password/PIN (Iterations: 1023)

Speed.Dev.#1.....: 12022.2 kH/s (35.74ms) @ Accel:16 Loops:511 Thr:1024 Vec:1
Speed.Dev.#2.....: 12022.9 kH/s (35.71ms) @ Accel:16 Loops:511 Thr:1024 Vec:1
Speed.Dev.#3.....: 11978.8 kH/s (35.83ms) @ Accel:16 Loops:511 Thr:1024 Vec:1
Speed.Dev.#4.....: 11996.3 kH/s (35.81ms) @ Accel:16 Loops:511 Thr:1024 Vec:1
Speed.Dev.#*.....: 48020.2 kH/s

Hashmode: 6000 - RIPEMD-160

Speed.Dev.#1.....: 10229.2 MH/s (65.54ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 10229.4 MH/s (65.51ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 10199.9 MH/s (65.68ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 10205.0 MH/s (65.69ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 40863.6 MH/s

Hashmode: 6100 - Whirlpool

Speed.Dev.#1.....:   806.0 MH/s (90.67ms) @ Accel:16 Loops:64 Thr:896 Vec:1
Speed.Dev.#2.....:   810.5 MH/s (90.46ms) @ Accel:16 Loops:64 Thr:896 Vec:1
Speed.Dev.#3.....:   806.8 MH/s (90.90ms) @ Accel:16 Loops:64 Thr:896 Vec:1
Speed.Dev.#4.....:   808.1 MH/s (90.72ms) @ Accel:16 Loops:64 Thr:896 Vec:1
Speed.Dev.#*.....:  3231.4 MH/s

Hashmode: 6211 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 2000)

Speed.Dev.#1.....:   577.9 kH/s (65.25ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#2.....:   577.9 kH/s (65.24ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#3.....:   576.7 kH/s (65.37ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#4.....:   576.8 kH/s (65.33ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#*.....:  2309.2 kH/s

Hashmode: 6212 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1024 bit (Iterations: 2000)

Speed.Dev.#1.....:   315.1 kH/s (50.70ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#2.....:   315.1 kH/s (50.69ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#3.....:   314.5 kH/s (50.76ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#4.....:   314.3 kH/s (50.80ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#*.....:  1259.0 kH/s

Hashmode: 6213 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1536 bit (Iterations: 2000)

Speed.Dev.#1.....:   247.6 kH/s (72.81ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#2.....:   247.6 kH/s (72.81ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#3.....:   247.1 kH/s (72.96ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#4.....:   247.0 kH/s (73.00ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#*.....:   989.2 kH/s

Hashmode: 6221 - TrueCrypt PBKDF2-HMAC-SHA512 + XTS 512 bit (Iterations: 1000)

Speed.Dev.#1.....:   899.3 kH/s (76.15ms) @ Accel:32 Loops:62 Thr:512 Vec:1
Speed.Dev.#2.....:   899.2 kH/s (76.15ms) @ Accel:32 Loops:62 Thr:512 Vec:1
Speed.Dev.#3.....:   897.2 kH/s (76.31ms) @ Accel:32 Loops:62 Thr:512 Vec:1
Speed.Dev.#4.....:   897.5 kH/s (76.29ms) @ Accel:32 Loops:62 Thr:512 Vec:1
Speed.Dev.#*.....:  3593.1 kH/s

Hashmode: 6222 - TrueCrypt PBKDF2-HMAC-SHA512 + XTS 1024 bit (Iterations: 1000)

Speed.Dev.#1.....:   419.6 kH/s (59.96ms) @ Accel:32 Loops:31 Thr:384 Vec:1
Speed.Dev.#2.....:   419.6 kH/s (59.95ms) @ Accel:32 Loops:31 Thr:384 Vec:1
Speed.Dev.#3.....:   418.5 kH/s (60.07ms) @ Accel:32 Loops:31 Thr:384 Vec:1
Speed.Dev.#4.....:   418.6 kH/s (60.06ms) @ Accel:32 Loops:31 Thr:384 Vec:1
Speed.Dev.#*.....:  1676.4 kH/s

Hashmode: 6223 - TrueCrypt PBKDF2-HMAC-SHA512 + XTS 1536 bit (Iterations: 1000)

Speed.Dev.#1.....:   274.7 kH/s (90.12ms) @ Accel:32 Loops:31 Thr:384 Vec:1
Speed.Dev.#2.....:   274.6 kH/s (90.11ms) @ Accel:32 Loops:31 Thr:384 Vec:1
Speed.Dev.#3.....:   273.9 kH/s (90.33ms) @ Accel:32 Loops:31 Thr:384 Vec:1
Speed.Dev.#4.....:   274.0 kH/s (90.30ms) @ Accel:32 Loops:31 Thr:384 Vec:1
Speed.Dev.#*.....:  1097.2 kH/s

Hashmode: 6231 - TrueCrypt PBKDF2-HMAC-Whirlpool + XTS 512 bit (Iterations: 1000)

Speed.Dev.#1.....:   119.6 kH/s (162.73ms) @ Accel:32 Loops:15 Thr:512 Vec:1
Speed.Dev.#2.....:   119.6 kH/s (162.68ms) @ Accel:32 Loops:15 Thr:512 Vec:1
Speed.Dev.#3.....:   119.4 kH/s (163.03ms) @ Accel:32 Loops:15 Thr:512 Vec:1
Speed.Dev.#4.....:   119.4 kH/s (162.95ms) @ Accel:32 Loops:15 Thr:512 Vec:1
Speed.Dev.#*.....:   477.9 kH/s

Hashmode: 6232 - TrueCrypt PBKDF2-HMAC-Whirlpool + XTS 1024 bit (Iterations: 1000)

Speed.Dev.#1.....:    59439 H/s (123.45ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.Dev.#2.....:    59451 H/s (123.42ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.Dev.#3.....:    59374 H/s (123.58ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.Dev.#4.....:    59210 H/s (123.92ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.Dev.#*.....:   237.5 kH/s

Hashmode: 6233 - TrueCrypt PBKDF2-HMAC-Whirlpool + XTS 1536 bit (Iterations: 1000)

Speed.Dev.#1.....:    39586 H/s (185.23ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.Dev.#2.....:    39591 H/s (185.20ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.Dev.#3.....:    39580 H/s (185.25ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.Dev.#4.....:    39585 H/s (185.23ms) @ Accel:16 Loops:15 Thr:384 Vec:1
Speed.Dev.#*.....:   158.3 kH/s

Hashmode: 6241 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 1000)

Speed.Dev.#1.....:  1069.8 kH/s (61.50ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.Dev.#2.....:  1069.6 kH/s (61.46ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.Dev.#3.....:  1067.1 kH/s (61.58ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.Dev.#4.....:  1069.8 kH/s (61.45ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.Dev.#*.....:  4276.3 kH/s

Hashmode: 6242 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 1000)

Speed.Dev.#1.....:   561.1 kH/s (48.45ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.Dev.#2.....:   561.1 kH/s (48.42ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.Dev.#3.....:   559.7 kH/s (48.51ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.Dev.#4.....:   559.9 kH/s (48.51ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.Dev.#*.....:  2241.9 kH/s

Hashmode: 6243 - TrueCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 1000)

Speed.Dev.#1.....:   380.5 kH/s (69.05ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.Dev.#2.....:   380.5 kH/s (69.02ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.Dev.#3.....:   379.6 kH/s (69.14ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.Dev.#4.....:   379.4 kH/s (69.16ms) @ Accel:16 Loops:31 Thr:896 Vec:1
Speed.Dev.#*.....:  1520.0 kH/s

Hashmode: 6300 - AIX {smd5} (Iterations: 1000)

Speed.Dev.#1.....: 24763.0 kH/s (51.26ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#2.....: 24718.2 kH/s (51.27ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#3.....: 24678.5 kH/s (51.35ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#4.....: 24705.9 kH/s (51.33ms) @ Accel:512 Loops:1000 Thr:32 Vec:1
Speed.Dev.#*.....: 98865.6 kH/s

Hashmode: 6400 - AIX {ssha256} (Iterations: 64)

Speed.Dev.#1.....: 40475.6 kH/s (25.15ms) @ Accel:16 Loops:64 Thr:896 Vec:1
Speed.Dev.#2.....: 40497.1 kH/s (25.13ms) @ Accel:16 Loops:64 Thr:896 Vec:1
Speed.Dev.#3.....: 40370.3 kH/s (25.20ms) @ Accel:16 Loops:64 Thr:896 Vec:1
Speed.Dev.#4.....: 40387.7 kH/s (25.20ms) @ Accel:16 Loops:64 Thr:896 Vec:1
Speed.Dev.#*.....:   161.7 MH/s

Hashmode: 6500 - AIX {ssha512} (Iterations: 64)

Speed.Dev.#1.....: 14555.5 kH/s (82.95ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#2.....: 14551.4 kH/s (82.85ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#3.....: 14525.8 kH/s (82.97ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#4.....: 14535.1 kH/s (83.06ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#*.....: 58167.8 kH/s

Hashmode: 6600 - 1Password, agilekeychain (Iterations: 1000)

Speed.Dev.#1.....:  6578.0 kH/s (48.75ms) @ Accel:16 Loops:250 Thr:1024 Vec:1
Speed.Dev.#2.....:  6574.1 kH/s (48.76ms) @ Accel:16 Loops:250 Thr:1024 Vec:1
Speed.Dev.#3.....:  6550.4 kH/s (48.91ms) @ Accel:16 Loops:250 Thr:1024 Vec:1
Speed.Dev.#4.....:  6554.2 kH/s (48.90ms) @ Accel:16 Loops:250 Thr:1024 Vec:1
Speed.Dev.#*.....: 26256.8 kH/s

Hashmode: 6700 - AIX {ssha1} (Iterations: 64)

Speed.Dev.#1.....: 80424.9 kH/s (12.64ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#2.....: 80418.0 kH/s (12.64ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#3.....: 80137.2 kH/s (12.67ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#4.....: 80192.9 kH/s (12.64ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#*.....:   321.2 MH/s

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 500)

Speed.Dev.#1.....:  5783.9 kH/s (68.65ms) @ Accel:32 Loops:125 Thr:640 Vec:1
Speed.Dev.#2.....:  5785.7 kH/s (68.62ms) @ Accel:32 Loops:125 Thr:640 Vec:1
Speed.Dev.#3.....:  5773.3 kH/s (68.73ms) @ Accel:32 Loops:125 Thr:640 Vec:1
Speed.Dev.#4.....:  5768.5 kH/s (68.83ms) @ Accel:32 Loops:125 Thr:640 Vec:1
Speed.Dev.#*.....: 23111.3 kH/s

Hashmode: 6900 - GOST R 34.11-94

Speed.Dev.#1.....:   770.6 MH/s (67.94ms) @ Accel:32 Loops:32 Thr:640 Vec:1
Speed.Dev.#2.....:   772.5 MH/s (67.83ms) @ Accel:32 Loops:32 Thr:640 Vec:1
Speed.Dev.#3.....:   772.3 MH/s (67.81ms) @ Accel:32 Loops:32 Thr:640 Vec:1
Speed.Dev.#4.....:   770.1 MH/s (67.94ms) @ Accel:32 Loops:32 Thr:640 Vec:1
Speed.Dev.#*.....:  3085.5 MH/s

Hashmode: 7000 - FortiGate (FortiOS)

Speed.Dev.#1.....: 13945.6 MH/s (48.08ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 13945.0 MH/s (48.03ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 13893.0 MH/s (48.15ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 13908.1 MH/s (48.15ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 55691.7 MH/s

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 35000)

Speed.Dev.#1.....:    28682 H/s (82.78ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#2.....:    28711 H/s (82.76ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#3.....:    28661 H/s (82.90ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#4.....:    28638 H/s (82.98ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#*.....:   114.7 kH/s

Hashmode: 7200 - GRUB 2 (Iterations: 10000)

Speed.Dev.#1.....:   100.5 kH/s (82.79ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#2.....:   100.3 kH/s (82.77ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#3.....:   100.2 kH/s (82.92ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#4.....:   100.2 kH/s (82.99ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#*.....:   401.2 kH/s

Hashmode: 7300 - IPMI2 RAKP HMAC-SHA1

Speed.Dev.#1.....:  3199.5 MH/s (65.47ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:  3199.3 MH/s (65.46ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:  3190.0 MH/s (65.61ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:  3187.8 MH/s (65.68ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....: 12776.5 MH/s

Hashmode: 7400 - sha256crypt $5$, SHA256 (Unix) (Iterations: 5000)

Speed.Dev.#1.....:  1014.6 kH/s (63.92ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  1014.5 kH/s (63.93ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  1012.2 kH/s (64.06ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  1011.5 kH/s (64.11ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....:  4052.8 kH/s

Hashmode: 7500 - Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.Dev.#1.....:   996.2 MH/s (84.18ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#2.....:   997.6 MH/s (84.02ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#3.....:   996.6 MH/s (84.03ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#4.....:   992.1 MH/s (84.45ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#*.....:  3982.5 MH/s

Hashmode: 7700 - SAP CODVN B (BCODE)

Speed.Dev.#1.....:  4086.7 MH/s (82.11ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  4085.0 MH/s (82.12ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  4091.7 MH/s (82.14ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  4131.7 MH/s (81.13ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 16395.0 MH/s

Hashmode: 7800 - SAP CODVN F/G (PASSCODE)

Speed.Dev.#1.....:  2601.9 MH/s (80.49ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:  2603.1 MH/s (80.50ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:  2598.5 MH/s (80.57ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:  2601.5 MH/s (80.50ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....: 10405.0 MH/s

Hashmode: 7900 - Drupal7 (Iterations: 16384)

Speed.Dev.#1.....:   126.8 kH/s (80.16ms) @ Accel:32 Loops:128 Thr:512 Vec:1
Speed.Dev.#2.....:   126.8 kH/s (80.15ms) @ Accel:32 Loops:128 Thr:512 Vec:1
Speed.Dev.#3.....:   126.8 kH/s (80.16ms) @ Accel:32 Loops:128 Thr:512 Vec:1
Speed.Dev.#4.....:   126.9 kH/s (80.08ms) @ Accel:32 Loops:128 Thr:512 Vec:1
Speed.Dev.#*.....:   507.3 kH/s

Hashmode: 8000 - Sybase ASE

Speed.Dev.#1.....:   871.4 MH/s (60.08ms) @ Accel:32 Loops:32 Thr:640 Vec:2
Speed.Dev.#2.....:   872.5 MH/s (60.05ms) @ Accel:32 Loops:32 Thr:640 Vec:2
Speed.Dev.#3.....:   871.1 MH/s (60.06ms) @ Accel:32 Loops:32 Thr:640 Vec:2
Speed.Dev.#4.....:   869.3 MH/s (60.18ms) @ Accel:32 Loops:32 Thr:640 Vec:2
Speed.Dev.#*.....:  3484.3 MH/s

Hashmode: 8100 - Citrix NetScaler

Speed.Dev.#1.....: 14716.7 MH/s (91.11ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 14719.0 MH/s (91.11ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 14661.3 MH/s (91.31ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 14669.5 MH/s (91.37ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....: 58766.5 MH/s

Hashmode: 8200 - 1Password, cloudkeychain (Iterations: 40000)

Speed.Dev.#1.....:    26146 H/s (79.28ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#2.....:    26149 H/s (79.26ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#3.....:    26156 H/s (79.24ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#4.....:    26116 H/s (79.37ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#*.....:   104.6 kH/s

Hashmode: 8300 - DNSSEC (NSEC3)

Speed.Dev.#1.....:  6484.4 MH/s (45.24ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#2.....:  6484.0 MH/s (45.19ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#3.....:  6465.2 MH/s (45.24ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#4.....:  6464.7 MH/s (45.24ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#*.....: 25898.3 MH/s

Hashmode: 8400 - WBB3 (Woltlab Burning Board)

Speed.Dev.#1.....:  2540.6 MH/s (82.49ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:  2542.4 MH/s (82.43ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:  2535.0 MH/s (82.54ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:  2533.7 MH/s (82.66ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....: 10151.7 MH/s

Hashmode: 8500 - RACF

Speed.Dev.#1.....:  6371.5 MH/s (52.61ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  6368.3 MH/s (52.60ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  6353.8 MH/s (52.69ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  6352.7 MH/s (52.74ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 25446.4 MH/s

Hashmode: 8600 - Lotus Notes/Domino 5

Speed.Dev.#1.....:   719.0 MH/s (58.26ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.Dev.#2.....:   718.9 MH/s (58.26ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.Dev.#3.....:   715.9 MH/s (58.42ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.Dev.#4.....:   716.5 MH/s (58.43ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.Dev.#*.....:  2870.2 MH/s

Hashmode: 8700 - Lotus Notes/Domino 6

Speed.Dev.#1.....:   236.8 MH/s (88.48ms) @ Accel:16 Loops:16 Thr:1024 Vec:1
Speed.Dev.#2.....:   236.8 MH/s (88.50ms) @ Accel:16 Loops:16 Thr:1024 Vec:1
Speed.Dev.#3.....:   235.9 MH/s (88.72ms) @ Accel:16 Loops:16 Thr:1024 Vec:1
Speed.Dev.#4.....:   236.0 MH/s (88.73ms) @ Accel:16 Loops:16 Thr:1024 Vec:1
Speed.Dev.#*.....:   945.4 MH/s

Hashmode: 8800 - Android FDE <= 4.3 (Iterations: 2000)

Speed.Dev.#1.....:  1653.7 kH/s (49.04ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#2.....:  1653.7 kH/s (49.04ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#3.....:  1649.4 kH/s (49.16ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#4.....:  1649.3 kH/s (49.18ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#*.....:  6606.1 kH/s

Hashmode: 8900 - scrypt (Iterations: 1)

Speed.Dev.#1.....:  1149.6 kH/s (17.48ms) @ Accel:16 Loops:1 Thr:16 Vec:1
Speed.Dev.#2.....:  1153.7 kH/s (17.48ms) @ Accel:16 Loops:1 Thr:16 Vec:1
Speed.Dev.#3.....:  1149.3 kH/s (17.48ms) @ Accel:16 Loops:1 Thr:16 Vec:1
Speed.Dev.#4.....:  1150.6 kH/s (17.46ms) @ Accel:16 Loops:1 Thr:16 Vec:1
Speed.Dev.#*.....:  4603.3 kH/s

Hashmode: 9000 - Password Safe v2 (Iterations: 1000)

Speed.Dev.#1.....:  1149.4 kH/s (45.78ms) @ Accel:512 Loops:250 Thr:8 Vec:1
Speed.Dev.#2.....:  1150.0 kH/s (45.75ms) @ Accel:512 Loops:250 Thr:8 Vec:1
Speed.Dev.#3.....:  1149.3 kH/s (45.75ms) @ Accel:512 Loops:250 Thr:8 Vec:1
Speed.Dev.#4.....:  1150.1 kH/s (45.75ms) @ Accel:512 Loops:250 Thr:8 Vec:1
Speed.Dev.#*.....:  4598.8 kH/s

Hashmode: 9100 - Lotus Notes/Domino 8 (Iterations: 5000)

Speed.Dev.#1.....:  1334.1 kH/s (48.79ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  1334.0 kH/s (48.75ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  1328.8 kH/s (48.90ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  1330.0 kH/s (48.88ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....:  5326.9 kH/s

Hashmode: 9200 - Cisco-IOS $8$ (PBKDF2-SHA256) (Iterations: 20000)

Speed.Dev.#1.....:   147.8 kH/s (70.27ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:   148.1 kH/s (70.15ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:   148.1 kH/s (70.14ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:   147.6 kH/s (70.36ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:   591.6 kH/s

Hashmode: 9300 - Cisco-IOS $9$ (scrypt) (Iterations: 1)

Speed.Dev.#1.....:        0 H/s (0.00ms) @ Accel:32 Loops:128 Thr:8 Vec:1
Speed.Dev.#2.....:        0 H/s (0.00ms) @ Accel:32 Loops:128 Thr:8 Vec:1
Speed.Dev.#3.....:        0 H/s (0.00ms) @ Accel:32 Loops:128 Thr:8 Vec:1
Speed.Dev.#4.....:        0 H/s (0.00ms) @ Accel:32 Loops:128 Thr:8 Vec:1
Speed.Dev.#*.....:        0 H/s

Hashmode: 9400 - MS Office 2007 (Iterations: 50000)

Speed.Dev.#1.....:   269.0 kH/s (49.53ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:   269.7 kH/s (49.42ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:   269.0 kH/s (49.54ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:   268.8 kH/s (49.58ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....:  1076.5 kH/s

Hashmode: 9500 - MS Office 2010 (Iterations: 100000)

Speed.Dev.#1.....:   134.6 kH/s (49.50ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:   134.8 kH/s (49.41ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:   134.4 kH/s (49.56ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:   134.4 kH/s (49.58ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....:   538.3 kH/s

Hashmode: 9600 - MS Office 2013 (Iterations: 100000)

Speed.Dev.#1.....:    22367 H/s (74.45ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#2.....:    22394 H/s (74.37ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#3.....:    22339 H/s (74.54ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#4.....:    22340 H/s (74.55ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#*.....:    89440 H/s

Hashmode: 9700 - MS Office <= 2003 $0/$1, MD5 + RC4

Speed.Dev.#1.....:   843.8 MH/s (49.72ms) @ Accel:128 Loops:64 Thr:64 Vec:1
Speed.Dev.#2.....:   834.3 MH/s (50.16ms) @ Accel:128 Loops:64 Thr:64 Vec:1
Speed.Dev.#3.....:   838.8 MH/s (49.87ms) @ Accel:128 Loops:64 Thr:64 Vec:1
Speed.Dev.#4.....:   837.0 MH/s (49.98ms) @ Accel:128 Loops:64 Thr:64 Vec:1
Speed.Dev.#*.....:  3353.9 MH/s

Hashmode: 9710 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.Dev.#1.....:  1149.0 MH/s (67.96ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#2.....:  1148.2 MH/s (67.96ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#3.....:  1147.8 MH/s (68.02ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#4.....:  1147.3 MH/s (68.03ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#*.....:  4592.3 MH/s

Hashmode: 9720 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #2

Speed.Dev.#1.....:  4548.7 MH/s (73.68ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  4548.5 MH/s (73.68ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  4531.7 MH/s (73.93ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  4534.9 MH/s (73.89ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 18163.9 MH/s

Hashmode: 9800 - MS Office <= 2003 $3/$4, SHA1 + RC4

Speed.Dev.#1.....:  1058.9 MH/s (79.13ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#2.....:  1055.7 MH/s (79.34ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#3.....:  1066.3 MH/s (78.64ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#4.....:  1056.6 MH/s (79.34ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#*.....:  4237.5 MH/s

Hashmode: 9810 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.Dev.#1.....:  1138.9 MH/s (63.57ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#2.....:  1139.1 MH/s (63.59ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#3.....:  1135.6 MH/s (63.64ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#4.....:  1136.6 MH/s (63.66ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#*.....:  4550.3 MH/s

Hashmode: 9820 - MS Office <= 2003 $3, SHA1 + RC4, collider #2

Speed.Dev.#1.....:  6858.8 MH/s (48.83ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:  6857.9 MH/s (48.84ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:  6827.9 MH/s (49.01ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:  6832.9 MH/s (49.00ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....: 27377.4 MH/s

Hashmode: 9900 - Radmin2

Speed.Dev.#1.....: 19780.3 MH/s (67.80ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#2.....: 19777.4 MH/s (67.75ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#3.....: 19706.6 MH/s (67.99ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#4.....: 19745.5 MH/s (67.91ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#*.....: 79009.7 MH/s

Hashmode: 10000 - Django (PBKDF2-SHA256) (Iterations: 20000)

Speed.Dev.#1.....:   148.1 kH/s (70.15ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:   148.1 kH/s (70.15ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:   147.8 kH/s (70.28ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:   147.6 kH/s (70.35ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:   591.6 kH/s

Hashmode: 10100 - SipHash

Speed.Dev.#1.....: 60443.6 MH/s (22.11ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#2.....: 60436.9 MH/s (22.11ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#3.....: 60318.4 MH/s (22.16ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#4.....: 60316.2 MH/s (22.16ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#*.....:   241.5 GH/s

Hashmode: 10200 - CRAM-MD5

Speed.Dev.#1.....:  8894.2 MH/s (75.32ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:  8898.7 MH/s (75.32ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:  8865.0 MH/s (75.57ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:  8869.3 MH/s (75.58ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 35527.2 MH/s

Hashmode: 10300 - SAP CODVN H (PWDSALTEDHASH) iSSHA-1 (Iterations: 1023)

Speed.Dev.#1.....: 11633.3 kH/s (55.36ms) @ Accel:32 Loops:511 Thr:768 Vec:1
Speed.Dev.#2.....: 11636.1 kH/s (55.36ms) @ Accel:32 Loops:511 Thr:768 Vec:1
Speed.Dev.#3.....: 11602.6 kH/s (55.51ms) @ Accel:32 Loops:511 Thr:768 Vec:1
Speed.Dev.#4.....: 11603.2 kH/s (55.54ms) @ Accel:32 Loops:511 Thr:768 Vec:1
Speed.Dev.#*.....: 46475.2 kH/s

Hashmode: 10400 - PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.Dev.#1.....:  1281.5 MH/s (65.37ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#2.....:  1280.7 MH/s (65.41ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#3.....:  1279.5 MH/s (65.44ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#4.....:  1278.2 MH/s (65.51ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#*.....:  5119.9 MH/s

Hashmode: 10410 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.Dev.#1.....:  1240.7 MH/s (59.16ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#2.....:  1240.4 MH/s (59.17ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#3.....:  1237.6 MH/s (59.26ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#4.....:  1238.5 MH/s (59.24ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#*.....:  4957.3 MH/s

Hashmode: 10420 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #2

Speed.Dev.#1.....: 17090.5 MH/s (78.44ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 17090.4 MH/s (78.48ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 17037.2 MH/s (78.66ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 17038.5 MH/s (78.67ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....: 68256.5 MH/s

Hashmode: 10500 - PDF 1.4 - 1.6 (Acrobat 5 - 8) (Iterations: 70)

Speed.Dev.#1.....: 55722.9 kH/s (21.63ms) @ Accel:256 Loops:70 Thr:64 Vec:1
Speed.Dev.#2.....: 55643.8 kH/s (21.64ms) @ Accel:256 Loops:70 Thr:64 Vec:1
Speed.Dev.#3.....: 55618.3 kH/s (21.67ms) @ Accel:256 Loops:70 Thr:64 Vec:1
Speed.Dev.#4.....: 55584.0 kH/s (21.67ms) @ Accel:256 Loops:70 Thr:64 Vec:1
Speed.Dev.#*.....:   222.6 MH/s

Hashmode: 10600 - PDF 1.7 Level 3 (Acrobat 9)

Speed.Dev.#1.....:  7601.8 MH/s (88.20ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:  7600.9 MH/s (88.21ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:  7569.8 MH/s (88.50ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:  7576.4 MH/s (88.49ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 30348.9 MH/s

Hashmode: 10700 - PDF 1.7 Level 8 (Acrobat 10 - 11) (Iterations: 64)

Speed.Dev.#1.....:    80915 H/s (126.31ms) @ Accel:8 Loops:2 Thr:512 Vec:1
Speed.Dev.#2.....:    81112 H/s (126.01ms) @ Accel:8 Loops:2 Thr:512 Vec:1
Speed.Dev.#3.....:    81285 H/s (125.74ms) @ Accel:8 Loops:2 Thr:512 Vec:1
Speed.Dev.#4.....:    80947 H/s (126.27ms) @ Accel:8 Loops:2 Thr:512 Vec:1
Speed.Dev.#*.....:   324.3 kH/s

Hashmode: 10800 - SHA-384

Speed.Dev.#1.....:  2382.9 MH/s (87.94ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:  2382.6 MH/s (87.94ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:  2376.8 MH/s (88.08ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:  2374.4 MH/s (88.17ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:  9516.8 MH/s

Hashmode: 10900 - PBKDF2-HMAC-SHA256 (Iterations: 999)

Speed.Dev.#1.....:  2952.1 kH/s (60.96ms) @ Accel:32 Loops:124 Thr:640 Vec:1
Speed.Dev.#2.....:  2951.9 kH/s (60.97ms) @ Accel:32 Loops:124 Thr:640 Vec:1
Speed.Dev.#3.....:  2945.6 kH/s (61.08ms) @ Accel:32 Loops:124 Thr:640 Vec:1
Speed.Dev.#4.....:  2941.7 kH/s (61.18ms) @ Accel:32 Loops:124 Thr:640 Vec:1
Speed.Dev.#*.....: 11791.3 kH/s

Hashmode: 11000 - PrestaShop

Speed.Dev.#1.....: 19212.8 MH/s (69.77ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#2.....: 19211.7 MH/s (69.78ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#3.....: 19149.6 MH/s (69.96ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#4.....: 19139.2 MH/s (70.04ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#*.....: 76713.3 MH/s

Hashmode: 11100 - PostgreSQL CRAM (MD5)

Speed.Dev.#1.....: 15479.2 MH/s (86.61ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#2.....: 15478.3 MH/s (86.62ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#3.....: 15433.4 MH/s (86.90ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#4.....: 15435.1 MH/s (86.88ms) @ Accel:16 Loops:1024 Thr:1024 Vec:2
Speed.Dev.#*.....: 61825.9 MH/s

Hashmode: 11200 - MySQL CRAM (SHA1)

Speed.Dev.#1.....:  4512.2 MH/s (64.98ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#2.....:  4512.5 MH/s (64.98ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#3.....:  4499.8 MH/s (65.11ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#4.....:  4496.9 MH/s (65.22ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#*.....: 18021.4 MH/s

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 199999)

Speed.Dev.#1.....:    11238 H/s (74.08ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#2.....:    11242 H/s (74.06ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#3.....:    11198 H/s (74.35ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#4.....:    11246 H/s (74.04ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#*.....:    44924 H/s

Hashmode: 11400 - SIP digest authentication (MD5)

Speed.Dev.#1.....:  7938.5 MH/s (52.74ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#2.....:  7939.5 MH/s (52.75ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#3.....:  7929.3 MH/s (52.82ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#4.....:  7931.8 MH/s (52.82ms) @ Accel:32 Loops:256 Thr:640 Vec:1
Speed.Dev.#*.....: 31739.0 MH/s

Hashmode: 11500 - CRC32

Speed.Dev.#1.....: 12280.8 MH/s (54.49ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....: 12284.2 MH/s (54.50ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....: 12280.6 MH/s (54.55ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....: 12314.5 MH/s (54.43ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 49160.1 MH/s

Hashmode: 11600 - 7-Zip (Iterations: 524288)

Speed.Dev.#1.....:    21309 H/s (44.49ms) @ Accel:32 Loops:256 Thr:768 Vec:1
Speed.Dev.#2.....:    21299 H/s (44.50ms) @ Accel:32 Loops:256 Thr:768 Vec:1
Speed.Dev.#3.....:    21264 H/s (44.58ms) @ Accel:32 Loops:256 Thr:768 Vec:1
Speed.Dev.#4.....:    21302 H/s (44.51ms) @ Accel:32 Loops:256 Thr:768 Vec:1
Speed.Dev.#*.....:    85175 H/s

Hashmode: 11700 - GOST R 34.11-2012 (Streebog) 256-bit

Speed.Dev.#1.....:   166.8 MH/s (62.77ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.Dev.#2.....:   166.7 MH/s (62.80ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.Dev.#3.....:   166.8 MH/s (62.76ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.Dev.#4.....:   166.2 MH/s (62.99ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.Dev.#*.....:   666.6 MH/s

Hashmode: 11800 - GOST R 34.11-2012 (Streebog) 512-bit

Speed.Dev.#1.....:   166.7 MH/s (62.77ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.Dev.#2.....:   166.7 MH/s (62.79ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.Dev.#3.....:   166.8 MH/s (62.75ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.Dev.#4.....:   166.2 MH/s (62.99ms) @ Accel:32 Loops:8 Thr:512 Vec:1
Speed.Dev.#*.....:   666.4 MH/s

Hashmode: 11900 - PBKDF2-HMAC-MD5 (Iterations: 999)

Speed.Dev.#1.....: 16945.0 kH/s (14.28ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.Dev.#2.....: 16935.2 kH/s (14.28ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.Dev.#3.....: 16933.9 kH/s (14.28ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.Dev.#4.....: 16924.9 kH/s (14.29ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.Dev.#*.....: 67739.0 kH/s

Hashmode: 12000 - PBKDF2-HMAC-SHA1 (Iterations: 999)

Speed.Dev.#1.....:  6410.4 kH/s (39.67ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.Dev.#2.....:  6411.1 kH/s (39.68ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.Dev.#3.....:  6410.3 kH/s (39.72ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.Dev.#4.....:  6401.8 kH/s (39.71ms) @ Accel:16 Loops:249 Thr:1024 Vec:1
Speed.Dev.#*.....: 25633.6 kH/s

Hashmode: 12001 - Atlassian (PBKDF2-HMAC-SHA1) (Iterations: 9999)

Speed.Dev.#1.....:   664.4 kH/s (49.13ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:   664.4 kH/s (49.13ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:   664.5 kH/s (49.13ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:   664.1 kH/s (49.16ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....:  2657.5 kH/s

Hashmode: 12100 - PBKDF2-HMAC-SHA512 (Iterations: 999)

Speed.Dev.#1.....:  1006.9 kH/s (76.06ms) @ Accel:32 Loops:62 Thr:512 Vec:1
Speed.Dev.#2.....:  1006.7 kH/s (76.03ms) @ Accel:32 Loops:62 Thr:512 Vec:1
Speed.Dev.#3.....:  1004.8 kH/s (76.22ms) @ Accel:32 Loops:62 Thr:512 Vec:1
Speed.Dev.#4.....:  1004.2 kH/s (76.21ms) @ Accel:32 Loops:62 Thr:512 Vec:1
Speed.Dev.#*.....:  4022.7 kH/s

Hashmode: 12200 - eCryptfs (Iterations: 65535)

Speed.Dev.#1.....:    34326 H/s (74.03ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#2.....:    34318 H/s (74.04ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#3.....:    34181 H/s (74.35ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#4.....:    34230 H/s (74.23ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#*.....:   137.1 kH/s

Hashmode: 12300 - Oracle T: Type (Oracle 12+) (Iterations: 4095)

Speed.Dev.#1.....:   254.5 kH/s (79.55ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#2.....:   255.5 kH/s (79.25ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#3.....:   254.9 kH/s (79.44ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#4.....:   255.2 kH/s (79.33ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#*.....:  1020.1 kH/s

Hashmode: 12400 - BSDi Crypt, Extended DES (Iterations: 2899)

Speed.Dev.#1.....:  4089.2 kH/s (13.44ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#2.....:  4086.3 kH/s (13.43ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#3.....:  4087.2 kH/s (13.46ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#4.....:  4081.4 kH/s (13.47ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#*.....: 16344.0 kH/s

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.Dev.#1.....:    84818 H/s (45.20ms) @ Accel:2 Loops:16384 Thr:384 Vec:1
Speed.Dev.#2.....:    84750 H/s (45.23ms) @ Accel:2 Loops:16384 Thr:384 Vec:1
Speed.Dev.#3.....:    84788 H/s (45.21ms) @ Accel:2 Loops:16384 Thr:384 Vec:1
Speed.Dev.#4.....:    84785 H/s (45.21ms) @ Accel:2 Loops:16384 Thr:384 Vec:1
Speed.Dev.#*.....:   339.1 kH/s

Hashmode: 12600 - ColdFusion 10+

Speed.Dev.#1.....:  4266.6 MH/s (68.69ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#2.....:  4266.4 MH/s (68.70ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#3.....:  4257.7 MH/s (68.87ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#4.....:  4254.5 MH/s (68.90ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#*.....: 17045.3 MH/s

Hashmode: 12700 - Blockchain, My Wallet (Iterations: 10)

Speed.Dev.#1.....:   126.4 MH/s (4.28ms) @ Accel:16 Loops:10 Thr:1024 Vec:1
Speed.Dev.#2.....:   126.2 MH/s (4.28ms) @ Accel:16 Loops:10 Thr:1024 Vec:1
Speed.Dev.#3.....:   126.8 MH/s (4.28ms) @ Accel:16 Loops:10 Thr:1024 Vec:1
Speed.Dev.#4.....:   126.9 MH/s (4.29ms) @ Accel:16 Loops:10 Thr:1024 Vec:1
Speed.Dev.#*.....:   506.2 MH/s

Hashmode: 12800 - MS-AzureSync PBKDF2-HMAC-SHA256 (Iterations: 99)

Speed.Dev.#1.....: 26093.7 kH/s (54.36ms) @ Accel:32 Loops:99 Thr:640 Vec:1
Speed.Dev.#2.....: 26086.2 kH/s (54.38ms) @ Accel:32 Loops:99 Thr:640 Vec:1
Speed.Dev.#3.....: 26008.0 kH/s (54.52ms) @ Accel:32 Loops:99 Thr:640 Vec:1
Speed.Dev.#4.....: 26016.0 kH/s (54.61ms) @ Accel:32 Loops:99 Thr:640 Vec:1
Speed.Dev.#*.....:   104.2 MH/s

Hashmode: 12900 - Android FDE (Samsung DEK) (Iterations: 4095)

Speed.Dev.#1.....:   727.6 kH/s (70.13ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:   727.6 kH/s (70.13ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:   725.8 kH/s (70.30ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:   725.2 kH/s (70.35ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:  2906.1 kH/s

Hashmode: 13000 - RAR5 (Iterations: 32767)

Speed.Dev.#1.....:    90370 H/s (70.15ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:    90367 H/s (70.16ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:    90140 H/s (70.34ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:    90089 H/s (70.38ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:   361.0 kH/s

Hashmode: 13100 - Kerberos 5 TGS-REP etype 23

Speed.Dev.#1.....:   997.1 MH/s (84.07ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#2.....:   997.5 MH/s (84.00ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#3.....:   999.9 MH/s (83.80ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#4.....:   999.4 MH/s (83.89ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.Dev.#*.....:  3994.0 MH/s

Hashmode: 13200 - AxCrypt (Iterations: 10000)

Speed.Dev.#1.....:   358.6 kH/s (91.39ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:   358.6 kH/s (91.33ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:   357.7 kH/s (91.56ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:   357.8 kH/s (91.55ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....:  1432.6 kH/s

Hashmode: 13300 - AxCrypt in-memory SHA1

Speed.Dev.#1.....: 15862.3 MH/s (52.79ms) @ Accel:32 Loops:512 Thr:640 Vec:1
Speed.Dev.#2.....: 15864.1 MH/s (52.80ms) @ Accel:32 Loops:512 Thr:640 Vec:1
Speed.Dev.#3.....: 15810.2 MH/s (52.96ms) @ Accel:32 Loops:512 Thr:640 Vec:1
Speed.Dev.#4.....: 15810.1 MH/s (52.92ms) @ Accel:32 Loops:512 Thr:640 Vec:1
Speed.Dev.#*.....: 63346.7 MH/s

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 6000)

Speed.Dev.#1.....:   335.6 kH/s (82.91ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.Dev.#2.....:   335.5 kH/s (82.91ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.Dev.#3.....:   335.3 kH/s (82.96ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.Dev.#4.....:   335.6 kH/s (82.92ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.Dev.#*.....:  1341.9 kH/s

Hashmode: 13500 - PeopleSoft PS_TOKEN

Speed.Dev.#1.....:  6302.4 MH/s (79.77ms) @ Accel:32 Loops:256 Thr:768 Vec:1
Speed.Dev.#2.....:  6300.8 MH/s (79.79ms) @ Accel:32 Loops:256 Thr:768 Vec:1
Speed.Dev.#3.....:  6284.0 MH/s (79.99ms) @ Accel:32 Loops:256 Thr:768 Vec:1
Speed.Dev.#4.....:  6277.3 MH/s (80.08ms) @ Accel:32 Loops:256 Thr:768 Vec:1
Speed.Dev.#*.....: 25164.4 MH/s

Hashmode: 13600 - WinZip (Iterations: 1000)

Speed.Dev.#1.....:  2168.1 kH/s (34.69ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.Dev.#2.....:  2167.2 kH/s (34.69ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.Dev.#3.....:  2163.2 kH/s (34.76ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.Dev.#4.....:  2162.0 kH/s (34.78ms) @ Accel:16 Loops:62 Thr:1024 Vec:1
Speed.Dev.#*.....:  8660.5 kH/s

Hashmode: 13711 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit (Iterations: 655331)

Speed.Dev.#1.....:     1890 H/s (66.80ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#2.....:     1891 H/s (66.78ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#3.....:     1888 H/s (66.89ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#4.....:     1886 H/s (66.95ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#*.....:     7555 H/s

Hashmode: 13712 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1024 bit (Iterations: 655331)

Speed.Dev.#1.....:     1079 H/s (51.13ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#2.....:     1080 H/s (51.08ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#3.....:     1079 H/s (51.17ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#4.....:     1077 H/s (51.21ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#*.....:     4316 H/s

Hashmode: 13713 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1536 bit (Iterations: 655331)

Speed.Dev.#1.....:      755 H/s (72.82ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#2.....:      756 H/s (72.80ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#3.....:      754 H/s (72.93ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#4.....:      753 H/s (73.02ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#*.....:     3019 H/s

Hashmode: 13721 - VeraCrypt PBKDF2-HMAC-SHA512 + XTS 512 bit (Iterations: 500000)

Speed.Dev.#1.....:     2007 H/s (82.81ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#2.....:     2008 H/s (82.77ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#3.....:     2008 H/s (82.79ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#4.....:     2003 H/s (82.99ms) @ Accel:32 Loops:64 Thr:512 Vec:1
Speed.Dev.#*.....:     8027 H/s

Hashmode: 13722 - VeraCrypt PBKDF2-HMAC-SHA512 + XTS 1024 bit (Iterations: 500000)

Speed.Dev.#1.....:      970 H/s (63.82ms) @ Accel:64 Loops:16 Thr:384 Vec:1
Speed.Dev.#2.....:      974 H/s (63.63ms) @ Accel:64 Loops:16 Thr:384 Vec:1
Speed.Dev.#3.....:      972 H/s (63.76ms) @ Accel:64 Loops:16 Thr:384 Vec:1
Speed.Dev.#4.....:      972 H/s (63.75ms) @ Accel:64 Loops:16 Thr:384 Vec:1
Speed.Dev.#*.....:     3887 H/s

Hashmode: 13723 - VeraCrypt PBKDF2-HMAC-SHA512 + XTS 1536 bit (Iterations: 500000)

Speed.Dev.#1.....:      644 H/s (96.07ms) @ Accel:64 Loops:16 Thr:384 Vec:1
Speed.Dev.#2.....:      646 H/s (95.76ms) @ Accel:64 Loops:16 Thr:384 Vec:1
Speed.Dev.#3.....:      645 H/s (95.92ms) @ Accel:64 Loops:16 Thr:384 Vec:1
Speed.Dev.#4.....:      645 H/s (95.88ms) @ Accel:64 Loops:16 Thr:384 Vec:1
Speed.Dev.#*.....:     2580 H/s

Hashmode: 13731 - VeraCrypt PBKDF2-HMAC-Whirlpool + XTS 512 bit (Iterations: 500000)

Speed.Dev.#1.....:      239 H/s (173.55ms) @ Accel:32 Loops:16 Thr:512 Vec:1
Speed.Dev.#2.....:      239 H/s (173.52ms) @ Accel:32 Loops:16 Thr:512 Vec:1
Speed.Dev.#3.....:      239 H/s (173.74ms) @ Accel:32 Loops:16 Thr:512 Vec:1
Speed.Dev.#4.....:      239 H/s (173.49ms) @ Accel:32 Loops:16 Thr:512 Vec:1
Speed.Dev.#*.....:      956 H/s

Hashmode: 13732 - VeraCrypt PBKDF2-HMAC-Whirlpool + XTS 1024 bit (Iterations: 500000)

Speed.Dev.#1.....:      118 H/s (131.75ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.Dev.#2.....:      118 H/s (131.71ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.Dev.#3.....:      118 H/s (131.91ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.Dev.#4.....:      118 H/s (131.73ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.Dev.#*.....:      472 H/s

Hashmode: 13733 - VeraCrypt PBKDF2-HMAC-Whirlpool + XTS 1536 bit (Iterations: 500000)

Speed.Dev.#1.....:       78 H/s (198.44ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.Dev.#2.....:       78 H/s (198.40ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.Dev.#3.....:       78 H/s (198.50ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.Dev.#4.....:       78 H/s (199.22ms) @ Accel:32 Loops:8 Thr:384 Vec:1
Speed.Dev.#*.....:      313 H/s

Hashmode: 13741 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 327661)

Speed.Dev.#1.....:     3778 H/s (66.84ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#2.....:     3782 H/s (66.78ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#3.....:     3773 H/s (66.93ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#4.....:     3772 H/s (66.94ms) @ Accel:16 Loops:64 Thr:1024 Vec:1
Speed.Dev.#*.....:    15105 H/s

Hashmode: 13742 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 327661)

Speed.Dev.#1.....:     2160 H/s (51.09ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#2.....:     2157 H/s (51.17ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#3.....:     2155 H/s (51.20ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#4.....:     2155 H/s (51.21ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#*.....:     8628 H/s

Hashmode: 13743 - VeraCrypt PBKDF2-HMAC-RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 327661)

Speed.Dev.#1.....:     1511 H/s (72.82ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#2.....:     1511 H/s (72.81ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#3.....:     1507 H/s (72.99ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#4.....:     1507 H/s (73.03ms) @ Accel:16 Loops:32 Thr:896 Vec:1
Speed.Dev.#*.....:     6036 H/s

Hashmode: 13751 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 512 bit (Iterations: 500000)

Speed.Dev.#1.....:     2759 H/s (89.93ms) @ Accel:32 Loops:64 Thr:768 Vec:1
Speed.Dev.#2.....:     2759 H/s (89.93ms) @ Accel:32 Loops:64 Thr:768 Vec:1
Speed.Dev.#3.....:     2753 H/s (90.15ms) @ Accel:32 Loops:64 Thr:768 Vec:1
Speed.Dev.#4.....:     2757 H/s (89.93ms) @ Accel:32 Loops:64 Thr:768 Vec:1
Speed.Dev.#*.....:    11028 H/s

Hashmode: 13752 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 1024 bit (Iterations: 500000)

Speed.Dev.#1.....:     1364 H/s (90.43ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#2.....:     1369 H/s (90.09ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#3.....:     1366 H/s (90.29ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#4.....:     1366 H/s (90.35ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#*.....:     5465 H/s

Hashmode: 13753 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 1536 bit (Iterations: 500000)

Speed.Dev.#1.....:      899 H/s (68.27ms) @ Accel:32 Loops:16 Thr:768 Vec:1
Speed.Dev.#2.....:      902 H/s (68.04ms) @ Accel:32 Loops:16 Thr:768 Vec:1
Speed.Dev.#3.....:      900 H/s (68.15ms) @ Accel:32 Loops:16 Thr:768 Vec:1
Speed.Dev.#4.....:      900 H/s (68.20ms) @ Accel:32 Loops:16 Thr:768 Vec:1
Speed.Dev.#*.....:     3600 H/s

Hashmode: 13761 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 512 bit + boot-mode (Iterations: 200000)

Speed.Dev.#1.....:     6799 H/s (45.59ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#2.....:     6813 H/s (45.50ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#3.....:     6806 H/s (45.55ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#4.....:     6804 H/s (45.55ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#*.....:    27222 H/s

Hashmode: 13762 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 1024 bit + boot-mode (Iterations: 200000)

Speed.Dev.#1.....:     3412 H/s (90.42ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#2.....:     3423 H/s (90.09ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#3.....:     3416 H/s (90.30ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#4.....:     3414 H/s (90.34ms) @ Accel:32 Loops:32 Thr:768 Vec:1
Speed.Dev.#*.....:    13665 H/s

Hashmode: 13763 - VeraCrypt PBKDF2-HMAC-SHA256 + XTS 1536 bit + boot-mode (Iterations: 200000)

Speed.Dev.#1.....:     2253 H/s (68.06ms) @ Accel:32 Loops:16 Thr:768 Vec:1
Speed.Dev.#2.....:     2253 H/s (68.04ms) @ Accel:32 Loops:16 Thr:768 Vec:1
Speed.Dev.#3.....:     2249 H/s (68.19ms) @ Accel:32 Loops:16 Thr:768 Vec:1
Speed.Dev.#4.....:     2249 H/s (68.20ms) @ Accel:32 Loops:16 Thr:768 Vec:1
Speed.Dev.#*.....:     9004 H/s

Hashmode: 13800 - Windows Phone 8+ PIN/password

Speed.Dev.#1.....:  1760.7 MH/s (71.39ms) @ Accel:32 Loops:64 Thr:768 Vec:1
Speed.Dev.#2.....:  1760.5 MH/s (71.35ms) @ Accel:32 Loops:64 Thr:768 Vec:1
Speed.Dev.#3.....:  1754.2 MH/s (71.53ms) @ Accel:32 Loops:64 Thr:768 Vec:1
Speed.Dev.#4.....:  1756.1 MH/s (71.57ms) @ Accel:32 Loops:64 Thr:768 Vec:1
Speed.Dev.#*.....:  7031.5 MH/s

Hashmode: 13900 - OpenCart

Speed.Dev.#1.....:  4161.0 MH/s (70.50ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#2.....:  4160.8 MH/s (70.47ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#3.....:  4149.3 MH/s (70.65ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#4.....:  4148.4 MH/s (70.68ms) @ Accel:16 Loops:256 Thr:896 Vec:1
Speed.Dev.#*.....: 16619.6 MH/s

Hashmode: 14000 - DES (PT = $salt, key = $pass)

Speed.Dev.#1.....: 46519.7 MH/s (28.68ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.Dev.#2.....: 46524.3 MH/s (28.68ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.Dev.#3.....: 46442.1 MH/s (28.73ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.Dev.#4.....: 46462.3 MH/s (28.72ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.Dev.#*.....:   185.9 GH/s

Hashmode: 14100 - 3DES (PT = $salt, key = $pass)

Speed.Dev.#1.....:  2899.2 MH/s (57.76ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.Dev.#2.....:  2900.4 MH/s (57.75ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.Dev.#3.....:  2892.0 MH/s (57.89ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.Dev.#4.....:  2892.6 MH/s (57.89ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.Dev.#*.....: 11584.2 MH/s

Hashmode: 14400 - sha1(CX)

Speed.Dev.#1.....:   696.0 MH/s (90.32ms) @ Accel:64 Loops:32 Thr:384 Vec:1
Speed.Dev.#2.....:   696.3 MH/s (90.33ms) @ Accel:64 Loops:32 Thr:384 Vec:1
Speed.Dev.#3.....:   694.4 MH/s (90.48ms) @ Accel:64 Loops:32 Thr:384 Vec:1
Speed.Dev.#4.....:   695.3 MH/s (90.40ms) @ Accel:64 Loops:32 Thr:384 Vec:1
Speed.Dev.#*.....:  2782.0 MH/s

Hashmode: 14600 - LUKS (Iterations: 163044)

Speed.Dev.#1.....:    20451 H/s (50.51ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....:    20455 H/s (50.56ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....:    20408 H/s (50.59ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....:    20404 H/s (50.68ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....:    81718 H/s

Hashmode: 14700 - iTunes backup < 10.0 (Iterations: 9999)

Speed.Dev.#1.....:   331.8 kH/s (49.67ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#2.....:   331.8 kH/s (49.67ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#3.....:   331.0 kH/s (49.80ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#4.....:   330.9 kH/s (49.80ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#*.....:  1325.5 kH/s

Hashmode: 14800 - iTunes backup >= 10.0 (Iterations: 9999999)

Speed.Dev.#1.....:      297 H/s (8.57ms) @ Accel:2 Loops:250 Thr:640 Vec:1
Speed.Dev.#2.....:      297 H/s (8.57ms) @ Accel:2 Loops:250 Thr:640 Vec:1
Speed.Dev.#3.....:      296 H/s (8.59ms) @ Accel:2 Loops:250 Thr:640 Vec:1
Speed.Dev.#4.....:      296 H/s (8.59ms) @ Accel:2 Loops:250 Thr:640 Vec:1
Speed.Dev.#*.....:     1187 H/s

Hashmode: 14900 - Skip32 (PT = $salt, key = $pass)

Speed.Dev.#1.....: 15995.0 MH/s (4.10ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....:        0 H/s (0.00ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....:        0 H/s (0.00ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....:        0 H/s (0.00ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....: 15995.0 MH/s

Hashmode: 15000 - FileZilla Server >= 0.9.55

Speed.Dev.#1.....:  2209.5 MH/s (56.86ms) @ Accel:64 Loops:64 Thr:384 Vec:1
Speed.Dev.#2.....:  2208.1 MH/s (56.85ms) @ Accel:64 Loops:64 Thr:384 Vec:1
Speed.Dev.#3.....:  2205.0 MH/s (56.96ms) @ Accel:64 Loops:64 Thr:384 Vec:1
Speed.Dev.#4.....:  2207.1 MH/s (56.92ms) @ Accel:64 Loops:64 Thr:384 Vec:1
Speed.Dev.#*.....:  8829.7 MH/s

Hashmode: 15100 - Juniper/NetBSD sha1crypt (Iterations: 19999)

Speed.Dev.#1.....:   340.0 kH/s (48.61ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#2.....:   339.9 kH/s (48.61ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#3.....:   338.7 kH/s (48.79ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#4.....:   338.8 kH/s (48.78ms) @ Accel:16 Loops:256 Thr:1024 Vec:1
Speed.Dev.#*.....:  1357.4 kH/s

Hashmode: 15200 - Blockchain, My Wallet, V2 (Iterations: 5000)

Speed.Dev.#1.....:   665.7 kH/s (49.05ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#2.....:   665.8 kH/s (49.04ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#3.....:   664.0 kH/s (49.17ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#4.....:   663.6 kH/s (49.19ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#*.....:  2659.1 kH/s

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.Dev.#1.....:   138.0 kH/s (50.25ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#2.....:   138.0 kH/s (50.26ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#3.....:   137.6 kH/s (50.39ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#4.....:   137.6 kH/s (50.38ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.Dev.#*.....:   551.2 kH/s

Hashmode: 15400 - ChaCha20

Speed.Dev.#1.....:  8113.7 MH/s (82.60ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:  8191.8 MH/s (81.86ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:  8168.1 MH/s (82.04ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:  8115.2 MH/s (82.57ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 32588.7 MH/s

Hashmode: 15500 - JKS Java Key Store Private Keys (SHA1)

Speed.Dev.#1.....: 16428.1 MH/s (50.98ms) @ Accel:32 Loops:512 Thr:640 Vec:1
Speed.Dev.#2.....: 16428.3 MH/s (50.97ms) @ Accel:32 Loops:512 Thr:640 Vec:1
Speed.Dev.#3.....: 16386.7 MH/s (51.12ms) @ Accel:32 Loops:512 Thr:640 Vec:1
Speed.Dev.#4.....: 16377.7 MH/s (51.14ms) @ Accel:32 Loops:512 Thr:640 Vec:1
Speed.Dev.#*.....: 65620.8 MH/s

Hashmode: 15600 - Ethereum Wallet, PBKDF2-HMAC-SHA256 (Iterations: 262143)

Speed.Dev.#1.....:    11295 H/s (70.16ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:    11295 H/s (70.16ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:    11271 H/s (70.31ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:    11269 H/s (70.33ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:    45128 H/s

Hashmode: 15700 - Ethereum Wallet, SCRYPT (Iterations: 1)

Speed.Dev.#1.....:        6 H/s (8463.52ms) @ Accel:1 Loops:1 Thr:1 Vec:1
Speed.Dev.#2.....:        6 H/s (8469.75ms) @ Accel:1 Loops:1 Thr:1 Vec:1
Speed.Dev.#3.....:        6 H/s (8456.68ms) @ Accel:1 Loops:1 Thr:1 Vec:1
Speed.Dev.#4.....:        6 H/s (8494.32ms) @ Accel:1 Loops:1 Thr:1 Vec:1
Speed.Dev.#*.....:       23 H/s

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 7999)

Speed.Dev.#1.....:   119.1 kH/s (87.50ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.Dev.#2.....:   119.2 kH/s (87.44ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.Dev.#3.....:   119.3 kH/s (87.40ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.Dev.#4.....:   119.0 kH/s (87.55ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.Dev.#*.....:   476.7 kH/s

Hashmode: 16000 - Tripcode

Speed.Dev.#1.....:   583.8 MH/s (71.75ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.Dev.#2.....:   583.7 MH/s (71.76ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.Dev.#3.....:   582.4 MH/s (71.94ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.Dev.#4.....:   582.2 MH/s (71.95ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.Dev.#*.....:  2332.1 MH/s

Hashmode: 16100 - TACACS+

Speed.Dev.#1.....: 31318.4 MH/s (42.78ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 31319.6 MH/s (42.76ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 31209.0 MH/s (42.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 31238.1 MH/s (42.87ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....:   125.1 GH/s

Hashmode: 16200 - Apple Secure Notes (Iterations: 19999)

Speed.Dev.#1.....:   147.8 kH/s (70.28ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:   147.9 kH/s (70.26ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:   147.6 kH/s (70.38ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:   147.5 kH/s (70.45ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:   590.8 kH/s

Hashmode: 16300 - Ethereum Pre-Sale Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1999)

Speed.Dev.#1.....:  1470.5 kH/s (68.48ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#2.....:  1470.6 kH/s (68.48ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#3.....:  1470.7 kH/s (68.47ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#4.....:  1465.7 kH/s (68.68ms) @ Accel:32 Loops:128 Thr:640 Vec:1
Speed.Dev.#*.....:  5877.6 kH/s

Hashmode: 16400 - CRAM-MD5 Dovecot

Speed.Dev.#1.....: 52473.1 MH/s (25.48ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#2.....: 52465.2 MH/s (25.48ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#3.....: 52463.9 MH/s (25.48ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#4.....: 52287.1 MH/s (25.56ms) @ Accel:16 Loops:1024 Thr:1024 Vec:1
Speed.Dev.#*.....:   209.7 GH/s

Hashmode: 16500 - JWT (JSON Web Token)

Speed.Dev.#1.....:  1216.0 MH/s (51.65ms) @ Accel:64 Loops:32 Thr:384 Vec:1
Speed.Dev.#2.....:  1214.7 MH/s (51.69ms) @ Accel:64 Loops:32 Thr:384 Vec:1
Speed.Dev.#3.....:  1215.8 MH/s (51.64ms) @ Accel:64 Loops:32 Thr:384 Vec:1
Speed.Dev.#4.....:  1213.6 MH/s (51.75ms) @ Accel:64 Loops:32 Thr:384 Vec:1
Speed.Dev.#*.....:  4860.1 MH/s

Hashmode: 16600 - Electrum Wallet (Salt-Type 1-3)

Speed.Dev.#1.....:   733.0 MH/s (57.22ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.Dev.#2.....:   733.0 MH/s (57.15ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.Dev.#3.....:   731.8 MH/s (57.23ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.Dev.#4.....:   730.2 MH/s (57.27ms) @ Accel:16 Loops:32 Thr:1024 Vec:1
Speed.Dev.#*.....:  2927.9 MH/s
```
