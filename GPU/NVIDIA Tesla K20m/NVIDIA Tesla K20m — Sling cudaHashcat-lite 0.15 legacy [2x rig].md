# NVIDIA Tesla K20m

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** Tesla K20m (2 устройства, 4799 MB, 13 MCU каждое)
- **Версия / Version:** cudaHashcat-lite 0.15 (legacy benchmark runner)
- **Источник / Source:** [Hashcat Forum — Tesla K20 (Kepler GK110) benchmark](https://hashcat.net/forum/thread-2340.html)
- **Параметры / Options:** `./cudaHashcat-lite64.bin -b --benchmark-mode 1`; stock clocks
- **Примечание / Note:** это итоговая скорость двух карт (`Speed.GPU.#*`); источник не приводит отдельных скоростей по устройствам, поэтому значения не делю и не использую как результат одной карты. Исторический CUDA-only Lite benchmark, не эквивалент современному `hashcat -b`.

## Результаты / Results (2× rig total)

| Алгоритм | 2 карты, сумма |
|----------|---------------:|
| MD4 | 14.038 GH/s |
| MD5 | 8.287 GH/s |
| SHA1 | 2.849 GH/s |
| SHA256 | 1.365 GH/s |
| NTLM | 13.385 GH/s |

## Исходные строки / Raw excerpt

```text
--- Benchmark @ 2x Tesla K20m ---
./cudaHashcat-lite64.bin -b --benchmark-mode 1
Device #1: Tesla K20m, 4799MB, 705Mhz, 13MCU
Device #2: Tesla K20m, 4799MB, 705Mhz, 13MCU

Hash.Type....: MD5
Speed.GPU.#*.: 8287.0M/s
Hash.Type....: SHA1
Speed.GPU.#*.: 2848.8M/s
Hash.Type....: MD4
Speed.GPU.#*.: 14037.5M/s
Hash.Type....: NTLM
Speed.GPU.#*.: 13385.2M/s
```
