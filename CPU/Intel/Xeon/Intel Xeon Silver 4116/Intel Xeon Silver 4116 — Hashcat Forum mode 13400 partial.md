# Intel Xeon Silver 4116 — KeePass mode excerpt

- **Вендор / Vendor:** Intel
- **Процессор / CPU:** Intel Xeon Silver 4116 CPU @ 2.10GHz, Device #1.
- **Версия hashcat / Version:** not stated in the benchmark excerpt.
- **Бэкенд / Backend:** Intel OpenCL device; exact runtime not stated.
- **Источник / Source:** [Hashcat Forum — CL_DEVICE_NOT_AVAILABLE / KeePass pass recovery](https://hashcat.net/forum/thread-10220-post-53112.html), reply #2.
- **Примечание / Note:** One-mode benchmark snippet posted as an example. The original user's CPU was skipped; the result below is the separate Xeon Silver 4116 benchmark in the reply, not a result from that skipped device.

## Результат / Result

| Mode | Algorithm | Speed |
|-----:|-----------|------:|
| 13400 | KeePass 1 / KeePass 2 | 4043 H/s |

```text
* Device #1: Intel(R) Xeon(R) Silver 4116 CPU @ 2.10GHz, 130658/130722 MB (32680 MB allocatable), 48MCU
Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)
Speed.#1.........: 4043 H/s (63.13ms) @ Accel:128 Loops:1024 Thr:1 Vec:8
```
