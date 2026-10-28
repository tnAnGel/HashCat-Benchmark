# NVIDIA GeForce GTX 1660 SUPER

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** GeForce GTX 1660 SUPER, 6 GB
- **Конфигурация / Setup:** 1 GPU
- **Версия hashcat / Version:** v6.1.1 (версия, указанная автором для примера)
- **Источник / Source:** [Overclockers.ru — тема «Тестируем видеокарты в hashcat»](https://forums.overclockers.ru/viewtopic.php?f=31&t=626128), сообщение Jordan от 10.11.2020
- **Параметры / Options:** `hashcat.exe -b`; `--optimized-kernel-enable`; OpenCL / CUDA 11.1.96
- **Примечание / Note:** сообщение приводит демонстрационный вывод, а не отдельный пользовательский запуск.

## Результаты / Results

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 17830.3 MH/s |
| 100 | SHA1 | 6083.9 MH/s |
| 1400 | SHA2-256 | 2607.6 MH/s |
| 1700 | SHA2-512 | 770.0 MH/s |
| 1000 | NTLM | 32733.6 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 301.9 kH/s |
| 3200 | bcrypt | 12282 H/s |
