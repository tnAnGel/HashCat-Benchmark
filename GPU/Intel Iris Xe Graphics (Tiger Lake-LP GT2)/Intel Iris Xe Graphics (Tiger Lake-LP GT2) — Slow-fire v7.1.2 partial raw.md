# Intel Iris Xe Graphics (Tiger Lake-LP GT2) — Slow-fire Hashcat v7.1.2 (partial raw)

- **GPU:** Intel Iris Xe Graphics; PCI identity TigerLake-LP GT2 `[8086:9a49]`, paired with Intel Core i7-1165G7.
- **Hashcat:** v7.1.2.
- **Backend:** Intel OpenCL Graphics, OpenCL 3.0 NEO, driver 25.31.34666.
- **Source:** [Slow-fire hacking next — CPU built-in GPU comparison](https://blog.slow-fire.net/2025/09/05/cpu%E3%81%AB%E5%86%85%E8%94%B5%E3%81%95%E3%82%8C%E3%81%A6%E3%81%84%E3%82%8Bgpu%E3%82%92%E7%B0%BF%E5%8D%98%E3%81%AB%E4%BD%BF%E3%81%A3%E3%81%A6%E3%81%BF%E3%82%8b/).
- **Тип свидетельства:** опубликованные команда, backend information и отдельные GPU `Speed.#01` строки; не полный stdout.

| Workload | Command | Mode | GPU speed |
|---|---|---:|---:|
| Benchmark | `hashcat -b -m 0 -O -w 4 -D 2 -d 1` | 0, MD5 | 2967.1 MH/s |
| Mask demonstration | `hashcat -m 0 -a 3 -O -w 4 -D 2 -d 1 --runtime 10` | 0, MD5 | 2911.0 MH/s |
| Wordlist demonstration | `hashcat -m 0 -a 0 -O -w 4 -D 2 -d 1` | 0, MD5 | 1715 H/s |

The mask and wordlist runs are demonstrations on a single known hash, not sustained benchmark results. The wordlist contains five candidates. A separate PoCL CPU backend is present on the same host; its figures are recorded in the [CPU card](<../../CPU/Intel/Core i7/Intel Core i7-1165G7/Intel Core i7-1165G7 — Slow-fire v7.1.2 CPU benchmark partial.md>), not attributed to this GPU.
