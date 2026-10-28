# NVIDIA GeForce 940MX

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce 940MX
- **Версия hashcat / Version:** v3.6.0
- **Источник / Source:** [hashcat/hashcat issue #1366 (mehrad100)](https://github.com/hashcat/hashcat/issues/1366)
- **Особенности прогона / Run options:** нестандартный запуск `hashcat64.exe -b -w 4 -D 1,2 --force` (workload profile 4, ограничение типов устройств, `--force`). Прогон многокарточный, но GeForce 940MX однозначно определена как `Device #1`, поэтому берутся строки `Speed.Dev.#1` (Device #2 — Intel HD Graphics 620, Device #3 — CPU). Вывод неполный: автор привёл только первые четыре алгоритма (MD4, MD5, Half MD5, SHA1). Формат hashcat 3.x (`Hashtype:` / `Speed.Dev.#N`), номера режимов в выводе не печатаются.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 1726.3 MH/s |
| 100 | SHA1 | 734.7 MH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
c:\hashcat>hashcat64.exe -b -w 4 -D 1,2 --force
hashcat (v3.6.0) starting in benchmark mode...

OpenCL Platform #1: NVIDIA Corporation
======================================
* Device #1: GeForce 940MX, 512/2048 MB allocatable, 3MCU

OpenCL Platform #2: Intel(R) Corporation
========================================
* Device #2: Intel(R) HD Graphics 620, 2047/4859 MB allocatable, 24MCU
* Device #3: Intel(R) Core(TM) i7-7500U CPU @ 2.70GHz, 3042/12168 MB allocatable, 4MCU

Hashtype: MD4

Speed.Dev.#1.....:  2794.6 MH/s (287.88ms)
Speed.Dev.#2.....:   849.8 MH/s (469.33ms)
Speed.Dev.#3.....:   285.6 MH/s (14.25ms)
Speed.Dev.#*.....:  3930.0 MH/s

Hashtype: MD5

Speed.Dev.#1.....:  1726.3 MH/s (465.98ms)
Speed.Dev.#2.....:   505.3 MH/s (393.49ms)
Speed.Dev.#3.....:   168.4 MH/s (24.76ms)
Speed.Dev.#*.....:  2400.0 MH/s

Hashtype: Half MD5

Speed.Dev.#1.....:  1144.6 MH/s (351.30ms)
Speed.Dev.#2.....:   338.8 MH/s (294.88ms)
Speed.Dev.#3.....: 97375.8 kH/s (42.87ms)
Speed.Dev.#*.....:  1580.7 MH/s

Hashtype: SHA1

Speed.Dev.#1.....:   734.7 MH/s (273.67ms)
Speed.Dev.#2.....: 26695.9 kH/s (463.11ms)
Speed.Dev.#3.....: 68081.6 kH/s (61.25ms)
Speed.Dev.#*.....:   829.5 MH/s
```
