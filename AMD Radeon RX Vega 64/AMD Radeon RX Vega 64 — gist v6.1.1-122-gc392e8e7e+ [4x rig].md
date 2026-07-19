# AMD Radeon RX Vega 64 (4x rig)

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX Vega 64
- **Конфигурация / Setup:** 4x rig
- **Версия hashcat / Version:** v6.1.1-122-gc392e8e7e+
- **Источник / Source:** [gist](https://gist.github.com/9c8a4618f5b96572ba7f1d1191ef9195)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 126.1 GH/s |
| 100 | SHA1 | 43182.0 MH/s |
| 1400 | SHA2-256 | 18165.5 MH/s |
| 1700 | SHA2-512 | 4748.1 MH/s |
| 1000 | NTLM | 206.7 GH/s |
| 3200 | bcrypt | 82630 H/s |
| 1800 | sha512crypt | 581.3 kH/s |
| 500 | md5crypt | 47861.4 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 2088.9 kH/s |
| 2500 | WPA/WPA2 (legacy) | 2091.7 kH/s |
| 7500 | Kerberos AS-REQ (23) | 1303.2 MH/s |
| 13100 | Kerberos TGS-REP (23) | 1297.8 MH/s |
| 11300 | Bitcoin wallet.dat | 21227 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 1491.5 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.1.1-122-gc392e8e7e+) starting in benchmark mode...

OpenCL API (OpenCL 2.0 AMD-APP (3186.0)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: gfx900, 8064/8176 MB (6949 MB allocatable), 64MCU
* Device #2: gfx900, 8064/8176 MB (6949 MB allocatable), 64MCU
* Device #3: gfx900, 8064/8176 MB (6949 MB allocatable), 64MCU
* Device #4: gfx900, 8064/8176 MB (6949 MB allocatable), 64MCU

OpenCL API (OpenCL 2.1 LINUX) - Platform #2 [Intel(R) Corporation]
==================================================================
* Device #5: Intel(R) Xeon(R) Silver 4114 CPU @ 2.20GHz, skipped

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable
* --workload-profile=4

Hashmode: 0 - MD5

Speed.#1.........: 31600.8 MH/s (67.49ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 31600.9 MH/s (67.54ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 31265.5 MH/s (68.24ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 31632.3 MH/s (67.65ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   126.1 GH/s

Hashmode: 10 - md5($pass.$salt)

Speed.#1.........: 31581.2 MH/s (67.57ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 31592.6 MH/s (67.65ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 31190.2 MH/s (68.41ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 31592.9 MH/s (67.73ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   126.0 GH/s

Hashmode: 11 - Joomla < 2.5.18

Speed.#1.........: 31533.2 MH/s (67.79ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 31476.1 MH/s (67.78ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 31090.0 MH/s (68.63ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 31502.6 MH/s (67.93ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   125.6 GH/s

Hashmode: 12 - PostgreSQL

Speed.#1.........: 31581.0 MH/s (67.68ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 31484.7 MH/s (67.78ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 31139.4 MH/s (68.53ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 31546.6 MH/s (67.84ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   125.8 GH/s

Hashmode: 20 - md5($salt.$pass)

Speed.#1.........: 16451.4 MH/s (130.21ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 16433.9 MH/s (130.24ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 16268.0 MH/s (131.62ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 16437.3 MH/s (130.41ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 65590.5 MH/s

Hashmode: 21 - osCommerce, xt:Commerce

Speed.#1.........: 16369.4 MH/s (130.82ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 16364.9 MH/s (130.93ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 16161.4 MH/s (132.49ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 16340.1 MH/s (131.19ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 65235.8 MH/s

Hashmode: 22 - Juniper NetScreen/SSG (ScreenOS)

Speed.#1.........: 16743.7 MH/s (127.81ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 16720.4 MH/s (127.99ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 16512.0 MH/s (129.59ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 16723.0 MH/s (128.17ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 66699.2 MH/s

Hashmode: 23 - Skype

Speed.#1.........: 16486.2 MH/s (129.83ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 16476.7 MH/s (129.91ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 16308.0 MH/s (131.33ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 16478.2 MH/s (130.09ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 65749.1 MH/s

Hashmode: 30 - md5(utf16le($pass).$salt)

Speed.#1.........: 31599.1 MH/s (67.56ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 31589.5 MH/s (67.57ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 31267.1 MH/s (68.24ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 31613.9 MH/s (67.69ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   126.1 GH/s

Hashmode: 40 - md5($salt.utf16le($pass))

Speed.#1.........: 16461.7 MH/s (130.07ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 16467.2 MH/s (129.99ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 16287.1 MH/s (131.45ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 16487.9 MH/s (130.01ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 65703.9 MH/s

Hashmode: 50 - HMAC-MD5 (key = $pass)

Speed.#1.........:  4834.8 MH/s (443.70ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4828.9 MH/s (444.29ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4775.4 MH/s (449.24ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4825.2 MH/s (444.82ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 19264.3 MH/s

Hashmode: 60 - HMAC-MD5 (key = $salt)

Speed.#1.........:  9717.7 MH/s (220.54ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  9740.5 MH/s (220.03ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9615.4 MH/s (222.95ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  9722.5 MH/s (220.63ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 38796.1 MH/s

Hashmode: 100 - SHA1

Speed.#1.........: 10815.0 MH/s (198.13ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10829.4 MH/s (197.86ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10714.4 MH/s (200.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10823.2 MH/s (198.17ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 43182.0 MH/s

Hashmode: 101 - nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.#1.........: 10823.0 MH/s (198.01ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10823.5 MH/s (198.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10701.9 MH/s (200.23ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10814.1 MH/s (198.35ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 43162.5 MH/s

Hashmode: 110 - sha1($pass.$salt)

Speed.#1.........: 10858.0 MH/s (197.32ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10853.8 MH/s (197.46ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10743.3 MH/s (199.45ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10853.3 MH/s (197.62ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 43308.4 MH/s

Hashmode: 111 - nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.#1.........: 10778.0 MH/s (198.84ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10780.0 MH/s (198.79ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10670.7 MH/s (200.81ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10767.7 MH/s (199.20ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 42996.4 MH/s

Hashmode: 112 - Oracle S: Type (Oracle 11+)

Speed.#1.........: 10819.0 MH/s (198.05ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10819.4 MH/s (198.06ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10709.3 MH/s (200.09ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10813.4 MH/s (198.36ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 43161.1 MH/s

Hashmode: 120 - sha1($salt.$pass)

Speed.#1.........:  8248.9 MH/s (259.90ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  8260.4 MH/s (259.67ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  8166.0 MH/s (262.54ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  8255.0 MH/s (259.90ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 32930.2 MH/s

Hashmode: 121 - SMF (Simple Machines Forum) > v1.1

Speed.#1.........:  8244.0 MH/s (260.10ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  8243.9 MH/s (260.05ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  8160.5 MH/s (262.71ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  8247.4 MH/s (260.14ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 32895.9 MH/s

Hashmode: 122 - macOS v10.4, macOS v10.5, MacOS v10.6

Speed.#1.........:  8233.8 MH/s (260.38ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  8234.3 MH/s (260.39ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  8144.0 MH/s (263.24ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  8234.6 MH/s (260.55ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 32846.8 MH/s

Hashmode: 124 - Django (SHA-1)

Speed.#1.........:  8235.3 MH/s (260.38ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  8237.7 MH/s (260.25ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  8157.8 MH/s (262.84ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  8239.3 MH/s (260.39ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 32870.1 MH/s

Hashmode: 125 - ArubaOS

Speed.#1.........:  8219.3 MH/s (260.91ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  8220.9 MH/s (260.83ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  8134.5 MH/s (263.62ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  8218.3 MH/s (261.05ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 32793.1 MH/s

Hashmode: 130 - sha1(utf16le($pass).$salt)

Speed.#1.........: 10923.9 MH/s (196.25ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10923.9 MH/s (196.18ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10811.7 MH/s (198.19ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10922.8 MH/s (196.38ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 43582.2 MH/s

Hashmode: 131 - MSSQL (2000)

Speed.#1.........: 10889.7 MH/s (196.76ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10886.0 MH/s (196.89ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10781.6 MH/s (198.79ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10905.9 MH/s (196.68ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 43463.1 MH/s

Hashmode: 132 - MSSQL (2005)

Speed.#1.........: 10914.6 MH/s (196.30ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10915.0 MH/s (196.38ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10810.4 MH/s (198.21ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10919.2 MH/s (196.43ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 43559.3 MH/s

Hashmode: 133 - PeopleSoft

Speed.#1.........: 10850.0 MH/s (197.51ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10853.6 MH/s (197.53ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10728.2 MH/s (199.73ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10851.1 MH/s (197.67ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 43283.0 MH/s

Hashmode: 140 - sha1($salt.utf16le($pass))

Speed.#1.........:  8292.4 MH/s (258.57ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  8291.7 MH/s (258.57ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  8198.8 MH/s (261.48ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  8297.4 MH/s (258.57ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 33080.3 MH/s

Hashmode: 141 - Episerver 6.x < .NET 4

Speed.#1.........:  8293.8 MH/s (258.62ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  8293.1 MH/s (258.54ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  8198.8 MH/s (261.50ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  8297.4 MH/s (258.58ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 33083.1 MH/s

Hashmode: 150 - HMAC-SHA1 (key = $pass)

Speed.#1.........:  2391.0 MH/s (448.60ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  2394.7 MH/s (448.05ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  2373.4 MH/s (451.92ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  2391.9 MH/s (448.68ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  9551.0 MH/s

Hashmode: 160 - HMAC-SHA1 (key = $salt)

Speed.#1.........:  4518.2 MH/s (474.91ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4517.9 MH/s (474.89ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4469.5 MH/s (480.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4513.5 MH/s (475.58ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 18019.2 MH/s

Hashmode: 200 - MySQL323

Speed.#1.........: 78391.0 MH/s (27.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 78090.9 MH/s (27.12ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 78029.3 MH/s (27.13ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 78863.9 MH/s (27.03ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   313.4 GH/s

Hashmode: 300 - MySQL4.1/MySQL5

Speed.#1.........:  4714.7 MH/s (455.14ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4719.7 MH/s (454.61ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4667.7 MH/s (459.64ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4713.1 MH/s (455.44ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 18815.2 MH/s

Hashmode: 400 - phpass (Iterations: 2048)

Speed.#1.........:  9234.2 kH/s (110.65ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  9209.0 kH/s (110.96ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9116.0 kH/s (112.05ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  9271.9 kH/s (110.44ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 36831.1 kH/s

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#1.........: 12027.4 kH/s (169.16ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#2.........: 11968.5 kH/s (169.87ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#3.........: 11819.8 kH/s (172.04ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#4.........: 12045.6 kH/s (169.04ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#*.........: 47861.4 kH/s

Hashmode: 501 - Juniper IVE (Iterations: 1000)

Speed.#1.........: 12055.4 kH/s (168.84ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#2.........: 12016.5 kH/s (169.19ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#3.........: 11810.4 kH/s (172.13ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#4.........: 12061.5 kH/s (168.83ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#*.........: 47943.8 kH/s

Hashmode: 600 - BLAKE2b-512

Speed.#1.........:  2799.4 MH/s (383.16ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  2800.2 MH/s (383.01ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  2771.3 MH/s (386.99ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  2799.0 MH/s (383.37ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 11169.9 MH/s

Hashmode: 900 - MD4

Speed.#1.........: 51499.6 MH/s (41.32ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 51660.8 MH/s (41.29ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 50888.1 MH/s (41.76ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 51647.9 MH/s (41.38ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   205.7 GH/s

Hashmode: 1000 - NTLM

Speed.#1.........: 51729.9 MH/s (41.16ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 51899.1 MH/s (41.11ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 51151.7 MH/s (41.55ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 51889.7 MH/s (41.20ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   206.7 GH/s

Hashmode: 1100 - Domain Cached Credentials (DCC), MS Cache

Speed.#1.........: 16582.2 MH/s (129.06ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 16582.8 MH/s (129.07ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 16359.8 MH/s (130.82ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 16566.0 MH/s (129.40ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 66090.8 MH/s

Hashmode: 1300 - SHA2-224

Speed.#1.........:  4450.5 MH/s (482.03ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4454.6 MH/s (481.62ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4412.0 MH/s (486.31ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4451.1 MH/s (482.21ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 17768.1 MH/s

Hashmode: 1400 - SHA2-256

Speed.#1.........:  4550.4 MH/s (471.56ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4557.6 MH/s (470.78ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4506.3 MH/s (476.12ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4551.2 MH/s (471.61ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 18165.5 MH/s

Hashmode: 1410 - sha256($pass.$salt)

Speed.#1.........:  4568.8 MH/s (469.58ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4575.0 MH/s (468.92ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4526.8 MH/s (473.92ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4571.3 MH/s (469.53ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 18241.9 MH/s

Hashmode: 1411 - SSHA-256(Base64), LDAP {SSHA256}

Speed.#1.........:  4538.7 MH/s (472.73ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4542.3 MH/s (472.43ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4489.9 MH/s (477.94ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4534.7 MH/s (473.31ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 18105.6 MH/s

Hashmode: 1420 - sha256($salt.$pass)

Speed.#1.........:  4124.1 MH/s (259.93ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4131.3 MH/s (259.44ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4082.9 MH/s (262.55ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4127.5 MH/s (259.90ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 16465.9 MH/s

Hashmode: 1421 - hMailServer

Speed.#1.........:  4116.6 MH/s (260.45ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4119.3 MH/s (260.28ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4072.1 MH/s (263.29ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4115.3 MH/s (260.69ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 16423.3 MH/s

Hashmode: 1430 - sha256(utf16le($pass).$salt)

Speed.#1.........:  4561.2 MH/s (470.35ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4573.8 MH/s (469.18ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4522.0 MH/s (474.43ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4565.4 MH/s (470.13ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 18222.5 MH/s

Hashmode: 1440 - sha256($salt.utf16le($pass))

Speed.#1.........:  4131.1 MH/s (259.61ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4136.3 MH/s (259.13ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4088.7 MH/s (262.16ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4132.2 MH/s (259.60ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 16488.2 MH/s

Hashmode: 1441 - Episerver 6.x >= .NET 4

Speed.#1.........:  4120.8 MH/s (260.16ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4123.2 MH/s (259.99ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4072.8 MH/s (263.19ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4120.4 MH/s (260.34ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 16437.3 MH/s

Hashmode: 1450 - HMAC-SHA256 (key = $pass)

Speed.#1.........:   900.2 MH/s (297.83ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:   899.1 MH/s (298.22ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:   890.1 MH/s (301.20ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#4.........:   898.3 MH/s (298.60ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:  3587.7 MH/s

Hashmode: 1460 - HMAC-SHA256 (key = $salt)

Speed.#1.........:  1952.5 MH/s (274.60ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1957.2 MH/s (273.96ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1937.1 MH/s (276.82ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1954.3 MH/s (274.48ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  7801.2 MH/s

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#1.........:   995.4 MH/s (269.11ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   996.6 MH/s (268.84ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   985.1 MH/s (271.91ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   996.3 MH/s (269.08ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  3973.5 MH/s

Hashmode: 1600 - Apache $apr1$ MD5, md5apr1, MD5 (APR) (Iterations: 1000)

Speed.#1.........: 12091.7 kH/s (168.17ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#2.........: 12001.8 kH/s (169.47ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#3.........: 11903.4 kH/s (170.70ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#4.........: 12169.2 kH/s (167.31ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#*.........: 48166.1 kH/s

Hashmode: 1700 - SHA2-512

Speed.#1.........:  1189.8 MH/s (450.84ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#2.........:  1190.6 MH/s (450.50ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#3.........:  1178.6 MH/s (455.19ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#4.........:  1189.1 MH/s (451.26ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#*.........:  4748.1 MH/s

Hashmode: 1710 - sha512($pass.$salt)

Speed.#1.........:  1046.1 MH/s (256.17ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:  1046.0 MH/s (256.20ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:  1035.4 MH/s (258.82ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:  1046.1 MH/s (256.39ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  4173.6 MH/s

Hashmode: 1711 - SSHA-512(Base64), LDAP {SSHA512}

Speed.#1.........:  1039.2 MH/s (257.93ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:  1039.5 MH/s (257.80ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:  1028.2 MH/s (260.62ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#4.........:  1039.4 MH/s (258.04ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:  4146.3 MH/s

Hashmode: 1720 - sha512($salt.$pass)

Speed.#1.........:  1128.0 MH/s (475.64ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#2.........:  1127.1 MH/s (475.95ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#3.........:  1116.1 MH/s (480.60ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#4.........:  1128.0 MH/s (475.73ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#*.........:  4499.2 MH/s

Hashmode: 1722 - macOS v10.7

Speed.#1.........:  1123.3 MH/s (477.52ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1122.5 MH/s (477.84ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1112.4 MH/s (482.29ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1123.4 MH/s (477.66ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  4481.6 MH/s

Hashmode: 1730 - sha512(utf16le($pass).$salt)

Speed.#1.........:  1040.4 MH/s (257.56ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:  1040.5 MH/s (257.55ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:  1031.8 MH/s (259.69ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#4.........:  1042.7 MH/s (257.20ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:  4155.4 MH/s

Hashmode: 1731 - MSSQL (2012, 2014)

Speed.#1.........:  1040.3 MH/s (257.60ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#2.........:  1040.0 MH/s (257.74ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#3.........:  1029.1 MH/s (260.38ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#4.........:  1041.3 MH/s (257.55ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#*.........:  4150.6 MH/s

Hashmode: 1740 - sha512($salt.utf16le($pass))

Speed.#1.........:  1033.4 MH/s (259.33ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:  1034.1 MH/s (259.22ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:  1024.1 MH/s (261.69ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#4.........:  1034.6 MH/s (259.22ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:  4126.1 MH/s

Hashmode: 1750 - HMAC-SHA512 (key = $pass)

Speed.#1.........:   231.6 MH/s (289.34ms) @ Accel:32 Loops:512 Thr:64 Vec:1
Speed.#2.........:   230.9 MH/s (290.29ms) @ Accel:32 Loops:512 Thr:64 Vec:1
Speed.#3.........:   228.3 MH/s (293.47ms) @ Accel:32 Loops:512 Thr:64 Vec:1
Speed.#4.........:   231.7 MH/s (289.37ms) @ Accel:32 Loops:512 Thr:64 Vec:1
Speed.#*.........:   922.6 MH/s

Hashmode: 1760 - HMAC-SHA512 (key = $salt)

Speed.#1.........:   518.9 MH/s (258.26ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#2.........:   518.9 MH/s (258.31ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#3.........:   514.1 MH/s (260.64ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#4.........:   519.5 MH/s (258.11ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#*.........:  2071.5 MH/s

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:   145.5 kH/s (356.73ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   144.9 kH/s (358.15ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   145.6 kH/s (355.86ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   145.3 kH/s (357.16ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   581.3 kH/s

Hashmode: 2000 - STDOUT

Speed.#1.........: 12076.4 GH/s (0.08ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  9848.5 GH/s (0.10ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9077.7 GH/s (0.11ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  8908.0 GH/s (0.11ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 39910.6 GH/s

Hashmode: 2100 - Domain Cached Credentials 2 (DCC2), MS Cache 2 (Iterations: 10239)

Speed.#1.........:   425.7 kH/s (491.56ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   425.4 kH/s (491.88ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   421.2 kH/s (496.83ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   425.8 kH/s (491.61ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  1698.2 kH/s

Hashmode: 2400 - Cisco-PIX MD5

Speed.#1.........: 21168.3 MH/s (101.05ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 21183.5 MH/s (100.99ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 20981.9 MH/s (101.99ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 21190.4 MH/s (101.13ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 84524.1 MH/s

Hashmode: 2410 - Cisco-ASA MD5

Speed.#1.........: 21158.5 MH/s (101.10ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 21175.2 MH/s (101.07ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 20949.8 MH/s (102.09ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 21183.1 MH/s (101.16ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 84466.6 MH/s

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#1.........:   523.4 kH/s (499.09ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   524.7 kH/s (498.00ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   519.7 kH/s (502.86ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   523.9 kH/s (498.82ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  2091.7 kH/s

Hashmode: 2501 - WPA-EAPOL-PMK (Iterations: 0)

Speed.#1.........:   329.8 MH/s (0.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   305.7 MH/s (0.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   333.3 MH/s (0.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   314.3 MH/s (0.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  1283.1 MH/s

Hashmode: 2600 - md5(md5($pass))

Speed.#1.........:  9409.2 MH/s (227.77ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  9408.2 MH/s (227.85ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9310.8 MH/s (230.19ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  9407.9 MH/s (228.02ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 37536.1 MH/s

Hashmode: 2611 - vBulletin < v3.8.5

Speed.#1.........:  9382.7 MH/s (228.45ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  9387.9 MH/s (228.44ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9288.6 MH/s (230.76ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  9387.2 MH/s (228.55ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 37446.5 MH/s

Hashmode: 2612 - PHPS

Speed.#1.........:  9370.1 MH/s (228.75ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  9368.5 MH/s (228.82ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9267.9 MH/s (231.27ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  9367.2 MH/s (229.02ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 37373.7 MH/s

Hashmode: 2711 - vBulletin >= v3.8.5

Speed.#1.........:  6364.3 MH/s (337.02ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  6362.6 MH/s (337.10ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  6296.8 MH/s (340.59ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  6357.8 MH/s (337.53ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 25381.5 MH/s

Hashmode: 2811 - MyBB 1.2+, IPB2+ (Invision Power Board)

Speed.#1.........:  6606.2 MH/s (324.76ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  6605.3 MH/s (324.70ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  6535.0 MH/s (328.23ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  6603.0 MH/s (324.99ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 26349.6 MH/s

Hashmode: 3000 - LM

Speed.#1.........: 27222.1 MH/s (78.45ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 27213.7 MH/s (78.36ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 26892.6 MH/s (79.28ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 27248.6 MH/s (78.45ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   108.6 GH/s

Hashmode: 3100 - Oracle H: Type (Oracle 7+)

Speed.#1.........:  1003.9 MH/s (266.93ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:  1003.7 MH/s (267.10ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:   992.5 MH/s (269.99ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:  1003.0 MH/s (267.39ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  4003.1 MH/s

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    20684 H/s (192.32ms) @ Accel:4 Loops:32 Thr:16 Vec:1
Speed.#2.........:    21037 H/s (189.40ms) @ Accel:4 Loops:32 Thr:16 Vec:1
Speed.#3.........:    20148 H/s (196.35ms) @ Accel:4 Loops:32 Thr:16 Vec:1
Speed.#4.........:    20762 H/s (191.69ms) @ Accel:4 Loops:32 Thr:16 Vec:1
Speed.#*.........:    82630 H/s

Hashmode: 3710 - md5($salt.md5($pass))

Speed.#1.........:  8604.3 MH/s (249.27ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  8600.8 MH/s (249.32ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  8498.1 MH/s (252.26ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  8599.0 MH/s (249.49ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 34302.3 MH/s

Hashmode: 3711 - MediaWiki B type

Speed.#1.........:  8565.4 MH/s (250.33ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  8562.9 MH/s (250.39ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  8470.4 MH/s (253.16ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  8572.5 MH/s (250.27ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 34171.2 MH/s

Hashmode: 3800 - md5($salt.$pass.$salt)

Speed.#1.........: 16278.4 MH/s (131.57ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 16275.1 MH/s (131.59ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 16088.3 MH/s (133.05ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 16283.4 MH/s (131.68ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 64925.2 MH/s

Hashmode: 3910 - md5(md5($pass).md5($salt))

Speed.#1.........:  6387.3 MH/s (335.81ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  6386.7 MH/s (335.87ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  6312.5 MH/s (339.72ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  6391.6 MH/s (335.75ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 25478.1 MH/s

Hashmode: 4010 - md5($salt.md5($salt.$pass))

Speed.#1.........:  7617.9 MH/s (281.62ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  7603.1 MH/s (282.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  7520.2 MH/s (285.18ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  7608.8 MH/s (282.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 30349.9 MH/s

Hashmode: 4110 - md5($salt.md5($pass.$salt))

Speed.#1.........:  8395.2 MH/s (255.36ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  8399.6 MH/s (255.26ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  8304.0 MH/s (258.27ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  8400.1 MH/s (255.41ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 33498.9 MH/s

Hashmode: 4300 - md5(strtoupper(md5($pass)))

Speed.#1.........:  9339.0 MH/s (229.53ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  9335.3 MH/s (229.62ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9234.8 MH/s (232.07ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  9341.0 MH/s (229.65ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 37250.1 MH/s

Hashmode: 4400 - md5(sha1($pass))

Speed.#1.........:  5738.4 MH/s (373.78ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  5751.3 MH/s (372.91ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  5683.7 MH/s (377.37ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  5741.2 MH/s (373.79ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 22914.6 MH/s

Hashmode: 4500 - sha1(sha1($pass))

Speed.#1.........:  4224.9 MH/s (253.83ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#2.........:  4225.7 MH/s (253.71ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#3.........:  4177.4 MH/s (256.59ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#4.........:  4223.1 MH/s (254.04ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#*.........: 16851.2 MH/s

Hashmode: 4510 - sha1(sha1($pass).$salt)

Speed.#1.........:  4059.8 MH/s (264.07ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#2.........:  4060.5 MH/s (264.03ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#3.........:  4014.9 MH/s (266.98ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#4.........:  4062.1 MH/s (264.10ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#*.........: 16197.3 MH/s

Hashmode: 4520 - sha1($salt.sha1($pass))

Speed.#1.........:  2585.7 MH/s (414.88ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#2.........:  2589.1 MH/s (414.29ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#3.........:  2562.3 MH/s (418.62ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#4.........:  2586.7 MH/s (414.86ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#*.........: 10323.8 MH/s

Hashmode: 4521 - Redmine

Speed.#1.........:  2577.9 MH/s (416.12ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  2584.6 MH/s (415.05ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  2556.0 MH/s (419.70ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  2580.9 MH/s (415.83ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 10299.4 MH/s

Hashmode: 4522 - PunBB

Speed.#1.........:  3900.8 MH/s (274.87ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#2.........:  3908.0 MH/s (274.35ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#3.........:  3862.9 MH/s (277.57ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#4.........:  3904.3 MH/s (274.77ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#*.........: 15576.0 MH/s

Hashmode: 4700 - sha1(md5($pass))

Speed.#1.........:  5860.9 MH/s (366.08ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  5871.0 MH/s (365.35ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  5801.5 MH/s (369.72ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  5867.0 MH/s (365.78ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 23400.3 MH/s

Hashmode: 4710 - sha1(md5($pass).$salt)

Speed.#1.........:  5522.6 MH/s (388.50ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  5534.0 MH/s (387.64ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  5472.3 MH/s (392.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  5531.8 MH/s (387.96ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 22060.7 MH/s

Hashmode: 4711 - Huawei sha1(md5($pass).$salt)

Speed.#1.........:  5513.2 MH/s (389.09ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  5518.5 MH/s (388.69ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  5459.6 MH/s (392.92ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  5513.4 MH/s (389.26ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 22004.7 MH/s

Hashmode: 4800 - iSCSI CHAP authentication, MD5(CHAP)

Speed.#1.........: 20790.4 MH/s (102.94ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 20806.8 MH/s (102.85ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 20564.8 MH/s (104.01ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 20791.6 MH/s (103.04ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 82953.7 MH/s

Hashmode: 4900 - sha1($salt.$pass.$salt)

Speed.#1.........:  8098.6 MH/s (264.72ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  8108.2 MH/s (264.40ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  8032.9 MH/s (266.89ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  8109.3 MH/s (264.57ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 32349.2 MH/s

Hashmode: 5100 - Half MD5

Speed.#1.........: 19192.3 MH/s (111.63ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 19182.8 MH/s (111.62ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 18991.4 MH/s (112.71ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 19206.7 MH/s (111.62ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 76573.2 MH/s

Hashmode: 5200 - Password Safe v3 (Iterations: 2049)

Speed.#1.........:  1798.8 kH/s (193.03ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1799.7 kH/s (192.99ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1775.9 kH/s (195.48ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1798.6 kH/s (193.10ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  7173.1 kH/s

Hashmode: 5300 - IKE-PSK MD5

Speed.#1.........:  1070.5 MH/s (250.31ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1072.2 MH/s (250.03ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1058.4 MH/s (253.20ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1069.2 MH/s (250.81ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  4270.5 MH/s

Hashmode: 5400 - IKE-PSK SHA1

Speed.#1.........:   480.8 MH/s (278.74ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#2.........:   479.4 MH/s (279.54ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#3.........:   474.6 MH/s (282.48ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#4.........:   479.6 MH/s (279.61ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#*.........:  1914.4 MH/s

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........: 32529.4 MH/s (65.58ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 32562.4 MH/s (65.55ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 32181.0 MH/s (66.29ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 32604.6 MH/s (65.63ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   129.9 GH/s

Hashmode: 5600 - NetNTLMv2

Speed.#1.........:  2120.5 MH/s (252.80ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  2124.4 MH/s (252.40ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  2100.5 MH/s (255.15ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  2121.7 MH/s (252.80ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  8467.1 MH/s

Hashmode: 5700 - Cisco-IOS type 4 (SHA256)

Speed.#1.........:  4536.8 MH/s (472.90ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4546.4 MH/s (471.92ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4493.2 MH/s (477.51ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4540.1 MH/s (472.74ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 18116.5 MH/s

Hashmode: 5800 - Samsung Android Password/PIN (Iterations: 1023)

Speed.#1.........:  7120.9 kH/s (288.61ms) @ Accel:512 Loops:1023 Thr:64 Vec:1
Speed.#2.........:  7172.9 kH/s (286.87ms) @ Accel:512 Loops:1023 Thr:64 Vec:1
Speed.#3.........:  7062.7 kH/s (291.31ms) @ Accel:512 Loops:1023 Thr:64 Vec:1
Speed.#4.........:  7185.8 kH/s (286.71ms) @ Accel:512 Loops:1023 Thr:64 Vec:1
Speed.#*.........: 28542.2 kH/s

Hashmode: 6000 - RIPEMD-160

Speed.#1.........:  6589.9 MH/s (325.48ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  6594.6 MH/s (325.33ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  6521.7 MH/s (328.82ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  6592.7 MH/s (325.50ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 26298.8 MH/s

Hashmode: 6100 - Whirlpool

Speed.#1.........:   604.7 MH/s (443.54ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:   602.2 MH/s (445.37ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:   607.1 MH/s (441.71ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:   604.6 MH/s (443.72ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  2418.7 MH/s

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#1.........:   374.0 kH/s (345.49ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:   373.6 kH/s (345.05ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:   370.5 kH/s (348.11ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#4.........:   373.4 kH/s (345.50ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:  1491.5 kH/s

Hashmode: 6212 - TrueCrypt RIPEMD160 + XTS 1024 bit (Iterations: 1999)

Speed.#1.........:   210.5 kH/s (301.96ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   210.5 kH/s (301.82ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   210.9 kH/s (303.47ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   213.6 kH/s (299.85ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   845.5 kH/s

Hashmode: 6213 - TrueCrypt RIPEMD160 + XTS 1536 bit (Iterations: 1999)

Speed.#1.........:   147.3 kH/s (427.55ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   147.7 kH/s (426.87ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   145.9 kH/s (431.90ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   147.3 kH/s (428.13ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   588.2 kH/s

Hashmode: 6221 - TrueCrypt SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:   457.6 kH/s (272.51ms) @ Accel:32 Loops:999 Thr:64 Vec:1
Speed.#2.........:   478.5 kH/s (266.69ms) @ Accel:32 Loops:999 Thr:64 Vec:1
Speed.#3.........:   476.0 kH/s (267.63ms) @ Accel:32 Loops:999 Thr:64 Vec:1
Speed.#4.........:   475.9 kH/s (267.87ms) @ Accel:32 Loops:999 Thr:64 Vec:1
Speed.#*.........:  1888.0 kH/s

Hashmode: 6222 - TrueCrypt SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:   226.2 kH/s (272.63ms) @ Accel:16 Loops:999 Thr:64 Vec:1
Speed.#2.........:   236.9 kH/s (266.23ms) @ Accel:16 Loops:999 Thr:64 Vec:1
Speed.#3.........:   235.6 kH/s (267.29ms) @ Accel:16 Loops:999 Thr:64 Vec:1
Speed.#4.........:   237.2 kH/s (265.90ms) @ Accel:16 Loops:999 Thr:64 Vec:1
Speed.#*.........:   935.9 kH/s

Hashmode: 6223 - TrueCrypt SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:   157.8 kH/s (357.21ms) @ Accel:128 Loops:124 Thr:64 Vec:1
Speed.#2.........:   158.1 kH/s (356.90ms) @ Accel:128 Loops:124 Thr:64 Vec:1
Speed.#3.........:   156.6 kH/s (360.32ms) @ Accel:128 Loops:124 Thr:64 Vec:1
Speed.#4.........:   157.8 kH/s (357.40ms) @ Accel:128 Loops:124 Thr:64 Vec:1
Speed.#*.........:   630.3 kH/s

Hashmode: 6231 - TrueCrypt Whirlpool + XTS 512 bit (Iterations: 999)

Speed.#1.........:    32209 H/s (250.93ms) @ Accel:64 Loops:31 Thr:64 Vec:1
Speed.#2.........:    32066 H/s (252.02ms) @ Accel:64 Loops:31 Thr:64 Vec:1
Speed.#3.........:    32243 H/s (250.59ms) @ Accel:64 Loops:31 Thr:64 Vec:1
Speed.#4.........:    32194 H/s (251.20ms) @ Accel:64 Loops:31 Thr:64 Vec:1
Speed.#*.........:   128.7 kH/s

Hashmode: 6232 - TrueCrypt Whirlpool + XTS 1024 bit (Iterations: 999)

Speed.#1.........:    15585 H/s (259.61ms) @ Accel:32 Loops:31 Thr:64 Vec:1
Speed.#2.........:    15511 H/s (260.71ms) @ Accel:32 Loops:31 Thr:64 Vec:1
Speed.#3.........:    15595 H/s (259.16ms) @ Accel:32 Loops:31 Thr:64 Vec:1
Speed.#4.........:    15568 H/s (259.88ms) @ Accel:32 Loops:31 Thr:64 Vec:1
Speed.#*.........:    62258 H/s

Hashmode: 6233 - TrueCrypt Whirlpool + XTS 1536 bit (Iterations: 999)

Speed.#1.........:    10339 H/s (376.06ms) @ Accel:64 Loops:15 Thr:64 Vec:1
Speed.#2.........:    10294 H/s (377.69ms) @ Accel:64 Loops:15 Thr:64 Vec:1
Speed.#3.........:    10356 H/s (375.32ms) @ Accel:64 Loops:15 Thr:64 Vec:1
Speed.#4.........:    10384 H/s (376.04ms) @ Accel:64 Loops:15 Thr:64 Vec:1
Speed.#*.........:    41373 H/s

Hashmode: 6241 - TrueCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 999)

Speed.#1.........:   726.5 kH/s (345.27ms) @ Accel:64 Loops:999 Thr:64 Vec:1
Speed.#2.........:   745.7 kH/s (341.08ms) @ Accel:64 Loops:999 Thr:64 Vec:1
Speed.#3.........:   735.3 kH/s (345.91ms) @ Accel:64 Loops:999 Thr:64 Vec:1
Speed.#4.........:   744.3 kH/s (342.33ms) @ Accel:64 Loops:999 Thr:64 Vec:1
Speed.#*.........:  2951.8 kH/s

Hashmode: 6242 - TrueCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 999)

Speed.#1.........:   417.8 kH/s (300.04ms) @ Accel:32 Loops:999 Thr:64 Vec:1
Speed.#2.........:   420.0 kH/s (298.04ms) @ Accel:32 Loops:999 Thr:64 Vec:1
Speed.#3.........:   413.3 kH/s (302.99ms) @ Accel:32 Loops:999 Thr:64 Vec:1
Speed.#4.........:   420.3 kH/s (298.54ms) @ Accel:32 Loops:999 Thr:64 Vec:1
Speed.#*.........:  1671.4 kH/s

Hashmode: 6243 - TrueCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 999)

Speed.#1.........:   282.7 kH/s (383.68ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#2.........:   282.9 kH/s (383.23ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#3.........:   280.1 kH/s (387.48ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#4.........:   282.7 kH/s (383.78ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#*.........:  1128.4 kH/s

Hashmode: 6300 - AIX {smd5} (Iterations: 1000)

Speed.#1.........: 12040.5 kH/s (168.78ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#2.........: 11974.8 kH/s (169.80ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#3.........: 11822.6 kH/s (171.94ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#4.........: 12083.3 kH/s (168.48ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#*.........: 47921.1 kH/s

Hashmode: 6400 - AIX {ssha256} (Iterations: 63)

Speed.#1.........: 25822.3 kH/s (73.46ms) @ Accel:512 Loops:63 Thr:64 Vec:1
Speed.#2.........: 25795.2 kH/s (73.64ms) @ Accel:512 Loops:63 Thr:64 Vec:1
Speed.#3.........: 25718.5 kH/s (73.54ms) @ Accel:512 Loops:63 Thr:64 Vec:1
Speed.#4.........: 26278.4 kH/s (72.36ms) @ Accel:512 Loops:63 Thr:64 Vec:1
Speed.#*.........:   103.6 MH/s

Hashmode: 6500 - AIX {ssha512} (Iterations: 63)

Speed.#1.........:  6762.2 kH/s (270.56ms) @ Accel:512 Loops:63 Thr:64 Vec:1
Speed.#2.........:  6761.0 kH/s (270.88ms) @ Accel:512 Loops:63 Thr:64 Vec:1
Speed.#3.........:  6702.2 kH/s (273.54ms) @ Accel:512 Loops:63 Thr:64 Vec:1
Speed.#4.........:  6788.7 kH/s (269.72ms) @ Accel:512 Loops:63 Thr:64 Vec:1
Speed.#*.........: 27014.1 kH/s

Hashmode: 6600 - 1Password, agilekeychain (Iterations: 999)

Speed.#1.........:  4319.9 kH/s (475.50ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#2.........:  4302.8 kH/s (477.27ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#3.........:  4251.7 kH/s (483.27ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#4.........:  4327.4 kH/s (475.18ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#*.........: 17201.7 kH/s

Hashmode: 6700 - AIX {ssha1} (Iterations: 63)

Speed.#1.........: 61828.8 kH/s (26.34ms) @ Accel:512 Loops:63 Thr:64 Vec:1
Speed.#2.........: 60931.4 kH/s (26.53ms) @ Accel:512 Loops:63 Thr:64 Vec:1
Speed.#3.........: 61570.7 kH/s (26.25ms) @ Accel:512 Loops:63 Thr:64 Vec:1
Speed.#4.........: 62155.9 kH/s (26.42ms) @ Accel:512 Loops:63 Thr:64 Vec:1
Speed.#*.........:   246.5 MH/s

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#1.........:  3658.3 kH/s (185.83ms) @ Accel:512 Loops:249 Thr:64 Vec:1
Speed.#2.........:  3644.6 kH/s (186.74ms) @ Accel:512 Loops:249 Thr:64 Vec:1
Speed.#3.........:  3596.1 kH/s (189.22ms) @ Accel:512 Loops:249 Thr:64 Vec:1
Speed.#4.........:  3658.0 kH/s (186.05ms) @ Accel:512 Loops:249 Thr:64 Vec:1
Speed.#*.........: 14556.9 kH/s

Hashmode: 6900 - GOST R 34.11-94

Speed.#1.........:   652.9 MH/s (410.84ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:   652.1 MH/s (411.30ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:   648.8 MH/s (413.30ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:   652.6 MH/s (411.09ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  2606.3 MH/s

Hashmode: 7000 - FortiGate (FortiOS)

Speed.#1.........:  9553.2 MH/s (224.36ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  9544.9 MH/s (224.56ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9472.7 MH/s (226.38ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  9561.5 MH/s (224.36ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 38132.3 MH/s

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

Speed.#1.........:   462.5 kH/s (184.39ms) @ Accel:64 Loops:511 Thr:64 Vec:1
Speed.#2.........:   471.7 kH/s (183.01ms) @ Accel:64 Loops:511 Thr:64 Vec:1
Speed.#3.........:   468.3 kH/s (184.16ms) @ Accel:64 Loops:511 Thr:64 Vec:1
Speed.#4.........:   462.7 kH/s (184.30ms) @ Accel:64 Loops:511 Thr:64 Vec:1
Speed.#*.........:  1865.2 kH/s

Hashmode: 7200 - GRUB 2 (Iterations: 1023)

Speed.#1.........:   470.5 kH/s (244.71ms) @ Accel:256 Loops:127 Thr:64 Vec:1
Speed.#2.........:   470.4 kH/s (244.95ms) @ Accel:256 Loops:127 Thr:64 Vec:1
Speed.#3.........:   466.3 kH/s (246.94ms) @ Accel:256 Loops:127 Thr:64 Vec:1
Speed.#4.........:   470.9 kH/s (244.55ms) @ Accel:256 Loops:127 Thr:64 Vec:1
Speed.#*.........:  1878.1 kH/s

Hashmode: 7300 - IPMI2 RAKP HMAC-SHA1

Speed.#1.........:  1396.6 MH/s (384.09ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1396.3 MH/s (384.04ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1383.0 MH/s (387.76ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1396.2 MH/s (384.30ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  5572.1 MH/s

Hashmode: 7400 - sha256crypt $5$, SHA256 (Unix) (Iterations: 5000)

Speed.#1.........:   378.9 kH/s (272.91ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#2.........:   376.8 kH/s (272.89ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#3.........:   373.3 kH/s (275.39ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#4.........:   378.0 kH/s (273.81ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#*.........:  1507.0 kH/s

Hashmode: 7401 - MySQL $A$ (sha256crypt) (Iterations: 5000)

Speed.#1.........:   342.1 kH/s (301.03ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   342.9 kH/s (301.41ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   338.8 kH/s (303.47ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   341.9 kH/s (300.82ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  1365.7 kH/s

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#1.........:   326.5 MH/s (410.74ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#2.........:   324.3 MH/s (413.41ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:   326.5 MH/s (410.61ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:   325.9 MH/s (411.56ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  1303.2 MH/s

Hashmode: 7700 - SAP CODVN B (BCODE)

Speed.#1.........:  1334.1 MH/s (401.97ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#2.........:  1309.7 MH/s (409.44ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#3.........:  1320.7 MH/s (406.07ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#4.........:  1308.5 MH/s (410.05ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#*.........:  5272.9 MH/s

Hashmode: 7701 - SAP CODVN B (BCODE) from RFC_READ_TABLE

Speed.#1.........:  1323.3 MH/s (405.29ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#2.........:  1298.7 MH/s (412.95ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#3.........:  1303.1 MH/s (411.55ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#4.........:  1306.1 MH/s (410.81ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#*.........:  5231.2 MH/s

Hashmode: 7800 - SAP CODVN F/G (PASSCODE)

Speed.#1.........:   965.4 MH/s (277.63ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:   966.9 MH/s (277.19ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:   956.9 MH/s (280.10ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:   967.2 MH/s (277.28ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  3856.4 MH/s

Hashmode: 7801 - SAP CODVN F/G (PASSCODE) from RFC_READ_TABLE

Speed.#1.........:   969.4 MH/s (276.47ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:   970.8 MH/s (276.05ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:   960.6 MH/s (279.07ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:   971.5 MH/s (276.07ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  3872.4 MH/s

Hashmode: 7900 - Drupal7 (Iterations: 16384)

Speed.#1.........:    61909 H/s (264.27ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#2.........:    61945 H/s (264.02ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#3.........:    61245 H/s (267.02ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#4.........:    61877 H/s (264.46ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   247.0 kH/s

Hashmode: 8000 - Sybase ASE

Speed.#1.........:   541.5 MH/s (495.36ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#2.........:   542.2 MH/s (494.63ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#3.........:   536.6 MH/s (499.87ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#4.........:   542.5 MH/s (494.53ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#*.........:  2162.9 MH/s

Hashmode: 8100 - Citrix NetScaler (SHA1)

Speed.#1.........:  9282.8 MH/s (230.93ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  9306.1 MH/s (230.35ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9202.7 MH/s (232.90ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  9297.4 MH/s (230.74ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 37089.0 MH/s

Hashmode: 8200 - 1Password, cloudkeychain (Iterations: 39999)

Speed.#1.........:    12109 H/s (276.42ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#2.........:    12097 H/s (276.30ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#3.........:    12001 H/s (278.89ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#4.........:    12091 H/s (276.51ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#*.........:    48298 H/s

Hashmode: 8300 - DNSSEC (NSEC3)

Speed.#1.........:  4018.3 MH/s (266.78ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4022.3 MH/s (266.50ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  3983.0 MH/s (269.24ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4023.2 MH/s (266.64ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 16046.7 MH/s

Hashmode: 8400 - WBB3 (Woltlab Burning Board)

Speed.#1.........:  1740.3 MH/s (308.06ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#2.........:  1743.6 MH/s (307.50ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#3.........:  1725.1 MH/s (310.75ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#4.........:  1742.6 MH/s (307.82ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#*.........:  6951.6 MH/s

Hashmode: 8500 - RACF

Speed.#1.........:  5161.1 MH/s (415.71ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  5163.5 MH/s (415.52ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  5106.3 MH/s (420.09ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  5167.2 MH/s (415.32ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 20598.1 MH/s

Hashmode: 8600 - Lotus Notes/Domino 5

Speed.#1.........:   578.9 MH/s (463.31ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:   579.5 MH/s (462.72ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:   575.9 MH/s (465.75ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:   581.0 MH/s (461.80ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  2315.3 MH/s

Hashmode: 8700 - Lotus Notes/Domino 6

Speed.#1.........:   188.2 MH/s (356.21ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#2.........:   187.8 MH/s (356.86ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#3.........:   187.8 MH/s (356.92ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#4.........:   188.6 MH/s (355.62ms) @ Accel:256 Loops:64 Thr:64 Vec:1
Speed.#*.........:   752.4 MH/s

Hashmode: 8800 - Android FDE <= 4.3 (Iterations: 1999)

Speed.#1.........:  1058.8 kH/s (489.47ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1063.9 kH/s (487.37ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1053.0 kH/s (492.82ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1059.6 kH/s (489.41ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  4235.2 kH/s

Hashmode: 8900 - scrypt (Iterations: 1)

Speed.#1.........:   238.7 kH/s (33.07ms) @ Accel:8 Loops:1 Thr:16 Vec:1
Speed.#2.........:   375.4 kH/s (20.90ms) @ Accel:8 Loops:1 Thr:16 Vec:1
Speed.#3.........:   330.8 kH/s (23.40ms) @ Accel:8 Loops:1 Thr:16 Vec:1
Speed.#4.........:   348.7 kH/s (22.70ms) @ Accel:8 Loops:1 Thr:16 Vec:1
Speed.#*.........:  1293.6 kH/s

Hashmode: 9000 - Password Safe v2 (Iterations: 1000)

Speed.#1.........:   494.2 kH/s (331.29ms) @ Accel:256 Loops:1000 Thr:16 Vec:1
Speed.#2.........:   500.6 kH/s (333.98ms) @ Accel:256 Loops:1000 Thr:16 Vec:1
Speed.#3.........:   487.3 kH/s (330.06ms) @ Accel:256 Loops:1000 Thr:16 Vec:1
Speed.#4.........:   496.0 kH/s (331.92ms) @ Accel:256 Loops:1000 Thr:16 Vec:1
Speed.#*.........:  1978.1 kH/s

Hashmode: 9100 - Lotus Notes/Domino 8 (Iterations: 4999)

Speed.#1.........:   728.9 kH/s (2.02ms) @ Accel:512 Loops:4 Thr:64 Vec:1
Speed.#2.........:   735.7 kH/s (2.01ms) @ Accel:512 Loops:4 Thr:64 Vec:1
Speed.#3.........:   719.4 kH/s (2.00ms) @ Accel:512 Loops:4 Thr:64 Vec:1
Speed.#4.........:   778.6 kH/s (2.01ms) @ Accel:512 Loops:4 Thr:64 Vec:1
Speed.#*.........:  2962.6 kH/s

Hashmode: 9200 - Cisco-IOS $8$ (PBKDF2-SHA256) (Iterations: 19999)

Speed.#1.........:    89091 H/s (300.72ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#2.........:    89178 H/s (300.25ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#3.........:    88311 H/s (303.23ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#4.........:    89185 H/s (300.58ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#*.........:   355.8 kH/s

Hashmode: 9300 - Cisco-IOS $9$ (scrypt) (Iterations: 1)

Speed.#1.........:    10759 H/s (760.16ms) @ Accel:16 Loops:1 Thr:8 Vec:1
Speed.#2.........:    10729 H/s (762.23ms) @ Accel:16 Loops:1 Thr:8 Vec:1
Speed.#3.........:    10770 H/s (759.38ms) @ Accel:16 Loops:1 Thr:8 Vec:1
Speed.#4.........:    12263 H/s (666.98ms) @ Accel:16 Loops:1 Thr:8 Vec:1
Speed.#*.........:    44521 H/s

Hashmode: 9400 - MS Office 2007 (Iterations: 50000)

Speed.#1.........:   172.1 kH/s (248.98ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   172.4 kH/s (248.49ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   170.4 kH/s (251.39ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   172.3 kH/s (248.84ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   687.3 kH/s

Hashmode: 9500 - MS Office 2010 (Iterations: 100000)

Speed.#1.........:    85906 H/s (249.42ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:    86014 H/s (249.11ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:    85068 H/s (251.85ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:    86006 H/s (249.25ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   343.0 kH/s

Hashmode: 9600 - MS Office 2013 (Iterations: 100000)

Speed.#1.........:    10582 H/s (504.47ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#2.........:    10591 H/s (504.26ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#3.........:    10482 H/s (509.60ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#4.........:    10591 H/s (504.04ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#*.........:    42246 H/s

Hashmode: 9700 - MS Office <= 2003 $0/$1, MD5 + RC4

Speed.#1.........:   313.4 MH/s (427.83ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#2.........:   311.9 MH/s (429.88ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:   314.3 MH/s (426.57ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:   313.1 MH/s (428.41ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  1252.8 MH/s

Hashmode: 9710 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #1

Speed.#1.........:   372.5 MH/s (359.89ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#2.........:   373.4 MH/s (358.94ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:   370.7 MH/s (361.64ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:   372.8 MH/s (359.79ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  1489.3 MH/s

Hashmode: 9720 - MS Office <= 2003 $0/$1, MD5 + RC4, collider #2

Speed.#1.........:  2609.4 MH/s (411.08ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#2.........:  2614.0 MH/s (410.44ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#3.........:  2587.6 MH/s (414.51ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#4.........:  2614.1 MH/s (410.50ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#*.........: 10425.1 MH/s

Hashmode: 9800 - MS Office <= 2003 $3/$4, SHA1 + RC4

Speed.#1.........:   329.3 MH/s (407.21ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#2.........:   327.7 MH/s (409.06ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:   330.6 MH/s (405.55ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:   329.1 MH/s (407.59ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  1316.8 MH/s

Hashmode: 9810 - MS Office <= 2003 $3, SHA1 + RC4, collider #1

Speed.#1.........:   375.3 MH/s (357.27ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#2.........:   375.1 MH/s (357.42ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:   372.4 MH/s (359.96ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:   375.1 MH/s (357.62ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  1497.8 MH/s

Hashmode: 9820 - MS Office <= 2003 $3, SHA1 + RC4, collider #2

Speed.#1.........:  2872.1 MH/s (373.40ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#2.........:  2860.3 MH/s (374.98ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#3.........:  2867.9 MH/s (373.94ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#4.........:  2877.7 MH/s (372.88ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#*.........: 11478.1 MH/s

Hashmode: 9900 - Radmin2

Speed.#1.........: 10289.0 MH/s (208.40ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10291.7 MH/s (208.26ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10189.6 MH/s (210.32ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10307.7 MH/s (208.11ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 41078.1 MH/s

Hashmode: 10000 - Django (PBKDF2-SHA256) (Iterations: 9999)

Speed.#1.........:   176.4 kH/s (303.94ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#2.........:   176.6 kH/s (303.20ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#3.........:   175.0 kH/s (306.02ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#4.........:   176.7 kH/s (303.42ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#*.........:   704.7 kH/s

Hashmode: 10100 - SipHash

Speed.#1.........: 39142.9 MH/s (54.45ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 39191.5 MH/s (54.36ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 38863.8 MH/s (54.82ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 39353.3 MH/s (54.33ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   156.6 GH/s

Hashmode: 10200 - CRAM-MD5

Speed.#1.........:  4801.7 MH/s (446.85ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4802.7 MH/s (446.70ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4756.0 MH/s (451.18ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4811.6 MH/s (446.08ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 19172.1 MH/s

Hashmode: 10300 - SAP CODVN H (PWDSALTEDHASH) iSSHA-1 (Iterations: 1023)

Speed.#1.........:  6451.9 kH/s (319.09ms) @ Accel:512 Loops:1023 Thr:64 Vec:1
Speed.#2.........:  6449.6 kH/s (319.58ms) @ Accel:512 Loops:1023 Thr:64 Vec:1
Speed.#3.........:  6340.0 kH/s (324.88ms) @ Accel:512 Loops:1023 Thr:64 Vec:1
Speed.#4.........:  6457.7 kH/s (319.21ms) @ Accel:512 Loops:1023 Thr:64 Vec:1
Speed.#*.........: 25699.2 kH/s

Hashmode: 10400 - PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.#1.........:   404.2 MH/s (331.62ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#2.........:   401.9 MH/s (333.49ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:   405.2 MH/s (330.80ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:   403.9 MH/s (332.11ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  1615.2 MH/s

Hashmode: 10410 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1

Speed.#1.........:   428.6 MH/s (312.73ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#2.........:   428.7 MH/s (312.81ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:   425.3 MH/s (315.13ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:   428.8 MH/s (312.81ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  1711.4 MH/s

Hashmode: 10420 - PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #2

Speed.#1.........:  9993.8 MH/s (214.49ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10012.6 MH/s (214.05ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9898.1 MH/s (216.59ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10010.0 MH/s (214.29ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 39914.6 MH/s

Hashmode: 10500 - PDF 1.4 - 1.6 (Acrobat 5 - 8) (Iterations: 70)

Speed.#1.........: 19003.0 kH/s (104.88ms) @ Accel:512 Loops:70 Thr:64 Vec:1
Speed.#2.........: 18783.2 kH/s (105.67ms) @ Accel:512 Loops:70 Thr:64 Vec:1
Speed.#3.........: 19060.7 kH/s (104.43ms) @ Accel:512 Loops:70 Thr:64 Vec:1
Speed.#4.........: 18991.4 kH/s (105.06ms) @ Accel:512 Loops:70 Thr:64 Vec:1
Speed.#*.........: 75838.3 kH/s

Hashmode: 10600 - PDF 1.7 Level 3 (Acrobat 9)

Speed.#1.........:  4543.3 MH/s (472.29ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4555.4 MH/s (470.97ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4509.0 MH/s (475.88ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4552.3 MH/s (471.49ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 18160.0 MH/s

Hashmode: 10700 - PDF 1.7 Level 8 (Acrobat 10 - 11) (Iterations: 64)

Speed.#1.........:    39957 H/s (409.21ms) @ Accel:8 Loops:32 Thr:64 Vec:1
Speed.#2.........:    39653 H/s (412.54ms) @ Accel:8 Loops:32 Thr:64 Vec:1
Speed.#3.........:    40041 H/s (408.39ms) @ Accel:8 Loops:32 Thr:64 Vec:1
Speed.#4.........:    39408 H/s (415.38ms) @ Accel:8 Loops:32 Thr:64 Vec:1
Speed.#*.........:   159.1 kH/s

Hashmode: 10800 - SHA2-384

Speed.#1.........:  1161.7 MH/s (461.77ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#2.........:  1161.2 MH/s (461.92ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#3.........:  1150.9 MH/s (466.08ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#4.........:  1160.9 MH/s (462.20ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#*.........:  4634.6 MH/s

Hashmode: 10900 - PBKDF2-HMAC-SHA256 (Iterations: 999)

Speed.#1.........:  1760.2 kH/s (236.20ms) @ Accel:512 Loops:249 Thr:64 Vec:1
Speed.#2.........:  1757.9 kH/s (236.72ms) @ Accel:512 Loops:249 Thr:64 Vec:1
Speed.#3.........:  1738.5 kH/s (239.22ms) @ Accel:512 Loops:249 Thr:64 Vec:1
Speed.#4.........:  1759.7 kH/s (236.14ms) @ Accel:512 Loops:249 Thr:64 Vec:1
Speed.#*.........:  7016.3 kH/s

Hashmode: 10901 - RedHat 389-DS LDAP (PBKDF2-HMAC-SHA256) (Iterations: 8191)

Speed.#1.........:   214.8 kH/s (304.42ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   214.4 kH/s (304.95ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   212.3 kH/s (307.88ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   214.6 kH/s (304.96ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   856.0 kH/s

Hashmode: 11000 - PrestaShop

Speed.#1.........: 10818.2 MH/s (198.10ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10820.0 MH/s (198.05ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10716.4 MH/s (200.03ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10841.6 MH/s (197.84ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 43196.2 MH/s

Hashmode: 11100 - PostgreSQL CRAM (MD5)

Speed.#1.........:  9331.1 MH/s (229.79ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  9335.6 MH/s (229.58ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9239.3 MH/s (231.99ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  9349.2 MH/s (229.45ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 37255.2 MH/s

Hashmode: 11200 - MySQL CRAM (SHA1)

Speed.#1.........:  2859.9 MH/s (375.10ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  2864.9 MH/s (374.35ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  2833.2 MH/s (378.52ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  2864.2 MH/s (374.64ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 11422.3 MH/s

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

Speed.#1.........:     5320 H/s (502.04ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:     5325 H/s (501.87ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:     5269 H/s (507.43ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:     5314 H/s (502.86ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:    21227 H/s

Hashmode: 11400 - SIP digest authentication (MD5)

Speed.#1.........:  3620.7 MH/s (279.96ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  3624.5 MH/s (279.64ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  3591.9 MH/s (282.14ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  3626.2 MH/s (279.64ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 14463.3 MH/s

Hashmode: 11500 - CRC32

Speed.#1.........: 46093.1 MH/s (46.22ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 46041.0 MH/s (46.21ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 45546.2 MH/s (46.72ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 46197.6 MH/s (46.25ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   183.9 GH/s

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#1.........:   465.1 kH/s (464.25ms) @ Accel:256 Loops:4096 Thr:64 Vec:1
Speed.#2.........:   522.8 kH/s (462.13ms) @ Accel:256 Loops:4096 Thr:64 Vec:1
Speed.#3.........:   466.8 kH/s (465.98ms) @ Accel:256 Loops:4096 Thr:64 Vec:1
Speed.#4.........:   466.4 kH/s (463.25ms) @ Accel:256 Loops:4096 Thr:64 Vec:1
Speed.#*.........:  1921.1 kH/s

Hashmode: 11700 - GOST R 34.11-2012 (Streebog) 256-bit, big-endian

Speed.#1.........:   113.0 MH/s (296.60ms) @ Accel:128 Loops:64 Thr:64 Vec:1
Speed.#2.........:   112.3 MH/s (298.25ms) @ Accel:128 Loops:64 Thr:64 Vec:1
Speed.#3.........:   113.0 MH/s (296.59ms) @ Accel:128 Loops:64 Thr:64 Vec:1
Speed.#4.........:   113.2 MH/s (296.28ms) @ Accel:128 Loops:64 Thr:64 Vec:1
Speed.#*.........:   451.5 MH/s

Hashmode: 11750 - HMAC-Streebog-256 (key = $pass), big-endian

Speed.#1.........: 33739.2 kH/s (478.31ms) @ Accel:128 Loops:32 Thr:64 Vec:1
Speed.#2.........: 33799.7 kH/s (477.33ms) @ Accel:128 Loops:32 Thr:64 Vec:1
Speed.#3.........: 33525.5 kH/s (481.37ms) @ Accel:128 Loops:32 Thr:64 Vec:1
Speed.#4.........: 33764.2 kH/s (477.93ms) @ Accel:128 Loops:32 Thr:64 Vec:1
Speed.#*.........:   134.8 MH/s

Hashmode: 11760 - HMAC-Streebog-256 (key = $salt), big-endian

Speed.#1.........: 43908.8 kH/s (362.03ms) @ Accel:64 Loops:64 Thr:64 Vec:1
Speed.#2.........: 43630.2 kH/s (364.39ms) @ Accel:64 Loops:64 Thr:64 Vec:1
Speed.#3.........: 43746.2 kH/s (363.46ms) @ Accel:64 Loops:64 Thr:64 Vec:1
Speed.#4.........: 43950.7 kH/s (361.72ms) @ Accel:64 Loops:64 Thr:64 Vec:1
Speed.#*.........:   175.2 MH/s

Hashmode: 11800 - GOST R 34.11-2012 (Streebog) 512-bit, big-endian

Speed.#1.........:   109.2 MH/s (306.82ms) @ Accel:32 Loops:256 Thr:64 Vec:1
Speed.#2.........:   108.7 MH/s (308.27ms) @ Accel:32 Loops:256 Thr:64 Vec:1
Speed.#3.........:   109.4 MH/s (306.20ms) @ Accel:32 Loops:256 Thr:64 Vec:1
Speed.#4.........:   109.4 MH/s (306.34ms) @ Accel:32 Loops:256 Thr:64 Vec:1
Speed.#*.........:   436.8 MH/s

Hashmode: 11850 - HMAC-Streebog-512 (key = $pass), big-endian

Speed.#1.........: 28974.4 kH/s (270.65ms) @ Accel:64 Loops:32 Thr:64 Vec:1
Speed.#2.........: 28907.4 kH/s (271.25ms) @ Accel:64 Loops:32 Thr:64 Vec:1
Speed.#3.........: 28843.0 kH/s (271.82ms) @ Accel:64 Loops:32 Thr:64 Vec:1
Speed.#4.........: 28858.5 kH/s (271.97ms) @ Accel:64 Loops:32 Thr:64 Vec:1
Speed.#*.........:   115.6 MH/s

Hashmode: 11860 - HMAC-Streebog-512 (key = $salt), big-endian

Speed.#1.........: 39323.3 kH/s (408.21ms) @ Accel:64 Loops:64 Thr:64 Vec:1
Speed.#2.........: 39086.6 kH/s (410.87ms) @ Accel:64 Loops:64 Thr:64 Vec:1
Speed.#3.........: 39432.2 kH/s (406.92ms) @ Accel:64 Loops:64 Thr:64 Vec:1
Speed.#4.........: 39274.3 kH/s (409.02ms) @ Accel:64 Loops:64 Thr:64 Vec:1
Speed.#*.........:   157.1 MH/s

Hashmode: 11900 - PBKDF2-HMAC-MD5 (Iterations: 999)

Speed.#1.........:  9288.2 kH/s (218.21ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#2.........:  9279.3 kH/s (218.81ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#3.........:  9149.6 kH/s (221.50ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#4.........:  9338.9 kH/s (217.31ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#*.........: 37055.9 kH/s

Hashmode: 12000 - PBKDF2-HMAC-SHA1 (Iterations: 999)

Speed.#1.........:  4243.8 kH/s (485.70ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#2.........:  4241.7 kH/s (485.96ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#3.........:  4177.8 kH/s (493.52ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#4.........:  4238.0 kH/s (485.93ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#*.........: 16901.3 kH/s

Hashmode: 12001 - Atlassian (PBKDF2-HMAC-SHA1) (Iterations: 9999)

Speed.#1.........:   425.8 kH/s (503.07ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   426.2 kH/s (502.63ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   422.7 kH/s (506.82ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   426.3 kH/s (502.62ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  1701.1 kH/s

Hashmode: 12100 - PBKDF2-HMAC-SHA512 (Iterations: 999)

Speed.#1.........:   476.5 kH/s (241.61ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#2.........:   476.2 kH/s (241.90ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#3.........:   471.0 kH/s (243.61ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#4.........:   477.2 kH/s (241.04ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#*.........:  1900.9 kH/s

Hashmode: 12200 - eCryptfs (Iterations: 65536)

Speed.#1.........:    16083 H/s (507.07ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#2.........:    16150 H/s (505.45ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#3.........:    16003 H/s (510.38ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#4.........:    16140 H/s (505.93ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#*.........:    64376 H/s

Hashmode: 12300 - Oracle T: Type (Oracle 12+) (Iterations: 4095)

Speed.#1.........:   116.1 kH/s (279.14ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   117.6 kH/s (277.51ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   115.1 kH/s (281.48ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   116.3 kH/s (278.79ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   465.0 kH/s

Hashmode: 12400 - BSDi Crypt, Extended DES (Iterations: 2194)

Speed.#1.........:  5021.7 kH/s (136.07ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  5026.0 kH/s (135.95ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4961.1 kH/s (137.65ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  5047.6 kH/s (135.58ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 20056.4 kH/s

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#1.........:    62258 H/s (262.12ms) @ Accel:64 Loops:16384 Thr:64 Vec:1
Speed.#2.........:    62456 H/s (261.31ms) @ Accel:64 Loops:16384 Thr:64 Vec:1
Speed.#3.........:    62153 H/s (262.73ms) @ Accel:64 Loops:16384 Thr:64 Vec:1
Speed.#4.........:    62612 H/s (260.81ms) @ Accel:64 Loops:16384 Thr:64 Vec:1
Speed.#*.........:   249.5 kH/s

Hashmode: 12600 - ColdFusion 10+

Speed.#1.........:  2639.0 MH/s (406.45ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  2639.8 MH/s (406.32ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  2616.7 MH/s (409.88ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  2643.7 MH/s (405.93ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 10539.2 MH/s

Hashmode: 12700 - Blockchain, My Wallet (Iterations: 9)

Speed.#1.........: 87733.0 kH/s (10.32ms) @ Accel:512 Loops:9 Thr:64 Vec:1
Speed.#2.........: 88962.5 kH/s (10.24ms) @ Accel:512 Loops:9 Thr:64 Vec:1
Speed.#3.........: 87659.9 kH/s (10.28ms) @ Accel:512 Loops:9 Thr:64 Vec:1
Speed.#4.........: 89243.5 kH/s (10.52ms) @ Accel:512 Loops:9 Thr:64 Vec:1
Speed.#*.........:   353.6 MH/s

Hashmode: 12800 - MS-AzureSync PBKDF2-HMAC-SHA256 (Iterations: 99)

Speed.#1.........: 17257.2 kH/s (111.19ms) @ Accel:512 Loops:99 Thr:64 Vec:1
Speed.#2.........: 17275.5 kH/s (111.09ms) @ Accel:512 Loops:99 Thr:64 Vec:1
Speed.#3.........: 17063.2 kH/s (112.45ms) @ Accel:512 Loops:99 Thr:64 Vec:1
Speed.#4.........: 17439.9 kH/s (110.30ms) @ Accel:512 Loops:99 Thr:64 Vec:1
Speed.#*.........: 69035.7 kH/s

Hashmode: 12900 - Android FDE (Samsung DEK) (Iterations: 4095)

Speed.#1.........:   450.8 kH/s (289.10ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   451.3 kH/s (288.94ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   447.9 kH/s (291.33ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   451.5 kH/s (288.99ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  1801.6 kH/s

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#1.........:    56584 H/s (288.75ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:    56714 H/s (288.17ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:    56082 H/s (291.40ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:    56666 H/s (288.51ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   226.0 kH/s

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#1.........:   324.6 MH/s (413.21ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#2.........:   322.9 MH/s (415.29ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:   325.7 MH/s (411.61ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:   324.6 MH/s (413.24ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  1297.8 MH/s

Hashmode: 13200 - AxCrypt 1 (Iterations: 10467)

Speed.#1.........:   299.6 kH/s (683.36ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   298.7 kH/s (685.41ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   297.5 kH/s (688.39ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   300.0 kH/s (682.84ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  1195.8 kH/s

Hashmode: 13300 - AxCrypt 1 in-memory SHA1

Speed.#1.........: 10004.0 MH/s (214.27ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10028.4 MH/s (213.73ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9920.1 MH/s (216.03ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10039.7 MH/s (213.67ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 39992.1 MH/s

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#1.........:    91725 H/s (951.19ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:    91557 H/s (952.91ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:    90904 H/s (960.10ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:    91795 H/s (950.60ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   366.0 kH/s

Hashmode: 13500 - PeopleSoft PS_TOKEN

Speed.#1.........:  7581.9 MH/s (282.83ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  7591.8 MH/s (282.43ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  7511.4 MH/s (285.45ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  7599.7 MH/s (282.34ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 30284.8 MH/s

Hashmode: 13600 - WinZip (Iterations: 999)

Speed.#1.........:  4210.2 kH/s (483.99ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#2.........:  4207.6 kH/s (484.90ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#3.........:  4123.4 kH/s (495.12ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#4.........:  4224.7 kH/s (482.35ms) @ Accel:512 Loops:999 Thr:64 Vec:1
Speed.#*.........: 16766.0 kH/s

Hashmode: 13711 - VeraCrypt RIPEMD160 + XTS 512 bit (Iterations: 655330)

Speed.#1.........:     1177 H/s (169.48ms) @ Accel:128 Loops:500 Thr:64 Vec:1
Speed.#2.........:     1177 H/s (169.52ms) @ Accel:128 Loops:500 Thr:64 Vec:1
Speed.#3.........:     1165 H/s (171.28ms) @ Accel:128 Loops:500 Thr:64 Vec:1
Speed.#4.........:     1177 H/s (169.54ms) @ Accel:128 Loops:500 Thr:64 Vec:1
Speed.#*.........:     4696 H/s

Hashmode: 13712 - VeraCrypt RIPEMD160 + XTS 1024 bit (Iterations: 655330)

Speed.#1.........:      667 H/s (148.67ms) @ Accel:32 Loops:1000 Thr:64 Vec:1
Speed.#2.........:      667 H/s (148.72ms) @ Accel:32 Loops:1000 Thr:64 Vec:1
Speed.#3.........:      655 H/s (151.46ms) @ Accel:32 Loops:1000 Thr:64 Vec:1
Speed.#4.........:      668 H/s (149.23ms) @ Accel:32 Loops:1000 Thr:64 Vec:1
Speed.#*.........:     2658 H/s

Hashmode: 13713 - VeraCrypt RIPEMD160 + XTS 1536 bit (Iterations: 655330)

Speed.#1.........:      467 H/s (213.13ms) @ Accel:32 Loops:1000 Thr:64 Vec:1
Speed.#2.........:      467 H/s (213.09ms) @ Accel:32 Loops:1000 Thr:64 Vec:1
Speed.#3.........:      464 H/s (214.65ms) @ Accel:32 Loops:1000 Thr:64 Vec:1
Speed.#4.........:      469 H/s (212.40ms) @ Accel:32 Loops:1000 Thr:64 Vec:1
Speed.#*.........:     1868 H/s

Hashmode: 13721 - VeraCrypt SHA512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:      955 H/s (136.69ms) @ Accel:32 Loops:1000 Thr:64 Vec:1
Speed.#2.........:      958 H/s (136.55ms) @ Accel:32 Loops:1000 Thr:64 Vec:1
Speed.#3.........:      944 H/s (138.30ms) @ Accel:32 Loops:1000 Thr:64 Vec:1
Speed.#4.........:      957 H/s (136.53ms) @ Accel:32 Loops:1000 Thr:64 Vec:1
Speed.#*.........:     3814 H/s

Hashmode: 13722 - VeraCrypt SHA512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      475 H/s (136.91ms) @ Accel:16 Loops:1000 Thr:64 Vec:1
Speed.#2.........:      476 H/s (136.99ms) @ Accel:16 Loops:1000 Thr:64 Vec:1
Speed.#3.........:      471 H/s (138.22ms) @ Accel:16 Loops:1000 Thr:64 Vec:1
Speed.#4.........:      477 H/s (136.66ms) @ Accel:16 Loops:1000 Thr:64 Vec:1
Speed.#*.........:     1899 H/s

Hashmode: 13723 - VeraCrypt SHA512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      318 H/s (205.39ms) @ Accel:16 Loops:1000 Thr:64 Vec:1
Speed.#2.........:      317 H/s (205.74ms) @ Accel:16 Loops:1000 Thr:64 Vec:1
Speed.#3.........:      315 H/s (207.28ms) @ Accel:16 Loops:1000 Thr:64 Vec:1
Speed.#4.........:      319 H/s (204.97ms) @ Accel:16 Loops:1000 Thr:64 Vec:1
Speed.#*.........:     1268 H/s

Hashmode: 13731 - VeraCrypt Whirlpool + XTS 512 bit (Iterations: 499999)

Speed.#1.........:       64 H/s (126.32ms) @ Accel:64 Loops:31 Thr:64 Vec:1
Speed.#2.........:       63 H/s (127.02ms) @ Accel:64 Loops:31 Thr:64 Vec:1
Speed.#3.........:       64 H/s (126.07ms) @ Accel:64 Loops:31 Thr:64 Vec:1
Speed.#4.........:       64 H/s (126.33ms) @ Accel:64 Loops:31 Thr:64 Vec:1
Speed.#*.........:      255 H/s

Hashmode: 13732 - VeraCrypt Whirlpool + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:       31 H/s (129.73ms) @ Accel:32 Loops:31 Thr:64 Vec:1
Speed.#2.........:       31 H/s (130.33ms) @ Accel:32 Loops:31 Thr:64 Vec:1
Speed.#3.........:       31 H/s (129.51ms) @ Accel:32 Loops:31 Thr:64 Vec:1
Speed.#4.........:       31 H/s (129.71ms) @ Accel:32 Loops:31 Thr:64 Vec:1
Speed.#*.........:      124 H/s

Hashmode: 13733 - VeraCrypt Whirlpool + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:       21 H/s (194.70ms) @ Accel:32 Loops:31 Thr:64 Vec:1
Speed.#2.........:       20 H/s (196.06ms) @ Accel:32 Loops:31 Thr:64 Vec:1
Speed.#3.........:       21 H/s (194.24ms) @ Accel:32 Loops:31 Thr:64 Vec:1
Speed.#4.........:       21 H/s (194.74ms) @ Accel:32 Loops:31 Thr:64 Vec:1
Speed.#*.........:       82 H/s

Hashmode: 13741 - VeraCrypt RIPEMD160 + XTS 512 bit + boot-mode (Iterations: 327660)

Speed.#1.........:     2343 H/s (174.58ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#2.........:     2327 H/s (175.73ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#3.........:     2323 H/s (176.06ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#4.........:     2348 H/s (174.27ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#*.........:     9341 H/s

Hashmode: 13742 - VeraCrypt RIPEMD160 + XTS 1024 bit + boot-mode (Iterations: 327660)

Speed.#1.........:     1345 H/s (151.53ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#2.........:     1344 H/s (151.65ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#3.........:     1331 H/s (153.07ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#4.........:     1351 H/s (151.05ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#*.........:     5371 H/s

Hashmode: 13743 - VeraCrypt RIPEMD160 + XTS 1536 bit + boot-mode (Iterations: 327660)

Speed.#1.........:      936 H/s (218.17ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#2.........:      936 H/s (218.15ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#3.........:      928 H/s (219.94ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#4.........:      939 H/s (217.58ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#*.........:     3740 H/s

Hashmode: 13751 - VeraCrypt SHA256 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:     1743 H/s (150.13ms) @ Accel:128 Loops:500 Thr:64 Vec:1
Speed.#2.........:     1743 H/s (150.12ms) @ Accel:128 Loops:500 Thr:64 Vec:1
Speed.#3.........:     1726 H/s (151.51ms) @ Accel:128 Loops:500 Thr:64 Vec:1
Speed.#4.........:     1745 H/s (149.96ms) @ Accel:128 Loops:500 Thr:64 Vec:1
Speed.#*.........:     6956 H/s

Hashmode: 13752 - VeraCrypt SHA256 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:      869 H/s (150.30ms) @ Accel:128 Loops:250 Thr:64 Vec:1
Speed.#2.........:      869 H/s (150.18ms) @ Accel:128 Loops:250 Thr:64 Vec:1
Speed.#3.........:      861 H/s (151.57ms) @ Accel:128 Loops:250 Thr:64 Vec:1
Speed.#4.........:      871 H/s (149.81ms) @ Accel:128 Loops:250 Thr:64 Vec:1
Speed.#*.........:     3470 H/s

Hashmode: 13753 - VeraCrypt SHA256 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:      580 H/s (225.33ms) @ Accel:128 Loops:250 Thr:64 Vec:1
Speed.#2.........:      580 H/s (225.14ms) @ Accel:128 Loops:250 Thr:64 Vec:1
Speed.#3.........:      575 H/s (226.95ms) @ Accel:128 Loops:250 Thr:64 Vec:1
Speed.#4.........:      582 H/s (224.51ms) @ Accel:128 Loops:250 Thr:64 Vec:1
Speed.#*.........:     2317 H/s

Hashmode: 13761 - VeraCrypt SHA256 + XTS 512 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     4327 H/s (154.76ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:     4332 H/s (154.55ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:     4296 H/s (155.81ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#4.........:     4346 H/s (154.13ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:    17301 H/s

Hashmode: 13762 - VeraCrypt SHA256 + XTS 1024 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     2164 H/s (154.25ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#2.........:     2171 H/s (153.94ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#3.........:     2151 H/s (155.31ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#4.........:     2178 H/s (153.53ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#*.........:     8663 H/s

Hashmode: 13763 - VeraCrypt SHA256 + XTS 1536 bit + boot-mode (Iterations: 199999)

Speed.#1.........:     1446 H/s (231.24ms) @ Accel:128 Loops:256 Thr:64 Vec:1
Speed.#2.........:     1447 H/s (231.17ms) @ Accel:128 Loops:256 Thr:64 Vec:1
Speed.#3.........:     1436 H/s (232.75ms) @ Accel:128 Loops:256 Thr:64 Vec:1
Speed.#4.........:     1453 H/s (230.21ms) @ Accel:128 Loops:256 Thr:64 Vec:1
Speed.#*.........:     5781 H/s

Hashmode: 13771 - VeraCrypt Streebog-512 + XTS 512 bit (Iterations: 499999)

Speed.#1.........:       72 H/s (223.15ms) @ Accel:64 Loops:62 Thr:64 Vec:1
Speed.#2.........:       72 H/s (224.73ms) @ Accel:64 Loops:62 Thr:64 Vec:1
Speed.#3.........:       72 H/s (223.12ms) @ Accel:64 Loops:62 Thr:64 Vec:1
Speed.#4.........:       72 H/s (223.18ms) @ Accel:64 Loops:62 Thr:64 Vec:1
Speed.#*.........:      289 H/s

Hashmode: 13772 - VeraCrypt Streebog-512 + XTS 1024 bit (Iterations: 499999)

Speed.#1.........:       35 H/s (227.26ms) @ Accel:32 Loops:62 Thr:64 Vec:1
Speed.#2.........:       35 H/s (227.39ms) @ Accel:32 Loops:62 Thr:64 Vec:1
Speed.#3.........:       36 H/s (225.72ms) @ Accel:32 Loops:62 Thr:64 Vec:1
Speed.#4.........:       36 H/s (225.29ms) @ Accel:32 Loops:62 Thr:64 Vec:1
Speed.#*.........:      142 H/s

Hashmode: 13773 - VeraCrypt Streebog-512 + XTS 1536 bit (Iterations: 499999)

Speed.#1.........:       22 H/s (269.83ms) @ Accel:512 Loops:3 Thr:64 Vec:1
Speed.#2.........:       22 H/s (271.85ms) @ Accel:512 Loops:3 Thr:64 Vec:1
Speed.#3.........:       22 H/s (269.76ms) @ Accel:512 Loops:3 Thr:64 Vec:1
Speed.#4.........:       22 H/s (268.96ms) @ Accel:512 Loops:3 Thr:64 Vec:1
Speed.#*.........:       87 H/s

Hashmode: 13800 - Windows Phone 8+ PIN/password

Speed.#1.........:  1078.5 MH/s (248.56ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1077.8 MH/s (248.61ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1068.5 MH/s (250.77ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1082.3 MH/s (247.78ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  4307.1 MH/s

Hashmode: 13900 - OpenCart

Speed.#1.........:  2711.9 MH/s (395.54ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  2713.4 MH/s (395.29ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  2688.3 MH/s (398.95ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  2718.0 MH/s (394.77ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 10831.6 MH/s

Hashmode: 14000 - DES (PT = $salt, key = $pass)

Speed.#1.........: 23750.0 MH/s (89.86ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 23786.7 MH/s (89.71ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 23547.8 MH/s (90.63ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 23886.2 MH/s (89.54ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 94970.7 MH/s

Hashmode: 14100 - 3DES (PT = $salt, key = $pass)

Speed.#1.........:  5319.0 MH/s (403.29ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  5309.0 MH/s (404.06ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  5262.5 MH/s (407.61ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  5333.0 MH/s (402.41ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 21223.5 MH/s

Hashmode: 14400 - sha1(CX)

Speed.#1.........:   475.3 MH/s (281.94ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#2.........:   476.4 MH/s (281.36ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#3.........:   472.0 MH/s (283.93ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#4.........:   476.5 MH/s (281.44ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#*.........:  1900.2 MH/s

Hashmode: 14600 - LUKS (Iterations: 163044)

Speed.#1.........:    13060 H/s (503.02ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:    13093 H/s (502.01ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:    12984 H/s (506.27ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:    13105 H/s (501.44ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:    52242 H/s

Hashmode: 14700 - iTunes backup < 10.0 (Iterations: 9999)

Speed.#1.........:   212.6 kH/s (503.98ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   213.2 kH/s (502.74ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   211.6 kH/s (506.61ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   213.2 kH/s (502.74ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   850.7 kH/s

Hashmode: 14800 - iTunes backup >= 10.0 (Iterations: 9999999)

Speed.#1.........:      176 H/s (303.53ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:      177 H/s (302.90ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:      175 H/s (305.68ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:      177 H/s (302.90ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:      705 H/s

Hashmode: 14900 - Skip32 (PT = $salt, key = $pass)

Speed.#1.........:  3597.2 MH/s (4.24ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  3596.7 MH/s (4.28ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  3607.5 MH/s (4.22ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  3736.4 MH/s (4.25ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 14537.7 MH/s

Hashmode: 15000 - FileZilla Server >= 0.9.55

Speed.#1.........:  1129.8 MH/s (474.75ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#2.........:  1132.2 MH/s (473.85ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#3.........:  1119.1 MH/s (479.36ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#4.........:  1132.5 MH/s (473.78ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#*.........:  4513.6 MH/s

Hashmode: 15100 - Juniper/NetBSD sha1crypt (Iterations: 19999)

Speed.#1.........:   216.8 kH/s (494.16ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   217.2 kH/s (493.25ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   214.8 kH/s (498.75ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   217.5 kH/s (492.85ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   866.4 kH/s

Hashmode: 15200 - Blockchain, My Wallet, V2 (Iterations: 4999)

Speed.#1.........:   425.0 kH/s (503.93ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#2.........:   426.0 kH/s (502.84ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#3.........:   422.4 kH/s (507.18ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#4.........:   425.5 kH/s (503.23ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#*.........:  1698.9 kH/s

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

Speed.#1.........:    89012 H/s (501.48ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:    89290 H/s (499.99ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:    87922 H/s (507.80ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:    88988 H/s (500.51ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   355.2 kH/s

Hashmode: 15400 - ChaCha20

Speed.#1.........:  5732.7 MH/s (374.18ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  5749.3 MH/s (373.07ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  5703.2 MH/s (376.19ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  5754.4 MH/s (372.92ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 22939.6 MH/s

Hashmode: 15500 - JKS Java Key Store Private Keys (SHA1)

Speed.#1.........: 10349.6 MH/s (207.03ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10368.8 MH/s (206.77ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10239.0 MH/s (209.27ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10375.5 MH/s (206.73ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 41332.8 MH/s

Hashmode: 15600 - Ethereum Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1023)

Speed.#1.........:  1773.0 kH/s (290.16ms) @ Accel:128 Loops:1023 Thr:64 Vec:1
Speed.#2.........:  1809.4 kH/s (285.92ms) @ Accel:128 Loops:1023 Thr:64 Vec:1
Speed.#3.........:  1779.1 kH/s (290.50ms) @ Accel:128 Loops:1023 Thr:64 Vec:1
Speed.#4.........:  1775.7 kH/s (290.20ms) @ Accel:128 Loops:1023 Thr:64 Vec:1
Speed.#*.........:  7137.1 kH/s

Hashmode: 15700 - Ethereum Wallet, SCRYPT (Iterations: 1)

Speed.#1.........:        0 H/s (317151.47ms) @ Accel:1 Loops:1 Thr:1 Vec:1
Speed.#2.........:        0 H/s (319702.14ms) @ Accel:1 Loops:1 Thr:1 Vec:1
Speed.#3.........:        0 H/s (316258.95ms) @ Accel:1 Loops:1 Thr:1 Vec:1
Speed.#4.........:        0 H/s (318252.73ms) @ Accel:1 Loops:1 Thr:1 Vec:1
Speed.#*.........:        1 H/s

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

Speed.#1.........:    37019 H/s (280.28ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#2.........:    36781 H/s (281.65ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#3.........:    36570 H/s (283.23ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#4.........:    36972 H/s (280.31ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#*.........:   147.3 kH/s

Hashmode: 16000 - Tripcode

Speed.#1.........:   398.1 MH/s (336.83ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#2.........:   397.1 MH/s (337.57ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:   394.4 MH/s (339.82ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:   398.5 MH/s (336.58ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  1588.1 MH/s

Hashmode: 16100 - TACACS+

Speed.#1.........: 18365.2 MH/s (116.49ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 18311.9 MH/s (116.85ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 18173.1 MH/s (117.74ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 18396.8 MH/s (116.49ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 73247.0 MH/s

Hashmode: 16200 - Apple Secure Notes (Iterations: 19999)

Speed.#1.........:    91666 H/s (292.40ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:    91535 H/s (292.73ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:    90779 H/s (295.20ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:    91735 H/s (292.28ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   365.7 kH/s

Hashmode: 16300 - Ethereum Pre-Sale Wallet, PBKDF2-HMAC-SHA256 (Iterations: 1999)

Speed.#1.........:   913.4 kH/s (282.48ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   910.8 kH/s (283.42ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   901.2 kH/s (286.34ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   915.0 kH/s (282.12ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  3640.5 kH/s

Hashmode: 16400 - CRAM-MD5 Dovecot

Speed.#1.........: 30971.6 MH/s (69.01ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 30892.1 MH/s (69.08ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 30635.7 MH/s (69.66ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 31026.8 MH/s (68.98ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   123.5 GH/s

Hashmode: 16500 - JWT (JSON Web Token)

Speed.#1.........:   865.0 MH/s (309.99ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:   865.0 MH/s (309.91ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:   857.9 MH/s (312.42ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#4.........:   865.5 MH/s (309.90ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:  3453.5 MH/s

Hashmode: 16600 - Electrum Wallet (Salt-Type 1-3)

Speed.#1.........:   673.2 MH/s (398.36ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:   672.2 MH/s (398.87ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:   668.3 MH/s (401.20ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#4.........:   674.7 MH/s (397.62ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:  2688.5 MH/s

Hashmode: 16700 - FileVault 2 (Iterations: 19999)

Speed.#1.........:    91183 H/s (293.81ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#2.........:    91226 H/s (293.46ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#3.........:    90526 H/s (295.66ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#4.........:    91346 H/s (293.21ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#*.........:   364.3 kH/s

Hashmode: 16800 - WPA-PMKID-PBKDF2 (Iterations: 4095)

Speed.#1.........:   515.4 kH/s (506.39ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   516.9 kH/s (505.55ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   512.7 kH/s (509.80ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   515.6 kH/s (506.41ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  2060.6 kH/s

Hashmode: 16801 - WPA-PMKID-PMK (Iterations: 0)

Speed.#1.........:   326.7 MH/s (0.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   337.6 MH/s (0.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   322.0 MH/s (0.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   340.7 MH/s (0.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  1327.0 MH/s

Hashmode: 16900 - Ansible Vault (Iterations: 9999)

Speed.#1.........:   184.4 kH/s (283.77ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   184.5 kH/s (283.52ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   182.3 kH/s (286.99ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   184.5 kH/s (283.56ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   735.7 kH/s

Hashmode: 17200 - PKZIP (Compressed)

* Device #1: Skipping hash-mode 17200 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #2: Skipping hash-mode 17200 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #3: Skipping hash-mode 17200 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #4: Skipping hash-mode 17200 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
Speed.#*.........:        0 H/s

Hashmode: 17210 - PKZIP (Uncompressed)

Speed.#1.........:  1186.4 MH/s (225.81ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:  1171.7 MH/s (228.67ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:  1193.1 MH/s (224.56ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:  1181.9 MH/s (226.88ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  4733.1 MH/s

Hashmode: 17220 - PKZIP (Compressed Multi-File)

* Device #1: Skipping hash-mode 17220 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #2: Skipping hash-mode 17220 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #3: Skipping hash-mode 17220 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #4: Skipping hash-mode 17220 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
Speed.#*.........:        0 H/s

Hashmode: 17225 - PKZIP (Mixed Multi-File)

* Device #1: Skipping hash-mode 17225 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #2: Skipping hash-mode 17225 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #3: Skipping hash-mode 17225 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #4: Skipping hash-mode 17225 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
Speed.#*.........:        0 H/s

Hashmode: 17230 - PKZIP (Mixed Multi-File Checksum-Only)

Speed.#1.........: 11455.0 MH/s (187.15ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 11467.4 MH/s (186.90ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 11350.2 MH/s (188.76ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 11478.1 MH/s (186.86ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 45750.7 MH/s

Hashmode: 17300 - SHA3-224

Speed.#1.........:   766.1 MH/s (350.04ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:   766.8 MH/s (349.59ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:   759.4 MH/s (353.02ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:   768.4 MH/s (349.07ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  3060.8 MH/s

Hashmode: 17400 - SHA3-256

Speed.#1.........:   765.1 MH/s (350.42ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:   766.5 MH/s (349.77ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:   759.4 MH/s (353.03ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#4.........:   767.4 MH/s (349.55ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:  3058.5 MH/s

Hashmode: 17500 - SHA3-384

Speed.#1.........:   764.0 MH/s (350.91ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:   764.9 MH/s (350.57ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:   757.9 MH/s (353.70ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#4.........:   766.0 MH/s (350.17ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:  3052.8 MH/s

Hashmode: 17600 - SHA3-512

Speed.#1.........:   765.0 MH/s (350.53ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:   764.6 MH/s (350.63ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:   758.0 MH/s (353.77ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#4.........:   765.5 MH/s (350.41ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:  3053.1 MH/s

Hashmode: 17700 - Keccak-224

Speed.#1.........:   766.6 MH/s (349.81ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#2.........:   767.4 MH/s (349.41ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#3.........:   760.3 MH/s (352.65ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#4.........:   768.6 MH/s (349.02ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#*.........:  3063.0 MH/s

Hashmode: 17800 - Keccak-256

Speed.#1.........:   766.1 MH/s (349.97ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#2.........:   767.5 MH/s (349.34ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#3.........:   760.5 MH/s (352.60ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#4.........:   768.1 MH/s (349.25ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#*.........:  3062.1 MH/s

Hashmode: 17900 - Keccak-384

Speed.#1.........:   765.6 MH/s (350.21ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:   766.3 MH/s (349.93ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:   759.4 MH/s (353.01ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#4.........:   768.0 MH/s (349.25ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:  3059.4 MH/s

Hashmode: 18000 - Keccak-512

Speed.#1.........:   764.3 MH/s (350.81ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   765.4 MH/s (350.28ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   758.6 MH/s (353.39ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   766.0 MH/s (350.18ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  3054.3 MH/s

Hashmode: 18100 - TOTP (HMAC-SHA1)

Speed.#1.........:  2083.4 MH/s (257.25ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  2087.2 MH/s (256.78ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  2065.0 MH/s (259.55ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  2089.1 MH/s (256.74ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  8324.7 MH/s

Hashmode: 18200 - Kerberos 5, etype 23, AS-REP

Speed.#1.........:   322.2 MH/s (416.06ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#2.........:   321.2 MH/s (417.42ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:   323.5 MH/s (414.47ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:   322.1 MH/s (416.47ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  1289.1 MH/s

Hashmode: 18300 - Apple File System (APFS) (Iterations: 19999)

Speed.#1.........:    92405 H/s (289.84ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#2.........:    92544 H/s (289.20ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#3.........:    91513 H/s (292.45ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#4.........:    92574 H/s (289.50ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#*.........:   369.0 kH/s

Hashmode: 18400 - Open Document Format (ODF) 1.2 (SHA-256, AES) (Iterations: 99999)

Speed.#1.........:    21352 H/s (501.97ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:    21439 H/s (499.93ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:    21233 H/s (504.94ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:    21422 H/s (500.52ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:    85446 H/s

Hashmode: 18500 - sha1(md5(md5($pass)))

Speed.#1.........:  4024.3 MH/s (266.39ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#2.........:  4031.0 MH/s (265.97ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#3.........:  3978.5 MH/s (269.40ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#4.........:  4024.4 MH/s (266.55ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#*.........: 16058.2 MH/s

Hashmode: 18600 - Open Document Format (ODF) 1.1 (SHA-1, Blowfish) (Iterations: 1023)

Speed.#1.........:   610.1 kH/s (284.83ms) @ Accel:1024 Loops:511 Thr:16 Vec:1
Speed.#2.........:   607.8 kH/s (285.16ms) @ Accel:1024 Loops:511 Thr:16 Vec:1
Speed.#3.........:   611.6 kH/s (284.47ms) @ Accel:1024 Loops:511 Thr:16 Vec:1
Speed.#4.........:   611.4 kH/s (282.20ms) @ Accel:1024 Loops:511 Thr:16 Vec:1
Speed.#*.........:  2441.0 kH/s

Hashmode: 18700 - Java Object hashCode()

Speed.#1.........:   103.0 GH/s (20.48ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   102.3 GH/s (20.64ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   104.0 GH/s (20.34ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   104.2 GH/s (20.43ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   413.6 GH/s

Hashmode: 18800 - Blockchain, My Wallet, Second Password (SHA256) (Iterations: 9999)

Speed.#1.........:   366.6 kH/s (292.21ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#2.........:   367.6 kH/s (291.47ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#3.........:   363.3 kH/s (295.00ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#4.........:   367.1 kH/s (291.96ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#*.........:  1464.6 kH/s

Hashmode: 18900 - Android Backup (Iterations: 9999)

Speed.#1.........:   213.1 kH/s (502.90ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   213.9 kH/s (501.10ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   211.9 kH/s (505.82ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   213.5 kH/s (502.06ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   852.4 kH/s

Hashmode: 19000 - QNX /etc/shadow (MD5) (Iterations: 1000)

Speed.#1.........:  8281.7 kH/s (246.20ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#2.........:  8255.7 kH/s (247.12ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#3.........:  8261.9 kH/s (246.97ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#4.........:  8365.9 kH/s (244.06ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#*.........: 33165.3 kH/s

Hashmode: 19100 - QNX /etc/shadow (SHA256) (Iterations: 1000)

Speed.#1.........:  7816.8 kH/s (261.29ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#2.........:  7854.2 kH/s (259.93ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#3.........:  7717.5 kH/s (264.63ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#4.........:  7866.6 kH/s (259.85ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#*.........: 31255.2 kH/s

Hashmode: 19200 - QNX /etc/shadow (SHA512) (Iterations: 1000)

Speed.#1.........:  5198.9 kH/s (377.90ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#2.........:  5163.0 kH/s (380.36ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#3.........:  5136.4 kH/s (382.77ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#4.........:  5197.5 kH/s (378.28ms) @ Accel:512 Loops:1000 Thr:64 Vec:1
Speed.#*.........: 20695.7 kH/s

Hashmode: 19300 - sha1($salt1.$pass.$salt2)

Speed.#1.........:   593.1 MH/s (452.26ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   591.9 MH/s (453.06ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   593.6 MH/s (451.76ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   593.7 MH/s (451.87ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  2372.3 MH/s

Hashmode: 19500 - Ruby on Rails Restful-Authentication

Speed.#1.........:   170.4 MH/s (393.42ms) @ Accel:16 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   169.6 MH/s (395.44ms) @ Accel:16 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   171.2 MH/s (391.48ms) @ Accel:16 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   171.1 MH/s (391.87ms) @ Accel:16 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   682.3 MH/s

Hashmode: 19600 - Kerberos 5, etype 17, TGS-REP (Iterations: 4095)

Speed.#1.........:  1042.1 kH/s (499.86ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1044.6 kH/s (498.78ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1034.0 kH/s (503.87ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1044.6 kH/s (498.95ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  4165.2 kH/s

Hashmode: 19700 - Kerberos 5, etype 18, TGS-REP (Iterations: 4095)

Speed.#1.........:   518.6 kH/s (502.53ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   520.5 kH/s (500.56ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   515.9 kH/s (505.24ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   519.4 kH/s (501.63ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  2074.3 kH/s

Hashmode: 19800 - Kerberos 5, etype 17, Pre-Auth (Iterations: 4095)

Speed.#1.........:  1037.9 kH/s (501.92ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1041.7 kH/s (500.14ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1030.6 kH/s (505.60ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1040.8 kH/s (500.53ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  4151.0 kH/s

Hashmode: 19900 - Kerberos 5, etype 18, Pre-Auth (Iterations: 4095)

Speed.#1.........:   519.1 kH/s (503.20ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#2.........:   520.7 kH/s (501.78ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#3.........:   516.2 kH/s (506.35ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#4.........:   520.3 kH/s (502.23ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#*.........:  2076.4 kH/s

Hashmode: 20011 - DiskCryptor SHA512 + XTS 512 bit (Iterations: 999)

Speed.#1.........:   473.5 kH/s (240.50ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#2.........:   474.3 kH/s (240.25ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#3.........:   468.3 kH/s (242.36ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#4.........:   474.0 kH/s (240.21ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#*.........:  1890.2 kH/s

Hashmode: 20012 - DiskCryptor SHA512 + XTS 1024 bit (Iterations: 999)

Speed.#1.........:   236.1 kH/s (266.47ms) @ Accel:16 Loops:999 Thr:64 Vec:1
Speed.#2.........:   235.0 kH/s (268.35ms) @ Accel:16 Loops:999 Thr:64 Vec:1
Speed.#3.........:   234.0 kH/s (269.19ms) @ Accel:16 Loops:999 Thr:64 Vec:1
Speed.#4.........:   236.0 kH/s (267.05ms) @ Accel:16 Loops:999 Thr:64 Vec:1
Speed.#*.........:   941.2 kH/s

Hashmode: 20013 - DiskCryptor SHA512 + XTS 1536 bit (Iterations: 999)

Speed.#1.........:   157.3 kH/s (358.64ms) @ Accel:128 Loops:124 Thr:64 Vec:1
Speed.#2.........:   157.7 kH/s (358.14ms) @ Accel:128 Loops:124 Thr:64 Vec:1
Speed.#3.........:   155.8 kH/s (361.57ms) @ Accel:128 Loops:124 Thr:64 Vec:1
Speed.#4.........:   157.4 kH/s (358.48ms) @ Accel:128 Loops:124 Thr:64 Vec:1
Speed.#*.........:   628.3 kH/s

Hashmode: 20200 - Python passlib pbkdf2-sha512 (Iterations: 24999)

Speed.#1.........:    19324 H/s (276.94ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#2.........:    19329 H/s (276.82ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#3.........:    19139 H/s (279.56ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#4.........:    19391 H/s (276.54ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#*.........:    77182 H/s

Hashmode: 20300 - Python passlib pbkdf2-sha256 (Iterations: 28999)

Speed.#1.........:    60902 H/s (303.18ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#2.........:    61034 H/s (302.38ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#3.........:    60427 H/s (305.51ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#4.........:    61025 H/s (302.68ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#*.........:   243.4 kH/s

Hashmode: 20400 - Python passlib pbkdf2-sha1 (Iterations: 130999)

Speed.#1.........:    32469 H/s (503.67ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:    32537 H/s (502.66ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:    32274 H/s (506.72ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:    32545 H/s (502.57ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   129.8 kH/s

Hashmode: 20500 - PKZIP Master Key

Speed.#1.........:   120.6 GH/s (17.38ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   121.3 GH/s (17.32ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   119.6 GH/s (17.57ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   122.5 GH/s (17.34ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   484.0 GH/s

Hashmode: 20510 - PKZIP Master Key (6 byte optimization)

Speed.#1.........: 10770.2 MH/s (199.04ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 10686.3 MH/s (200.52ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 10814.7 MH/s (198.12ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 10758.7 MH/s (199.37ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 43029.8 MH/s

Hashmode: 20600 - Oracle Transportation Management (SHA256) (Iterations: 999)

Speed.#1.........:  3678.1 kH/s (188.03ms) @ Accel:512 Loops:499 Thr:64 Vec:1
Speed.#2.........:  3676.5 kH/s (188.06ms) @ Accel:512 Loops:499 Thr:64 Vec:1
Speed.#3.........:  3620.0 kH/s (190.88ms) @ Accel:512 Loops:499 Thr:64 Vec:1
Speed.#4.........:  3691.2 kH/s (187.41ms) @ Accel:512 Loops:499 Thr:64 Vec:1
Speed.#*.........: 14665.8 kH/s

Hashmode: 20710 - sha256(sha256($pass).$salt)

Speed.#1.........:  1159.0 MH/s (462.81ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1161.4 MH/s (461.84ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1150.7 MH/s (466.16ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1161.2 MH/s (462.09ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  4632.2 MH/s

Hashmode: 20711 - AuthMe sha256

Speed.#1.........:  1064.1 MH/s (251.90ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1065.3 MH/s (251.65ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1054.1 MH/s (254.29ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1065.4 MH/s (251.71ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  4249.0 MH/s

Hashmode: 20800 - sha256(md5($pass))

Speed.#1.........:  3453.2 MH/s (310.58ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  3458.9 MH/s (310.01ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  3420.0 MH/s (313.53ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  3453.0 MH/s (310.71ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 13785.1 MH/s

Hashmode: 20900 - md5(sha1($pass).md5($pass).sha1($pass))

Speed.#1.........:  3260.1 MH/s (328.99ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#2.........:  3267.5 MH/s (328.18ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#3.........:  3233.3 MH/s (331.63ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#4.........:  3266.1 MH/s (328.51ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#*.........: 13027.0 MH/s

Hashmode: 21000 - BitShares v0.x - sha512(sha512_bin(pass))

Speed.#1.........:   547.5 MH/s (244.72ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#2.........:   548.1 MH/s (244.43ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:   541.8 MH/s (247.39ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:   547.7 MH/s (244.81ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  2185.1 MH/s

Hashmode: 21100 - sha1(md5($pass.$salt))

Speed.#1.........:  5875.8 MH/s (365.09ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  5880.0 MH/s (364.87ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  5815.5 MH/s (368.80ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  5880.7 MH/s (364.93ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 23451.9 MH/s

Hashmode: 21200 - md5(sha1($salt).md5($pass))

Speed.#1.........:  6635.1 MH/s (323.33ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  6639.7 MH/s (322.96ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  6566.2 MH/s (326.58ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  6641.2 MH/s (323.11ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 26482.2 MH/s

Hashmode: 21300 - md5($salt.sha1($salt.$pass))

Speed.#1.........:  3021.1 MH/s (355.05ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  3005.2 MH/s (356.87ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  3013.3 MH/s (355.87ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  3024.9 MH/s (354.74ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 12064.5 MH/s

Hashmode: 21400 - sha256(sha256_bin($pass))

Speed.#1.........:  2045.0 MH/s (262.20ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  2049.4 MH/s (261.51ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  2027.7 MH/s (264.32ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  2049.1 MH/s (261.76ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  8171.3 MH/s

Hashmode: 21500 - SolarWinds Orion (Iterations: 999)

Speed.#1.........:    81841 H/s (354.60ms) @ Accel:64 Loops:124 Thr:64 Vec:1
Speed.#2.........:    81943 H/s (354.17ms) @ Accel:64 Loops:124 Thr:64 Vec:1
Speed.#3.........:    81174 H/s (356.73ms) @ Accel:64 Loops:124 Thr:64 Vec:1
Speed.#4.........:    81845 H/s (354.00ms) @ Accel:64 Loops:124 Thr:64 Vec:1
Speed.#*.........:   326.8 kH/s

Hashmode: 21600 - Web2py pbkdf2-sha512 (Iterations: 999)

Speed.#1.........:   480.5 kH/s (239.55ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#2.........:   480.6 kH/s (239.72ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#3.........:   475.1 kH/s (242.36ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#4.........:   480.1 kH/s (239.13ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#*.........:  1916.2 kH/s

Hashmode: 21700 - Electrum Wallet (Salt-Type 4) (Iterations: 1023)

* Device #1: Skipping hash-mode 21700 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #2: Skipping hash-mode 21700 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #3: Skipping hash-mode 21700 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #4: Skipping hash-mode 21700 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
Speed.#*.........:        0 H/s

Hashmode: 21800 - Electrum Wallet (Salt-Type 5) (Iterations: 1023)

* Device #1: Skipping hash-mode 21800 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #2: Skipping hash-mode 21800 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #3: Skipping hash-mode 21800 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #4: Skipping hash-mode 21800 - known CUDA/OpenCL Runtime/Driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
Speed.#*.........:        0 H/s

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#1.........:   522.3 kH/s (500.04ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   524.4 kH/s (498.15ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   518.7 kH/s (503.81ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   523.4 kH/s (499.30ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  2088.9 kH/s

Hashmode: 22001 - WPA-PMK-PMKID+EAPOL (Iterations: 0)

Speed.#1.........:   322.9 MH/s (0.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   323.2 MH/s (0.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   329.2 MH/s (0.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   342.0 MH/s (0.00ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  1317.3 MH/s

Hashmode: 22100 - BitLocker (Iterations: 1048576)

Speed.#1.........:     2013 H/s (508.28ms) @ Accel:64 Loops:4096 Thr:64 Vec:1
Speed.#2.........:     2020 H/s (506.56ms) @ Accel:64 Loops:4096 Thr:64 Vec:1
Speed.#3.........:     1994 H/s (513.09ms) @ Accel:64 Loops:4096 Thr:64 Vec:1
Speed.#4.........:     2014 H/s (508.05ms) @ Accel:64 Loops:4096 Thr:64 Vec:1
Speed.#*.........:     8041 H/s

Hashmode: 22200 - Citrix NetScaler (SHA512)

Speed.#1.........:  1161.1 MH/s (461.99ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#2.........:  1163.8 MH/s (460.85ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#3.........:  1153.3 MH/s (465.09ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#4.........:  1163.8 MH/s (461.05ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#*.........:  4642.0 MH/s

Hashmode: 22300 - sha256($salt.$pass.$salt)

Speed.#1.........:  4034.7 MH/s (265.66ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4041.9 MH/s (265.19ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  3997.9 MH/s (268.10ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4044.3 MH/s (265.24ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 16118.8 MH/s

Hashmode: 22301 - Telegram Mobile App Passcode (SHA256)

Speed.#1.........:  4049.5 MH/s (264.71ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  4055.7 MH/s (264.38ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  4011.9 MH/s (267.20ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  4058.3 MH/s (264.34ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 16175.5 MH/s

Hashmode: 22400 - AES Crypt (SHA256) (Iterations: 8191)

Speed.#1.........:   416.0 kH/s (311.53ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   417.1 kH/s (310.66ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   412.7 kH/s (314.19ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   416.8 kH/s (311.03ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  1662.7 kH/s

Hashmode: 22500 - MultiBit Classic .key (MD5)

Speed.#1.........:   746.2 MH/s (359.41ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:   741.9 MH/s (361.35ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:   747.8 MH/s (358.49ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:   745.7 MH/s (359.75ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  2981.6 MH/s

Hashmode: 22600 - Telegram Desktop App Passcode (PBKDF2-HMAC-SHA1) (Iterations: 3999)

Speed.#1.........:   151.3 kH/s (430.21ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#2.........:   152.3 kH/s (428.70ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#3.........:   150.5 kH/s (432.77ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   151.7 kH/s (429.72ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   605.8 kH/s

Hashmode: 22700 - MultiBit HD (scrypt) (Iterations: 1)

Speed.#1.........:       29 H/s (35850.60ms) @ Accel:1 Loops:1 Thr:16 Vec:1
Speed.#2.........:       29 H/s (35851.61ms) @ Accel:1 Loops:1 Thr:16 Vec:1
Speed.#3.........:       29 H/s (35601.07ms) @ Accel:1 Loops:1 Thr:16 Vec:1
Speed.#4.........:       29 H/s (35833.01ms) @ Accel:1 Loops:1 Thr:16 Vec:1
Speed.#*.........:      114 H/s

Hashmode: 22911 - RSA/DSA/EC/OpenSSH Private Keys ($0$)

Speed.#1.........:   659.0 MH/s (406.94ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:   656.3 MH/s (408.58ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:   660.9 MH/s (405.75ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:   661.1 MH/s (405.79ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  2637.3 MH/s

Hashmode: 22921 - RSA/DSA/EC/OpenSSH Private Keys ($6$)

Speed.#1.........:  3008.6 MH/s (356.45ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#2.........:  3012.0 MH/s (356.06ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#3.........:  2977.2 MH/s (360.17ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#4.........:  3009.9 MH/s (356.47ms) @ Accel:512 Loops:512 Thr:64 Vec:1
Speed.#*.........: 12007.7 MH/s

Hashmode: 22931 - RSA/DSA/EC/OpenSSH Private Keys ($1, $3$)

Speed.#1.........:  1442.8 MH/s (371.60ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#2.........:  1437.0 MH/s (373.14ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#3.........:  1443.8 MH/s (371.36ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#4.........:  1446.3 MH/s (370.96ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#*.........:  5769.9 MH/s

Hashmode: 22941 - RSA/DSA/EC/OpenSSH Private Keys ($4$)

Speed.#1.........:   849.7 MH/s (315.47ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:   843.9 MH/s (317.73ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:   853.2 MH/s (314.15ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:   852.9 MH/s (314.59ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  3399.7 MH/s

Hashmode: 22951 - RSA/DSA/EC/OpenSSH Private Keys ($5$)

Speed.#1.........:   674.6 MH/s (397.44ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:   671.2 MH/s (399.45ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:   676.9 MH/s (396.17ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:   674.2 MH/s (397.92ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  2696.9 MH/s

Hashmode: 23001 - SecureZIP AES-128

Speed.#1.........:  1074.3 MH/s (249.43ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#2.........:  1071.7 MH/s (250.15ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#3.........:  1066.6 MH/s (251.22ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#4.........:  1075.3 MH/s (249.38ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#*.........:  4288.0 MH/s

Hashmode: 23002 - SecureZIP AES-192

Speed.#1.........:   784.4 MH/s (341.80ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#2.........:   783.9 MH/s (341.95ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#3.........:   777.4 MH/s (344.88ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:   785.3 MH/s (341.57ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  3131.0 MH/s

Hashmode: 23003 - SecureZIP AES-256

Speed.#1.........:   465.8 MH/s (287.66ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#2.........:   463.6 MH/s (289.15ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:   465.8 MH/s (287.72ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:   466.6 MH/s (287.41ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  1861.8 MH/s

Hashmode: 23100 - Apple Keychain (Iterations: 999)

Speed.#1.........:  2112.8 kH/s (490.60ms) @ Accel:256 Loops:999 Thr:64 Vec:1
Speed.#2.........:  2116.1 kH/s (489.53ms) @ Accel:256 Loops:999 Thr:64 Vec:1
Speed.#3.........:  2104.6 kH/s (492.76ms) @ Accel:256 Loops:999 Thr:64 Vec:1
Speed.#4.........:  2092.1 kH/s (493.65ms) @ Accel:256 Loops:999 Thr:64 Vec:1
Speed.#*.........:  8425.6 kH/s

Hashmode: 23200 - XMPP SCRAM PBKDF2-SHA1 (Iterations: 4095)

Speed.#1.........:  1045.7 kH/s (498.85ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1047.4 kH/s (498.11ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1035.5 kH/s (503.76ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1047.5 kH/s (498.19ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  4176.1 kH/s

Hashmode: 23300 - Apple iWork (Iterations: 3999)

Speed.#1.........:  1088.4 kH/s (478.33ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1085.8 kH/s (479.41ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1073.7 kH/s (484.80ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1087.3 kH/s (478.91ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  4335.1 kH/s

Hashmode: 23400 - Bitwarden (Iterations: 99999)

Speed.#1.........:    18479 H/s (289.81ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#2.........:    18507 H/s (289.38ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#3.........:    18280 H/s (292.78ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#4.........:    18499 H/s (289.70ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#*.........:    73766 H/s

Hashmode: 23500 - AxCrypt 2 AES-128 (Iterations: 999)

Speed.#1.........:    77950 H/s (148.92ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#2.........:    77515 H/s (149.80ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#3.........:    78091 H/s (148.50ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#4.........:    77962 H/s (149.00ms) @ Accel:256 Loops:124 Thr:64 Vec:1
Speed.#*.........:   311.5 kH/s

Hashmode: 23600 - AxCrypt 2 AES-256 (Iterations: 999)

Speed.#1.........:    38050 H/s (285.81ms) @ Accel:32 Loops:999 Thr:64 Vec:1
Speed.#2.........:    37914 H/s (287.46ms) @ Accel:32 Loops:999 Thr:64 Vec:1
Speed.#3.........:    38319 H/s (284.46ms) @ Accel:32 Loops:999 Thr:64 Vec:1
Speed.#4.........:    38142 H/s (285.88ms) @ Accel:32 Loops:999 Thr:64 Vec:1
Speed.#*.........:   152.4 kH/s

Hashmode: 23700 - RAR3-p (Uncompressed) (Iterations: 262144)

Speed.#1.........:    62198 H/s (262.52ms) @ Accel:64 Loops:16384 Thr:64 Vec:1
Speed.#2.........:    62468 H/s (261.42ms) @ Accel:64 Loops:16384 Thr:64 Vec:1
Speed.#3.........:    61985 H/s (263.46ms) @ Accel:64 Loops:16384 Thr:64 Vec:1
Speed.#4.........:    62391 H/s (261.79ms) @ Accel:64 Loops:16384 Thr:64 Vec:1
Speed.#*.........:   249.0 kH/s

Hashmode: 23800 - RAR3-p (Compressed) (Iterations: 262144)

Speed.#1.........:    62194 H/s (262.53ms) @ Accel:64 Loops:16384 Thr:64 Vec:1
Speed.#2.........:    62433 H/s (261.60ms) @ Accel:64 Loops:16384 Thr:64 Vec:1
Speed.#3.........:    61970 H/s (263.44ms) @ Accel:64 Loops:16384 Thr:64 Vec:1
Speed.#4.........:    62429 H/s (261.60ms) @ Accel:64 Loops:16384 Thr:64 Vec:1
Speed.#*.........:   249.0 kH/s

Hashmode: 23900 - BestCrypt v3 Volume Encryption (Iterations: 1)

Speed.#1.........:  2664.7 kH/s (381.00ms) @ Accel:256 Loops:1 Thr:64 Vec:1
Speed.#2.........:  2669.2 kH/s (379.93ms) @ Accel:256 Loops:1 Thr:64 Vec:1
Speed.#3.........:  2638.8 kH/s (384.92ms) @ Accel:256 Loops:1 Thr:64 Vec:1
Speed.#4.........:  2665.8 kH/s (380.81ms) @ Accel:256 Loops:1 Thr:64 Vec:1
Speed.#*.........: 10638.5 kH/s

Hashmode: 24410 - PKCS#8 Private Keys (PBKDF2-HMAC-SHA1 + 3DES/AES) (Iterations: 2047)

Speed.#1.........:  1034.3 kH/s (502.59ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  1036.3 kH/s (501.61ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  1029.0 kH/s (505.39ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  1033.1 kH/s (502.59ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  4132.8 kH/s

Hashmode: 24420 - PKCS#8 Private Keys (PBKDF2-HMAC-SHA256 + 3DES/AES) (Iterations: 2047)

Speed.#1.........:   864.2 kH/s (301.76ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#2.........:   864.9 kH/s (301.27ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#3.........:   855.0 kH/s (304.05ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#4.........:   864.1 kH/s (301.20ms) @ Accel:256 Loops:512 Thr:64 Vec:1
Speed.#*.........:  3448.1 kH/s

Hashmode: 99999 - Plaintext

Speed.#1.........: 51302.5 MH/s (41.48ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 51463.1 MH/s (41.33ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 50817.0 MH/s (41.84ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#4.........: 51565.2 MH/s (41.43ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   205.1 GH/s

Started: Thu Jan 21 10:28:58 2021
Stopped: Thu Jan 21 14:13:19 2021
```
