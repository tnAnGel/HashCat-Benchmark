# NVIDIA GeForce GTX 660

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 660, 2 GB
- **Конфигурация / Setup:** 1 GPU
- **Версия hashcat / Version:** не указана
- **Источник / Source:** [Overclockers.ru — тема «Тестируем видеокарты в hashcat»](https://forums.overclockers.ru/viewtopic.php?f=31&t=626128), сообщение Litium от 20.11.2021
- **Параметры / Options:** `--optimized-kernel-enable`; OpenCL 3.0 CUDA 11.3.113
- **Примечание / Note:** сохранены основные режимы из опубликованного вывода.

## Результаты / Results

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 2161.7 MH/s |
| 100 | SHA1 | 620.1 MH/s |
| 1400 | SHA2-256 | 297.4 MH/s |
| 1700 | SHA2-512 | 68056.4 kH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 35776 H/s |
| 1000 | NTLM | 3608.7 MH/s |
