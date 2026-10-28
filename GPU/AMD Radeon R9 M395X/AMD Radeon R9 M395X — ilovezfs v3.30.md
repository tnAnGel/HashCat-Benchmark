# AMD Radeon R9 M395X

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon R9 M395X
- **Версия hashcat / Version:** v3.30
- **Источник / Source:** [ilovezfs](https://gist.github.com/ilovezfs/0bbd138a6c0d4d1dcbd4da613ee2eaa0)
- **Примечание / Note:** прогон с `--force` на macOS (iMac Retina 5K), вывод неполный — бенчмарк оборвался на Cisco $9$ («Device does not provide enough allocatable device-memory»). Строки скорости — `Speed.Dev.#2` (устройство #2, сама GPU; CPU #1 пропущен).

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 6880.9 MH/s |
| 100 | SHA1 | 2310.1 MH/s |
| 1400 | SHA2-256 | 980.5 MH/s |
| 1700 | SHA2-512 | 148.6 MH/s |
| 1000 | NTLM | 11090.0 MH/s |
| 3200 | bcrypt | 3478 H/s |
| 1800 | sha512crypt | 20581 H/s |
| 500 | md5crypt | 2834.2 kH/s |
| 7500 | Kerberos 5 AS-REQ Pre-Auth etype 23 | 36376.0 kH/s |
| 13100 | Kerberos 5 TGS-REP etype 23 | 26137.6 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
iMac-TMP:homebrew-core joe$ hashcat -b --force
hashcat (v3.30) starting in benchmark mode...

OpenCL Platform #1: Apple
=========================
* Device #1: Intel(R) Core(TM) i7-6700K CPU @ 4.00GHz, skipped
* Device #2: AMD Radeon R9 M395X Compute Engine, 1024/4096 MB allocatable, 32MCU

Hashtype: MD4

Speed.Dev.#2.....: 11111.2 MH/s (95.41ms)

Hashtype: MD5

Speed.Dev.#2.....:  6880.9 MH/s (76.98ms)

Hashtype: Half MD5

Speed.Dev.#2.....:  4240.0 MH/s (61.63ms)

Hashtype: SHA1

Speed.Dev.#2.....:  2310.1 MH/s (56.92ms)

Hashtype: SHA256

Speed.Dev.#2.....:   980.5 MH/s (67.03ms)

Hashtype: SHA384

Speed.Dev.#2.....:   146.9 MH/s (55.99ms)

Hashtype: SHA512

Speed.Dev.#2.....:   148.6 MH/s (55.17ms)

Hashtype: SHA-3(Keccak)

Speed.Dev.#2.....: 11634.3 kH/s (84.10ms)

Hashtype: SipHash

Speed.Dev.#2.....:  5305.1 MH/s (49.23ms)

Hashtype: RipeMD160

Speed.Dev.#2.....:  1543.2 MH/s (85.77ms)

Hashtype: Whirlpool

Speed.Dev.#2.....:   183.1 MH/s (90.60ms)

Hashtype: GOST R 34.11-94

Speed.Dev.#2.....:   104.0 MH/s (79.50ms)

Hashtype: GOST R 34.11-2012 (Streebog) 256-bit

Speed.Dev.#2.....: 15394.4 kH/s (63.14ms)

Hashtype: GOST R 34.11-2012 (Streebog) 512-bit

Speed.Dev.#2.....: 15433.3 kH/s (63.11ms)

Hashtype: DES (PT = $salt, key = $pass)

Speed.Dev.#2.....:  5943.9 MH/s (88.55ms)

Hashtype: 3DES (PT = $salt, key = $pass)

Speed.Dev.#2.....:   243.2 MH/s (67.83ms)

Hashtype: phpass, MD5(Wordpress), MD5(phpBB3), MD5(Joomla)

Speed.Dev.#2.....:  1919.1 kH/s (61.01ms)

Hashtype: scrypt

Speed.Dev.#2.....:    13847 H/s (110.44ms)

Hashtype: PBKDF2-HMAC-MD5

Speed.Dev.#2.....:  2127.1 kH/s (52.35ms)

Hashtype: PBKDF2-HMAC-SHA1

Speed.Dev.#2.....:   951.7 kH/s (61.96ms)

Hashtype: PBKDF2-HMAC-SHA256

Speed.Dev.#2.....:   424.0 kH/s (71.18ms)

Hashtype: PBKDF2-HMAC-SHA512

Speed.Dev.#2.....:    25161 H/s (76.70ms)

Hashtype: Skype

Speed.Dev.#2.....:  3990.7 MH/s (65.78ms)

Hashtype: WPA/WPA2

Speed.Dev.#2.....:   117.4 kH/s (69.26ms)

Hashtype: IKE-PSK MD5

Speed.Dev.#2.....:   527.3 MH/s (62.43ms)

Hashtype: IKE-PSK SHA1

Speed.Dev.#2.....:   221.7 MH/s (74.50ms)

Hashtype: NetNTLMv1-VANILLA / NetNTLMv1+ESS

Speed.Dev.#2.....:  6570.3 MH/s (80.52ms)

Hashtype: NetNTLMv2

Speed.Dev.#2.....:   485.4 MH/s (67.89ms)

Hashtype: IPMI2 RAKP HMAC-SHA1

Speed.Dev.#2.....:   481.0 MH/s (68.68ms)

Hashtype: Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.Dev.#2.....: 36376.0 kH/s (56.48ms)

Hashtype: Kerberos 5 TGS-REP etype 23

Speed.Dev.#2.....: 26137.6 kH/s (58.53ms)

Hashtype: DNSSEC (NSEC3)

Speed.Dev.#2.....:   937.9 MH/s (70.34ms)

Hashtype: PostgreSQL Challenge-Response Authentication (MD5)

Speed.Dev.#2.....:  1969.4 MH/s (67.05ms)

Hashtype: MySQL Challenge-Response Authentication (SHA1)

Speed.Dev.#2.....:   649.9 MH/s (50.56ms)

Hashtype: SIP digest authentication (MD5)

Speed.Dev.#2.....:   920.3 MH/s (71.48ms)

Hashtype: SMF > v1.1

Speed.Dev.#2.....:  1932.6 MH/s (68.12ms)

Hashtype: vBulletin < v3.8.5

Speed.Dev.#2.....:  2007.2 MH/s (65.55ms)

Hashtype: vBulletin > v3.8.5

Speed.Dev.#2.....:  1391.6 MH/s (95.16ms)

Hashtype: IPB2+, MyBB1.2+

Speed.Dev.#2.....:  1395.4 MH/s (94.94ms)

Hashtype: WBB3, Woltlab Burning Board 3

Speed.Dev.#2.....:   380.5 MH/s (86.84ms)

Hashtype: OpenCart

Speed.Dev.#2.....:   583.3 MH/s (56.48ms)

Hashtype: Joomla < 2.5.18

Speed.Dev.#2.....:  6861.4 MH/s (76.95ms)

Hashtype: PHPS

Speed.Dev.#2.....:  2022.2 MH/s (65.34ms)

Hashtype: Drupal7

Speed.Dev.#2.....:     8432 H/s (60.32ms)

Hashtype: osCommerce, xt:Commerce

Speed.Dev.#2.....:  3980.6 MH/s (65.77ms)

Hashtype: PrestaShop

Speed.Dev.#2.....:  2113.1 MH/s (62.09ms)

Hashtype: Django (SHA-1)

Speed.Dev.#2.....:  1946.6 MH/s (67.94ms)

Hashtype: Django (PBKDF2-SHA256)

Speed.Dev.#2.....:    21373 H/s (77.81ms)

Hashtype: Mediawiki B type

Speed.Dev.#2.....:  1773.9 MH/s (74.56ms)

Hashtype: Redmine Project Management Web App

Speed.Dev.#2.....:   622.0 MH/s (52.88ms)

Hashtype: PostgreSQL

Speed.Dev.#2.....:  6854.3 MH/s (76.98ms)

Hashtype: MSSQL(2000)

Speed.Dev.#2.....:  2298.5 MH/s (57.29ms)

Hashtype: MSSQL(2005)

Speed.Dev.#2.....:  2295.3 MH/s (57.22ms)

Hashtype: MSSQL(2012)

Speed.Dev.#2.....:   122.5 MH/s (67.40ms)

Hashtype: MySQL323

Speed.Dev.#2.....: 20136.6 MH/s (52.18ms)

Hashtype: MySQL4.1/MySQL5

Speed.Dev.#2.....:  1049.2 MH/s (62.46ms)

Hashtype: Oracle H: Type (Oracle 7+)

Speed.Dev.#2.....:   196.0 MH/s (84.37ms)

Hashtype: Oracle S: Type (Oracle 11+)

Speed.Dev.#2.....:  2313.0 MH/s (56.92ms)

Hashtype: Oracle T: Type (Oracle 12+)

Speed.Dev.#2.....:     6187 H/s (81.01ms)

Hashtype: Sybase ASE

Speed.Dev.#2.....:   123.7 MH/s (66.52ms)

Hashtype: EPiServer 6.x < v4

Speed.Dev.#2.....:  1931.2 MH/s (68.10ms)

Hashtype: EPiServer 6.x > v4

Speed.Dev.#2.....:   925.2 MH/s (71.11ms)

Hashtype: md5apr1, MD5(APR), Apache MD5

Speed.Dev.#2.....:  2833.5 kH/s (90.35ms)

Hashtype: ColdFusion 10+

Speed.Dev.#2.....:   578.8 MH/s (56.68ms)

Hashtype: hMailServer

Speed.Dev.#2.....:   926.8 MH/s (71.11ms)

Hashtype: SHA-1(Base64), nsldap, Netscape LDAP SHA

Speed.Dev.#2.....:  2317.3 MH/s (56.72ms)

Hashtype: SSHA-1(Base64), nsldaps, Netscape LDAP SSHA

Speed.Dev.#2.....:  2308.2 MH/s (56.87ms)

Hashtype: SSHA-512(Base64), LDAP {SSHA512}

Speed.Dev.#2.....:   148.5 MH/s (55.17ms)

Hashtype: LM

Speed.Dev.#2.....:  5951.7 MH/s (88.22ms)

Hashtype: NTLM

Speed.Dev.#2.....: 11090.0 MH/s (95.41ms)

Hashtype: Domain Cached Credentials (DCC), MS Cache

Speed.Dev.#2.....:  3143.5 MH/s (83.60ms)

Hashtype: Domain Cached Credentials 2 (DCC2), MS Cache 2

Speed.Dev.#2.....:    93923 H/s (69.20ms)

Hashtype: MS-AzureSync PBKDF2-HMAC-SHA256

Speed.Dev.#2.....:  3823.8 kH/s (60.27ms)

Hashtype: descrypt, DES(Unix), Traditional DES

Speed.Dev.#2.....:   188.9 MH/s (87.17ms)

Hashtype: BSDiCrypt, Extended DES

Speed.Dev.#2.....:  1006.3 kH/s (85.60ms)

Hashtype: md5crypt, MD5(Unix), FreeBSD MD5, Cisco-IOS MD5

Speed.Dev.#2.....:  2834.2 kH/s (90.34ms)

Hashtype: bcrypt, Blowfish(OpenBSD)

Speed.Dev.#2.....:     3478 H/s (71.40ms)

Hashtype: sha256crypt, SHA256(Unix)

Speed.Dev.#2.....:   137.1 kH/s (95.02ms)

Hashtype: sha512crypt, SHA512(Unix)

Speed.Dev.#2.....:    20581 H/s (78.46ms)

Hashtype: OSX v10.4, v10.5, v10.6

Speed.Dev.#2.....:  1940.2 MH/s (68.10ms)

Hashtype: OSX v10.7

Speed.Dev.#2.....:   119.8 MH/s (68.94ms)

Hashtype: OSX v10.8+

Speed.Dev.#2.....:      714 H/s (80.91ms)

Hashtype: AIX {smd5}

Speed.Dev.#2.....:  2840.4 kH/s (90.35ms)

Hashtype: AIX {ssha1}

Speed.Dev.#2.....: 13627.1 kH/s (69.18ms)

Hashtype: AIX {ssha256}

Speed.Dev.#2.....:  5825.7 kH/s (77.55ms)

Hashtype: AIX {ssha512}

Speed.Dev.#2.....:   347.1 kH/s (78.97ms)

Hashtype: Cisco-PIX MD5

Speed.Dev.#2.....:  4637.0 MH/s (56.63ms)

Hashtype: Cisco-ASA MD5

Speed.Dev.#2.....:  4625.0 MH/s (56.52ms)

Hashtype: Cisco-IOS SHA256

Speed.Dev.#2.....:   974.7 MH/s (67.23ms)

Hashtype: Cisco $8$

Speed.Dev.#2.....:    21379 H/s (77.81ms)

Hashtype: Cisco $9$

* Device #2: Device does not provide enough allocatable device-memory to handle this attack

Started: Wed Feb 22 02:25:17 2017
Stopped: Wed Feb 22 02:31:54 2017
iMac-TMP:homebrew-core joe$ echo $?
255
```
