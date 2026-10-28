# NVIDIA GeForce GTX 770

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 770, 2 GB
- **Конфигурация / Setup:** 1 GPU
- **Версия hashcat / Version:** не указана
- **Источник / Source:** [Overclockers.ru — тема «Тестируем видеокарты в hashcat»](https://forums.overclockers.ru/viewtopic.php?f=31&t=626128), сообщение Litium, декабрь 2021
- **Параметры / Options:** `--optimized-kernel-enable`; OpenCL 3.0 CUDA 11.4.136
- **Примечание / Note:** сохранена выборка режимов из длинного вывода.

## Результаты / Results

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 3801.1 MH/s |
| 100 | SHA1 | 1134.5 MH/s |
| 1400 | SHA2-256 | 521.7 MH/s |
| 1700 | SHA2-512 | 121.2 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 62844 H/s |
| 1000 | NTLM | 6300.3 MH/s |
| 3200 | bcrypt | 936 H/s |
