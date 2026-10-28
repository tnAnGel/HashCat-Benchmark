# NVIDIA GeForce RTX 3090 — hashcat v6.2.6-851-g6716447df+ (raw benchmark)

- **Тип свидетельства:** полный опубликованный stdout `hashcat -b --benchmark-all`.
- **Устройство:** NVIDIA GeForce RTX 3090, 82 MCU; CUDA 12.8. В логе также перечислен Ryzen 7 7800X3D, но CPU-устройство пропущено; виртуальное устройство GPU включено.
- **Опции:** `--backend-devices-virtual=1`, optimized kernel.
- **Источник:** [0x3444 — исходный файл](https://github.com/0x3444/hashcat_benchmarks/blob/main/NVIDIA_GeForce_RTX_3090.txt) · [полный raw stdout](https://raw.githubusercontent.com/0x3444/hashcat_benchmarks/main/NVIDIA_GeForce_RTX_3090.txt).
- **Отличие от имеющихся данных:** локальные raw-карточки RTX 3090 используют v6.1.1-83 и v6.2.6-813; эта запись — отдельный build v6.2.6-851 и CUDA 12.8.

| Mode | Алгоритм | `Speed.#1` |
|---:|---|---:|
| 0 | MD5 | 64,264.4 MH/s |
| 100 | SHA1 | 20,575.8 MH/s |
| 1400 | SHA2-256 | 8,863.8 MH/s |
| 1700 | SHA2-512 | 2,964.9 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 1,011.1 kH/s |
| 1000 | NTLM | 112.6 GH/s |
| 3200 | bcrypt | 96,289 H/s |
