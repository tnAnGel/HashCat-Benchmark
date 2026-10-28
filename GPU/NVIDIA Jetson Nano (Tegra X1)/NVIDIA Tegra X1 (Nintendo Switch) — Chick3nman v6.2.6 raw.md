# NVIDIA Tegra X1 — Nintendo Switch (Hashcat v6.2.6)

- **Тип свидетельства:** raw benchmark `hashcat -b -O -w 4 --benchmark-all`; отдельный Nintendo Switch под Linux 4 Tegra, не Jetson Nano. Это другая платформа на GPU Tegra X1, а не новый GPU-архитектурный продукт.
- **Hashcat:** v6.2.6, CUDA 10.0, optimized kernel, workload profile 4.
- **Устройство:** NVIDIA Tegra X1, 1763/3990 MB, 2 MCU.
- **Источник:** [Chick3nman — Hashcat v6.2.6 benchmark on a Nintendo Switch Tegra X1](https://gist.github.com/Chick3nman/2072be6640cd4f661669cae94f8b2788).

| Mode | Алгоритм | `Speed.#1` |
|---:|---|---:|
| 0 | MD5 | 950.6 MH/s |
| 10 | md5($pass.$salt) | 968.2 MH/s |
| 100 | SHA1 | 330.7 MH/s |
| 1400 | SHA2-256 | 121.0 MH/s |
| 1700 | SHA2-512 | 40.9646 MH/s |
| 1000 | NTLM | 1.6654 GH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 16.573 kH/s |

Источник публикует полный `--benchmark-all` stdout с дополнительными режимами; таблица здесь — выбранные типовые режимы. Значения относятся к Switch/Tegra X1 платформе и не должны подменять результаты Jetson Nano.
