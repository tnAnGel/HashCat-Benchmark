# Apple M5 Max — Hashcat-ng fork, WPA mode only

- **Вендор / Vendor:** Apple
- **GPU:** Apple M5 Max, GPU device #02, 40 MCU; the Metal device is skipped in this run and OpenCL is used.
- **Версия / Version string:** `hashcat (v7.1.2)`; the Gist is explicitly titled as a proprietary `Hashcat-ng` fork, so this is **not verified as an upstream Hashcat build**.
- **Источник / Source:** [GermanAizek Gist — Hashcat-ng GPU benchmark](https://gist.github.com/GermanAizek/f968d0bb213b2b7c8d9b35bbc4d031e4), M5 Max 128 GB excerpt.
- **Параметры / Options:** `--backend-devices-virtmulti=1`, `--backend-devices-virthost=1`, `--optimized-kernel-enable`.
- **Примечание / Note:** Raw console fragment for one mode. Keep separate from upstream Hashcat rankings: the source identifies the program as a proprietary fork and the virtual-device options are fork-specific.

## Результат / Result

| Mode | Algorithm | Speed |
|-----:|-----------|------:|
| 22000 | WPA-PBKDF2-PMKID+EAPOL, 4095 iterations | 413.5 kH/s |

```text
hashcat (v7.1.2) starting in benchmark mode
METAL API (Metal 373.2)
* Device #01: Apple M5 Max, skipped
OpenCL API (OpenCL 1.2 (Apr 18 2026 19:20:04)) - Platform #1 [Apple]
* Device #02: Apple M5 Max, GPU, 55050/110100 MB (10321 MB allocatable), 40MCU
* --backend-devices-virtmulti=1
* --backend-devices-virthost=1
* --optimized-kernel-enable
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
Speed.#02........:   413.5 kH/s (103.84ms) @ Accel:704 Loops:1024 Thr:256 Vec:1
```
