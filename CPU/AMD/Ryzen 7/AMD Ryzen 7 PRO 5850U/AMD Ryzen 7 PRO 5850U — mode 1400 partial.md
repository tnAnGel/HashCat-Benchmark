# AMD Ryzen 7 PRO 5850U — benchmark fragment

- **Процессор:** AMD Ryzen 7 PRO 5850U with Radeon Graphics.
- **Дата:** 2024-11-06.
- **Запуск:** `hashcat -m 1400 -D 1 -b --cpu-affinity=1 -w 1`.
- **Backend:** PoCL CPU, Device #1.
- **Режим:** SHA2-256 (mode 1400), `Speed.#1 24930.3 kH/s`.
- **Источник:** [hashbench-intellij README, benchmark output](https://github.com/bjoernfi/hashbench-intellij/blob/main/README.md#L268-L296).
- **Примечание:** CPU-only результат, но нестандартный workload `-w 1`, affinity на один CPU и один hash mode; не сравнивать напрямую с полными оптимизированными прогонами.

```text
hashcat -m 1400 -D 1 -b --cpu-affinity=1 -w 1
* Device #1: cpu-haswell-AMD Ryzen 7 PRO 5850U with Radeon Graphics
Hash-Mode 1400 (SHA2-256)
Speed.#1.........: 24930.3 kH/s
```
