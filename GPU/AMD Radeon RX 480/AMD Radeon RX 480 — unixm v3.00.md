# AMD Radeon RX 480

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 480 (XFX, 8 GB, Ellesmere)
- **Версия hashcat / Version:** v3.00-1-g67a8d97
- **Источник / Source:** [unixm — hashcat Forum, thread-5557](https://hashcat.net/forum/thread-5557.html)
- **Примечание / Note:** прогон с двумя устройствами (Device #1 — Ellesmere = RX 480, Device #2 — Hawaii = R9 290); в таблице ниже используются только строки `Speed.Dev.#1.`. Вывод старого формата hashcat 3.x (`Hashtype:` / `Speed.Dev.#N`), режимы указаны по названию алгоритма. Вывод неполный: часть режимов завершилась ошибкой сборки кернелов (sha512crypt = 0 H/s), режимы 22000 и 11300 в этой версии отсутствуют.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 12465.0 MH/s |
| 100 | SHA1 | 4438.8 MH/s |
| 1400 | SHA2-256 | 1783.0 MH/s |
| 1700 | SHA2-512 | 390.8 MH/s |
| 1000 | NTLM | 24579.2 MH/s |
| 3200 | bcrypt | 8732 H/s |
| 500 | md5crypt | 5129.8 kH/s |
| 7500 | Kerberos AS-REQ (23) | 124.6 MH/s |
| 13100 | Kerberos TGS-REP (23) | 127.1 MH/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 136.9 kH/s |

## Полный вывод `hashcat --benchmark` / Full benchmark output

```text
hashcat (v3.00-1-g67a8d97) starting in benchmark-mode...

OpenCL Platform #1: Advanced Micro Devices, Inc.
================================================
- Device #1: Ellesmere, 4048/8192 MB allocatable, 36MCU
- Device #2: Hawaii, 2880/4096 MB allocatable, 40MCU
- Device #3: AMD FX(tm)-8350 Eight-Core Processor           , skipped

Hashtype: MD4

Speed.Dev.#1.: 24479.4 MH/s (89.83ms)
Speed.Dev.#2.: 20334.2 MH/s (95.72ms)
Speed.Dev.#*.: 44813.7 MH/s

Hashtype: MD5

Speed.Dev.#1.: 12465.0 MH/s (89.89ms)
Speed.Dev.#2.: 10334.6 MH/s (95.77ms)
Speed.Dev.#*.: 22799.6 MH/s

Hashtype: Half MD5

Speed.Dev.#1.:  6594.5 MH/s (107.14ms)
Speed.Dev.#2.:  6583.0 MH/s (95.59ms)
Speed.Dev.#*.: 13177.5 MH/s

Hashtype: SHA1

Speed.Dev.#1.:  4438.8 MH/s (91.20ms)
Speed.Dev.#2.:  3709.7 MH/s (95.49ms)
Speed.Dev.#*.:  8148.5 MH/s

Hashtype: SHA256

Speed.Dev.#1.:  1783.0 MH/s (88.38ms)
Speed.Dev.#2.:  1496.7 MH/s (95.65ms)
Speed.Dev.#*.:  3279.7 MH/s

Hashtype: SHA384

Speed.Dev.#1.:   384.7 MH/s (104.43ms)
Speed.Dev.#2.:   363.1 MH/s (95.49ms)
Speed.Dev.#*.:   747.7 MH/s

Hashtype: SHA512

Speed.Dev.#1.:   390.8 MH/s (104.69ms)
Speed.Dev.#2.:   367.4 MH/s (95.82ms)
Speed.Dev.#*.:   758.2 MH/s

Hashtype: SHA-3(Keccak)

Speed.Dev.#1.:   334.1 MH/s (93.85ms)
Speed.Dev.#2.:   177.1 MH/s (93.94ms)
Speed.Dev.#*.:   511.1 MH/s

Hashtype: SipHash

Speed.Dev.#1.: 13412.0 MH/s (106.01ms)
Speed.Dev.#2.: 13609.6 MH/s (95.73ms)
Speed.Dev.#*.: 27021.6 MH/s

Hashtype: RipeMD160

Speed.Dev.#1.:  2553.7 MH/s (94.02ms)
Speed.Dev.#2.:  2250.4 MH/s (96.47ms)
Speed.Dev.#*.:  4804.1 MH/s

Hashtype: Whirlpool

Speed.Dev.#1.:   283.5 MH/s (109.09ms)
Speed.Dev.#2.:   172.8 MH/s (96.00ms)
Speed.Dev.#*.:   456.3 MH/s

Hashtype: GOST R 34.11-94

Speed.Dev.#1.:   180.3 MH/s (94.30ms)
Speed.Dev.#2.: 62725.4 kH/s (93.20ms)
Speed.Dev.#*.:   243.0 MH/s

Hashtype: GOST R 34.11-2012 (Streebog) 256-bit

Speed.Dev.#1.: 60347.9 kH/s (154.32ms)
Speed.Dev.#2.: 41577.5 kH/s (98.34ms)
Speed.Dev.#*.:   101.9 MH/s

Speed.Dev.#1.: 61375.3 kH/s (148.12ms)
Speed.Dev.#2.: 42413.8 kH/s (101.15ms)
Speed.Dev.#*.:   103.8 MH/s

Hashtype: phpass, MD5(Wordpress), MD5(phpBB3), MD5(Joomla)

Speed.Dev.#1.:  2922.2 kH/s (110.97ms)
Speed.Dev.#2.:  2980.5 kH/s (87.34ms)
Speed.Dev.#*.:  5902.7 kH/s

Hashtype: scrypt

Speed.Dev.#1.:   171.3 kH/s (106.57ms)
Speed.Dev.#2.:   103.5 kH/s (122.20ms)
Speed.Dev.#*.:   274.8 kH/s

Hashtype: PBKDF2-HMAC-MD5

Speed.Dev.#1.:  3347.1 kH/s (91.21ms)
Speed.Dev.#2.:  3337.3 kH/s (84.25ms)
Speed.Dev.#*.:  6684.4 kH/s

Hashtype: PBKDF2-HMAC-SHA1

Speed.Dev.#1.:  1530.5 kH/s (97.11ms)
Speed.Dev.#2.:  1492.5 kH/s (88.39ms)
Speed.Dev.#*.:  3023.0 kH/s

Hashtype: PBKDF2-HMAC-SHA256

Speed.Dev.#1.:   665.0 kH/s (109.72ms)
Speed.Dev.#2.:   678.5 kH/s (89.57ms)
Speed.Dev.#*.:  1343.5 kH/s

Hashtype: PBKDF2-HMAC-SHA512

Speed.Dev.#1.:   161.9 kH/s (102.25ms)
Speed.Dev.#2.:   149.6 kH/s (93.92ms)
Speed.Dev.#*.:   311.6 kH/s

Hashtype: Skype

Speed.Dev.#1.:  6254.8 MH/s (105.06ms)
Speed.Dev.#2.:  6077.4 MH/s (95.60ms)
Speed.Dev.#*.: 12332.1 MH/s

Hashtype: WPA/WPA2

Speed.Dev.#1.:   162.9 kH/s (112.64ms)
Speed.Dev.#2.:   182.8 kH/s (95.60ms)
Speed.Dev.#*.:   345.7 kH/s

Hashtype: IKE-PSK MD5

Speed.Dev.#1.:   829.1 MH/s (102.26ms)
Speed.Dev.#2.:   823.1 MH/s (95.00ms)
Speed.Dev.#*.:  1652.3 MH/s

Hashtype: IKE-PSK SHA1

Speed.Dev.#1.:   284.3 MH/s (97.84ms)
Speed.Dev.#2.:   150.7 MH/s (95.35ms)
Speed.Dev.#*.:   435.0 MH/s

Hashtype: NetNTLMv1-VANILLA / NetNTLMv1+ESS

Speed.Dev.#1.: 11980.6 MH/s (106.94ms)
Speed.Dev.#2.: 11537.8 MH/s (96.64ms)
Speed.Dev.#*.: 23518.4 MH/s

Hashtype: NetNTLMv2

Speed.Dev.#1.:   732.0 MH/s (111.42ms)
Speed.Dev.#2.:   765.0 MH/s (94.85ms)
Speed.Dev.#*.:  1496.9 MH/s

Hashtype: IPMI2 RAKP HMAC-SHA1

Speed.Dev.#1.:   768.3 MH/s (105.49ms)
Speed.Dev.#2.:   753.4 MH/s (95.21ms)
Speed.Dev.#*.:  1521.7 MH/s

Hashtype: Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.Dev.#1.:   124.6 MH/s (97.56ms)
Speed.Dev.#2.: 68908.1 kH/s (99.65ms)
Speed.Dev.#*.:   193.5 MH/s

Hashtype: Kerberos 5 TGS-REP etype 23

Speed.Dev.#1.:   127.1 MH/s (98.77ms)
Speed.Dev.#2.: 71966.9 kH/s (96.92ms)
Speed.Dev.#*.:   199.1 MH/s

Hashtype: DNSSEC (NSEC3)

Speed.Dev.#1.:  1527.4 MH/s (105.69ms)
Speed.Dev.#2.:  1484.1 MH/s (95.69ms)
Speed.Dev.#*.:  3011.6 MH/s

Hashtype: PostgreSQL Challenge-Response Authentication (MD5)

Speed.Dev.#1.:  3144.7 MH/s (103.80ms)
Speed.Dev.#2.:  3047.5 MH/s (95.74ms)
Speed.Dev.#*.:  6192.2 MH/s

Hashtype: MySQL Challenge-Response Authentication (SHA1)

Speed.Dev.#1.:  1262.0 MH/s (89.74ms)
Speed.Dev.#2.:  1043.3 MH/s (95.20ms)
Speed.Dev.#*.:  2305.3 MH/s

Hashtype: SIP digest authentication (MD5)

Speed.Dev.#1.:  1835.5 MH/s (103.14ms)
Speed.Dev.#2.:  1369.8 MH/s (95.27ms)
Speed.Dev.#*.:  3205.4 MH/s

Hashtype: SMF > v1.1

Speed.Dev.#1.:  3058.5 MH/s (107.81ms)
Speed.Dev.#2.:  3053.8 MH/s (95.55ms)
Speed.Dev.#*.:  6112.3 MH/s

Hashtype: vBulletin < v3.8.5

Speed.Dev.#1.:  3183.6 MH/s (105.79ms)
Speed.Dev.#2.:  3116.0 MH/s (95.30ms)
Speed.Dev.#*.:  6299.5 MH/s

Hashtype: vBulletin > v3.8.5

Speed.Dev.#1.:  2624.3 MH/s (88.20ms)
Speed.Dev.#2.:  2142.4 MH/s (95.73ms)
Speed.Dev.#*.:  4766.7 MH/s

Hashtype: IPB2+, MyBB1.2+

Speed.Dev.#1.:  2732.2 MH/s (89.60ms)
Speed.Dev.#2.:  2229.8 MH/s (95.82ms)
Speed.Dev.#*.:  4962.1 MH/s

Hashtype: WBB3, Woltlab Burning Board 3

Speed.Dev.#1.:   731.3 MH/s (88.75ms)
Speed.Dev.#2.:   600.7 MH/s (95.59ms)
Speed.Dev.#*.:  1331.9 MH/s

Hashtype: Joomla < 2.5.18

Speed.Dev.#1.: 12490.1 MH/s (90.42ms)
Speed.Dev.#2.: 10337.7 MH/s (95.77ms)
Speed.Dev.#*.: 22827.8 MH/s

Hashtype: PHPS

Speed.Dev.#1.:  3197.2 MH/s (104.46ms)
Speed.Dev.#2.:  3118.0 MH/s (95.30ms)
Speed.Dev.#*.:  6315.1 MH/s

Hashtype: Drupal7

Speed.Dev.#1.:    21471 H/s (103.84ms)
Speed.Dev.#2.:    20147 H/s (94.99ms)
Speed.Dev.#*.:    41618 H/s

Hashtype: osCommerce, xt:Commerce

Speed.Dev.#1.:  6077.7 MH/s (105.40ms)
Speed.Dev.#2.:  6072.7 MH/s (95.60ms)
Speed.Dev.#*.: 12150.4 MH/s

Hashtype: PrestaShop

Speed.Dev.#1.:  3510.9 MH/s (108.70ms)
Speed.Dev.#2.:  3538.6 MH/s (96.00ms)
Speed.Dev.#*.:  7049.5 MH/s

Hashtype: Django (SHA-1)

Speed.Dev.#1.:  3147.8 MH/s (105.56ms)
Speed.Dev.#2.:  3055.3 MH/s (95.56ms)
Speed.Dev.#*.:  6203.0 MH/s

Hashtype: Django (PBKDF2-SHA256)

Speed.Dev.#1.:    33508 H/s (109.72ms)
Speed.Dev.#2.:    34100 H/s (95.58ms)
Speed.Dev.#*.:    67608 H/s

Hashtype: Mediawiki B type

Speed.Dev.#1.:  2986.1 MH/s (106.45ms)
Speed.Dev.#2.:  2916.6 MH/s (95.48ms)
Speed.Dev.#*.:  5902.7 MH/s

Hashtype: Redmine Project Management Web App

Speed.Dev.#1.:  1194.4 MH/s (86.75ms)
Speed.Dev.#2.:   987.6 MH/s (95.91ms)
Speed.Dev.#*.:  2182.0 MH/s

Hashtype: PostgreSQL

Speed.Dev.#1.: 12492.4 MH/s (89.73ms)
Speed.Dev.#2.: 10331.9 MH/s (95.77ms)
Speed.Dev.#*.: 22824.3 MH/s

Hashtype: MSSQL(2000)

Speed.Dev.#1.:  4513.5 MH/s (89.75ms)
Speed.Dev.#2.:  3693.7 MH/s (95.98ms)
Speed.Dev.#*.:  8207.2 MH/s

Hashtype: MSSQL(2005)

Speed.Dev.#1.:  4513.1 MH/s (89.75ms)
Speed.Dev.#2.:  3692.5 MH/s (95.98ms)
Speed.Dev.#*.:  8205.5 MH/s

Hashtype: MSSQL(2012)

Speed.Dev.#1.:   395.1 MH/s (105.34ms)
Speed.Dev.#2.:   367.4 MH/s (95.82ms)
Speed.Dev.#*.:   762.5 MH/s

Hashtype: MySQL323

Speed.Dev.#1.: 43323.9 MH/s (55.56ms)
Speed.Dev.#2.: 39444.0 MH/s (67.88ms)
Speed.Dev.#*.: 82767.9 MH/s

Hashtype: MySQL4.1/MySQL5

Speed.Dev.#1.:  1687.7 MH/s (105.89ms)
Speed.Dev.#2.:  1300.1 MH/s (95.89ms)
Speed.Dev.#*.:  2987.8 MH/s

Hashtype: Oracle H: Type (Oracle 7+)

Speed.Dev.#1.:   788.7 MH/s (104.14ms)
Speed.Dev.#2.:   720.6 MH/s (96.25ms)
Speed.Dev.#*.:  1509.3 MH/s

Hashtype: Oracle S: Type (Oracle 11+)

Speed.Dev.#1.:  4536.6 MH/s (90.53ms)
Speed.Dev.#2.:  3711.5 MH/s (95.50ms)
Speed.Dev.#*.:  8248.1 MH/s

Hashtype: Oracle T: Type (Oracle 12+)

Speed.Dev.#1.:    39798 H/s (102.07ms)
Speed.Dev.#2.:    36548 H/s (95.61ms)
Speed.Dev.#*.:    76345 H/s

Hashtype: Sybase ASE

Speed.Dev.#1.:   201.7 MH/s (95.32ms)
Speed.Dev.#2.:   136.6 MH/s (97.38ms)
Speed.Dev.#*.:   338.3 MH/s

Hashtype: EPiServer 6.x < v4

Speed.Dev.#1.:  3101.3 MH/s (104.71ms)
Speed.Dev.#2.:  3052.6 MH/s (95.55ms)
Speed.Dev.#*.:  6153.9 MH/s

Hashtype: EPiServer 6.x > v4

Speed.Dev.#1.:  1658.4 MH/s (90.86ms)
Speed.Dev.#2.:  1358.1 MH/s (95.23ms)
Speed.Dev.#*.:  3016.5 MH/s

Hashtype: md5apr1, MD5(APR), Apache MD5

Speed.Dev.#1.:  5621.3 kH/s (90.13ms)
Speed.Dev.#2.:  4784.7 kH/s (95.47ms)
Speed.Dev.#*.: 10406.0 kH/s

Hashtype: ColdFusion 10+

Speed.Dev.#1.:  1137.0 MH/s (83.83ms)
Speed.Dev.#2.:   934.4 MH/s (95.18ms)
Speed.Dev.#*.:  2071.4 MH/s

Hashtype: hMailServer

Speed.Dev.#1.:  1609.8 MH/s (93.60ms)
Speed.Dev.#2.:  1358.4 MH/s (95.23ms)
Speed.Dev.#*.:  2968.3 MH/s

Hashtype: SHA-1(Base64), nsldap, Netscape LDAP SHA

Speed.Dev.#1.:  4504.7 MH/s (90.92ms)
Speed.Dev.#2.:  3711.4 MH/s (95.49ms)
Speed.Dev.#*.:  8216.2 MH/s

Hashtype: SSHA-1(Base64), nsldaps, Netscape LDAP SSHA

Speed.Dev.#1.:  4512.6 MH/s (89.72ms)
Speed.Dev.#2.:  3711.2 MH/s (95.50ms)
Speed.Dev.#*.:  8223.8 MH/s

Hashtype: SSHA-512(Base64), LDAP {SSHA512}

Speed.Dev.#1.:   459.0 MH/s (90.58ms)
Speed.Dev.#2.:   242.7 MH/s (93.71ms)
Speed.Dev.#*.:   701.8 MH/s

Hashtype: LM

Speed.Dev.#1.:  2480.3 MH/s (96.61ms)
Speed.Dev.#2.:  1518.9 MH/s (94.54ms)
Speed.Dev.#*.:  3999.2 MH/s

Hashtype: NTLM

Speed.Dev.#1.: 24579.2 MH/s (88.54ms)
Speed.Dev.#2.: 20340.3 MH/s (95.71ms)
Speed.Dev.#*.: 44919.6 MH/s

Hashtype: Domain Cached Credentials (DCC), MS Cache

Speed.Dev.#1.:  5527.8 MH/s (108.84ms)
Speed.Dev.#2.:  5503.0 MH/s (95.88ms)
Speed.Dev.#*.: 11030.9 MH/s

Hashtype: Domain Cached Credentials 2 (DCC2), MS Cache 2

Speed.Dev.#1.:   144.1 kH/s (108.42ms)
Speed.Dev.#2.:   146.6 kH/s (95.29ms)
Speed.Dev.#*.:   290.7 kH/s

Hashtype: MS-AzureSync PBKDF2-HMAC-SHA256

Speed.Dev.#1.:  7352.5 kH/s (89.22ms)
Speed.Dev.#2.:  6306.0 kH/s (94.75ms)
Speed.Dev.#*.: 13658.4 kH/s

Hashtype: descrypt, DES(Unix), Traditional DES

Speed.Dev.#1.:   397.8 MH/s (100.42ms)
Speed.Dev.#2.:   325.8 MH/s (88.10ms)
Speed.Dev.#*.:   723.6 MH/s

Hashtype: BSDiCrypt, Extended DES

Speed.Dev.#1.:  1584.9 kH/s (94.13ms)
Speed.Dev.#2.:  1452.3 kH/s (90.90ms)
Speed.Dev.#*.:  3037.2 kH/s

Hashtype: md5crypt, MD5(Unix), FreeBSD MD5, Cisco-IOS MD5

Speed.Dev.#1.:  5129.8 kH/s (101.18ms)
Speed.Dev.#2.:  4785.8 kH/s (95.47ms)
Speed.Dev.#*.:  9915.6 kH/s

Hashtype: bcrypt, Blowfish(OpenBSD)

Speed.Dev.#1.:     8732 H/s (80.39ms)
Speed.Dev.#2.:     5029 H/s (92.81ms)
Speed.Dev.#*.:    13761 H/s

Hashtype: BSDiCrypt, Extended DES

Speed.Dev.#1.:  1584.9 kH/s (94.13ms)
Speed.Dev.#2.:  1452.3 kH/s (90.90ms)
Speed.Dev.#*.:  3037.2 kH/s

Hashtype: md5crypt, MD5(Unix), FreeBSD MD5, Cisco-IOS MD5

Speed.Dev.#1.:  5129.8 kH/s (101.18ms)
Speed.Dev.#2.:  4785.8 kH/s (95.47ms)
Speed.Dev.#*.:  9915.6 kH/s

Hashtype: sha256crypt, SHA256(Unix)

Speed.Dev.#1.:   221.9 kH/s (106.99ms)
Speed.Dev.#2.:   221.8 kH/s (94.91ms)
Speed.Dev.#*.:   443.8 kH/s

=== Build Log (end) ===
- Device #2: Kernel c:\Users\kyle\Desktop\hash\newhash5\hashcat-3.00/OpenCL/m01800.cl build failure. Proceeding without this device.
Hashtype: sha512crypt, SHA512(Unix)

Speed.Dev.#*.:        0 H/s

Hashtype: OSX v10.4, v10.5, v10.6

Speed.Dev.#1.:  3082.6 MH/s (105.45ms)
Speed.Dev.#2.:  3054.9 MH/s (95.47ms)
Speed.Dev.#*.:  6137.5 MH/s

Hashtype: OSX v10.7

Speed.Dev.#1.:   366.3 MH/s (103.79ms)
Speed.Dev.#2.:   309.9 MH/s (94.36ms)
Speed.Dev.#*.:   676.2 MH/s

Hashtype: OSX v10.8+

Speed.Dev.#1.:     4635 H/s (101.80ms)
Speed.Dev.#2.:     4282 H/s (95.46ms)
Speed.Dev.#*.:     8918 H/s

Hashtype: AIX {smd5}

Speed.Dev.#1.:  5151.5 kH/s (75.49ms)
Speed.Dev.#2.:  4784.2 kH/s (95.47ms)
Speed.Dev.#*.:  9935.7 kH/s

Hashtype: AIX {ssha1}

Speed.Dev.#1.: 19538.9 kH/s (114.77ms)
Speed.Dev.#2.: 21739.5 kH/s (46.51ms)
Speed.Dev.#*.: 41278.4 kH/s

Hashtype: AIX {ssha256}

Speed.Dev.#1.: 10999.0 kH/s (97.03ms)
Speed.Dev.#2.:  9498.6 kH/s (95.57ms)
Speed.Dev.#*.: 20497.6 kH/s

Hashtype: AIX {ssha512}

Speed.Dev.#1.:  2639.5 kH/s (90.73ms)
Speed.Dev.#2.:  2137.9 kH/s (95.33ms)
Speed.Dev.#*.:  4777.4 kH/s

Hashtype: Cisco-PIX MD5

Speed.Dev.#1.:  8764.6 MH/s (87.29ms)
Speed.Dev.#2.:  7260.4 MH/s (95.89ms)
Speed.Dev.#*.: 16025.1 MH/s

Hashtype: Cisco-ASA MD5

Speed.Dev.#1.:  8760.9 MH/s (89.24ms)
Speed.Dev.#2.:  7253.9 MH/s (95.63ms)
Speed.Dev.#*.: 16014.8 MH/s

Hashtype: Cisco-IOS SHA256

Speed.Dev.#1.:  1343.1 MH/s (119.29ms)
Speed.Dev.#2.:  1497.5 MH/s (95.65ms)
Speed.Dev.#*.:  2840.6 MH/s

Hashtype: Cisco $8$

Speed.Dev.#1.:    33465 H/s (107.73ms)
Speed.Dev.#2.:    34101 H/s (95.58ms)
Speed.Dev.#*.:    67566 H/s

Hashtype: Cisco $9$

Speed.Dev.#1.:     4658 H/s (493.69ms)
Speed.Dev.#2.:     1504 H/s (1700.61ms)
Speed.Dev.#*.:     6161 H/s

Hashtype: Juniper Netscreen/SSG (ScreenOS)

Speed.Dev.#1.:  6226.6 MH/s (102.47ms)
Speed.Dev.#2.:  6075.6 MH/s (95.60ms)
Speed.Dev.#*.: 12302.2 MH/s

Hashtype: Juniper IVE

Speed.Dev.#1.:  4972.2 kH/s (104.31ms)
Speed.Dev.#2.:  4784.0 kH/s (95.47ms)
Speed.Dev.#*.:  9756.1 kH/s

Hashtype: Android PIN

Speed.Dev.#1.:  2622.2 kH/s (86.61ms)
Speed.Dev.#2.:  2495.4 kH/s (82.60ms)
Speed.Dev.#*.:  5117.6 kH/s

Hashtype: Citrix NetScaler

Speed.Dev.#1.:  3331.2 MH/s (106.71ms)
Speed.Dev.#2.:  3283.0 MH/s (95.63ms)
Speed.Dev.#*.:  6614.2 MH/s

Hashtype: RACF

Speed.Dev.#1.:  2448.6 MH/s (84.64ms)
Speed.Dev.#2.:  1894.8 MH/s (95.35ms)
Speed.Dev.#*.:  4343.5 MH/s

Hashtype: GRUB 2

Speed.Dev.#1.:    16317 H/s (101.40ms)
Speed.Dev.#2.:    14989 H/s (95.46ms)
Speed.Dev.#*.:    31306 H/s

Hashtype: Radmin2

Speed.Dev.#1.:  4326.8 MH/s (90.30ms)
Speed.Dev.#2.:  3579.1 MH/s (95.75ms)
Speed.Dev.#*.:  7905.9 MH/s

Hashtype: SAP CODVN B (BCODE)

Speed.Dev.#1.:  1136.5 MH/s (134.73ms)
Speed.Dev.#2.:  1023.2 MH/s (134.35ms)
Speed.Dev.#*.:  2159.6 MH/s

Hashtype: SAP CODVN F/G (PASSCODE)

Speed.Dev.#1.:   257.8 MH/s (100.24ms)
Speed.Dev.#2.:   150.9 MH/s (138.78ms)
Speed.Dev.#*.:   408.7 MH/s

Hashtype: SAP CODVN H (PWDSALTEDHASH) iSSHA-1

Speed.Dev.#1.:  2708.5 kH/s (107.79ms)
Speed.Dev.#2.:  2748.5 kH/s (82.28ms)
Speed.Dev.#*.:  5457.0 kH/s

Hashtype: Lotus Notes/Domino 5

Speed.Dev.#1.:   275.6 MH/s (115.77ms)
Speed.Dev.#2.:   223.3 MH/s (92.23ms)
Speed.Dev.#*.:   498.9 MH/s

Hashtype: Lotus Notes/Domino 6

Speed.Dev.#1.: 60903.8 kH/s (100.70ms)
Speed.Dev.#2.: 26781.3 kH/s (104.93ms)
Speed.Dev.#*.: 87685.2 kH/s

Hashtype: Lotus Notes/Domino 8

Speed.Dev.#1.:   287.7 kH/s (107.88ms)
Speed.Dev.#2.:   296.1 kH/s (95.34ms)
Speed.Dev.#*.:   583.8 kH/s

Hashtype: PeopleSoft

Speed.Dev.#1.:  4508.2 MH/s (91.38ms)
Speed.Dev.#2.:  3693.8 MH/s (96.35ms)
Speed.Dev.#*.:  8201.9 MH/s

Hashtype: PeopleSoft PS_TOKEN

Speed.Dev.#1.:  1428.0 MH/s (106.42ms)
Speed.Dev.#2.:  1369.1 MH/s (95.31ms)
Speed.Dev.#*.:  2797.1 MH/s

Hashtype: 7-Zip

Speed.Dev.#1.:     5625 H/s (104.88ms)
Speed.Dev.#2.:     5201 H/s (95.43ms)
Speed.Dev.#*.:    10826 H/s

Hashtype: WinZip

Speed.Dev.#1.:   512.1 kH/s (106.51ms)
Speed.Dev.#2.:   495.2 kH/s (89.16ms)
Speed.Dev.#*.:  1007.3 kH/s

Hashtype: RAR3-hp

Speed.Dev.#1.:  4168.5 kH/s (60.24ms)
Speed.Dev.#2.:  3710.9 kH/s (74.10ms)
Speed.Dev.#*.:  7879.4 kH/s

Hashtype: RAR5

Speed.Dev.#1.:    20376 H/s (109.48ms)
Speed.Dev.#2.:    20812 H/s (95.58ms)
Speed.Dev.#*.:    41188 H/s

Hashtype: AxCrypt

Speed.Dev.#1.:   143.8 kH/s (189.73ms)
Speed.Dev.#2.:   124.4 kH/s (150.77ms)
Speed.Dev.#*.:   268.2 kH/s

Hashtype: AxCrypt in memory SHA1

Speed.Dev.#1.:  3413.7 MH/s (108.34ms)
Speed.Dev.#2.:  3310.0 MH/s (97.21ms)
Speed.Dev.#*.:  6723.7 MH/s

Hashtype: TrueCrypt PBKDF2-HMAC-RipeMD160 + XTS 512 bit

Speed.Dev.#1.:   136.9 kH/s (107.63ms)
Speed.Dev.#2.:   135.1 kH/s (93.68ms)
Speed.Dev.#*.:   272.1 kH/s

Hashtype: TrueCrypt PBKDF2-HMAC-SHA512 + XTS 512 bit

Speed.Dev.#1.:   161.8 kH/s (100.19ms)
Speed.Dev.#2.:   147.2 kH/s (93.25ms)
Speed.Dev.#*.:   309.0 kH/s

Hashtype: TrueCrypt PBKDF2-HMAC-Whirlpool + XTS 512 bit

Speed.Dev.#1.:    39262 H/s (113.57ms)
Speed.Dev.#2.:    15363 H/s (94.66ms)
Speed.Dev.#*.:    54625 H/s

Hashtype: TrueCrypt PBKDF2-HMAC-RipeMD160 + XTS 512 bit + boot-mode

Speed.Dev.#1.:   265.5 kH/s (105.15ms)
Speed.Dev.#2.:   265.3 kH/s (92.66ms)
Speed.Dev.#*.:   530.9 kH/s

Hashtype: VeraCrypt PBKDF2-HMAC-RipeMD160 + XTS 512 bit

Speed.Dev.#1.:      407 H/s (111.63ms)
Speed.Dev.#2.:      420 H/s (94.33ms)
Speed.Dev.#*.:      827 H/s

Hashtype: VeraCrypt PBKDF2-HMAC-SHA512 + XTS 512 bit

Speed.Dev.#1.:      326 H/s (102.09ms)
Speed.Dev.#2.:      301 H/s (94.98ms)
Speed.Dev.#*.:      627 H/s

Hashtype: VeraCrypt PBKDF2-HMAC-Whirlpool + XTS 512 bit

Speed.Dev.#1.:       78 H/s (111.33ms)
Speed.Dev.#2.:       30 H/s (96.16ms)
Speed.Dev.#*.:      108 H/s

Hashtype: VeraCrypt PBKDF2-HMAC-RipeMD160 + XTS 512 bit + boot-mode

Speed.Dev.#1.:      835 H/s (107.05ms)
Speed.Dev.#2.:      840 H/s (94.33ms)
Speed.Dev.#*.:     1675 H/s

Hashtype: VeraCrypt PBKDF2-HMAC-SHA256 + XTS 512 bit

Speed.Dev.#1.:      631 H/s (112.41ms)
Speed.Dev.#2.:      663 H/s (94.44ms)
Speed.Dev.#*.:     1294 H/s

Hashtype: VeraCrypt PBKDF2-HMAC-SHA256 + XTS 512 bit + boot-mode

Speed.Dev.#1.:     1649 H/s (85.59ms)
Speed.Dev.#2.:     1657 H/s (94.44ms)
Speed.Dev.#*.:     3307 H/s

Hashtype: Android FDE <= 4.3

Speed.Dev.#1.:   371.8 kH/s (97.35ms)
Speed.Dev.#2.:   370.7 kH/s (94.29ms)
Speed.Dev.#*.:   742.5 kH/s

Hashtype: Android FDE (Samsung DEK)

Speed.Dev.#1.:   162.2 kH/s (110.14ms)
Speed.Dev.#2.:   166.6 kH/s (95.58ms)
Speed.Dev.#*.:   328.7 kH/s

Hashtype: eCryptfs

Speed.Dev.#1.:     5736 H/s (106.83ms)
Speed.Dev.#2.:     6358 H/s (94.79ms)
Speed.Dev.#*.:    12094 H/s

Hashtype: MS Office <= 2003 MD5 + RC4, oldoffice$0, oldoffice$1

Speed.Dev.#1.:   118.0 MH/s (98.52ms)
Speed.Dev.#2.: 64444.5 kH/s (97.73ms)
Speed.Dev.#*.:   182.5 MH/s

Hashtype: MS Office <= 2003 MD5 + RC4, collision-mode #1

Speed.Dev.#1.:   158.0 MH/s (99.96ms)
Speed.Dev.#2.:   135.9 MH/s (98.39ms)
Speed.Dev.#*.:   293.9 MH/s

Hashtype: MS Office <= 2003 SHA1 + RC4, oldoffice$3, oldoffice$4

Speed.Dev.#1.:   128.6 MH/s (98.74ms)
Speed.Dev.#2.: 84561.2 kH/s (97.21ms)
Speed.Dev.#*.:   213.2 MH/s

Hashtype: MS Office <= 2003 SHA1 + RC4, collision-mode #1

Speed.Dev.#1.:   157.8 MH/s (100.06ms)
Speed.Dev.#2.:   138.6 MH/s (98.25ms)
Speed.Dev.#*.:   296.4 MH/s

Hashtype: Office 2007

Speed.Dev.#1.:    58660 H/s (107.54ms)
Speed.Dev.#2.:    59979 H/s (95.84ms)
Speed.Dev.#*.:   118.6 kH/s

Hashtype: Office 2010

Speed.Dev.#1.:    29258 H/s (106.18ms)
Speed.Dev.#2.:    29997 H/s (95.83ms)
Speed.Dev.#*.:    59256 H/s

Hashtype: Office 2013

Speed.Dev.#1.:     3760 H/s (106.75ms)
Speed.Dev.#2.:     4170 H/s (94.70ms)
Speed.Dev.#*.:     7930 H/s

Hashtype: PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.Dev.#1.:   172.0 MH/s (100.95ms)
Speed.Dev.#2.:   161.1 MH/s (99.72ms)
Speed.Dev.#*.:   333.1 MH/s

Hashtype: PDF 1.1 - 1.3 (Acrobat 2 - 4) + collider-mode #1

Speed.Dev.#1.:   186.3 MH/s (101.83ms)
Speed.Dev.#2.:   177.7 MH/s (100.70ms)
Speed.Dev.#*.:   364.0 MH/s

Hashtype: PDF 1.4 - 1.6 (Acrobat 5 - 8)

Speed.Dev.#1.:  8139.8 kH/s (56.77ms)
Speed.Dev.#2.:  7046.1 kH/s (73.09ms)
Speed.Dev.#*.: 15185.9 kH/s

Hashtype: Password Safe v2

Speed.Dev.#1.:   203.8 kH/s (87.94ms)
Speed.Dev.#2.:   144.4 kH/s (88.59ms)
Speed.Dev.#*.:   348.2 kH/s

Hashtype: Password Safe v3

Speed.Dev.#1.:   646.1 kH/s (106.90ms)
Speed.Dev.#2.:   673.0 kH/s (90.91ms)
Speed.Dev.#*.:  1319.1 kH/s

Hashtype: Lastpass

Speed.Dev.#1.:  1360.2 kH/s (103.38ms)
Speed.Dev.#2.:  1337.9 kH/s (84.03ms)
Speed.Dev.#*.:  2698.0 kH/s

Hashtype: 1Password, agilekeychain

Speed.Dev.#1.:  1520.4 kH/s (103.70ms)
Speed.Dev.#2.:  1490.8 kH/s (88.44ms)
Speed.Dev.#*.:  3011.2 kH/s

Hashtype: 1Password, cloudkeychain

Speed.Dev.#1.:     4051 H/s (102.65ms)
Speed.Dev.#2.:     3739 H/s (95.66ms)
Speed.Dev.#*.:     7790 H/s

Hashtype: Bitcoin/Litecoin wallet.dat

Speed.Dev.#1.:     1808 H/s (105.06ms)
Speed.Dev.#2.:     1705 H/s (95.14ms)
Speed.Dev.#*.:     3513 H/s

Hashtype: Blockchain, My Wallet

Speed.Dev.#1.: 45354.2 kH/s (60.74ms)
Speed.Dev.#2.: 46291.8 kH/s (95.88ms)
Speed.Dev.#*.: 91646.0 kH/s

Hashtype: Keepass 1 (AES/Twofish) and Keepass 2 (AES)

Speed.Dev.#1.:    64004 H/s (96.52ms)
Speed.Dev.#2.:    81883 H/s (95.63ms)
Speed.Dev.#*.:   145.9 kH/s

Hashtype: ArubaOS

Speed.Dev.#1.:  3087.6 MH/s (104.51ms)
Speed.Dev.#2.:  3055.8 MH/s (95.46ms)
Speed.Dev.#*.:  6143.4 MH/s

Started: Thu Jun 30 21:55:42 2016
Stopped: Thu Jun 30 22:23:05 2016
```
