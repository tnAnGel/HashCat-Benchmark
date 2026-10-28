# AMD Radeon Pro 5500M — отдельный benchmark mode 11600

- **Тип свидетельства:** прямой форумный фрагмент stdout `hashcat -b` (один режим; не полный прогон).
- **GPU:** `AMD Radeon Pro 5500M Compute Engine`, OpenCL Device #5. В том же выводе Intel UHD Graphics 630 — Device #4; для этого режима ей не хватило доступной памяти, поэтому её скорость не смешана с Radeon.
- **Команда:** `./hashcat -b -m 11600 -O -D 2`
- **Hashcat:** `v6.2.5-383-g6509351dc`
- **Режим:** 11600 — 7-Zip, 16 384 iterations.
- **Результат Radeon Pro 5500M:** **166.0 kH/s** (`Speed.#5`, 70.01 ms; Accel 16, Loops 4096, Thr 128, Vec 1).
- **Ограничение:** опубликован только mode 11600; это отдельный повторный результат, а не замена более полным прогонам этой модели. В логе отмечено, что Device #4 (Intel UHD 630) не хватило доступной памяти для режима.
- **Прямой источник:** [Hashcat Forum — Only getting 1% of the hashrate of the benchmark](https://hashcat.net/forum/thread-10718.html), сообщение #1, строки benchmark results.

```text
./hashcat -b -m 11600 -O -D 2
hashcat (v6.2.5-383-g6509351dc) starting in benchmark mode
* Device #4: Intel(R) UHD Graphics 630, 704/1536 MB (192 MB allocatable), 24MCU
* Device #5: AMD Radeon Pro 5500M Compute Engine, 3968/4080 MB (1020 MB allocatable), 24MCU
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
* Device #4: Not enough allocatable device memory for this attack.
Speed.#5.........: 166.0 kH/s (70.01ms) @ Accel:16 Loops:4096 Thr:128 Vec:1
Speed.#*.........: 166.0 kH/s
Started: Mon Apr 11 13:23:41 2022
Stopped: Mon Apr 11 13:23:44 2022
```
