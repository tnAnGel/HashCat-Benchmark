# NVIDIA GeForce RTX 3070 — hashcat v6.1.1 (raw benchmark)

- **Тип свидетельства:** полный опубликованный stdout `hashcat -b`.
- **Устройство:** GeForce RTX 3070, 46 MCU; CUDA 11.2, Windows WDDM, драйвер 460.79.
- **Опции:** optimized kernel; исходный лог также содержит `nvidia-smi` и полный вывод всех benchmark modes.
- **Источник:** [0x3444 — исходный файл](https://github.com/0x3444/hashcat_benchmarks/blob/main/NVIDIA_GeForce_RTX_3070.txt) · [полный raw stdout](https://raw.githubusercontent.com/0x3444/hashcat_benchmarks/main/NVIDIA_GeForce_RTX_3070.txt).
- **Отличие от карточек в репозитории:** текущая карточка RTX 3070 содержит v6.2.6-813; здесь сохранён отдельный v6.1.1 прогон на CUDA 11.2/драйвере 460.79.

| Mode | Алгоритм | `Speed.#1` |
|---:|---|---:|
| 0 | MD5 | 36,678.9 MH/s |
| 100 | SHA1 | 12,227.9 MH/s |
| 1400 | SHA2-256 | 5,276.1 MH/s |
| 1700 | SHA2-512 | 1,737.7 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 616.4 kH/s |
| 1000 | NTLM | 67,362.8 MH/s |
| 3200 | bcrypt | 50,224 H/s |
