# AMD Radeon RX Vega 64 Liquid Cooling

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX Vega 64 Liquid Cooling
- **Версия hashcat / Version:** v3.5.0
- **Источник / Source:** [Pastebin (anonymous) — «Hashcat Benchmark - RX Vega 64 Liquid»](https://pastebin.com/Y8qWe5Ug)
- **Особенности прогона / Run options:** вывод неполный — паста обрывается на `Hashtype: MS-AzureSync PBKDF2-HMAC-SHA256`, режимы bcrypt / md5crypt / sha512crypt / TrueCrypt / Bitcoin в неё не попали. Формат hashcat 3.x (`Hashtype:` / `Speed.Dev.#1`), номера режимов в выводе не печатаются. Устройство в выводе определяется как `gfx900` (Vega 10); принадлежность именно к версии Liquid Cooling указана автором в заголовке пасты.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 29011.8 MH/s |
| 100 | SHA1 | 12209.8 MH/s |
| 1400 | SHA2-256 | 4996.2 MH/s |
| 1700 | SHA2-512 | 1099.2 MH/s |
| 1000 | NTLM | 54809.1 MH/s |
| 7500 | Kerberos 5 AS-REQ Pre-Auth etype 23 | 368.3 MH/s |
| 13100 | Kerberos 5 TGS-REP etype 23 | 359.8 MH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v3.5.0) starting in benchmark mode...

* Device #2: Not a native Intel OpenCL runtime. Expect massive speed loss.
You can use --force to override, but do not report related errors.
OpenCL Platform #1: Advanced Micro Devices, Inc.
================================================
* Device #1: gfx900, 4048/8176 MB allocatable, 64MCU
* Device #2: Intel(R) Core(TM) i7-6700K CPU @ 4.00GHz, skipped.

Hashtype: MD4

Speed.Dev.#1.....: 54303.1 MH/s (78.13ms)

Hashtype: MD5

Speed.Dev.#1.....: 29011.8 MH/s (72.92ms)

Hashtype: Half MD5

Speed.Dev.#1.....: 19485.0 MH/s (53.98ms)

Hashtype: SHA1

Speed.Dev.#1.....: 12209.8 MH/s (87.07ms)

Hashtype: SHA-256

Speed.Dev.#1.....: 4996.2 MH/s (52.75ms)

Hashtype: SHA-384

Speed.Dev.#1.....: 1075.2 MH/s (61.28ms)

Hashtype: SHA-512

Speed.Dev.#1.....: 1099.2 MH/s (60.14ms)

Hashtype: SHA-3 (Keccak)

Speed.Dev.#1.....: 831.8 MH/s (79.29ms)

Hashtype: SipHash

Speed.Dev.#1.....: 36994.6 MH/s (56.87ms)

Hashtype: Skip32 (PT = $salt, key = $pass)

Speed.Dev.#1.....: 10494.8 MH/s (2.08ms)

Hashtype: RIPEMD-160

Speed.Dev.#1.....: 6637.7 MH/s (79.79ms)

Hashtype: Whirlpool

Speed.Dev.#1.....: 1401.6 MH/s (94.84ms)

Hashtype: GOST R 34.11-94

Speed.Dev.#1.....: 438.9 MH/s (74.76ms)

Hashtype: GOST R 34.11-2012 (Streebog) 256-bit

Speed.Dev.#1.....: 252.2 MH/s (65.76ms)

Hashtype: GOST R 34.11-2012 (Streebog) 512-bit

Speed.Dev.#1.....: 252.2 MH/s (65.14ms)

Hashtype: DES (PT = $salt, key = $pass)

Speed.Dev.#1.....: 34467.1 MH/s (60.34ms)

Hashtype: 3DES (PT = $salt, key = $pass)

Speed.Dev.#1.....: 651.6 MH/s (50.27ms)

Hashtype: phpass, WordPress (MD5), phpBB3 (MD5), Joomla (MD5)

Speed.Dev.#1.....: 8972.2 kH/s (55.70ms)

Hashtype: scrypt

Speed.Dev.#1.....: 579.5 kH/s (23.94ms)

Hashtype: PBKDF2-HMAC-MD5

Speed.Dev.#1.....: 7396.9 kH/s (46.71ms)

Hashtype: PBKDF2-HMAC-SHA1

Speed.Dev.#1.....: 4202.5 kH/s (52.46ms)

Hashtype: PBKDF2-HMAC-SHA256

Speed.Dev.#1.....: 2061.3 kH/s (56.28ms)

Hashtype: PBKDF2-HMAC-SHA512

Speed.Dev.#1.....: 380.6 kH/s (80.81ms)

Hashtype: Skype

Speed.Dev.#1.....: 19372.1 MH/s (54.63ms)

Hashtype: WPA/WPA2

Speed.Dev.#1.....: 493.6 kH/s (63.43ms)

Hashtype: IKE-PSK MD5

Speed.Dev.#1.....: 2498.5 MH/s (52.42ms)

Hashtype: IKE-PSK SHA1

Speed.Dev.#1.....: 762.9 MH/s (87.06ms)

Hashtype: NetNTLMv1 / NetNTLMv1+ESS

Speed.Dev.#1.....: 33953.1 MH/s (62.38ms)

Hashtype: NetNTLMv2

Speed.Dev.#1.....: 2323.1 MH/s (56.48ms)

Hashtype: IPMI2 RAKP HMAC-SHA1

Speed.Dev.#1.....: 2233.6 MH/s (59.02ms)

Hashtype: Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.Dev.#1.....: 368.3 MH/s (90.22ms)

Hashtype: Kerberos 5 TGS-REP etype 23

Speed.Dev.#1.....: 359.8 MH/s (92.04ms)

Hashtype: DNSSEC (NSEC3)

Speed.Dev.#1.....: 4348.6 MH/s (60.37ms)

Hashtype: PostgreSQL CRAM (MD5)

Speed.Dev.#1.....: 9557.6 MH/s (55.03ms)

Hashtype: MySQL CRAM (SHA1)

Speed.Dev.#1.....: 3065.5 MH/s (86.77ms)

Hashtype: SIP digest authentication (MD5)

Speed.Dev.#1.....: 6017.1 MH/s (87.99ms)

Hashtype: SMF (Simple Machines Forum) > v1.1

Speed.Dev.#1.....: 8927.0 MH/s (58.92ms)

Hashtype: vBulletin < v3.8.5

Speed.Dev.#1.....: 9669.3 MH/s (54.18ms)

Hashtype: vBulletin >= v3.8.5

Speed.Dev.#1.....: 6546.8 MH/s (80.40ms)

Hashtype: IPB2+ (Invision Power Board), MyBB 1.2+

Speed.Dev.#1.....: 6846.9 MH/s (77.27ms)

Hashtype: WBB3 (Woltlab Burning Board)

Speed.Dev.#1.....: 1797.8 MH/s (73.34ms)

Hashtype: OpenCart

Speed.Dev.#1.....: 2856.2 MH/s (92.70ms)

Hashtype: Joomla < 2.5.18

Speed.Dev.#1.....: 29142.9 MH/s (72.68ms)

Hashtype: PHPS

Speed.Dev.#1.....: 9650.9 MH/s (54.43ms)

Hashtype: Drupal7

Speed.Dev.#1.....: 59462 H/s (67.94ms)

Hashtype: osCommerce, xt:Commerce

Speed.Dev.#1.....: 19255.7 MH/s (54.64ms)

Hashtype: PrestaShop

Speed.Dev.#1.....: 10768.3 MH/s (48.33ms)

Hashtype: Django (SHA-1)

Speed.Dev.#1.....: 8977.7 MH/s (58.96ms)

Hashtype: Django (PBKDF2-SHA256)

Speed.Dev.#1.....: 104.5 kH/s (62.89ms)

Hashtype: MediaWiki B type

Speed.Dev.#1.....: 9018.9 MH/s (58.05ms)

Hashtype: Redmine

Speed.Dev.#1.....: 3982.2 MH/s (66.61ms)

Hashtype: PunBB

Speed.Dev.#1.....: 3974.1 MH/s (66.81ms)

Hashtype: PostgreSQL

Speed.Dev.#1.....: 29278.6 MH/s (72.55ms)

Hashtype: MSSQL (2000)

Speed.Dev.#1.....: 12167.6 MH/s (86.95ms)

Hashtype: MSSQL (2005)

Speed.Dev.#1.....: 12162.6 MH/s (87.03ms)

Hashtype: MSSQL (2012, 2014)

Speed.Dev.#1.....: 1089.9 MH/s (60.73ms)

Hashtype: MySQL323

Speed.Dev.#1.....: 104.6 GH/s (81.29ms)

Hashtype: MySQL4.1/MySQL5

Speed.Dev.#1.....: 5198.2 MH/s (50.75ms)

Hashtype: Oracle H: Type (Oracle 7+)

Speed.Dev.#1.....: 2387.8 MH/s (54.99ms)

Hashtype: Oracle S: Type (Oracle 11+)

Speed.Dev.#1.....: 12319.8 MH/s (86.04ms)

Hashtype: Oracle T: Type (Oracle 12+)

Speed.Dev.#1.....: 93686 H/s (85.22ms)

Hashtype: Sybase ASE

Speed.Dev.#1.....: 616.9 MH/s (52.95ms)

Hashtype: Episerver 6.x < .NET 4

Speed.Dev.#1.....: 8983.7 MH/s (58.62ms)

Hashtype: Episerver 6.x >= .NET 4

Speed.Dev.#1.....: 4631.6 MH/s (56.74ms)

Hashtype: Apache $apr1$ MD5, md5apr1, MD5 (APR)

Speed.Dev.#1.....: 14735.8 kH/s (50.06ms)

Hashtype: ColdFusion 10+

Speed.Dev.#1.....: 2853.1 MH/s (93.06ms)

Hashtype: hMailServer

Speed.Dev.#1.....: 4602.9 MH/s (57.04ms)

Hashtype: nsldap, SHA-1(Base64), Netscape LDAP SHA

Speed.Dev.#1.....: 12217.4 MH/s (87.08ms)

Hashtype: nsldaps, SSHA-1(Base64), Netscape LDAP SSHA

Speed.Dev.#1.....: 12298.3 MH/s (86.10ms)

Hashtype: SSHA-256(Base64), LDAP {SSHA256}

Speed.Dev.#1.....: 5039.2 MH/s (52.19ms)

Hashtype: SSHA-512(Base64), LDAP {SSHA512}

Speed.Dev.#1.....: 1108.2 MH/s (59.70ms)

Hashtype: LM

Speed.Dev.#1.....: 34997.2 MH/s (59.04ms)

Hashtype: NTLM

Speed.Dev.#1.....: 54809.1 MH/s (77.46ms)

Hashtype: Domain Cached Credentials (DCC), MS Cache

Speed.Dev.#1.....: 16843.9 MH/s (62.61ms)

Hashtype: Domain Cached Credentials 2 (DCC2), MS Cache 2

Speed.Dev.#1.....: 421.0 kH/s (61.15ms)

Hashtype: MS-AzureSync PBKDF2-HMAC-SHA256
```
