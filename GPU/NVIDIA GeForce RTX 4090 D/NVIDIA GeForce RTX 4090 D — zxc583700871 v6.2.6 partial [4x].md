# NVIDIA GeForce RTX 4090 D

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 4090 D, 24 GB
- **Версия / Version:** hashcat v6.2.6
- **Источник / Source:** [Hashcat Forum — How to increase the speed of 23800 mode?](https://hashcat.net/forum/thread-12249.html)
- **Параметры / Options:** benchmark mode `-m 23800`, optimized kernel; Windows 10, CUDA 12.4; система с 4× RTX 4090 D
- **Примечание / Note:** найден только один режим — RAR3-p (Compressed). Указаны отдельные показатели четырёх адаптеров и их сумма; это не полный набор режимов. Модель и VRAM прямо указаны в выводе Hashcat.

## Результат / Result

| GPU | Скорость, Hashmode 23800 |
|-----|------------------------:|
| #1 | 303 H/s |
| #2 | 266 H/s |
| #3 | 265 H/s |
| #4 | 286 H/s |
| Итого, 4× | 1119 H/s |

## Исходные строки / Raw excerpt

```text
hashcat (v6.2.6) starting in benchmark mode
* Device #1: NVIDIA GeForce RTX 4090 D, 23042/24563 MB, 114MCU
* Device #2: NVIDIA GeForce RTX 4090 D, 23042/24563 MB, 114MCU
* Device #3: NVIDIA GeForce RTX 4090 D, 23042/24563 MB, 114MCU
* Device #4: NVIDIA GeForce RTX 4090 D, 23042/24563 MB, 114MCU
* Hash-Mode 23800 (RAR3-p (Compressed)) [Iterations: 262144]
Speed.#1.........: 303 H/s
Speed.#2.........: 266 H/s
Speed.#3.........: 265 H/s
Speed.#4.........: 286 H/s
Speed.#*.........: 1119 H/s
```
