# NVIDIA GeForce GTX 750

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** GeForce GTX 750 (1023 MB; точный board partner не указан)
- **Версия / Version:** cudaHashcat v1.21
- **Источник / Source:** [Hashcat Forum — GTX 750](https://hashcat.net/forum/thread-3484.html)
- **Тип данных / Evidence:** опубликованный benchmark-mode вывод; legacy, не современный `hashcat -b`

## Результаты из исходного вывода

| Mode / hash type | Алгоритм | Скорость |
|---:|---|---:|
| 0 | MD5 | 2622.8 MH/s |
| 100 | SHA1 | 929.0 MH/s |
| 1400 | SHA-256 | 339.0 MH/s |
| 1700 | SHA-512 | 75.6265 MH/s |
| 1000 | NTLM | 4576.5 MH/s |
| 3200 | bcrypt | 1829 H/s |
| — (legacy WPA mode) | WPA/WPA2 | 45119 H/s |

В теме приведён большой benchmark-mode фрагмент (десятки типов хешей), включая
устройство и workload. Здесь сохранены representative-строки; полный исходный
публичный вывод доступен по ссылке выше. Режим WPA в той версии не следует
сравнивать напрямую с современным mode 22000.
