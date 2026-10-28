# NVIDIA GeForce GTX 660 Ti

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 660 Ti, 2 GB, 1137 MHz, 7 MCU
- **Версия / Version:** cudaHashcat v1.31 (legacy)
- **Источник / Source:** [Hashcat Forum — sapb, which card (est)](https://hashcat.net/forum/thread-3837.html)
- **Параметры / Options:** `cudaHashcat64.exe -b -m 7700`; SAP CODVN B (BCODE), 1024 loops, 256 accel
- **Примечание / Note:** опубликован один benchmark-режим; не сопоставим напрямую с современными `hashcat -b` наборами.

## Результат / Result

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 7700 | SAP CODVN B (BCODE) | 293.6 MH/s |

## Исходные строки / Raw excerpt

```text
cudaHashcat64.exe -b -m 7700
cudaHashcat v1.31 starting in benchmark-mode...
Device #1: GeForce GTX 660 Ti, 2048MB, 1137Mhz, 7MCU
Hashtype: SAP CODVN B (BCODE)
Workload: 1024 loops, 256 accel
Speed.GPU.#1.: 293.6 MH/s
```
