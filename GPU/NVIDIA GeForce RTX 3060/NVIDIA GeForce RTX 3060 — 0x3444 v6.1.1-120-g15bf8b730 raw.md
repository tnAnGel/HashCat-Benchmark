# NVIDIA GeForce RTX 3060 — hashcat v6.1.1-120-g15bf8b730 (raw benchmark)

- **Тип свидетельства:** опубликованный stdout `hashcat -b`; полный лог доступен по raw-ссылке.
- **Устройство:** GeForce RTX 3060, 28 MCU, 11,072/12,050 MB reported; CUDA backend не инициализировался, прогон использовал OpenCL NVIDIA 1.2 / CUDA 11.2.153.
- **Опции:** workload profile 4; версия Hashcat и backend сохранены как в источнике.
- **Дата прогона:** 2021-04-15 (из временной метки в raw).
- **Источник:** [0x3444 — исходный файл](https://github.com/0x3444/hashcat_benchmarks/blob/main/NVIDIA_GeForce_RTX_3060.txt) · [полный raw stdout](https://raw.githubusercontent.com/0x3444/hashcat_benchmarks/main/NVIDIA_GeForce_RTX_3060.txt).
- **Отличие от карточек в репозитории:** локальные результаты RTX 3060 относятся к v6.2.6; эта карточка фиксирует отдельный ранний v6.1.1 прогон и OpenCL fallback.

| Mode | Алгоритм | `Speed.#1` |
|---:|---|---:|
| 0 | MD5 | 10,000.4 MH/s |
| 100 | SHA1 | 4,909.0 MH/s |
| 1400 | SHA2-256 | 2,237.4 MH/s |
| 1700 | SHA2-512 | 946.7 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 398.8 kH/s |
| 1000 | NTLM | 13,858.5 MH/s |
| 3200 | bcrypt | 31,866 H/s |
