# AMD Radeon HD 6990

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** ASUS Radeon HD 6990 (dual-GPU, Cayman ×2; 2 GB per device)
- **Версия / Version:** oclHashcat v1.31 (legacy)
- **Источник / Source:** [Hashcat Forum — sapb, which card (est)](https://hashcat.net/forum/thread-3837.html)
- **Параметры / Options:** `oclHashcat64.exe -b -m 7700`; SAP CODVN B (BCODE), 1024 loops, 64 accel; AMD devices clocked at 830 MHz
- **Примечание / Note:** benchmark run includes the two HD 6990 Cayman devices plus separate Tahiti and Hawaii cards. The two per-device values below are the Cayman pair, identified in the same thread as the author's ASUS HD 6990; the forum does not publish a standalone physical-card aggregate.

## Результат / Result

| Device | Алгоритм | Скорость |
|-------:|----------|---------:|
| Cayman #1 | SAP CODVN B (BCODE) | 118.7 MH/s |
| Cayman #2 | SAP CODVN B (BCODE) | 118.7 MH/s |

## Исходные строки / Raw excerpt

```text
oclHashcat64.exe -b -m 7700
oclHashcat v1.31 starting in benchmark-mode...
Device #1: Cayman, 2048MB, 830Mhz, 24MCU
Device #2: Cayman, 2048MB, 830Mhz, 24MCU
Device #3: Tahiti, 3072MB, 830Mhz, 32MCU
Device #4: Hawaii, 3072MB, 830Mhz, 44MCU
Hashtype: SAP CODVN B (BCODE)
Workload: 1024 loops, 64 accel
Speed.GPU.#1.: 118.7 MH/s
Speed.GPU.#2.: 118.7 MH/s
Speed.GPU.#3.: 725.3 MH/s
Speed.GPU.#4.: 985.7 MH/s
Speed.GPU.#*.: 1948.4 MH/s
```
