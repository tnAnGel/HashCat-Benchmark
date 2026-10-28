# Intel Core i5-4250U — Apple OpenCL benchmark excerpt

- **Вендор / Vendor:** Intel
- **Процессор / CPU:** Intel Core i5-4250U CPU @ 1.30GHz, Device #1.
- **Версия hashcat / Version:** not stated in the comment.
- **Бэкенд / Backend:** Apple OpenCL; Intel CPU is Device #1, Intel HD Graphics 5000 is Device #2.
- **Источник / Source:** [chadmayfield/hashcat_macos.sh Gist, benchmark comment](https://gist.github.com/chadmayfield/600b211e9c309859f2bfb5dddc5de09c?permalink_comment_id=2898114).
- **Параметры / Options:** `--opencl-device-types=1,2`, `--optimized-kernel-enable`.
- **Примечание / Note:** Partial comment output, not a complete benchmark. Only CPU `Speed.#1` is recorded; GPU `Speed.#2` and combined `Speed.#*` are excluded. The bcrypt section reports repeated `CL_INVALID_WORK_GROUP_SIZE` messages but still ends with a CPU speed; mode 7100 begins at the end of the available excerpt and has no result line.

## Результаты CPU / CPU results

| Mode | Algorithm | CPU speed |
|-----:|-----------|----------:|
| 0 | MD5 | 73295.5 kH/s |
| 100 | SHA1 | 32115.1 kH/s |
| 1400 | SHA2-256 | 11977.6 kH/s |
| 1700 | SHA2-512 | 3166.8 kH/s |
| 2500 | WPA-EAPOL-PBKDF2 | 1436 H/s |
| 1000 | NTLM | 142.1 MH/s |
| 3000 | LM | 22319.2 kH/s |
| 5500 | NetNTLMv1 / NetNTLMv1+ESS | 80076.3 kH/s |
| 5600 | NetNTLMv2 | 4515.6 kH/s |
| 1500 | descrypt | 914.0 kH/s |
| 500 | md5crypt | 12469 H/s |
| 3200 | bcrypt | 893 H/s |
| 1800 | sha512crypt | 402 H/s |
| 7500 | Kerberos 5 AS-REQ | 1246.1 kH/s |
| 13100 | Kerberos 5 TGS-REP | 1035.6 kH/s |
| 15300 | DPAPI masterkey v1 | 312 H/s |
| 15900 | DPAPI masterkey v2 | 133 H/s |

## CPU raw excerpts / Исходные строки CPU

```text
* Device #1: Intel(R) Core(TM) i5-4250U CPU @ 1.30GHz, 1024/4096 MB allocatable, 4MCU
* Device #2: HD Graphics 5000, 384/1536 MB, 40MCU
* --opencl-device-types=1,2
* --optimized-kernel-enable
Hashmode: 0 - MD5
Speed.#1.........: 73295.5 kH/s (56.85ms) @ Accel:1024 Loops:1024 Thr:1 Vec:4
Hashmode: 100 - SHA1
Speed.#1.........: 32115.1 kH/s (64.99ms) @ Accel:1024 Loops:512 Thr:1 Vec:4
Hashmode: 1400 - SHA2-256
Speed.#1.........: 11977.6 kH/s (87.25ms) @ Accel:1024 Loops:256 Thr:1 Vec:4
Hashmode: 1700 - SHA2-512
Speed.#1.........: 3166.8 kH/s (82.49ms) @ Accel:512 Loops:128 Thr:1 Vec:2
Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)
Speed.#1.........:     1436 H/s (88.30ms) @ Accel:512 Loops:256 Thr:1 Vec:4
Hashmode: 1000 - NTLM
Speed.#1.........:   142.1 MH/s (29.22ms) @ Accel:1024 Loops:1024 Thr:1 Vec:4
Hashmode: 3000 - LM
Speed.#1.........: 22319.2 kH/s (93.14ms) @ Accel:512 Loops:1024 Thr:1 Vec:4
Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS
Speed.#1.........: 80076.3 kH/s (52.07ms) @ Accel:1024 Loops:1024 Thr:1 Vec:4
Hashmode: 5600 - NetNTLMv2
Speed.#1.........:  4515.6 kH/s (115.77ms) @ Accel:512 Loops:256 Thr:1 Vec:4
Hashmode: 1500 - descrypt, DES (Unix), Traditional DES
Speed.#1.........:   914.0 kH/s (70.91ms) @ Accel:16 Loops:1024 Thr:1 Vec:4
Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)
Speed.#1.........:    12469 H/s (81.13ms) @ Accel:512 Loops:500 Thr:1 Vec:4
Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)
Speed.#1.........:      893 H/s (69.57ms) @ Accel:32 Loops:16 Thr:1 Vec:4
Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)
Speed.#1.........:      402 H/s (63.00ms) @ Accel:256 Loops:128 Thr:1 Vec:2
Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth
Speed.#1.........:  1246.1 kH/s (52.34ms) @ Accel:32 Loops:8 Thr:64 Vec:4
Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP
Speed.#1.........:  1035.6 kH/s (63.05ms) @ Accel:32 Loops:8 Thr:64 Vec:4
Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)
Speed.#1.........:      312 H/s (69.73ms) @ Accel:512 Loops:256 Thr:1 Vec:4
Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)
Speed.#1.........:      133 H/s (76.27ms) @ Accel:256 Loops:128 Thr:1 Vec:2
```
