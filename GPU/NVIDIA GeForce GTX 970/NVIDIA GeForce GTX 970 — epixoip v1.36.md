# NVIDIA GeForce GTX 970

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 970
- **Версия hashcat / Version:** v1.36
- **Источник / Source:** [epixoip](https://gist.github.com/epixoip/e885edc473e74398faf6)

## Полный вывод `hashcat -b` / Full benchmark output

```text
cudaHashcat v1.36 starting in benchmark-mode...

Device #1: GeForce GTX 970, 4095MB, 1177Mhz, 13MCU

Hashtype: MD4
Workload: 1024 loops, 256 accel

Speed.GPU.#1.: 21746.2 MH/s

Hashtype: MD5
Workload: 1024 loops, 256 accel

Speed.GPU.#1.: 10443.1 MH/s

Hashtype: SHA1
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  3349.8 MH/s

Hashtype: SHA256
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  1321.8 MH/s

Hashtype: SHA384
Workload: 256 loops, 256 accel

Speed.GPU.#1.:   415.8 MH/s

Hashtype: SHA512
Workload: 256 loops, 256 accel

Speed.GPU.#1.:   410.4 MH/s

Hashtype: SHA-3(Keccak)
Workload: 128 loops, 32 accel

Speed.GPU.#1.:   292.2 MH/s

Hashtype: RipeMD160
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  2177.9 MH/s

Hashtype: Whirlpool
Workload: 512 loops, 256 accel

Speed.GPU.#1.:        0 H/s

Hashtype: GOST R 34.11-94
Workload: 512 loops, 256 accel

Speed.GPU.#1.:   124.8 MH/s

Hashtype: SAP CODVN B (BCODE)
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:   808.5 MH/s

Hashtype: SAP CODVN F/G (PASSCODE)
Workload: 1024 loops, 32 accel

Speed.GPU.#1.:   398.0 MH/s

Hashtype: SAP CODVN H (PWDSALTEDHASH) iSSHA-1
Workload: 1024 loops, 16 accel

Speed.GPU.#1.:  2537.6 kH/s

Hashtype: Lotus Notes/Domino 5
Workload: 256 loops, 32 accel

Speed.GPU.#1.:   111.4 MH/s

Hashtype: Lotus Notes/Domino 6
Workload: 256 loops, 32 accel

Speed.GPU.#1.: 36293.4 kH/s

Hashtype: Lotus Notes/Domino 8
Workload: 1024 loops, 64 accel

Speed.GPU.#1.:   282.7 kH/s

Hashtype: SHA-1(Base64), nsldap, Netscape LDAP SHA
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  3318.1 MH/s

Hashtype: SSHA-1(Base64), nsldaps, Netscape LDAP SSHA
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  3310.6 MH/s

Hashtype: descrypt, DES(Unix), Traditional DES
Workload: 128 loops, 256 accel

Speed.GPU.#1.: 89998.0 kH/s

Hashtype: md5crypt, MD5(Unix), FreeBSD MD5, Cisco-IOS MD5
Workload: 1000 loops, 32 accel

Speed.GPU.#1.:  4474.9 kH/s

Hashtype: sha256crypt, SHA256(Unix)
Workload: 1024 loops, 4 accel

Speed.GPU.#1.:   192.9 kH/s

Hashtype: sha512crypt, SHA512(Unix)
Workload: 1024 loops, 8 accel

Speed.GPU.#1.:    69709 H/s

Hashtype: bcrypt, Blowfish(OpenBSD)
Workload: 32 loops, 2 accel

Speed.GPU.#1.:     8984 H/s

Hashtype: LM
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  1343.7 MH/s

Hashtype: NTLM
Workload: 1024 loops, 256 accel

Speed.GPU.#1.: 21427.8 MH/s

Hashtype: DCC, mscash
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  5802.5 MH/s

Hashtype: NetNTLMv1-VANILLA / NetNTLMv1+ESS
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  8922.3 MH/s

Hashtype: NetNTLMv2
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:   672.4 MH/s

Hashtype: Kerberos 5 AS-REQ Pre-Auth etype 23
Workload: 256 loops, 32 accel

Speed.GPU.#1.:   116.3 MH/s

Hashtype: EPiServer 6.x < v4
Workload: 512 loops, 256 accel

Speed.GPU.#1.:  2427.4 MH/s

Hashtype: EPiServer 6.x > v4
Workload: 512 loops, 256 accel

Speed.GPU.#1.:  1212.9 MH/s

Hashtype: MSSQL(2000)
Workload: 512 loops, 256 accel

Speed.GPU.#1.:  3362.6 MH/s

Hashtype: MSSQL(2005)
Workload: 512 loops, 256 accel

Speed.GPU.#1.:  3358.4 MH/s

Hashtype: MSSQL(2012)
Workload: 256 loops, 256 accel

Speed.GPU.#1.:   415.0 MH/s

Hashtype: MySQL323
Workload: 512 loops, 256 accel

Speed.GPU.#1.: 23070.7 MH/s

Hashtype: MySQL4.1/MySQL5
Workload: 512 loops, 256 accel

Speed.GPU.#1.:  1539.5 MH/s

Hashtype: Oracle 7-10g
Workload: 512 loops, 32 accel

Speed.GPU.#1.:   387.5 MH/s

Hashtype: Sybase ASE
Workload: 512 loops, 32 accel

Speed.GPU.#1.:   120.7 MH/s

Hashtype: Oracle 11g/12c
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  3309.0 MH/s

Hashtype: PostgreSQL Challenge-Response Authentication (MD5)
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  2590.1 MH/s

Hashtype: MySQL Challenge-Response Authentication (SHA1)
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:   965.9 MH/s

Hashtype: OSX v10.4, v10.5, v10.6
Workload: 512 loops, 256 accel

Speed.GPU.#1.:  2423.1 MH/s

Hashtype: OSX v10.7
Workload: 128 loops, 256 accel

Speed.GPU.#1.:   408.4 MH/s

Hashtype: OSX v10.8+
Workload: 1024 loops, 2 accel

Speed.GPU.#1.:     5148 H/s

Hashtype: Android PIN
Workload: 1024 loops, 16 accel

Speed.GPU.#1.:  2533.4 kH/s

Hashtype: Android FDE <= 4.3
Workload: 1024 loops, 32 accel

Speed.GPU.#1.:   351.3 kH/s

Hashtype: scrypt
Workload: 1 loops, 64 accel

Speed.GPU.#1.:   191.9 kH/s

Hashtype: Cisco-PIX MD5
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  6479.7 MH/s

Hashtype: Cisco-ASA MD5
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  6736.0 MH/s

Hashtype: Cisco-IOS SHA256
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  1306.2 MH/s

Hashtype: Cisco $8$
Workload: 1024 loops, 8 accel

Speed.GPU.#1.:    29050 H/s

Hashtype: Cisco $9$
Workload: 1 loops, 4 accel

Speed.GPU.#1.:     1579 H/s

Hashtype: Juniper IVE
Workload: 1000 loops, 32 accel

Speed.GPU.#1.:  4475.6 kH/s

Hashtype: Citrix NetScaler
Workload: 512 loops, 256 accel

Speed.GPU.#1.:  3028.8 MH/s

Hashtype: DNSSEC (NSEC3)
Workload: 512 loops, 256 accel

Speed.GPU.#1.:  1438.3 MH/s

Hashtype: WPA/WPA2
Workload: 1024 loops, 32 accel

Speed.GPU.#1.:   173.4 kH/s

Hashtype: IKE-PSK MD5
Workload: 512 loops, 32 accel

Speed.GPU.#1.:   736.6 MH/s

Hashtype: IKE-PSK SHA1
Workload: 512 loops, 32 accel

Speed.GPU.#1.:   261.9 MH/s

Hashtype: Password Safe v2
Workload: 1000 loops, 16 accel

Speed.GPU.#1.:   127.1 kH/s

Hashtype: Password Safe v3
Workload: 1024 loops, 16 accel

Speed.GPU.#1.:   573.3 kH/s

Hashtype: 1Password, agilekeychain
Workload: 1000 loops, 64 accel

Speed.GPU.#1.:  1398.4 kH/s

Hashtype: 1Password, cloudkeychain
Workload: 1024 loops, 2 accel

Speed.GPU.#1.:     4510 H/s

Hashtype: AIX {ssha1}
Workload: 64 loops, 128 accel

Speed.GPU.#1.: 18115.2 kH/s

Hashtype: TrueCrypt 5.0+ PBKDF2-HMAC-RipeMD160 + AES
Workload: 1024 loops, 64 accel

Speed.GPU.#1.:   509.4 kH/s

Hashtype: TrueCrypt 5.0+ PBKDF2-HMAC-SHA512 + AES
Workload: 1000 loops, 16 accel

Speed.GPU.#1.:   185.1 kH/s

Hashtype: TrueCrypt 5.0+ PBKDF2-HMAC-Whirlpool + AES
Workload: 1000 loops, 8 accel

Speed.GPU.#1.:    18944 H/s

Hashtype: TrueCrypt 5.0+ PBKDF2-HMAC-RipeMD160 + AES + boot-mode
Workload: 1000 loops, 64 accel

Speed.GPU.#1.:  1007.0 kH/s

Hashtype: Office 2007
Workload: 1024 loops, 32 accel

Speed.GPU.#1.:    58094 H/s

Hashtype: Office 2010
Workload: 1024 loops, 32 accel

Speed.GPU.#1.:    29063 H/s

Hashtype: Office 2013
Workload: 1024 loops, 4 accel

Speed.GPU.#1.:     4219 H/s

Hashtype: MS Office <= 2003 MD5 + RC4, oldoffice$0, oldoffice$1
Workload: 1024 loops, 32 accel

Speed.GPU.#1.:   108.5 MH/s

Hashtype: MS Office <= 2003 SHA1 + RC4, oldoffice$3, oldoffice$4
Workload: 1024 loops, 32 accel

Speed.GPU.#1.:   148.6 MH/s

Hashtype: PDF 1.1 - 1.3 (Acrobat 2 - 4)
Workload: 1024 loops, 32 accel

Speed.GPU.#1.:   162.8 MH/s

Hashtype: PDF 1.1 - 1.3 (Acrobat 2 - 4) + collider-mode #1
Workload: 1024 loops, 32 accel

Speed.GPU.#1.:   183.2 MH/s

Hashtype: PDF 1.1 - 1.3 (Acrobat 2 - 4) + collider-mode #2
Workload: 1024 loops, 32 accel

Speed.GPU.#1.:  1653.7 MH/s

Hashtype: PDF 1.4 - 1.6 (Acrobat 5 - 8)
Workload: 70 loops, 256 accel

Speed.GPU.#1.:  7798.7 kH/s

Hashtype: PDF 1.7 Level 3 (Acrobat 9)
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  1319.1 MH/s

Hashtype: PDF 1.7 Level 8 (Acrobat 10 - 11)
Workload: 64 loops, 8 accel

Speed.GPU.#1.:    16484 H/s

Hashtype: Drupal7
Workload: 1024 loops, 8 accel

Speed.GPU.#1.:    25027 H/s

Hashtype: HMAC-MD5 (key = $pass)
Workload: 512 loops, 256 accel

Speed.GPU.#1.:  1121.4 MH/s

Hashtype: HMAC-MD5 (key = $salt)
Workload: 512 loops, 256 accel

Speed.GPU.#1.:  2907.2 MH/s

Hashtype: HMAC-SHA1 (key = $pass)
Workload: 256 loops, 256 accel

Speed.GPU.#1.:   227.4 MH/s

Hashtype: HMAC-SHA1 (key = $salt)
Workload: 256 loops, 256 accel

Speed.GPU.#1.:   387.5 MH/s

Hashtype: HMAC-SHA256 (key = $pass)
Workload: 128 loops, 128 accel

Speed.GPU.#1.:   258.8 MH/s

Hashtype: HMAC-SHA256 (key = $salt)
Workload: 128 loops, 128 accel

Speed.GPU.#1.:   563.8 MH/s

Hashtype: HMAC-SHA512 (key = $pass)
Workload: 128 loops, 128 accel

Speed.GPU.#1.: 57722.1 kH/s

Hashtype: HMAC-SHA512 (key = $salt)
Workload: 128 loops, 128 accel

Speed.GPU.#1.:   133.8 MH/s

Hashtype: IPMI2 RAKP HMAC-SHA1
Workload: 256 loops, 256 accel

Speed.GPU.#1.:   696.9 MH/s

Hashtype: Half MD5
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  6404.3 MH/s

Hashtype: Double MD5
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  2891.8 MH/s

Hashtype: GRUB 2
Workload: 1024 loops, 2 accel

Speed.GPU.#1.:    17847 H/s

Hashtype: phpass, MD5(Wordpress), MD5(phpBB3), MD5(Joomla)
Workload: 1024 loops, 32 accel

Speed.GPU.#1.:  2855.7 kH/s

Hashtype: SIP digest authentication (MD5)
Workload: 1024 loops, 32 accel

Speed.GPU.#1.:  1174.9 MH/s

Hashtype: SipHash
Workload: 1024 loops, 256 accel

Speed.GPU.#1.: 12621.3 MH/s

Hashtype: Joomla < 2.5.18
Workload: 1024 loops, 256 accel

Speed.GPU.#1.: 10297.3 MH/s

Hashtype: osCommerce, xt:Commerce
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  5722.3 MH/s

Hashtype: PrestaShop
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  3551.9 MH/s

Hashtype: IPB2+, MyBB1.2+
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  1436.4 MH/s

Hashtype: vBulletin < v3.8.5
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  2922.3 MH/s

Hashtype: PHPS
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  2907.8 MH/s

Hashtype: vBulletin > v3.8.5
Workload: 1024 loops, 256 accel

Speed.GPU.#1.:  1403.5 MH/s

Hashtype: SMF > v1.1
Workload: 512 loops, 256 accel

Speed.GPU.#1.:  2425.0 MH/s
</raw_output>
```
