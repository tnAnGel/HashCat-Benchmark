# Intel Core i7-11800H — Hashcat v7.1.2 mode 23410 CPU backend result

- **CPU device:** Intel Core i7-11800H.
- **Hashcat:** v7.1.2-based build; exact benchmark binary is v7.1.2-173-g81ba0c1a3.
- **Hash mode:** 23410, Bitwarden-server custom hash; benchmark mode `-b`.
- **CPU-backend evidence:** the source's benchmark table names the CPU model as the device and reports OpenCL (Intel) as the backend; no raw `hashcat -I` banner is reproduced. This is a published CPU-attributed aggregate, not raw stdout.
- **Source:** [iVision Research — Hashcat v7: Python Bridge in Practice](https://research.ivision.com/hashcat-v7.html), benchmark table and methodology.
- **Classification:** published partial/aggregate.

| Backend | Speed |
|---|---:|
| OpenCL (Intel) | 12,934 H/s |

The article reports a separate Python mode 73000 result for this processor; it is not included here because it is not a CPU OpenCL backend measurement.
