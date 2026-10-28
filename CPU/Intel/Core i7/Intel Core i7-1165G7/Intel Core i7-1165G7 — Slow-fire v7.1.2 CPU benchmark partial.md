# Intel Core i7-1165G7 — Slow-fire Hashcat v7.1.2 CPU results (partial raw)

- **CPU:** Intel Core i7-1165G7 @ 2.80 GHz, 4 cores / 8 threads.
- **Hashcat:** v7.1.2.
- **CPU device:** PoCL `cpu-skylake-avx512-11th Gen Intel(R) Core(TM) i7-1165G7`, 8 processors.
- **Backend:** PoCL 5.0; Intel Iris Xe GPU is a separate device and is not included in these CPU figures.
- **Source:** [Slow-fire hacking next — CPU built-in GPU comparison](https://blog.slow-fire.net/2025/09/05/cpu%E3%81%AB%E5%86%85%E8%94%B5%E3%81%95%E3%82%8C%E3%81%A6%E3%81%84%E3%82%8Bgpu%E3%82%92%E7%B0%A1%E5%8D%98%E3%81%AB%E4%BD%BF%E3%81%A3%E3%81%A6%E3%81%BF%E3%82%8b/).
- **Тип свидетельства:** опубликованные команды и CPU `Speed.#02` lines; не полный raw log.

| Workload | Command | Mode | CPU speed |
|---|---|---:|---:|
| Benchmark | `hashcat -b -m 0 -O -w 3 -D 1` | 0, MD5 | 1647.2 MH/s |
| Mask demonstration | `hashcat -m 0 -a 3 -O -w 3 -D 1 --runtime 10` | 0, MD5 | 1601.5 MH/s |
| Wordlist demonstration | `hashcat -m 0 -a 0 -O -w 3 -D 1` | 0, MD5 | 153 H/s |

The benchmark run is the comparable CPU measurement. The other two are demonstrations on a single known hash; the dictionary run has only five candidates and must not be treated as sustained throughput.
