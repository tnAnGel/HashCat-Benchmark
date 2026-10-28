# NVIDIA GeForce RTX 5090 — Hashcat v6.2.6 (raw benchmark)

- **Тип свидетельства:** полный публичный raw stdout benchmark; в источнике также обнаружен AMD iGPU, но выбран `--backend-devices=1`, и устройство #1 однозначно указано как RTX 5090.
- **Hashcat:** v6.2.6, CUDA 12.8, optimized kernel (`-O`).
- **Источник:** [0x3444/hashcat_benchmarks — NVIDIA_GeForce_RTX_5090.txt](https://github.com/0x3444/hashcat_benchmarks/blob/main/NVIDIA_GeForce_RTX_5090.txt) · [raw file](https://raw.githubusercontent.com/0x3444/hashcat_benchmarks/main/NVIDIA_GeForce_RTX_5090.txt).
- **Дата прогона:** 2025-01-30.

| Mode | Алгоритм | `Speed.#1` |
|---:|---|---:|
| 0 | MD5 | 215.8 GH/s |
| 100 | SHA1 | 69.769 GH/s |
| 1400 | SHA2-256 | 26.8233 GH/s |
| 1700 | SHA2-512 | 9.9855 GH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 3,368.1 kH/s |
| 1000 | NTLM | 331.2 GH/s |
| 3200 | bcrypt | 255.3 kH/s |

Это отдельный исходный прогон и версия Hashcat, не новая модель. В источнике доступны остальные режимы и полный stdout.
