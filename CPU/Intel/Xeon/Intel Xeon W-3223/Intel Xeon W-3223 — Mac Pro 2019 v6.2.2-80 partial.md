# Intel Xeon W-3223 — Mac Pro (2019), partial benchmark excerpt

- **Вендор / Vendor:** Intel
- **Процессор / CPU:** Intel Xeon W-3223 @ 3.50GHz, 8/16
- **Версия hashcat / Version:** v6.2.2-80-gc32242980
- **Бэкенд / Backend:** Apple OpenCL 1.2; CPU is Device #1; AMD Radeon Pro W5700X is Device #2.
- **Источник / Source:** [Hashcat Forum — MacOS Catalina](https://hashcat.net/forum/thread-10189-post-52991.html), reply with benchmarks.
- **Параметры / Options:** `hashcat -b -D 1,2`; `--opencl-device-types=1,2`; `--optimized-kernel-enable`.
- **Примечание / Note:** Extracted CPU `Speed.#1` rows from a mixed CPU+GPU run. The source reports two CPU-skipped modes (3000 and 1500); GPU `Speed.#2` and combined `Speed.#*` are intentionally omitted. This is a selected-device excerpt, not the full original console transcript.

## Результаты CPU / CPU results

| Mode | Algorithm | CPU speed |
|-----:|-----------|----------:|
| 0 | MD5 | 640.7 MH/s |
| 100 | SHA1 | 319.8 MH/s |
| 1400 | SHA2-256 | 113.6 MH/s |
| 1700 | SHA2-512 | 37948.3 kH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 14862 H/s |
| 1000 | NTLM | 1077.8 MH/s |
| 5500 | NetNTLMv1 / NetNTLMv1+ESS | 659.3 MH/s |
| 5600 | NetNTLMv2 | 61737.9 kH/s |
| 500 | md5crypt | 102.0 kH/s |
| 3200 | bcrypt | 8363 H/s |
| 1800 | sha512crypt | 4234 H/s |
| 7500 | Kerberos 5 AS-REQ | 9259.5 kH/s |
| 13100 | Kerberos 5 TGS-REP | 8973.0 kH/s |
| 15300 | DPAPI masterkey v1 | 2603 H/s |
| 15900 | DPAPI masterkey v2 | 1315 H/s |
| 7100 | macOS v10.8+ PBKDF2-SHA512 | 16364 H/s |
| 11600 | 7-Zip | 4692 H/s |
| 12500 | RAR3-hp | 711 H/s |
| 13000 | RAR5 | 1444 H/s |
| 6211 | TrueCrypt RIPEMD160 + XTS | 11567 H/s |
| 13400 | KeePass | 2602 H/s |
| 6800 | LastPass | 91807 H/s |
| 11300 | Bitcoin/Litecoin wallet.dat | 189 H/s |

## CPU raw excerpts / Исходные строки CPU

```text
Hashmode: 0 - MD5
Speed.#1.........:   640.7 MH/s (26.17ms) @ Accel:1024 Loops:1024 Thr:1 Vec:4
Hashmode: 100 - SHA1
Speed.#1.........:   319.8 MH/s (52.34ms) @ Accel:1024 Loops:1024 Thr:1 Vec:4
Hashmode: 1400 - SHA2-256
Speed.#1.........:   113.6 MH/s (73.70ms) @ Accel:512 Loops:1024 Thr:1 Vec:4
Hashmode: 1700 - SHA2-512
Speed.#1.........: 37948.3 kH/s (55.13ms) @ Accel:128 Loops:1024 Thr:1 Vec:2
Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)
Speed.#1.........:    14862 H/s (68.67ms) @ Accel:256 Loops:1024 Thr:1 Vec:4
Hashmode: 1000 - NTLM
Speed.#1.........:  1077.8 MH/s (15.45ms) @ Accel:1024 Loops:1024 Thr:1 Vec:4
Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS
Speed.#1.........:   659.3 MH/s (25.32ms) @ Accel:1024 Loops:1024 Thr:1 Vec:4
Hashmode: 5600 - NetNTLMv2
Speed.#1.........: 61737.9 kH/s (67.80ms) @ Accel:256 Loops:1024 Thr:1 Vec:4
Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)
Speed.#1.........:   102.0 kH/s (79.77ms) @ Accel:1024 Loops:500 Thr:1 Vec:4
Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)
Speed.#1.........:     8363 H/s (29.64ms) @ Accel:16 Loops:32 Thr:1 Vec:1
Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)
Speed.#1.........:     4234 H/s (48.14ms) @ Accel:128 Loops:512 Thr:1 Vec:2
Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth
Speed.#1.........:  9259.5 kH/s (56.49ms) @ Accel:32 Loops:1024 Thr:1 Vec:4
Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP
Speed.#1.........:  8973.0 kH/s (58.29ms) @ Accel:32 Loops:1024 Thr:1 Vec:4
Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)
Speed.#1.........:     2603 H/s (65.41ms) @ Accel:256 Loops:1024 Thr:1 Vec:4
Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)
Speed.#1.........:     1315 H/s (59.77ms) @ Accel:128 Loops:512 Thr:1 Vec:2
Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)
Speed.#1.........:    16364 H/s (41.16ms) @ Accel:128 Loops:511 Thr:1 Vec:2
Hashmode: 11600 - 7-Zip (Iterations: 16384)
Speed.#1.........:     4692 H/s (54.30ms) @ Accel:64 Loops:4096 Thr:1 Vec:4
Hashmode: 12500 - RAR3-hp (Iterations: 262144)
Speed.#1.........:      711 H/s (89.98ms) @ Accel:64 Loops:16384 Thr:1 Vec:4
Hashmode: 13000 - RAR5 (Iterations: 32799)
Speed.#1.........:     1444 H/s (88.47ms) @ Accel:512 Loops:512 Thr:1 Vec:4
Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)
Speed.#1.........:    11567 H/s (87.93ms) @ Accel:256 Loops:512 Thr:1 Vec:4
Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)
Speed.#1.........:     2602 H/s (65.49ms) @ Accel:512 Loops:512 Thr:1 Vec:4
Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)
Speed.#1.........:    91807 H/s (87.06ms) @ Accel:512 Loops:499 Thr:1 Vec:4
Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)
Speed.#1.........:      189 H/s (55.14ms) @ Accel:128 Loops:1024 Thr:1 Vec:2
```
