# AMD Radeon RX 570 Series — partial multi-GPU benchmark

- **Вендор / Vendor:** AMD
- **Устройство / GPU:** AMD Radeon RX 570 Series, 3 devices, each reported as 3968/4096 MB; exact board/SKU is not identified.
- **Версия hashcat / Version:** v6.2.6-813-g686bc227c (successful run); v6.2.6-905-gf9822fe56 (failed repeat).
- **Backend:** HIP 4.4 for the successful run; OpenCL devices were skipped.
- **Источник / Source:** [hashcat/hashcat issue #4221](https://github.com/hashcat/hashcat/issues/4221), benchmark output in the issue comments.
- **Параметры / Options:** `hashcat -m 100 -b`; `--backend-devices-virtual=1`; `--optimized-kernel-enable`.
- **Примечание / Note:** One successful mode only (SHA1, mode 100), measured on three similarly named devices. Do not treat `Speed.#*` as one-card throughput or infer an exact RX 570 SKU from the generic backend string. A later build failed to initialize HIP and exited without speeds.

## Результаты / Results

| Mode | Algorithm | Device | Speed |
|-----:|-----------|-------:|------:|
| 100 | SHA1 | #1 | 3304.8 MH/s |
| 100 | SHA1 | #2 | 3175.5 MH/s |
| 100 | SHA1 | #3 | 3304.8 MH/s |
| 100 | SHA1 | 3-device sum (not per-card) | 9785.1 MH/s |

```text
* Device #1: Radeon RX 570 Series, 3968/4096 MB, 32MCU
* Device #2: Radeon RX 570 Series, 3968/4096 MB, 32MCU
* Device #3: Radeon RX 570 Series, 3968/4096 MB, 32MCU
* Hash-Mode 100 (SHA1)
Speed.#1.........:  3304.8 MH/s (80.28ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#2.........:  3175.5 MH/s (83.55ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#3.........:  3304.8 MH/s (80.22ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#*.........:  9785.1 MH/s
```
