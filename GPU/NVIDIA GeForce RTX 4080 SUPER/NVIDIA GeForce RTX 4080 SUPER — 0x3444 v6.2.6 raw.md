# NVIDIA GeForce RTX 4080 SUPER — hashcat v6.2.6 (raw benchmark)

- **Тип свидетельства:** полный опубликованный stdout Hashcat benchmark mode; raw-файл содержит результаты по hash modes.
- **Устройство:** NVIDIA GeForce RTX 4080 SUPER, 80 MCU, 16 GB.
- **Источник:** [0x3444 — исходный файл](https://github.com/0x3444/hashcat_benchmarks/blob/main/NVIDIA_GeForce_RTX_4080_SUPER.txt) · [полный raw stdout](https://raw.githubusercontent.com/0x3444/hashcat_benchmarks/main/NVIDIA_GeForce_RTX_4080_SUPER.txt).
- **Отличие от имеющихся данных:** локальная raw-карточка its5Q относится к build v6.2.6-813; здесь сохранён отдельный прогон релизной v6.2.6, не объединённый с результатами другого build.

| Mode | Алгоритм | `Speed.#1` |
|---:|---|---:|
| 0 | MD5 | 90,280.1 MH/s |
| 100 | SHA1 | 30,397.6 MH/s |
| 1400 | SHA2-256 | 12,723.3 MH/s |
| 1700 | SHA2-512 | 4,412.2 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 1,496.7 kH/s |
| 1000 | NTLM | 163.0 GH/s |
| 3200 | bcrypt | 120.3 kH/s |
