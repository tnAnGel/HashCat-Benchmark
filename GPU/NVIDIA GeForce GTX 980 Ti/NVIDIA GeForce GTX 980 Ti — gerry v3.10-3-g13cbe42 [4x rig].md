# NVIDIA GeForce GTX 980 Ti (4x rig)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 980 Ti
- **Конфигурация / Setup:** 4x rig
- **Версия hashcat / Version:** v3.10-3-g13cbe42
- **Источник / Source:** [gerry](https://gist.github.com/gerry/4c78fe1fafe90d882e607889be110a4f)

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v3.10-3-g13cbe42) starting in benchmark-mode...

OpenCL Platform #1: NVIDIA Corporation
======================================
- Device #1: GeForce GTX 980 Ti, 1519/6077 MB allocatable, 22MCU
- Device #2: GeForce GTX 980 Ti, 1519/6077 MB allocatable, 22MCU
- Device #3: GeForce GTX 980 Ti, 1519/6077 MB allocatable, 22MCU
- Device #4: GeForce GTX 980 Ti, 1519/6077 MB allocatable, 22MCU

Hashtype: MD4

Speed.Dev.#1.: 34403.3 MH/s (96.17ms)
Speed.Dev.#2.: 34046.3 MH/s (96.34ms)
Speed.Dev.#3.: 33647.5 MH/s (96.45ms)
Speed.Dev.#4.: 33733.5 MH/s (96.38ms)
Speed.Dev.#*.:   135.8 GH/s

Hashtype: MD5

Speed.Dev.#1.: 18880.2 MH/s (96.32ms)
Speed.Dev.#2.: 18719.3 MH/s (96.38ms)
Speed.Dev.#3.: 18521.6 MH/s (96.17ms)
Speed.Dev.#4.: 18553.2 MH/s (96.31ms)
Speed.Dev.#*.: 74674.3 MH/s

Hashtype: Half MD5

Speed.Dev.#1.: 11930.9 MH/s (96.14ms)
Speed.Dev.#2.: 11796.4 MH/s (96.26ms)
Speed.Dev.#3.: 11685.2 MH/s (96.19ms)
Speed.Dev.#4.: 11706.0 MH/s (96.02ms)
Speed.Dev.#*.: 47118.5 MH/s

Hashtype: SHA1

Speed.Dev.#1.:  6490.6 MH/s (95.91ms)
Speed.Dev.#2.:  6426.8 MH/s (95.07ms)
Speed.Dev.#3.:  6355.6 MH/s (95.68ms)
Speed.Dev.#4.:  6374.8 MH/s (95.75ms)
Speed.Dev.#*.: 25647.7 MH/s

Hashtype: SHA256

Speed.Dev.#1.:  2302.7 MH/s (95.74ms)
Speed.Dev.#2.:  2274.6 MH/s (95.92ms)
Speed.Dev.#3.:  2198.7 MH/s (95.85ms)
Speed.Dev.#4.:  2250.5 MH/s (96.44ms)
Speed.Dev.#*.:  9026.5 MH/s

Hashtype: SHA384

Speed.Dev.#1.:   778.3 MH/s (95.61ms)
Speed.Dev.#2.:   768.4 MH/s (96.02ms)
Speed.Dev.#3.:   758.6 MH/s (95.59ms)
Speed.Dev.#4.:   760.4 MH/s (96.07ms)
Speed.Dev.#*.:  3065.7 MH/s

Hashtype: SHA512

Speed.Dev.#1.:   793.3 MH/s (96.20ms)
Speed.Dev.#2.:   789.3 MH/s (95.90ms)
Speed.Dev.#3.:   772.6 MH/s (96.33ms)
Speed.Dev.#4.:   779.5 MH/s (96.29ms)
Speed.Dev.#*.:  3134.6 MH/s

Hashtype: SHA-3(Keccak)

Speed.Dev.#1.:   621.6 MH/s (94.21ms)
Speed.Dev.#2.:   609.3 MH/s (94.99ms)
Speed.Dev.#3.:   611.7 MH/s (93.58ms)
Speed.Dev.#4.:   604.1 MH/s (93.80ms)
Speed.Dev.#*.:  2446.7 MH/s

Hashtype: SipHash

Speed.Dev.#1.: 22690.0 MH/s (96.15ms)
Speed.Dev.#2.: 22457.5 MH/s (96.12ms)
Speed.Dev.#3.: 22176.4 MH/s (96.43ms)
Speed.Dev.#4.: 21866.1 MH/s (96.40ms)
Speed.Dev.#*.: 89190.0 MH/s

Hashtype: RipeMD160

Speed.Dev.#1.:  3636.1 MH/s (95.95ms)
Speed.Dev.#2.:  3655.5 MH/s (96.13ms)
Speed.Dev.#3.:  3624.6 MH/s (95.68ms)
Speed.Dev.#4.:  3634.8 MH/s (95.72ms)
Speed.Dev.#*.: 14550.9 MH/s

Hashtype: Whirlpool

Speed.Dev.#1.:   200.6 MH/s (177.30ms)
Speed.Dev.#2.:   199.8 MH/s (175.81ms)
Speed.Dev.#3.:   195.7 MH/s (177.24ms)
Speed.Dev.#4.:   196.7 MH/s (176.37ms)
Speed.Dev.#*.:   792.9 MH/s

Hashtype: GOST R 34.11-94

Speed.Dev.#1.:   188.5 MH/s (135.11ms)
Speed.Dev.#2.:   184.3 MH/s (135.82ms)
Speed.Dev.#3.:   182.1 MH/s (137.43ms)
Speed.Dev.#4.:   182.7 MH/s (136.97ms)
Speed.Dev.#*.:   737.6 MH/s

Hashtype: GOST R 34.11-2012 (Streebog) 256-bit

Speed.Dev.#1.: 40265.6 kH/s (335.58ms)
Speed.Dev.#2.: 39239.6 kH/s (342.22ms)
Speed.Dev.#3.: 39472.6 kH/s (332.64ms)
Speed.Dev.#4.: 39017.7 kH/s (339.39ms)
Speed.Dev.#*.:   158.0 MH/s

Hashtype: GOST R 34.11-2012 (Streebog) 512-bit

Speed.Dev.#1.: 40294.8 kH/s (335.47ms)
Speed.Dev.#2.: 39220.4 kH/s (345.83ms)
Speed.Dev.#3.: 38765.7 kH/s (346.54ms)
Speed.Dev.#4.: 38606.0 kH/s (339.36ms)
Speed.Dev.#*.:   156.9 MH/s

Hashtype: phpass, MD5(Wordpress), MD5(phpBB3), MD5(Joomla)

Speed.Dev.#1.:  5167.4 kH/s (95.86ms)
Speed.Dev.#2.:  5198.4 kH/s (96.16ms)
Speed.Dev.#3.:  5139.0 kH/s (96.21ms)
Speed.Dev.#4.:  5186.1 kH/s (96.04ms)
Speed.Dev.#*.: 20690.8 kH/s

Hashtype: scrypt

Speed.Dev.#1.:   589.2 kH/s (18.75ms)
Speed.Dev.#2.:   579.9 kH/s (19.06ms)
Speed.Dev.#3.:   573.3 kH/s (19.28ms)
Speed.Dev.#4.:   573.1 kH/s (19.27ms)
Speed.Dev.#*.:  2315.5 kH/s

Hashtype: PBKDF2-HMAC-MD5

Speed.Dev.#1.:  5896.3 kH/s (65.29ms)
Speed.Dev.#2.:  5569.6 kH/s (65.28ms)
Speed.Dev.#3.:  5747.6 kH/s (96.08ms)
Speed.Dev.#4.:  5592.8 kH/s (65.53ms)
Speed.Dev.#*.: 22806.3 kH/s

Hashtype: PBKDF2-HMAC-SHA1

Speed.Dev.#1.:  2418.7 kH/s (80.84ms)
Speed.Dev.#2.:  2474.1 kH/s (80.55ms)
Speed.Dev.#3.:  2369.1 kH/s (80.99ms)
Speed.Dev.#4.:  2459.7 kH/s (80.72ms)
Speed.Dev.#*.:  9721.7 kH/s

Hashtype: PBKDF2-HMAC-SHA256

Speed.Dev.#1.:   913.7 kH/s (88.42ms)
Speed.Dev.#2.:   884.7 kH/s (88.55ms)
Speed.Dev.#3.:   867.1 kH/s (87.39ms)
Speed.Dev.#4.:   867.4 kH/s (87.68ms)
Speed.Dev.#*.:  3532.9 kH/s

Hashtype: PBKDF2-HMAC-SHA512

Speed.Dev.#1.:   308.5 kH/s (91.26ms)
Speed.Dev.#2.:   312.2 kH/s (90.36ms)
Speed.Dev.#3.:   303.9 kH/s (90.07ms)
Speed.Dev.#4.:   304.9 kH/s (90.87ms)
Speed.Dev.#*.:  1229.5 kH/s

Hashtype: Skype

Speed.Dev.#1.: 10145.3 MH/s (96.13ms)
Speed.Dev.#2.: 10043.3 MH/s (96.16ms)
Speed.Dev.#3.:  9940.4 MH/s (96.28ms)
Speed.Dev.#4.:  9954.7 MH/s (96.14ms)
Speed.Dev.#*.: 40083.7 MH/s

Hashtype: WPA/WPA2

Speed.Dev.#1.:   306.3 kH/s (91.73ms)
Speed.Dev.#2.:   295.6 kH/s (92.10ms)
Speed.Dev.#3.:   294.8 kH/s (93.09ms)
Speed.Dev.#4.:   301.5 kH/s (92.32ms)
Speed.Dev.#*.:  1198.2 kH/s

Hashtype: IKE-PSK MD5

Speed.Dev.#1.:  1379.4 MH/s (96.12ms)
Speed.Dev.#2.:  1369.0 MH/s (95.81ms)
Speed.Dev.#3.:  1354.1 MH/s (95.80ms)
Speed.Dev.#4.:  1355.4 MH/s (96.23ms)
Speed.Dev.#*.:  5457.9 MH/s

Hashtype: IKE-PSK SHA1

Speed.Dev.#1.:   596.9 MH/s (95.92ms)
Speed.Dev.#2.:   586.0 MH/s (96.63ms)
Speed.Dev.#3.:   575.8 MH/s (97.24ms)
Speed.Dev.#4.:   574.7 MH/s (97.41ms)
Speed.Dev.#*.:  2333.3 MH/s

Hashtype: NetNTLMv1-VANILLA / NetNTLMv1+ESS

Speed.Dev.#1.: 17651.4 MH/s (96.34ms)
Speed.Dev.#2.: 17474.6 MH/s (96.50ms)
Speed.Dev.#3.: 17296.9 MH/s (96.32ms)
Speed.Dev.#4.: 17312.0 MH/s (96.57ms)
Speed.Dev.#*.: 69735.0 MH/s

Hashtype: NetNTLMv2

Speed.Dev.#1.:  1256.1 MH/s (94.86ms)
Speed.Dev.#2.:  1268.0 MH/s (95.29ms)
Speed.Dev.#3.:  1252.1 MH/s (95.55ms)
Speed.Dev.#4.:  1193.5 MH/s (95.29ms)
Speed.Dev.#*.:  4969.7 MH/s

Hashtype: IPMI2 RAKP HMAC-SHA1

Speed.Dev.#1.:  1265.2 MH/s (95.49ms)
Speed.Dev.#2.:  1250.9 MH/s (95.93ms)
Speed.Dev.#3.:  1232.1 MH/s (96.07ms)
Speed.Dev.#4.:  1237.2 MH/s (95.66ms)
Speed.Dev.#*.:  4985.4 MH/s

Hashtype: Kerberos 5 AS-REQ Pre-Auth etype 23

Speed.Dev.#1.:   229.0 MH/s (105.34ms)
Speed.Dev.#2.:   226.8 MH/s (105.73ms)
Speed.Dev.#3.:   223.1 MH/s (106.16ms)
Speed.Dev.#4.:   224.8 MH/s (105.97ms)
Speed.Dev.#*.:   903.6 MH/s

Hashtype: Kerberos 5 TGS-REP etype 23

Speed.Dev.#1.:   229.3 MH/s (106.19ms)
Speed.Dev.#2.:   226.5 MH/s (106.32ms)
Speed.Dev.#3.:   222.7 MH/s (106.79ms)
Speed.Dev.#4.:   224.2 MH/s (105.92ms)
Speed.Dev.#*.:   902.7 MH/s

Hashtype: DNSSEC (NSEC3)

Speed.Dev.#1.:  2522.9 MH/s (95.87ms)
Speed.Dev.#2.:  2498.2 MH/s (95.62ms)
Speed.Dev.#3.:  2465.7 MH/s (95.95ms)
Speed.Dev.#4.:  2474.2 MH/s (96.08ms)
Speed.Dev.#*.:  9960.9 MH/s

Hashtype: PostgreSQL Challenge-Response Authentication (MD5)

Speed.Dev.#1.:  5224.5 MH/s (96.26ms)
Speed.Dev.#2.:  5178.3 MH/s (96.02ms)
Speed.Dev.#3.:  5102.8 MH/s (96.59ms)
Speed.Dev.#4.:  5109.6 MH/s (96.17ms)
Speed.Dev.#*.: 20615.2 MH/s

Hashtype: MySQL Challenge-Response Authentication (SHA1)

Speed.Dev.#1.:  1728.0 MH/s (95.94ms)
Speed.Dev.#2.:  1748.6 MH/s (95.89ms)
Speed.Dev.#3.:  1724.5 MH/s (96.01ms)
Speed.Dev.#4.:  1734.6 MH/s (95.96ms)
Speed.Dev.#*.:  6935.7 MH/s

Hashtype: SIP digest authentication (MD5)

Speed.Dev.#1.:  1513.9 MH/s (98.22ms)
Speed.Dev.#2.:  1570.0 MH/s (98.02ms)
Speed.Dev.#3.:  1550.7 MH/s (98.13ms)
Speed.Dev.#4.:  1491.6 MH/s (98.31ms)
Speed.Dev.#*.:  6126.2 MH/s

Hashtype: SMF > v1.1

Speed.Dev.#1.:  5214.2 MH/s (96.08ms)
Speed.Dev.#2.:  5164.5 MH/s (96.27ms)
Speed.Dev.#3.:  5109.8 MH/s (96.17ms)
Speed.Dev.#4.:  5112.3 MH/s (96.05ms)
Speed.Dev.#*.: 20600.8 MH/s

Hashtype: vBulletin < v3.8.5

Speed.Dev.#1.:  5260.7 MH/s (95.97ms)
Speed.Dev.#2.:  5383.7 MH/s (96.36ms)
Speed.Dev.#3.:  5228.1 MH/s (96.54ms)
Speed.Dev.#4.:  5332.5 MH/s (96.47ms)
Speed.Dev.#*.: 21205.0 MH/s

Hashtype: vBulletin > v3.8.5

Speed.Dev.#1.:  3653.6 MH/s (95.83ms)
Speed.Dev.#2.:  3724.3 MH/s (95.90ms)
Speed.Dev.#3.:  3678.7 MH/s (96.15ms)
Speed.Dev.#4.:  3689.1 MH/s (95.87ms)
Speed.Dev.#*.: 14745.7 MH/s

Hashtype: IPB2+, MyBB1.2+

Speed.Dev.#1.:  3960.4 MH/s (95.96ms)
Speed.Dev.#2.:  3811.4 MH/s (95.93ms)
Speed.Dev.#3.:  3877.4 MH/s (95.89ms)
Speed.Dev.#4.:  3873.8 MH/s (95.75ms)
Speed.Dev.#*.: 15523.0 MH/s

Hashtype: WBB3, Woltlab Burning Board 3

Speed.Dev.#1.:   979.9 MH/s (95.63ms)
Speed.Dev.#2.:   971.3 MH/s (95.94ms)
Speed.Dev.#3.:   953.1 MH/s (95.79ms)
Speed.Dev.#4.:   960.6 MH/s (95.91ms)
Speed.Dev.#*.:  3864.9 MH/s

Hashtype: OpenCart

Speed.Dev.#1.:  1585.3 MH/s (95.97ms)
Speed.Dev.#2.:  1569.0 MH/s (95.86ms)
Speed.Dev.#3.:  1552.5 MH/s (96.16ms)
Speed.Dev.#4.:  1553.6 MH/s (96.28ms)
Speed.Dev.#*.:  6260.5 MH/s

Hashtype: Joomla < 2.5.18

Speed.Dev.#1.: 18856.9 MH/s (96.29ms)
Speed.Dev.#2.: 18681.3 MH/s (96.42ms)
Speed.Dev.#3.: 18502.1 MH/s (96.43ms)
Speed.Dev.#4.: 17782.8 MH/s (96.26ms)
Speed.Dev.#*.: 73823.2 MH/s

Hashtype: PHPS

Speed.Dev.#1.:  5439.7 MH/s (96.69ms)
Speed.Dev.#2.:  5394.3 MH/s (96.44ms)
Speed.Dev.#3.:  5323.7 MH/s (96.63ms)
Speed.Dev.#4.:  5343.7 MH/s (96.27ms)
Speed.Dev.#*.: 21501.4 MH/s

Hashtype: Drupal7

Speed.Dev.#1.:    41666 H/s (96.63ms)
Speed.Dev.#2.:    41278 H/s (96.05ms)
Speed.Dev.#3.:    40830 H/s (96.19ms)
Speed.Dev.#4.:    41089 H/s (95.52ms)
Speed.Dev.#*.:   164.9 kH/s

Hashtype: osCommerce, xt:Commerce

Speed.Dev.#1.: 10141.5 MH/s (96.20ms)
Speed.Dev.#2.: 10045.2 MH/s (96.26ms)
Speed.Dev.#3.:  9937.4 MH/s (96.29ms)
Speed.Dev.#4.:  9955.8 MH/s (96.26ms)
Speed.Dev.#*.: 40079.9 MH/s

Hashtype: PrestaShop

Speed.Dev.#1.:  6432.5 MH/s (96.03ms)
Speed.Dev.#2.:  6424.8 MH/s (96.00ms)
Speed.Dev.#3.:  6357.5 MH/s (96.33ms)
Speed.Dev.#4.:  6051.2 MH/s (96.17ms)
Speed.Dev.#*.: 25266.1 MH/s

Hashtype: Django (SHA-1)

Speed.Dev.#1.:  5212.9 MH/s (96.10ms)
Speed.Dev.#2.:  5165.0 MH/s (96.26ms)
Speed.Dev.#3.:  5111.6 MH/s (96.42ms)
Speed.Dev.#4.:  5111.0 MH/s (96.04ms)
Speed.Dev.#*.: 20600.6 MH/s

Hashtype: Django (PBKDF2-SHA256)

Speed.Dev.#1.:    45602 H/s (95.27ms)
Speed.Dev.#2.:    45086 H/s (95.52ms)
Speed.Dev.#3.:    44563 H/s (95.17ms)
Speed.Dev.#4.:    44666 H/s (95.87ms)
Speed.Dev.#*.:   179.9 kH/s

Hashtype: Mediawiki B type

Speed.Dev.#1.:  5130.4 MH/s (96.62ms)
Speed.Dev.#2.:  5080.4 MH/s (96.73ms)
Speed.Dev.#3.:  5014.6 MH/s (96.85ms)
Speed.Dev.#4.:  4908.4 MH/s (96.89ms)
Speed.Dev.#*.: 20133.8 MH/s

Hashtype: Redmine Project Management Web App

Speed.Dev.#1.:  1593.0 MH/s (95.85ms)
Speed.Dev.#2.:  1592.9 MH/s (95.97ms)
Speed.Dev.#3.:  1574.7 MH/s (96.09ms)
Speed.Dev.#4.:  1579.5 MH/s (96.25ms)
Speed.Dev.#*.:  6340.1 MH/s

Hashtype: PostgreSQL

Speed.Dev.#1.: 18886.5 MH/s (96.29ms)
Speed.Dev.#2.: 18675.2 MH/s (96.30ms)
Speed.Dev.#3.: 18496.0 MH/s (96.14ms)
Speed.Dev.#4.: 18516.9 MH/s (96.34ms)
Speed.Dev.#*.: 74574.6 MH/s

Hashtype: MSSQL(2000)

Speed.Dev.#1.:  6623.1 MH/s (93.99ms)
Speed.Dev.#2.:  6523.1 MH/s (94.33ms)
Speed.Dev.#3.:  6454.5 MH/s (94.44ms)
Speed.Dev.#4.:  6285.3 MH/s (94.05ms)
Speed.Dev.#*.: 25886.0 MH/s

Hashtype: MSSQL(2005)

Speed.Dev.#1.:  6623.5 MH/s (93.98ms)
Speed.Dev.#2.:  6522.5 MH/s (94.56ms)
Speed.Dev.#3.:  6452.8 MH/s (93.79ms)
Speed.Dev.#4.:  6357.1 MH/s (94.15ms)
Speed.Dev.#*.: 25956.0 MH/s

Hashtype: MSSQL(2012)

Speed.Dev.#1.:   793.8 MH/s (96.15ms)
Speed.Dev.#2.:   786.9 MH/s (96.19ms)
Speed.Dev.#3.:   776.6 MH/s (96.65ms)
Speed.Dev.#4.:   775.7 MH/s (96.76ms)
Speed.Dev.#*.:  3133.0 MH/s

Hashtype: MySQL323

Speed.Dev.#1.: 40626.2 MH/s (36.30ms)
Speed.Dev.#2.: 40214.5 MH/s (36.67ms)
Speed.Dev.#3.: 39806.8 MH/s (37.05ms)
Speed.Dev.#4.: 39865.9 MH/s (36.99ms)
Speed.Dev.#*.:   160.5 GH/s

Hashtype: MySQL4.1/MySQL5

Speed.Dev.#1.:  2918.8 MH/s (95.60ms)
Speed.Dev.#2.:  2886.8 MH/s (95.46ms)
Speed.Dev.#3.:  2860.7 MH/s (95.13ms)
Speed.Dev.#4.:  2865.9 MH/s (95.36ms)
Speed.Dev.#*.: 11532.2 MH/s

Hashtype: Oracle H: Type (Oracle 7+)

Speed.Dev.#1.:   773.1 MH/s (111.89ms)
Speed.Dev.#2.:   765.8 MH/s (112.13ms)
Speed.Dev.#3.:   759.4 MH/s (111.41ms)
Speed.Dev.#4.:   761.8 MH/s (112.02ms)
Speed.Dev.#*.:  3060.2 MH/s

Hashtype: Oracle S: Type (Oracle 11+)

Speed.Dev.#1.:  6487.6 MH/s (95.95ms)
Speed.Dev.#2.:  6385.3 MH/s (95.69ms)
Speed.Dev.#3.:  5444.6 MH/s (95.96ms)
Speed.Dev.#4.:  6368.7 MH/s (95.84ms)
Speed.Dev.#*.: 24686.2 MH/s

Hashtype: Oracle T: Type (Oracle 12+)

Speed.Dev.#1.:    74842 H/s (94.75ms)
Speed.Dev.#2.:    75466 H/s (94.64ms)
Speed.Dev.#3.:    74055 H/s (94.99ms)
Speed.Dev.#4.:    74078 H/s (94.07ms)
Speed.Dev.#*.:   298.4 kH/s

Hashtype: Sybase ASE

Speed.Dev.#1.:   284.0 MH/s (97.65ms)
Speed.Dev.#2.:   282.0 MH/s (97.09ms)
Speed.Dev.#3.:   283.0 MH/s (96.75ms)
Speed.Dev.#4.:   287.9 MH/s (95.10ms)
Speed.Dev.#*.:  1136.9 MH/s

Hashtype: EPiServer 6.x < v4

Speed.Dev.#1.:  5215.4 MH/s (96.05ms)
Speed.Dev.#2.:  5172.1 MH/s (96.12ms)
Speed.Dev.#3.:  5116.2 MH/s (96.33ms)
Speed.Dev.#4.:  5118.8 MH/s (96.28ms)
Speed.Dev.#*.: 20622.6 MH/s

Hashtype: EPiServer 6.x > v4

Speed.Dev.#1.:  2076.1 MH/s (96.24ms)
Speed.Dev.#2.:  2061.2 MH/s (95.82ms)
Speed.Dev.#3.:  2037.4 MH/s (95.82ms)
Speed.Dev.#4.:  1981.7 MH/s (95.35ms)
Speed.Dev.#*.:  8156.4 MH/s

Hashtype: md5apr1, MD5(APR), Apache MD5

Speed.Dev.#1.:  7926.0 kH/s (96.39ms)
Speed.Dev.#2.:  7832.7 kH/s (96.84ms)
Speed.Dev.#3.:  7326.4 kH/s (95.81ms)
Speed.Dev.#4.:  7407.8 kH/s (95.95ms)
Speed.Dev.#*.: 30493.0 kH/s

Hashtype: ColdFusion 10+

Speed.Dev.#1.:  1348.2 MH/s (95.65ms)
Speed.Dev.#2.:  1339.8 MH/s (95.73ms)
Speed.Dev.#3.:  1322.2 MH/s (95.91ms)
Speed.Dev.#4.:  1287.9 MH/s (95.70ms)
Speed.Dev.#*.:  5298.0 MH/s

Hashtype: hMailServer

Speed.Dev.#1.:  2082.2 MH/s (95.96ms)
Speed.Dev.#2.:  2060.8 MH/s (95.84ms)
Speed.Dev.#3.:  2037.5 MH/s (95.81ms)
Speed.Dev.#4.:  2046.5 MH/s (95.39ms)
Speed.Dev.#*.:  8226.9 MH/s

Hashtype: SHA-1(Base64), nsldap, Netscape LDAP SHA

Speed.Dev.#1.:  6249.4 MH/s (95.95ms)
Speed.Dev.#2.:  6415.4 MH/s (95.91ms)
Speed.Dev.#3.:  6147.5 MH/s (95.45ms)
Speed.Dev.#4.:  6372.6 MH/s (95.78ms)
Speed.Dev.#*.: 25184.9 MH/s

Hashtype: SSHA-1(Base64), nsldaps, Netscape LDAP SSHA

Speed.Dev.#1.:  6492.2 MH/s (95.94ms)
Speed.Dev.#2.:  6079.0 MH/s (96.04ms)
Speed.Dev.#3.:  5868.3 MH/s (95.93ms)
Speed.Dev.#4.:  6376.4 MH/s (95.79ms)
Speed.Dev.#*.: 24815.9 MH/s

Hashtype: SSHA-512(Base64), LDAP {SSHA512}

Speed.Dev.#1.:   795.2 MH/s (96.08ms)
Speed.Dev.#2.:   788.6 MH/s (96.04ms)
Speed.Dev.#3.:   775.5 MH/s (96.02ms)
Speed.Dev.#4.:   777.6 MH/s (95.75ms)
Speed.Dev.#*.:  3137.0 MH/s

Hashtype: LM

Speed.Dev.#1.: 14240.1 MH/s (96.79ms)
Speed.Dev.#2.: 14160.5 MH/s (97.08ms)
Speed.Dev.#3.: 13967.7 MH/s (97.08ms)
Speed.Dev.#4.: 13975.8 MH/s (96.90ms)
Speed.Dev.#*.: 56344.1 MH/s

Hashtype: NTLM

Speed.Dev.#1.: 31745.4 MH/s (96.10ms)
Speed.Dev.#2.: 31384.6 MH/s (96.29ms)
Speed.Dev.#3.: 31065.3 MH/s (96.17ms)
Speed.Dev.#4.: 31135.9 MH/s (96.13ms)
Speed.Dev.#*.:   125.3 GH/s

Hashtype: Domain Cached Credentials (DCC), MS Cache

Speed.Dev.#1.:  8583.2 MH/s (96.99ms)
Speed.Dev.#2.:  8614.5 MH/s (96.40ms)
Speed.Dev.#3.:  8501.7 MH/s (96.32ms)
Speed.Dev.#4.:  8544.3 MH/s (96.18ms)
Speed.Dev.#*.: 34243.7 MH/s

Hashtype: Domain Cached Credentials 2 (DCC2), MS Cache 2

Speed.Dev.#1.:   249.6 kH/s (96.43ms)
Speed.Dev.#2.:   249.2 kH/s (95.60ms)
Speed.Dev.#3.:   244.9 kH/s (96.26ms)
Speed.Dev.#4.:   248.1 kH/s (95.97ms)
Speed.Dev.#*.:   991.8 kH/s

Hashtype: MS-AzureSync PBKDF2-HMAC-SHA256

Speed.Dev.#1.:  8210.1 kH/s (64.34ms)
Speed.Dev.#2.:  8083.1 kH/s (64.96ms)
Speed.Dev.#3.:  8104.4 kH/s (65.78ms)
Speed.Dev.#4.:  8267.3 kH/s (65.66ms)
Speed.Dev.#*.: 32664.8 kH/s

Hashtype: descrypt, DES(Unix), Traditional DES

Speed.Dev.#1.:   749.7 MH/s (96.07ms)
Speed.Dev.#2.:   739.6 MH/s (95.45ms)
Speed.Dev.#3.:   726.3 MH/s (97.21ms)
Speed.Dev.#4.:   725.8 MH/s (97.27ms)
Speed.Dev.#*.:  2941.5 MH/s

Hashtype: BSDiCrypt, Extended DES

Speed.Dev.#1.:  1176.3 kH/s (103.37ms)
Speed.Dev.#2.:  1186.1 kH/s (103.10ms)
Speed.Dev.#3.:  1148.0 kH/s (103.40ms)
Speed.Dev.#4.:  1153.0 kH/s (103.19ms)
Speed.Dev.#*.:  4663.3 kH/s

Hashtype: md5crypt, MD5(Unix), FreeBSD MD5, Cisco-IOS MD5

Speed.Dev.#1.:  7929.2 kH/s (96.38ms)
Speed.Dev.#2.:  7836.8 kH/s (96.83ms)
Speed.Dev.#3.:  7396.3 kH/s (95.82ms)
Speed.Dev.#4.:  7851.0 kH/s (96.01ms)
Speed.Dev.#*.: 31013.2 kH/s

Hashtype: bcrypt, Blowfish(OpenBSD)

Speed.Dev.#1.:    10936 H/s (43.04ms)
Speed.Dev.#2.:    10249 H/s (42.83ms)
Speed.Dev.#3.:    10653 H/s (43.19ms)
Speed.Dev.#4.:    10167 H/s (43.28ms)
Speed.Dev.#*.:    42005 H/s

Hashtype: sha256crypt, SHA256(Unix)

Speed.Dev.#1.:   282.8 kH/s (93.83ms)
Speed.Dev.#2.:   280.2 kH/s (94.05ms)
Speed.Dev.#3.:   275.9 kH/s (93.84ms)
Speed.Dev.#4.:   276.5 kH/s (93.82ms)
Speed.Dev.#*.:  1115.4 kH/s

Hashtype: sha512crypt, SHA512(Unix)

Speed.Dev.#1.:   104.1 kH/s (105.35ms)
Speed.Dev.#2.:   118.7 kH/s (95.26ms)
Speed.Dev.#3.:   102.3 kH/s (108.26ms)
Speed.Dev.#4.:   102.6 kH/s (107.39ms)
Speed.Dev.#*.:   427.7 kH/s

Hashtype: OSX v10.4, v10.5, v10.6

Speed.Dev.#1.:  5226.2 MH/s (95.98ms)
Speed.Dev.#2.:  5167.6 MH/s (96.23ms)
Speed.Dev.#3.:  5113.1 MH/s (96.13ms)
Speed.Dev.#4.:  5117.0 MH/s (96.34ms)
Speed.Dev.#*.: 20623.9 MH/s

Hashtype: OSX v10.7

Speed.Dev.#1.:   577.3 MH/s (96.64ms)
Speed.Dev.#2.:   624.8 MH/s (95.72ms)
Speed.Dev.#3.:   596.9 MH/s (96.64ms)
Speed.Dev.#4.:   585.1 MH/s (95.39ms)
Speed.Dev.#*.:  2384.1 MH/s

Hashtype: OSX v10.8+

Speed.Dev.#1.:     8953 H/s (95.26ms)
Speed.Dev.#2.:     8784 H/s (96.43ms)
Speed.Dev.#3.:     8694 H/s (95.64ms)
Speed.Dev.#4.:     8710 H/s (94.09ms)
Speed.Dev.#*.:    35141 H/s

Hashtype: AIX {smd5}

Speed.Dev.#1.:  7920.3 kH/s (96.49ms)
Speed.Dev.#2.:  7835.9 kH/s (96.84ms)
Speed.Dev.#3.:  7676.0 kH/s (95.77ms)
Speed.Dev.#4.:  7855.0 kH/s (95.95ms)
Speed.Dev.#*.: 31287.3 kH/s

Hashtype: AIX {ssha1}

Speed.Dev.#1.: 33215.4 kH/s (96.16ms)
Speed.Dev.#2.: 33071.1 kH/s (70.51ms)
Speed.Dev.#3.: 30785.9 kH/s (96.40ms)
Speed.Dev.#4.: 31432.1 kH/s (96.48ms)
Speed.Dev.#*.:   128.5 MH/s

Hashtype: AIX {ssha256}

Speed.Dev.#1.: 13081.0 kH/s (41.57ms)
Speed.Dev.#2.: 12624.7 kH/s (41.94ms)
Speed.Dev.#3.: 11748.6 kH/s (42.50ms)
Speed.Dev.#4.: 12315.3 kH/s (42.48ms)
Speed.Dev.#*.: 49769.5 kH/s

Hashtype: AIX {ssha512}

Speed.Dev.#1.:  4481.2 kH/s (95.78ms)
Speed.Dev.#2.:  4588.9 kH/s (95.79ms)
Speed.Dev.#3.:  4403.8 kH/s (95.58ms)
Speed.Dev.#4.:  4381.7 kH/s (94.90ms)
Speed.Dev.#*.: 17855.6 kH/s

Hashtype: Cisco-PIX MD5

Speed.Dev.#1.: 12462.0 MH/s (59.20ms)
Speed.Dev.#2.: 12336.8 MH/s (59.80ms)
Speed.Dev.#3.: 12222.6 MH/s (60.36ms)
Speed.Dev.#4.: 12237.2 MH/s (60.29ms)
Speed.Dev.#*.: 49258.6 MH/s

Hashtype: Cisco-ASA MD5

Speed.Dev.#1.: 13913.8 MH/s (96.13ms)
Speed.Dev.#2.: 13775.5 MH/s (96.05ms)
Speed.Dev.#3.: 13631.2 MH/s (95.80ms)
Speed.Dev.#4.: 13627.8 MH/s (96.24ms)
Speed.Dev.#*.: 54948.4 MH/s

Hashtype: Cisco-IOS SHA256

Speed.Dev.#1.:  2302.1 MH/s (95.74ms)
Speed.Dev.#2.:  2273.4 MH/s (95.99ms)
Speed.Dev.#3.:  2253.1 MH/s (95.83ms)
Speed.Dev.#4.:  2253.1 MH/s (96.34ms)
Speed.Dev.#*.:  9081.8 MH/s

Hashtype: Cisco $8$

Speed.Dev.#1.:    45133 H/s (95.23ms)
Speed.Dev.#2.:    45115 H/s (95.51ms)
Speed.Dev.#3.:    44441 H/s (95.33ms)
Speed.Dev.#4.:    44040 H/s (95.95ms)
Speed.Dev.#*.:   178.7 kH/s

Hashtype: Cisco $9$

Speed.Dev.#1.:     2537 H/s (550.60ms)
Speed.Dev.#2.:     5064 H/s (555.23ms)
Speed.Dev.#3.:     5013 H/s (561.37ms)
Speed.Dev.#4.:     5022 H/s (560.39ms)
Speed.Dev.#*.:    17636 H/s

Hashtype: Juniper Netscreen/SSG (ScreenOS)

Speed.Dev.#1.: 10148.2 MH/s (96.14ms)
Speed.Dev.#2.: 10042.6 MH/s (96.15ms)
Speed.Dev.#3.:  9938.9 MH/s (96.29ms)
Speed.Dev.#4.:  9949.6 MH/s (96.18ms)
Speed.Dev.#*.: 40079.3 MH/s

Hashtype: Juniper IVE

Speed.Dev.#1.:  7926.0 kH/s (96.41ms)
Speed.Dev.#2.:  7832.9 kH/s (96.86ms)
Speed.Dev.#3.:  7802.5 kH/s (95.81ms)
Speed.Dev.#4.:  7595.5 kH/s (96.00ms)
Speed.Dev.#*.: 31156.9 kH/s

Hashtype: Android PIN

Speed.Dev.#1.:  4181.2 kH/s (95.74ms)
Speed.Dev.#2.:  4129.5 kH/s (63.95ms)
Speed.Dev.#3.:  3997.9 kH/s (96.14ms)
Speed.Dev.#4.:  4104.3 kH/s (96.09ms)
Speed.Dev.#*.: 16412.9 kH/s

Hashtype: Citrix NetScaler

Speed.Dev.#1.:  5471.0 MH/s (96.20ms)
Speed.Dev.#2.:  5661.1 MH/s (96.23ms)
Speed.Dev.#3.:  5596.6 MH/s (96.31ms)
Speed.Dev.#4.:  5572.1 MH/s (96.29ms)
Speed.Dev.#*.: 22300.8 MH/s

Hashtype: RACF

Speed.Dev.#1.:  2014.3 MH/s (103.18ms)
Speed.Dev.#2.:  1996.9 MH/s (102.95ms)
Speed.Dev.#3.:  1937.5 MH/s (102.85ms)
Speed.Dev.#4.:  1908.1 MH/s (106.53ms)
Speed.Dev.#*.:  7856.7 MH/s

Hashtype: GRUB 2

Speed.Dev.#1.:    31277 H/s (94.67ms)
Speed.Dev.#2.:    31060 H/s (94.02ms)
Speed.Dev.#3.:    30563 H/s (95.46ms)
Speed.Dev.#4.:    30479 H/s (94.93ms)
Speed.Dev.#*.:   123.4 kH/s

Hashtype: Radmin2

Speed.Dev.#1.:  6561.9 MH/s (96.19ms)
Speed.Dev.#2.:  6489.5 MH/s (96.38ms)
Speed.Dev.#3.:  6427.5 MH/s (96.19ms)
Speed.Dev.#4.:  6435.6 MH/s (96.30ms)
Speed.Dev.#*.: 25914.6 MH/s

Hashtype: SAP CODVN B (BCODE)

Speed.Dev.#1.:  1578.3 MH/s (130.26ms)
Speed.Dev.#2.:  1555.1 MH/s (132.21ms)
Speed.Dev.#3.:  1542.0 MH/s (134.47ms)
Speed.Dev.#4.:  1514.1 MH/s (133.11ms)
Speed.Dev.#*.:  6189.5 MH/s

Hashtype: SAP CODVN F/G (PASSCODE)

Speed.Dev.#1.:   750.2 MH/s (119.47ms)
Speed.Dev.#2.:   743.1 MH/s (119.86ms)
Speed.Dev.#3.:   734.0 MH/s (119.71ms)
Speed.Dev.#4.:   734.4 MH/s (119.54ms)
Speed.Dev.#*.:  2961.7 MH/s

Hashtype: SAP CODVN H (PWDSALTEDHASH) iSSHA-1

Speed.Dev.#1.:  4548.5 kH/s (64.57ms)
Speed.Dev.#2.:  4702.9 kH/s (64.13ms)
Speed.Dev.#3.:  4390.1 kH/s (64.58ms)
Speed.Dev.#4.:  4553.1 kH/s (96.03ms)
Speed.Dev.#*.: 18194.5 kH/s

Hashtype: Lotus Notes/Domino 5

Speed.Dev.#1.:   170.3 MH/s (148.40ms)
Speed.Dev.#2.:   167.0 MH/s (149.57ms)
Speed.Dev.#3.:   163.9 MH/s (150.67ms)
Speed.Dev.#4.:   160.8 MH/s (144.76ms)
Speed.Dev.#*.:   662.1 MH/s

Hashtype: Lotus Notes/Domino 6

Speed.Dev.#1.: 52456.3 kH/s (140.74ms)
Speed.Dev.#2.: 54205.3 kH/s (142.09ms)
Speed.Dev.#3.: 53351.0 kH/s (144.37ms)
Speed.Dev.#4.: 52137.6 kH/s (143.60ms)
Speed.Dev.#*.:   212.2 MH/s

Hashtype: Lotus Notes/Domino 8

Speed.Dev.#1.:   517.1 kH/s (94.29ms)
Speed.Dev.#2.:   510.1 kH/s (93.89ms)
Speed.Dev.#3.:   497.8 kH/s (94.76ms)
Speed.Dev.#4.:   499.5 kH/s (94.39ms)
Speed.Dev.#*.:  2024.4 kH/s

Hashtype: PeopleSoft

Speed.Dev.#1.:  6587.7 MH/s (94.28ms)
Speed.Dev.#2.:  6529.3 MH/s (94.25ms)
Speed.Dev.#3.:  6459.4 MH/s (94.38ms)
Speed.Dev.#4.:  6461.0 MH/s (94.35ms)
Speed.Dev.#*.: 26037.4 MH/s

Hashtype: PeopleSoft PS_TOKEN

Speed.Dev.#1.:  2323.0 MH/s (95.95ms)
Speed.Dev.#2.:  2362.9 MH/s (96.23ms)
Speed.Dev.#3.:  2337.3 MH/s (95.81ms)
Speed.Dev.#4.:  2239.0 MH/s (96.15ms)
Speed.Dev.#*.:  9262.2 MH/s

Hashtype: 7-Zip

Speed.Dev.#1.:     7156 H/s (96.08ms)
Speed.Dev.#2.:     7013 H/s (96.26ms)
Speed.Dev.#3.:     6827 H/s (96.21ms)
Speed.Dev.#4.:     6973 H/s (96.18ms)
Speed.Dev.#*.:    27969 H/s

Hashtype: WinZip

Speed.Dev.#1.:   829.9 kH/s (83.30ms)
Speed.Dev.#2.:   810.3 kH/s (88.77ms)
Speed.Dev.#3.:   823.4 kH/s (88.84ms)
Speed.Dev.#4.:   819.2 kH/s (88.62ms)
Speed.Dev.#*.:  3282.7 kH/s

Hashtype: RAR3-hp

Speed.Dev.#1.:    30959 H/s (77.50ms)
Speed.Dev.#2.:    31126 H/s (78.00ms)
Speed.Dev.#3.:    30347 H/s (78.48ms)
Speed.Dev.#4.:    30685 H/s (78.82ms)
Speed.Dev.#*.:   123.1 kH/s

Hashtype: RAR5

Speed.Dev.#1.:    27766 H/s (95.21ms)
Speed.Dev.#2.:    27700 H/s (95.45ms)
Speed.Dev.#3.:    26668 H/s (96.15ms)
Speed.Dev.#4.:    27199 H/s (95.36ms)
Speed.Dev.#*.:   109.3 kH/s

Hashtype: AxCrypt

Speed.Dev.#1.:    91520 H/s (277.73ms)
Speed.Dev.#2.:    90378 H/s (266.85ms)
Speed.Dev.#3.:    88920 H/s (270.12ms)
Speed.Dev.#4.:    89410 H/s (268.71ms)
Speed.Dev.#*.:   360.2 kH/s

Hashtype: AxCrypt in memory SHA1

Speed.Dev.#1.:  6001.2 MH/s (95.90ms)
Speed.Dev.#2.:  5966.2 MH/s (96.14ms)
Speed.Dev.#3.:  5904.0 MH/s (95.93ms)
Speed.Dev.#4.:  5887.7 MH/s (96.09ms)
Speed.Dev.#*.: 23759.1 MH/s

Hashtype: TrueCrypt PBKDF2-HMAC-RipeMD160 + XTS 512 bit

Speed.Dev.#1.:   213.6 kH/s (93.85ms)
Speed.Dev.#2.:   210.5 kH/s (94.59ms)
Speed.Dev.#3.:   203.5 kH/s (95.24ms)
Speed.Dev.#4.:   205.1 kH/s (94.89ms)
Speed.Dev.#*.:   832.7 kH/s

Hashtype: TrueCrypt PBKDF2-HMAC-SHA512 + XTS 512 bit

Speed.Dev.#1.:   301.1 kH/s (89.82ms)
Speed.Dev.#2.:   296.8 kH/s (88.61ms)
Speed.Dev.#3.:   294.5 kH/s (89.16ms)
Speed.Dev.#4.:   295.4 kH/s (90.31ms)
Speed.Dev.#*.:  1187.8 kH/s

Hashtype: TrueCrypt PBKDF2-HMAC-Whirlpool + XTS 512 bit

Speed.Dev.#1.:    29049 H/s (265.90ms)
Speed.Dev.#2.:    29048 H/s (268.77ms)
Speed.Dev.#3.:    28794 H/s (264.64ms)
Speed.Dev.#4.:    28379 H/s (264.56ms)
Speed.Dev.#*.:   115.3 kH/s

Hashtype: TrueCrypt PBKDF2-HMAC-RipeMD160 + XTS 512 bit + boot-mode

Speed.Dev.#1.:   401.3 kH/s (90.45ms)
Speed.Dev.#2.:   393.0 kH/s (91.04ms)
Speed.Dev.#3.:   378.8 kH/s (91.71ms)
Speed.Dev.#4.:   390.1 kH/s (89.83ms)
Speed.Dev.#*.:  1563.1 kH/s

Hashtype: VeraCrypt PBKDF2-HMAC-RipeMD160 + XTS 512 bit

Speed.Dev.#1.:      690 H/s (95.19ms)
Speed.Dev.#2.:      678 H/s (95.89ms)
Speed.Dev.#3.:      662 H/s (96.46ms)
Speed.Dev.#4.:      658 H/s (96.18ms)
Speed.Dev.#*.:     2688 H/s

Hashtype: VeraCrypt PBKDF2-HMAC-SHA512 + XTS 512 bit

Speed.Dev.#1.:      660 H/s (95.33ms)
Speed.Dev.#2.:      644 H/s (96.45ms)
Speed.Dev.#3.:      636 H/s (95.98ms)
Speed.Dev.#4.:      642 H/s (95.95ms)
Speed.Dev.#*.:     2583 H/s

Hashtype: VeraCrypt PBKDF2-HMAC-Whirlpool + XTS 512 bit

Speed.Dev.#1.:       58 H/s (265.86ms)
Speed.Dev.#2.:       58 H/s (269.91ms)
Speed.Dev.#3.:       57 H/s (265.47ms)
Speed.Dev.#4.:       57 H/s (265.27ms)
Speed.Dev.#*.:      230 H/s

Hashtype: VeraCrypt PBKDF2-HMAC-RipeMD160 + XTS 512 bit + boot-mode

Speed.Dev.#1.:     1374 H/s (95.18ms)
Speed.Dev.#2.:     1358 H/s (95.89ms)
Speed.Dev.#3.:     1326 H/s (96.53ms)
Speed.Dev.#4.:     1310 H/s (96.20ms)
Speed.Dev.#*.:     5368 H/s

Hashtype: VeraCrypt PBKDF2-HMAC-SHA256 + XTS 512 bit

Speed.Dev.#1.:      901 H/s (96.44ms)
Speed.Dev.#2.:      902 H/s (95.46ms)
Speed.Dev.#3.:      885 H/s (95.69ms)
Speed.Dev.#4.:      894 H/s (95.23ms)
Speed.Dev.#*.:     3581 H/s

Hashtype: VeraCrypt PBKDF2-HMAC-SHA256 + XTS 512 bit + boot-mode

Speed.Dev.#1.:     2294 H/s (94.72ms)
Speed.Dev.#2.:     2244 H/s (95.33ms)
Speed.Dev.#3.:     2240 H/s (95.93ms)
Speed.Dev.#4.:     2196 H/s (95.46ms)
Speed.Dev.#*.:     8973 H/s

Hashtype: Android FDE <= 4.3

Speed.Dev.#1.:   628.9 kH/s (94.07ms)
Speed.Dev.#2.:   605.5 kH/s (94.24ms)
Speed.Dev.#3.:   595.0 kH/s (95.42ms)
Speed.Dev.#4.:   610.0 kH/s (94.18ms)
Speed.Dev.#*.:  2439.3 kH/s

Hashtype: Android FDE (Samsung DEK)

Speed.Dev.#1.:   223.0 kH/s (93.26ms)
Speed.Dev.#2.:   221.1 kH/s (93.55ms)
Speed.Dev.#3.:   217.0 kH/s (93.14ms)
Speed.Dev.#4.:   216.0 kH/s (93.42ms)
Speed.Dev.#*.:   877.1 kH/s

Hashtype: eCryptfs

Speed.Dev.#1.:    10464 H/s (95.76ms)
Speed.Dev.#2.:    10361 H/s (95.43ms)
Speed.Dev.#3.:    10289 H/s (95.85ms)
Speed.Dev.#4.:    10127 H/s (96.21ms)
Speed.Dev.#*.:    41241 H/s

Hashtype: MS Office <= 2003 MD5 + RC4, oldoffice$0, oldoffice$1

Speed.Dev.#1.:   174.0 MH/s (109.77ms)
Speed.Dev.#2.:   179.9 MH/s (104.13ms)
Speed.Dev.#3.:   177.4 MH/s (105.29ms)
Speed.Dev.#4.:   170.8 MH/s (105.25ms)
Speed.Dev.#*.:   702.1 MH/s

Hashtype: MS Office <= 2003 MD5 + RC4, collision-mode #1

Speed.Dev.#1.:   234.3 MH/s (111.00ms)
Speed.Dev.#2.:   257.5 MH/s (111.27ms)
Speed.Dev.#3.:   250.3 MH/s (110.44ms)
Speed.Dev.#4.:   256.2 MH/s (111.09ms)
Speed.Dev.#*.:   998.3 MH/s

Hashtype: MS Office <= 2003 SHA1 + RC4, oldoffice$3, oldoffice$4

Speed.Dev.#1.:   238.1 MH/s (107.76ms)
Speed.Dev.#2.:   235.6 MH/s (107.78ms)
Speed.Dev.#3.:   232.4 MH/s (108.11ms)
Speed.Dev.#4.:   233.3 MH/s (107.71ms)
Speed.Dev.#*.:   939.4 MH/s

Hashtype: MS Office <= 2003 SHA1 + RC4, collision-mode #1

Speed.Dev.#1.:   264.8 MH/s (110.21ms)
Speed.Dev.#2.:   261.6 MH/s (110.19ms)
Speed.Dev.#3.:   258.4 MH/s (110.18ms)
Speed.Dev.#4.:   254.9 MH/s (110.67ms)
Speed.Dev.#*.:  1039.7 MH/s

Hashtype: Office 2007

Speed.Dev.#1.:   103.3 kH/s (96.29ms)
Speed.Dev.#2.:   102.1 kH/s (96.18ms)
Speed.Dev.#3.:   100.3 kH/s (96.16ms)
Speed.Dev.#4.:   100.7 kH/s (96.03ms)
Speed.Dev.#*.:   406.4 kH/s

Hashtype: Office 2010

Speed.Dev.#1.:    51159 H/s (96.30ms)
Speed.Dev.#2.:    50109 H/s (96.21ms)
Speed.Dev.#3.:    50563 H/s (96.20ms)
Speed.Dev.#4.:    49675 H/s (96.30ms)
Speed.Dev.#*.:   201.5 kH/s

Hashtype: Office 2013

Speed.Dev.#1.:     6759 H/s (95.89ms)
Speed.Dev.#2.:     6661 H/s (96.11ms)
Speed.Dev.#3.:     6485 H/s (96.77ms)
Speed.Dev.#4.:     6587 H/s (95.05ms)
Speed.Dev.#*.:    26492 H/s

Hashtype: PDF 1.1 - 1.3 (Acrobat 2 - 4)

Speed.Dev.#1.:   268.6 MH/s (109.34ms)
Speed.Dev.#2.:   265.6 MH/s (109.21ms)
Speed.Dev.#3.:   261.6 MH/s (109.52ms)
Speed.Dev.#4.:   262.9 MH/s (109.66ms)
Speed.Dev.#*.:  1058.6 MH/s

Hashtype: PDF 1.1 - 1.3 (Acrobat 2 - 4) + collider-mode #1

Speed.Dev.#1.:   289.8 MH/s (110.82ms)
Speed.Dev.#2.:   294.5 MH/s (110.19ms)
Speed.Dev.#3.:   289.9 MH/s (110.93ms)
Speed.Dev.#4.:   291.7 MH/s (110.24ms)
Speed.Dev.#*.:  1165.9 MH/s

Hashtype: PDF 1.4 - 1.6 (Acrobat 5 - 8)

Speed.Dev.#1.: 13401.3 kH/s (51.83ms)
Speed.Dev.#2.: 10643.5 kH/s (52.46ms)
Speed.Dev.#3.: 10862.8 kH/s (53.16ms)
Speed.Dev.#4.: 11241.7 kH/s (52.85ms)
Speed.Dev.#*.: 46149.3 kH/s

Hashtype: PDF 1.7 Level 3 (Acrobat 9)

Speed.Dev.#1.:  2111.5 MH/s (96.08ms)
Speed.Dev.#2.:  2270.6 MH/s (95.85ms)
Speed.Dev.#3.:  2240.1 MH/s (96.51ms)
Speed.Dev.#4.:  2227.8 MH/s (95.93ms)
Speed.Dev.#*.:  8849.9 MH/s

Hashtype: PDF 1.7 Level 8 (Acrobat 10 - 11)

Speed.Dev.#1.:    25647 H/s (437.70ms)
Speed.Dev.#2.:    25392 H/s (402.90ms)
Speed.Dev.#3.:    25116 H/s (444.49ms)
Speed.Dev.#4.:    25275 H/s (406.84ms)
Speed.Dev.#*.:   101.4 kH/s

Hashtype: Password Safe v2

Speed.Dev.#1.:   268.2 kH/s (53.57ms)
Speed.Dev.#2.:   262.3 kH/s (55.24ms)
Speed.Dev.#3.:   238.0 kH/s (55.02ms)
Speed.Dev.#4.:   253.1 kH/s (53.60ms)
Speed.Dev.#*.:  1021.6 kH/s

Hashtype: Password Safe v3

Speed.Dev.#1.:   919.2 kH/s (88.81ms)
Speed.Dev.#2.:   899.8 kH/s (88.86ms)
Speed.Dev.#3.:   887.4 kH/s (88.83ms)
Speed.Dev.#4.:   904.1 kH/s (89.98ms)
Speed.Dev.#*.:  3610.6 kH/s

Hashtype: Lastpass

Speed.Dev.#1.:  1802.2 kH/s (71.73ms)
Speed.Dev.#2.:  1737.3 kH/s (72.48ms)
Speed.Dev.#3.:  1728.3 kH/s (72.36ms)
Speed.Dev.#4.:  1734.9 kH/s (95.93ms)
Speed.Dev.#*.:  7002.7 kH/s

Hashtype: 1Password, agilekeychain

Speed.Dev.#1.:  2527.7 kH/s (72.19ms)
Speed.Dev.#2.:  2487.2 kH/s (72.14ms)
Speed.Dev.#3.:  2454.6 kH/s (73.16ms)
Speed.Dev.#4.:  2485.1 kH/s (96.19ms)
Speed.Dev.#*.:  9954.6 kH/s

Hashtype: 1Password, cloudkeychain

Speed.Dev.#1.:     7816 H/s (94.29ms)
Speed.Dev.#2.:     7768 H/s (94.49ms)
Speed.Dev.#3.:     7600 H/s (95.27ms)
Speed.Dev.#4.:     7605 H/s (96.04ms)
Speed.Dev.#*.:    30788 H/s

Hashtype: Bitcoin/Litecoin wallet.dat

Speed.Dev.#1.:     3410 H/s (95.76ms)
Speed.Dev.#2.:     3402 H/s (96.00ms)
Speed.Dev.#3.:     3307 H/s (95.92ms)
Speed.Dev.#4.:     3339 H/s (96.26ms)
Speed.Dev.#*.:    13458 H/s

Hashtype: Blockchain, My Wallet

Speed.Dev.#1.: 56292.5 kH/s (45.36ms)
Speed.Dev.#2.: 47800.8 kH/s (45.78ms)
Speed.Dev.#3.: 50901.7 kH/s (46.36ms)
Speed.Dev.#4.: 53772.1 kH/s (46.25ms)
Speed.Dev.#*.:   208.8 MH/s

Hashtype: Keepass 1 (AES/Twofish) and Keepass 2 (AES)

Speed.Dev.#1.:   109.7 kH/s (258.37ms)
Speed.Dev.#2.:   108.6 kH/s (260.02ms)
Speed.Dev.#3.:   108.5 kH/s (255.21ms)
Speed.Dev.#4.:   107.9 kH/s (257.42ms)
Speed.Dev.#*.:   434.8 kH/s

Hashtype: ArubaOS

Speed.Dev.#1.:  5223.8 MH/s (96.00ms)
Speed.Dev.#2.:  5169.8 MH/s (96.18ms)
Speed.Dev.#3.:  5083.6 MH/s (96.43ms)
Speed.Dev.#4.:  5117.9 MH/s (96.31ms)
Speed.Dev.#*.: 20595.0 MH/s

Started: Fri Aug 26 16:25:50 2016
Stopped: Fri Aug 26 16:50:55 2016
```
