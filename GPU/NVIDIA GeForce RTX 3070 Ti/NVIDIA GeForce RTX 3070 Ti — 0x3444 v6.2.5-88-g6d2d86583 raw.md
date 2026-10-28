# NVIDIA GeForce RTX 3070 Ti — hashcat v6.2.5-88-g6d2d86583 (raw benchmark)

- **Тип свидетельства:** полный опубликованный stdout `hashcat -b --benchmark-all`.
- **Устройство:** NVIDIA GeForce RTX 3070 Ti, 48 MCU, 8 GB; NVIDIA OpenCL 3.0 / CUDA 11.5.125. Ryzen 9 5900X присутствует в списке платформ, но помечен как skipped.
- **Опции:** optimized kernel; исходный вывод показывает отдельную скорость GPU `Speed.#1`.
- **Источник:** [0x3444 — исходный файл](https://github.com/0x3444/hashcat_benchmarks/blob/main/NVIDIA_GeForce_RTX_3070_Ti.txt) · [полный raw stdout](https://raw.githubusercontent.com/0x3444/hashcat_benchmarks/main/NVIDIA_GeForce_RTX_3070_Ti.txt).
- **Отличие от имеющихся данных:** в репозитории есть результаты v6.2.3; это отдельный более поздний prerelease v6.2.5 run.

| Mode | Алгоритм | `Speed.#1` |
|---:|---|---:|
| 0 | MD5 | 42,929.0 MH/s |
| 100 | SHA1 | 13,426.4 MH/s |
| 1400 | SHA2-256 | 5,736.1 MH/s |
| 1700 | SHA2-512 | 1,660.1 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 674.6 kH/s |
| 1000 | NTLM | 74,781.1 MH/s |
| 3200 | bcrypt | 57,831 H/s |
