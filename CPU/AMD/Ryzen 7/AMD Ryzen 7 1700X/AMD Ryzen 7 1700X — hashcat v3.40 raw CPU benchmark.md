# AMD Ryzen 7 1700X — Hashcat v3.40 CPU benchmark

- **CPU device:** AMD Ryzen 7 1700X Eight-Core Processor, Device #3.
- **Hashcat:** v3.40.
- **Command:** `hashcat64.exe -D 1 -b`; the two Fiji GPUs are explicitly `skipped`, and OpenCL device type 1 selects CPU.
- **Source:** [Hashcat Forum — “Ryzen OpenCL benchmarks?”, post #12](https://hashcat.net/forum/post-34016.html).
- **Classification:** partial raw stdout, CPU-only device selected.

| Mode / algorithm | CPU speed |
|---|---:|
| MD4 | 734.8 MH/s |
| MD5 | 602.2 MH/s |
| SHA1 | 271.4 MH/s |
| SHA256 | 81,382.7 kH/s |
| WPA/WPA2 | 10,278 H/s |

The cited post contains the complete benchmark fragment for many additional modes. These are a separate v3.40 run; the existing v5.1.0 result is not altered or merged with it.
