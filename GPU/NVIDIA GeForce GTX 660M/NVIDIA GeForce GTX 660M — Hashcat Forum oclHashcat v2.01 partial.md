# NVIDIA GeForce GTX 660M

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** GeForce GTX 660M, 128/512 MB allocatable, 950 MHz, 2 MCU
- **Версия / Version:** oclHashcat v2.01 (`g952c20e`)
- **Источник / Source:** [Hashcat Forum — oclHashcat benchmark with Apple CPU + GPU, post #22](https://hashcat.net/forum/post-28623.html)
- **Тип данных / Evidence:** опубликованный benchmark-mode raw fragment; CPU i5-3470S явно skipped, GPU — Device #2
- **Ограничение:** вывод заканчивается `Abort trap: 6` на Oracle H: Type; это partial, не полный набор режимов

## Результаты Device #2

| Тип хеша | Алгоритм | Скорость |
|---|---|---:|
| MD4 | MD4 | 1551.3 MH/s |
| MD5 | MD5 | 1548.7 MH/s |
| Half MD5 | Half MD5 | 180.6 MH/s |
| SHA1 | SHA-1 | 1359.2 MH/s |
| SHA256 | SHA-256 | 1544.5 MH/s |
| SHA384 | SHA-384 | 1574.8 MH/s |
| SHA512 | SHA-512 | 1546.4 MH/s |
| SHA-3 (Keccak) | SHA-3 | 3230.1 kH/s |
| SipHash | SipHash | 1528.8 MH/s |
| RipeMD160 | RIPEMD-160 | 68403.2 kH/s |
| Whirlpool | Whirlpool | 1307.3 kH/s |
| GOST R 34.11-94 | GOST | 9495.1 kH/s |
| GOST R 34.11-2012 (256-bit) | Streebog-256 | 445.3 kH/s |
| GOST R 34.11-2012 (512-bit) | Streebog-512 | 444.0 kH/s |
| phpass | phpass / WordPress | 103.2 kH/s |
| scrypt | scrypt | 36756 H/s |
| PBKDF2-HMAC-MD5 | PBKDF2-MD5 | 60474 H/s |
| PBKDF2-HMAC-SHA1 | PBKDF2-SHA1 | 42880 H/s |
| PBKDF2-HMAC-SHA256 | PBKDF2-SHA256 | 17750 H/s |
| PBKDF2-HMAC-SHA512 | PBKDF2-SHA512 | 6915 H/s |
| Skype | Skype | 204.0 MH/s |
| WPA/WPA2 (legacy mode) | WPA/WPA2 | 5427 H/s |
| IKE-PSK MD5 | IKE-PSK MD5 | 22448.4 kH/s |
| IKE-PSK SHA1 | IKE-PSK SHA1 | 12411.8 kH/s |
| NetNTLMv1-VANILLA / +ESS | NetNTLMv1 | 503.3 MH/s |
| NetNTLMv2 | NetNTLMv2 | 20983.9 kH/s |
| IPMI2 RAKP HMAC-SHA1 | IPMI2 | 24765.9 kH/s |
| Kerberos 5 AS-REQ Pre-Auth etype 23 | Kerberos | 1902.7 kH/s |
| DNSSEC (NSEC3) | NSEC3 | 42333.0 kH/s |
| PostgreSQL Challenge-Response (MD5) | PostgreSQL | 104.1 MH/s |
| MySQL Challenge-Response (SHA1) | MySQL SHA1 | 36226.7 kH/s |
| SIP digest authentication (MD5) | SIP-MD5 | 30477.1 kH/s |
| SMF > v1.1 | SMF | 97848.4 kH/s |
| vBulletin < v3.8.5 | vBulletin | 111.2 MH/s |
| vBulletin > v3.8.5 | vBulletin | 80814.6 kH/s |
| IPB2+, MyBB1.2+ | forum hash | 85843.7 kH/s |
| WBB3 | Woltlab Burning Board 3 | 20037.5 kH/s |
| Joomla < 2.5.18 | Joomla | 1512.9 MH/s |
| PHPS | PHPS | 111.1 MH/s |
| Drupal7 | Drupal7 | 658 H/s |
| osCommerce, xt:Commerce | osCommerce | 203.6 MH/s |
| PrestaShop | PrestaShop | 105.9 MH/s |
| Django (SHA-1) | Django SHA1 | 97849.0 kH/s |
| Django (PBKDF2-SHA256) | Django PBKDF2 | 760 H/s |
| Mediawiki B type | Mediawiki | 64685.5 kH/s |
| Redmine Project Management Web App | Redmine | 34788.0 kH/s |
| PostgreSQL | PostgreSQL | 1555.1 MH/s |
| MSSQL(2000) | MSSQL 2000 | 88061.3 kH/s |
| MSSQL(2005) | MSSQL 2005 | 88049.4 kH/s |
| MSSQL(2012) | MSSQL 2012 | 1207.2 MH/s |
| MySQL323 | MySQL323 | 1551.5 MH/s |
| MySQL4.1/MySQL5 | MySQL 4.1/5 | 1563.1 MH/s |

Это legacy benchmark оclHashcat, поэтому старые режимы и throughput не следует
считать напрямую эквивалентными современному `hashcat -b`.
