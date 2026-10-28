# Intel Arc A770M — ZerNox, hashcat v6.2.6 (raw, partial)

- **Тип данных:** опубликованный raw-вывод `hashcat -b -d 1`; частичный benchmark.
- **Устройство:** Intel Arc A770M, PCI ID `8086:5690`, 512 MCU; Intel Iris Xe и CPU перечислены отдельно и пропущены.
- **Система:** Intel NUC12SNKi7, Core i7-12700H, Ubuntu 23.10 (автор также упоминает Ubuntu 23.04 в начале заметки), Linux 6.5.0-14-generic, Intel OpenCL 3.0.
- **Версия hashcat:** v6.2.6.
- **Источник:** [ZerNox — Hashcat benchmark NUC12SNKi7 with Intel ARC A770M](https://gist.github.com/ZerNox/824938345b5e884530506bc7c521e95c) (создан 2024-01-06).
- **Классификация:** `hashcat -b` и `Speed.#1` подтверждают измерения именно на Arc A770M. Источник опубликован целиком только до пропуска DES; дальнейшие режимы не представлены, поэтому это не полный `--benchmark-all`-лог.

## Подтверждённые скорости

| Hash mode | Алгоритм | Скорость |
|---:|---|---:|
| 0 | MD5 | 27,578.9 MH/s |
| 100 | SHA1 | 528.2 MH/s |
| 1400 | SHA2-256 | 792.1 MH/s |
| 1700 | SHA2-512 | 842.6 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 135.4 kH/s |
| 1000 | NTLM | 44,945.7 MH/s |
| 3000 | LM | 604.2 MH/s |
| 5500 | NetNTLMv1 / NetNTLMv1+ESS | 28,088.1 MH/s |
| 5600 | NetNTLMv2 | 1,882.7 MH/s |

## Raw-вывод опубликованной части

```text
At time of installation 2024-01-06 on ubuntu 23.04 as of my understanding it would be included in the kernel but the
2.1.3. Install Compute, Media, and Display runtimes was essential to get it to work
according to the guide https://dgpu-docs.intel.com/driver/client/overview.html

$ uname -r
6.5.0-14-generic

$ lsb_release -a
Distributor ID: Ubuntu
Description: Ubuntu 23.10
Release: 23.10
Codename: mantic

$ lspci -nnn | grep -i ARC
03:00.0 VGA compatible controller [0300]: Intel Corporation DG2 [Arc A770M] [8086:5690] (rev 08)

hashcat -b -d 1
hashcat (v6.2.6) starting in benchmark mode

OpenCL API (OpenCL 3.0 ) - Platform #1 [Intel(R) Corporation]
* Device #1: Intel(R) Arc(TM) A770M Graphics, 15360/15473 MB (4095 MB allocatable), 512MCU

OpenCL API (OpenCL 3.0 ) - Platform #2 [Intel(R) Corporation]
* Device #2: Intel(R) Iris(R) Xe Graphics, skipped

OpenCL API (OpenCL 2.0 PoCL 4.0+debian Linux) - Platform #3 [The pocl project]
* Device #3: cpu-haswell-12th Gen Intel(R) Core(TM) i7-12700H, skipped

Benchmark relevant options:
* --backend-devices=1
* --optimized-kernel-enable

Hash-Mode 0 (MD5)
Speed.#1.........: 27578.9 MH/s (76.45ms) @ Accel:16 Loops:512 Thr:512 Vec:4

Hash-Mode 100 (SHA1)
Speed.#1.........: 528.2 MH/s (62.30ms) @ Accel:8 Loops:16 Thr:512 Vec:4

Hash-Mode 1400 (SHA2-256)
Speed.#1.........: 792.1 MH/s (41.36ms) @ Accel:16 Loops:8 Thr:512 Vec:4

Hash-Mode 1700 (SHA2-512)
Speed.#1.........: 842.6 MH/s (78.67ms) @ Accel:4 Loops:64 Thr:512 Vec:1

Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
Speed.#1.........: 135.4 kH/s (59.61ms) @ Accel:4 Loops:32 Thr:512 Vec:1

Hash-Mode 1000 (NTLM)
Speed.#1.........: 44945.7 MH/s (46.67ms) @ Accel:16 Loops:512 Thr:512 Vec:4

Hash-Mode 3000 (LM)
Speed.#1.........: 604.2 MH/s (886.50ms) @ Accel:4 Loops:1024 Thr:256 Vec:1

Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
Speed.#1.........: 28088.1 MH/s (37.27ms) @ Accel:16 Loops:256 Thr:512 Vec:4

Hash-Mode 5600 (NetNTLMv2)
Speed.#1.........: 1882.7 MH/s (70.06ms) @ Accel:16 Loops:32 Thr:512 Vec:4

Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
...
DES skipped due to https://github.com/hashcat/hashcat/issues/2986
```
