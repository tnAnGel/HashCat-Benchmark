# AMD Ryzen 9 9950X — Hashcat v7.1.2 mode 23410 CPU backend results

- **CPU device:** AMD Ryzen 9 9950X.
- **Hashcat:** v7.1.2-based build; exact benchmark binary is v7.1.2-173-g81ba0c1a3.
- **Hash mode:** 23410, Bitwarden-server custom hash; benchmark mode `-b`.
- **CPU-backend evidence:** the source's benchmark table names the CPU model as the device and reports separate Radeon iGPU rows. The measured CPU backends are PoCL and Intel OpenCL; no raw `hashcat -I` banner is reproduced, so this is an explicitly CPU-attributed published result, not raw stdout.
- **Source:** [iVision Research — Hashcat v7: Python Bridge in Practice](https://research.ivision.com/hashcat-v7.html), benchmark table and methodology.
- **Classification:** published partial/aggregate; not mixed with the separate Python mode 73000 rows or Radeon iGPU rows.

| Backend | Speed |
|---|---:|
| OpenCL (PoCL) | 10,042 H/s |
| OpenCL (Intel) | 6,234 H/s |

The table also reports a separate Python mode 73000 result for this processor; it is intentionally excluded because it is not a CPU OpenCL backend measurement.
