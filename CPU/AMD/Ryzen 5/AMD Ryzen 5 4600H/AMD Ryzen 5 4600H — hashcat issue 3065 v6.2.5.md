# AMD Ryzen 5 4600H

- **Вендор / Vendor:** AMD
- **Процессор / CPU:** AMD Ryzen 5 4600H with Radeon Graphics (Renoir, Zen 2, мобильный APU)
- **Версия hashcat / Version:** v6.2.5
- **Бэкенд / Backend:** pocl (`The pocl project`), устройство `pthread-AMD Ryzen 5 4600H with Radeon Graphics` — Device #2.
- **Источник / Source:** [hashcat/hashcat Issue #3065](https://github.com/hashcat/hashcat/issues/3065)
- **Примечание / Note:** ЧАСТИЧНЫЙ вывод — из bug-репорта показан только один режим (Hash-Mode 100 / SHA1) на CPU-устройстве (`-m 100`, прогон без CUDA-драйвера). Строка Speed имеет полный тюнинг (`@ Accel/Loops/Thr/Vec` + мс). Device #2 = pthread-CPU, однозначно процессор.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 100 | SHA1 | 478.2 MH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5) starting in benchmark mode

OpenCL Platform #1: The pocl project
* Device #2: pthread-AMD Ryzen 5 4600H with Radeon Graphics, 2637/5339 MB (1024 MB allocatable), 12MCU

* Hash-Mode 100 (SHA1)

Speed.#2.........:   478.2 MH/s (6.38ms) @ Accel:512 Loops:512 Thr:1 Vec:8
```
