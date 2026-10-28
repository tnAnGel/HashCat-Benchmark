# NVIDIA B200 (8x rig (AWS p6-b200) — Blackwell DC)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA B200
- **Конфигурация / Setup:** 8x rig (AWS p6-b200) — Blackwell DC
- **Версия hashcat / Version:** v7.1.2
- **Источник / Source:** [javydekoning](https://github.com/javydekoning/aws-hashcat)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 140.4 GH/s |
| 100 | SHA1 | 48807.9 MH/s |
| 1400 | SHA2-256 | 16383.0 MH/s |
| 1700 | SHA2-512 | 5700.1 MH/s |
| 1000 | NTLM | 247.6 GH/s |
| 3200 | bcrypt | 420.3 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 2388.5 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v7.1.2) starting in benchmark mode

CUDA API (CUDA 12.8)
====================
* Device #01: NVIDIA B200, 182014/182642 MB, 148MCU
* Device #02: NVIDIA B200, 182014/182642 MB, 148MCU
* Device #03: NVIDIA B200, 182014/182642 MB, 148MCU
* Device #04: NVIDIA B200, 182014/182642 MB, 148MCU
* Device #05: NVIDIA B200, 182014/182642 MB, 148MCU
* Device #06: NVIDIA B200, 182014/182642 MB, 148MCU
* Device #07: NVIDIA B200, 182014/182642 MB, 148MCU
* Device #08: NVIDIA B200, 182014/182642 MB, 148MCU

OpenCL API (OpenCL 3.0 CUDA 12.8.97) - Platform #1 [NVIDIA Corporation]
=======================================================================
* Device #09: NVIDIA B200, skipped
* Device #10: NVIDIA B200, skipped
* Device #11: NVIDIA B200, skipped
* Device #12: NVIDIA B200, skipped
* Device #13: NVIDIA B200, skipped
* Device #14: NVIDIA B200, skipped
* Device #15: NVIDIA B200, skipped
* Device #16: NVIDIA B200, skipped

Benchmark relevant options:
===========================
* --backend-devices-virtmulti=1
* --backend-devices-virthost=1
* --optimized-kernel-enable

---------------------
* Hash-Mode 900 (MD4)
---------------------

Speed.#01........:   250.6 GH/s (41.33ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#02........:   250.9 GH/s (41.33ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#03........:   250.6 GH/s (41.32ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#04........:   250.6 GH/s (41.33ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#05........:   250.7 GH/s (41.36ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#06........:   250.6 GH/s (41.37ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#07........:   250.9 GH/s (41.33ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#08........:   250.8 GH/s (41.34ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#*.........:  2005.7 GH/s

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#01........:   140.4 GH/s (73.96ms) @ Accel:96 Loops:1024 Thr:896 Vec:8
Speed.#02........:   140.5 GH/s (73.96ms) @ Accel:96 Loops:1024 Thr:896 Vec:8
Speed.#03........:   140.4 GH/s (73.91ms) @ Accel:96 Loops:1024 Thr:896 Vec:8
Speed.#04........:   140.4 GH/s (73.93ms) @ Accel:96 Loops:1024 Thr:896 Vec:8
Speed.#05........:   140.3 GH/s (74.03ms) @ Accel:96 Loops:1024 Thr:896 Vec:8
Speed.#06........:   140.4 GH/s (73.99ms) @ Accel:96 Loops:1024 Thr:896 Vec:8
Speed.#07........:   140.5 GH/s (73.92ms) @ Accel:96 Loops:1024 Thr:896 Vec:8
Speed.#08........:   140.4 GH/s (74.00ms) @ Accel:96 Loops:1024 Thr:896 Vec:8
Speed.#*.........:  1123.3 GH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#01........: 48807.9 MH/s (95.16ms) @ Accel:48 Loops:1024 Thr:640 Vec:1
Speed.#02........: 48863.8 MH/s (95.06ms) @ Accel:48 Loops:1024 Thr:640 Vec:1
Speed.#03........: 48790.1 MH/s (95.14ms) @ Accel:48 Loops:1024 Thr:640 Vec:1
Speed.#04........: 48815.4 MH/s (95.09ms) @ Accel:48 Loops:1024 Thr:640 Vec:1
Speed.#05........: 48804.8 MH/s (95.17ms) @ Accel:48 Loops:1024 Thr:640 Vec:1
Speed.#06........: 48797.7 MH/s (95.18ms) @ Accel:48 Loops:1024 Thr:640 Vec:1
Speed.#07........: 48888.2 MH/s (95.01ms) @ Accel:48 Loops:1024 Thr:640 Vec:1
Speed.#08........: 48788.5 MH/s (95.20ms) @ Accel:48 Loops:1024 Thr:640 Vec:1
Speed.#*.........:   390.6 GH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#01........: 16383.0 MH/s (94.49ms) @ Accel:20 Loops:1024 Thr:512 Vec:4
Speed.#02........: 16441.2 MH/s (94.21ms) @ Accel:20 Loops:1024 Thr:512 Vec:4
Speed.#03........: 16396.8 MH/s (94.40ms) @ Accel:20 Loops:1024 Thr:512 Vec:4
Speed.#04........: 16396.3 MH/s (94.41ms) @ Accel:20 Loops:1024 Thr:512 Vec:4
Speed.#05........: 16401.8 MH/s (94.43ms) @ Accel:20 Loops:1024 Thr:512 Vec:4
Speed.#06........: 16402.6 MH/s (94.42ms) @ Accel:20 Loops:1024 Thr:512 Vec:4
Speed.#07........: 16446.3 MH/s (94.17ms) @ Accel:20 Loops:1024 Thr:512 Vec:4
Speed.#08........: 16392.1 MH/s (94.49ms) @ Accel:20 Loops:1024 Thr:512 Vec:4
Speed.#*.........:   131.3 GH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#01........:  5700.1 MH/s (81.45ms) @ Accel:6 Loops:512 Thr:1024 Vec:1
Speed.#02........:  5707.4 MH/s (81.35ms) @ Accel:6 Loops:512 Thr:1024 Vec:1
Speed.#03........:  5703.1 MH/s (81.41ms) @ Accel:6 Loops:512 Thr:1024 Vec:1
Speed.#04........:  5702.6 MH/s (81.41ms) @ Accel:6 Loops:512 Thr:1024 Vec:1
Speed.#05........:  5704.2 MH/s (81.45ms) @ Accel:6 Loops:512 Thr:1024 Vec:1
Speed.#06........:  5701.9 MH/s (81.48ms) @ Accel:6 Loops:512 Thr:1024 Vec:1
Speed.#07........:  5712.6 MH/s (81.33ms) @ Accel:6 Loops:512 Thr:1024 Vec:1
Speed.#08........:  5703.2 MH/s (81.47ms) @ Accel:6 Loops:512 Thr:1024 Vec:1
Speed.#*.........: 45635.1 MH/s

---------------------------
* Hash-Mode 5100 (Half MD5)
---------------------------

Speed.#01........: 91250.2 MH/s (94.96ms) @ Accel:56 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:   722.7 GH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#01........:   247.6 GH/s (86.60ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#02........:   247.9 GH/s (86.50ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#03........:   247.7 GH/s (86.58ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#04........:   247.8 GH/s (86.54ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#05........:   247.8 GH/s (86.59ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#06........:   247.8 GH/s (86.61ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#07........:   248.2 GH/s (86.46ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#08........:   247.7 GH/s (86.63ms) @ Accel:192 Loops:1024 Thr:768 Vec:8
Speed.#*.........:  1982.4 GH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#01........:   107.5 GH/s (26.70ms) @ Accel:256 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   861.1 GH/s

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#01........:   420.3 kH/s (95.79ms) @ Accel:5 Loops:32 Thr:56 Vec:1
Speed.#02........:   420.3 kH/s (95.77ms) @ Accel:5 Loops:32 Thr:56 Vec:1
Speed.#03........:   420.0 kH/s (95.83ms) @ Accel:5 Loops:32 Thr:56 Vec:1
Speed.#04........:   419.9 kH/s (95.86ms) @ Accel:5 Loops:32 Thr:56 Vec:1
Speed.#05........:   420.0 kH/s (95.92ms) @ Accel:5 Loops:32 Thr:56 Vec:1
Speed.#06........:   419.8 kH/s (96.04ms) @ Accel:5 Loops:32 Thr:56 Vec:1
Speed.#07........:   421.1 kH/s (95.71ms) @ Accel:5 Loops:32 Thr:56 Vec:1
Speed.#08........:   420.2 kH/s (95.88ms) @ Accel:5 Loops:32 Thr:56 Vec:1
Speed.#*.........:  3361.5 kH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#01........:  2388.5 kH/s (79.08ms) @ Accel:10 Loops:1024 Thr:512 Vec:1
Speed.#02........:  2392.7 kH/s (78.99ms) @ Accel:10 Loops:1024 Thr:512 Vec:1
Speed.#03........:  2389.5 kH/s (79.04ms) @ Accel:10 Loops:1024 Thr:512 Vec:1
Speed.#04........:  2392.2 kH/s (79.01ms) @ Accel:10 Loops:1024 Thr:512 Vec:1
Speed.#05........:  2390.1 kH/s (79.07ms) @ Accel:10 Loops:1024 Thr:512 Vec:1
Speed.#06........:  2389.6 kH/s (79.08ms) @ Accel:10 Loops:1024 Thr:512 Vec:1
Speed.#07........:  2394.0 kH/s (78.94ms) @ Accel:10 Loops:1024 Thr:512 Vec:1
Speed.#08........:  2389.6 kH/s (79.09ms) @ Accel:10 Loops:1024 Thr:512 Vec:1
Speed.#*.........: 19126.2 kH/s

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#01........:   136.7 GH/s (70.32ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#*.........:  1094.8 GH/s

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#01........: 10727.6 MH/s (84.81ms) @ Accel:6 Loops:1024 Thr:1024 Vec:1
Speed.#*.........: 85927.9 MH/s

[Backend device-info header of the same run:]
Backend Device ID #01 (Alias: #09)
  Name...........: NVIDIA B200
  Processor(s)...: 148
  Clock..........: 1965
  Memory.Total...: 182642 MB
  Memory.Free....: 182014 MB
  PCI.Addr.BDFe..: 0000:51:00.0
[nvidia-smi: 8x NVIDIA B200, Driver Version 570.172.08, CUDA Version 12.8, 183359MiB each]
```
