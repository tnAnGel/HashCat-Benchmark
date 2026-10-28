# NVIDIA RTX A5000

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA RTX A5000 (8 одинаковых карт)
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [OnlineHashCrack](https://www.onlinehashcrack.com/tools-benchmark-hashcat-nvidia-rtx-A5000.php)
- **Параметры / Options:** `-b --benchmark-all -O -w 4`
- **Примечание / Note:** полный публичный сырой вывод восьмикартного прогона; `Speed.#1`–`Speed.#8` — отдельные RTX A5000, `Speed.#*` — сумма рига.

## Ключевые результаты / Highlights (Speed.#*)

| Mode | Алгоритм | Скорость рига |
|-----:|----------|--------------:|
| 0 | MD5 | 392.9 GH/s |
| 100 | SHA1 | 130.5 GH/s |
| 1400 | SHA2-256 | 55.8132 GH/s |
| 1700 | SHA2-512 | 18.6654 GH/s |
| 1000 | NTLM | 659.9 GH/s |
| 3200 | bcrypt | 686.5 kH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 6543.6 kH/s |

## Полный вывод `hashcat -b --benchmark-all` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

CUDA API (CUDA 12.0)
====================
* Device #1: NVIDIA RTX A5000, 24043/24247 MB, 64MCU
* Device #2: NVIDIA RTX A5000, 24043/24247 MB, 64MCU
* Device #3: NVIDIA RTX A5000, 24043/24247 MB, 64MCU
* Device #4: NVIDIA RTX A5000, 24043/24247 MB, 64MCU
* Device #5: NVIDIA RTX A5000, 24043/24247 MB, 64MCU
* Device #6: NVIDIA RTX A5000, 24043/24247 MB, 64MCU
* Device #7: NVIDIA RTX A5000, 24043/24247 MB, 64MCU
* Device #8: NVIDIA RTX A5000, 24043/24247 MB, 64MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable
* --workload-profile=4

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 48760.8 MH/s (87.18ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#2.........: 49965.6 MH/s (85.04ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#3.........: 48009.2 MH/s (88.55ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#4.........: 49150.9 MH/s (86.48ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#5.........: 48695.3 MH/s (87.31ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#6.........: 49137.5 MH/s (86.52ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#7.........: 49971.3 MH/s (85.03ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#8.........: 49210.6 MH/s (86.36ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#*.........:   392.9 GH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 16226.6 MH/s (131.56ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#2.........: 16634.9 MH/s (128.33ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#3.........: 15931.7 MH/s (133.93ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#4.........: 16368.0 MH/s (130.49ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#5.........: 16201.9 MH/s (131.76ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#6.........: 16250.0 MH/s (131.36ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#7.........: 16508.2 MH/s (129.26ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#8.........: 16364.3 MH/s (130.45ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#*.........:   130.5 GH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  6922.4 MH/s (308.97ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#2.........:  7104.5 MH/s (301.12ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#3.........:  6856.0 MH/s (311.87ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#4.........:  6983.3 MH/s (306.36ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#5.........:  6922.8 MH/s (309.04ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#6.........:  6983.4 MH/s (306.36ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#7.........:  7044.7 MH/s (303.68ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#8.........:  6996.1 MH/s (305.79ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#*.........: 55813.2 MH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  2318.4 MH/s (461.66ms) @ Accel:64 Loops:512 Thr:512 Vec:1
Speed.#2.........:  2374.7 MH/s (450.60ms) @ Accel:64 Loops:512 Thr:512 Vec:1
Speed.#3.........:  2275.2 MH/s (470.27ms) @ Accel:64 Loops:512 Thr:512 Vec:1
Speed.#4.........:  2332.0 MH/s (458.95ms) @ Accel:64 Loops:512 Thr:512 Vec:1
Speed.#5.........:  2317.2 MH/s (461.87ms) @ Accel:64 Loops:512 Thr:512 Vec:1
Speed.#6.........:  2337.8 MH/s (457.78ms) @ Accel:64 Loops:512 Thr:512 Vec:1
Speed.#7.........:  2355.4 MH/s (454.36ms) @ Accel:64 Loops:512 Thr:512 Vec:1
Speed.#8.........:  2354.6 MH/s (454.49ms) @ Accel:64 Loops:512 Thr:512 Vec:1
Speed.#*.........: 18665.4 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   816.4 kH/s (318.86ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#2.........:   831.3 kH/s (313.09ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#3.........:   799.8 kH/s (324.94ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#4.........:   819.0 kH/s (317.83ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#5.........:   809.6 kH/s (321.56ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#6.........:   816.2 kH/s (318.92ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#7.........:   827.6 kH/s (314.54ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#8.........:   823.7 kH/s (316.03ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#*.........:  6543.6 kH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 82244.5 MH/s (51.40ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#2.........: 84251.1 MH/s (50.10ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#3.........: 80372.3 MH/s (52.56ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#4.........: 82578.2 MH/s (51.16ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#5.........: 81547.2 MH/s (51.79ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#6.........: 82301.0 MH/s (51.33ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#7.........: 83520.5 MH/s (50.57ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#8.........: 83050.2 MH/s (50.89ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#*.........:   659.9 GH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 48341.5 MH/s (21.68ms) @ Accel:128 Loops:1024 Thr:128 Vec:1
Speed.#2.........: 49734.7 MH/s (21.11ms) @ Accel:128 Loops:1024 Thr:128 Vec:1
Speed.#3.........: 47587.7 MH/s (22.02ms) @ Accel:128 Loops:1024 Thr:128 Vec:1
Speed.#4.........: 48864.2 MH/s (21.43ms) @ Accel:128 Loops:1024 Thr:128 Vec:1
Speed.#5.........: 48197.8 MH/s (21.76ms) @ Accel:128 Loops:1024 Thr:128 Vec:1
Speed.#6.........: 48671.9 MH/s (21.57ms) @ Accel:128 Loops:1024 Thr:128 Vec:1
Speed.#7.........: 49400.7 MH/s (21.29ms) @ Accel:128 Loops:1024 Thr:128 Vec:1
Speed.#8.........: 48854.0 MH/s (21.44ms) @ Accel:128 Loops:1024 Thr:128 Vec:1
Speed.#*.........:   389.7 GH/s

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 49912.0 MH/s (85.16ms) @ Accel:512 Loops:1024 Thr:128 Vec:1
Speed.#2.........: 51268.8 MH/s (82.83ms) @ Accel:512 Loops:1024 Thr:128 Vec:1
Speed.#3.........: 49174.0 MH/s (86.34ms) @ Accel:512 Loops:1024 Thr:128 Vec:1
Speed.#4.........: 50303.9 MH/s (84.42ms) @ Accel:512 Loops:1024 Thr:128 Vec:1
Speed.#5.........: 49916.5 MH/s (85.16ms) @ Accel:512 Loops:1024 Thr:128 Vec:1
Speed.#6.........: 50305.8 MH/s (84.46ms) @ Accel:512 Loops:1024 Thr:128 Vec:1
Speed.#7.........: 51001.3 MH/s (83.30ms) @ Accel:512 Loops:1024 Thr:128 Vec:1
Speed.#8.........: 50482.8 MH/s (84.12ms) @ Accel:512 Loops:1024 Thr:128 Vec:1
Speed.#*.........:   402.4 GH/s

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  3607.7 MH/s (296.73ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  3702.3 MH/s (289.13ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  3541.3 MH/s (302.23ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  3638.1 MH/s (294.29ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#5.........:  3606.1 MH/s (296.90ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#6.........:  3638.2 MH/s (294.27ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#7.........:  3671.1 MH/s (291.56ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#8.........:  3639.9 MH/s (294.08ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#*.........: 29044.5 MH/s

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  1997.6 MH/s (268.04ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  2048.2 MH/s (261.44ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  1961.2 MH/s (272.95ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  2010.6 MH/s (266.32ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#5.........:  1985.4 MH/s (269.70ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#6.........:  2003.6 MH/s (267.24ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#7.........:  2031.4 MH/s (263.63ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#8.........:  2014.2 MH/s (265.83ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#*.........: 16052.3 MH/s

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 21165.3 kH/s (179.14ms) @ Accel:128 Loops:1000 Thr:512 Vec:1
Speed.#2.........: 21594.8 kH/s (175.39ms) @ Accel:128 Loops:1000 Thr:512 Vec:1
Speed.#3.........: 20401.9 kH/s (184.06ms) @ Accel:128 Loops:1000 Thr:512 Vec:1
Speed.#4.........: 21162.4 kH/s (178.91ms) @ Accel:128 Loops:1000 Thr:512 Vec:1
Speed.#5.........: 20942.2 kH/s (181.23ms) @ Accel:128 Loops:1000 Thr:512 Vec:1
Speed.#6.........: 21142.1 kH/s (179.28ms) @ Accel:128 Loops:1000 Thr:512 Vec:1
Speed.#7.........: 21341.9 kH/s (177.61ms) @ Accel:128 Loops:1000 Thr:512 Vec:1
Speed.#8.........: 21130.4 kH/s (179.06ms) @ Accel:128 Loops:1000 Thr:512 Vec:1
Speed.#*.........:   168.9 MH/s

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    85607 H/s (279.20ms) @ Accel:16 Loops:32 Thr:24 Vec:1
Speed.#2.........:    87337 H/s (273.49ms) @ Accel:16 Loops:32 Thr:24 Vec:1
Speed.#3.........:    81114 H/s (285.85ms) @ Accel:16 Loops:32 Thr:24 Vec:1
Speed.#4.........:    87329 H/s (273.72ms) @ Accel:16 Loops:32 Thr:24 Vec:1
Speed.#5.........:    84438 H/s (283.12ms) @ Accel:16 Loops:32 Thr:24 Vec:1
Speed.#6.........:    86229 H/s (277.06ms) @ Accel:16 Loops:32 Thr:24 Vec:1
Speed.#7.........:    86913 H/s (274.96ms) @ Accel:16 Loops:32 Thr:24 Vec:1
Speed.#8.........:    87563 H/s (272.86ms) @ Accel:16 Loops:32 Thr:24 Vec:1
Speed.#*.........:   686.5 kH/s

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:   347.3 kH/s (299.18ms) @ Accel:2048 Loops:1024 Thr:256 Vec:1
Speed.#2.........:   353.8 kH/s (293.55ms) @ Accel:2048 Loops:1024 Thr:256 Vec:1
Speed.#3.........:   340.5 kH/s (304.62ms) @ Accel:2048 Loops:1024 Thr:256 Vec:1
Speed.#4.........:   346.6 kH/s (299.84ms) @ Accel:2048 Loops:1024 Thr:256 Vec:1
Speed.#5.........:   345.0 kH/s (301.15ms) @ Accel:2048 Loops:1024 Thr:256 Vec:1
Speed.#6.........:   346.7 kH/s (299.69ms) @ Accel:2048 Loops:1024 Thr:256 Vec:1
Speed.#7.........:   352.8 kH/s (294.42ms) @ Accel:2048 Loops:1024 Thr:256 Vec:1
Speed.#8.........:   347.5 kH/s (298.86ms) @ Accel:2048 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  2780.2 kH/s

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  1169.2 MH/s (457.72ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#2.........:  1195.4 MH/s (447.63ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#3.........:  1149.2 MH/s (465.65ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#4.........:  1179.0 MH/s (453.93ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#5.........:  1169.1 MH/s (457.77ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#6.........:  1178.3 MH/s (454.16ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#7.........:  1188.4 MH/s (450.25ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#8.........:  1186.6 MH/s (450.98ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#*.........:  9415.1 MH/s

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:  1146.6 MH/s (466.73ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#2.........:  1177.2 MH/s (454.58ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#3.........:  1128.4 MH/s (474.30ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#4.........:  1155.0 MH/s (463.32ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#5.........:  1141.8 MH/s (468.75ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#6.........:  1153.4 MH/s (463.95ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#7.........:  1168.4 MH/s (458.00ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#8.........:  1159.5 MH/s (461.55ms) @ Accel:1024 Loops:256 Thr:32 Vec:1
Speed.#*.........:  9230.2 MH/s

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:   142.7 kH/s (312.55ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#2.........:   146.3 kH/s (304.82ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#3.........:   140.1 kH/s (318.06ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#4.........:   143.9 kH/s (309.92ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#5.........:   142.7 kH/s (312.68ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#6.........:   143.0 kH/s (311.98ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#7.........:   145.5 kH/s (306.66ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#8.........:   144.3 kH/s (309.13ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#*.........:  1148.5 kH/s

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    80558 H/s (256.84ms) @ Accel:32 Loops:256 Thr:512 Vec:1
Speed.#2.........:    82294 H/s (251.73ms) @ Accel:32 Loops:256 Thr:512 Vec:1
Speed.#3.........:    79353 H/s (261.05ms) @ Accel:32 Loops:256 Thr:512 Vec:1
Speed.#4.........:    80816 H/s (256.31ms) @ Accel:32 Loops:256 Thr:512 Vec:1
Speed.#5.........:    80593 H/s (257.02ms) @ Accel:32 Loops:256 Thr:512 Vec:1
Speed.#6.........:    80712 H/s (256.64ms) @ Accel:32 Loops:256 Thr:512 Vec:1
Speed.#7.........:    81825 H/s (253.16ms) @ Accel:32 Loops:256 Thr:512 Vec:1
Speed.#8.........:    81410 H/s (254.47ms) @ Accel:32 Loops:256 Thr:512 Vec:1
Speed.#*.........:   647.6 kH/s

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   992.4 kH/s (174.27ms) @ Accel:16 Loops:511 Thr:512 Vec:1
Speed.#2.........:  1009.0 kH/s (171.37ms) @ Accel:16 Loops:511 Thr:512 Vec:1
Speed.#3.........:   974.2 kH/s (177.56ms) @ Accel:16 Loops:511 Thr:512 Vec:1
Speed.#4.........:   980.0 kH/s (175.07ms) @ Accel:16 Loops:511 Thr:512 Vec:1
Speed.#5.........:   980.3 kH/s (176.45ms) @ Accel:16 Loops:511 Thr:512 Vec:1
Speed.#6.........:   991.2 kH/s (173.74ms) @ Accel:16 Loops:511 Thr:512 Vec:1
Speed.#7.........:  1007.8 kH/s (171.62ms) @ Accel:16 Loops:511 Thr:512 Vec:1
Speed.#8.........:   996.9 kH/s (173.44ms) @ Accel:16 Loops:511 Thr:512 Vec:1
Speed.#*.........:  7931.9 kH/s

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   667.1 kH/s (308.73ms) @ Accel:256 Loops:4096 Thr:64 Vec:1
Speed.#2.........:   678.8 kH/s (303.43ms) @ Accel:256 Loops:4096 Thr:64 Vec:1
Speed.#3.........:   666.3 kH/s (313.86ms) @ Accel:256 Loops:4096 Thr:64 Vec:1
Speed.#4.........:   667.9 kH/s (308.96ms) @ Accel:256 Loops:4096 Thr:64 Vec:1
Speed.#5.........:   669.7 kH/s (309.41ms) @ Accel:256 Loops:4096 Thr:64 Vec:1
Speed.#6.........:   671.1 kH/s (308.01ms) @ Accel:256 Loops:4096 Thr:64 Vec:1
Speed.#7.........:   682.1 kH/s (303.77ms) @ Accel:256 Loops:4096 Thr:64 Vec:1
Speed.#8.........:   672.9 kH/s (307.20ms) @ Accel:256 Loops:4096 Thr:64 Vec:1
Speed.#*.........:  5376.0 kH/s

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    94044 H/s (10.54ms) @ Accel:32 Loops:16384 Thr:256 Vec:1
Speed.#2.........:    95335 H/s (10.38ms) @ Accel:32 Loops:16384 Thr:256 Vec:1
Speed.#3.........:    88619 H/s (10.95ms) @ Accel:32 Loops:16384 Thr:256 Vec:1
Speed.#4.........:    94161 H/s (10.54ms) @ Accel:32 Loops:16384 Thr:256 Vec:1
Speed.#5.........:    92816 H/s (10.68ms) @ Accel:32 Loops:16384 Thr:256 Vec:1
Speed.#6.........:    94639 H/s (10.46ms) @ Accel:32 Loops:16384 Thr:256 Vec:1
Speed.#7.........:    94560 H/s (10.50ms) @ Accel:32 Loops:16384 Thr:256 Vec:1
Speed.#8.........:    94330 H/s (10.53ms) @ Accel:32 Loops:16384 Thr:256 Vec:1
Speed.#*.........:   748.5 kH/s

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    87534 H/s (373.07ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#2.........:    89753 H/s (363.80ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#3.........:    85996 H/s (379.39ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#4.........:    87852 H/s (371.68ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#5.........:    87593 H/s (372.78ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#6.........:    87774 H/s (372.02ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#7.........:    88760 H/s (367.93ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#8.........:    88378 H/s (369.46ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#*.........:   703.6 kH/s

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:   614.7 kH/s (391.34ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#2.........:   628.4 kH/s (382.63ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#3.........:   596.7 kH/s (400.03ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#4.........:   616.5 kH/s (390.36ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#5.........:   613.0 kH/s (392.50ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#6.........:   614.0 kH/s (391.32ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#7.........:   624.6 kH/s (385.19ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#8.........:   619.5 kH/s (388.64ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:  4927.5 kH/s

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:   109.5 kH/s (398.23ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#2.........:   112.5 kH/s (387.57ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#3.........:   107.7 kH/s (404.74ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#4.........:   111.1 kH/s (392.56ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#5.........:   109.4 kH/s (398.70ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#6.........:   110.2 kH/s (395.58ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#7.........:   111.5 kH/s (391.16ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#8.........:   111.3 kH/s (391.69ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   883.3 kH/s

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  5510.4 kH/s (243.48ms) @ Accel:128 Loops:249 Thr:512 Vec:1
Speed.#2.........:  5637.0 kH/s (237.90ms) @ Accel:128 Loops:249 Thr:512 Vec:1
Speed.#3.........:  5358.8 kH/s (249.31ms) @ Accel:128 Loops:249 Thr:512 Vec:1
Speed.#4.........:  5531.2 kH/s (242.45ms) @ Accel:128 Loops:249 Thr:512 Vec:1
Speed.#5.........:  5511.5 kH/s (243.33ms) @ Accel:128 Loops:249 Thr:512 Vec:1
Speed.#6.........:  5515.3 kH/s (243.31ms) @ Accel:128 Loops:249 Thr:512 Vec:1
Speed.#7.........:  5579.0 kH/s (240.40ms) @ Accel:128 Loops:249 Thr:512 Vec:1
Speed.#8.........:  5563.8 kH/s (240.96ms) @ Accel:128 Loops:249 Thr:512 Vec:1
Speed.#*.........: 44207.0 kH/s

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:    10633 H/s (251.33ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#2.........:    10934 H/s (244.40ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#3.........:    10459 H/s (255.53ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#4.........:    10680 H/s (250.23ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#5.........:    10648 H/s (250.98ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#6.........:    10654 H/s (250.84ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#7.........:    10836 H/s (246.53ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#8.........:    10749 H/s (248.61ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:    85593 H/s
```
