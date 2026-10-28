# AMD Ryzen 7 2700 — benchmark fragment

- **Процессор:** AMD Ryzen 7 2700 Eight-Core Processor.
- **Версия:** hashcat v6.2.6.
- **Режим:** MD5 (mode 0), CPU `Speed.#1 723.2 MH/s`.
- **Источник:** [raw Hashcat benchmark log](https://gist.githubusercontent.com/cococig/2b592488fcbdb8a0301b8c38acaee466/raw/3664cfb04822c6d3629b6ecd04037c3410462e62/hashcat_bench_ryzen7_2700.txt).
- **Примечание:** mixed NVIDIA GPU + CPU log; Device #1 is explicitly `pthread-haswell-AMD Ryzen 7 2700`. Не путать с соседним gist-файлом Ryzen 7 7700X.

```text
* Device #1: pthread-haswell-AMD Ryzen 7 2700 Eight-Core Processor

* Hash-Mode 0 (MD5)
Speed.#1.........: 723.2 MH/s (19.62ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8
```
