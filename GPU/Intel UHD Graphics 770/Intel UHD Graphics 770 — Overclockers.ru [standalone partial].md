# Intel UHD Graphics 770 (standalone)

- **Вендор / Vendor:** Intel
- **GPU:** Intel UHD Graphics 770 (встроенная графика Core i7-12700K)
- **Конфигурация / Setup:** одиночная iGPU; автор также указывает систему с Core i7-12700K
- **Версия hashcat / Version:** не указана
- **Источник / Source:** [Overclockers.ru — тема «Тестируем видеокарты в hashcat»](https://forums.overclockers.ru/viewtopic.php?f=31&t=626128), сообщение Litium от 12.12.2021
- **Параметры / Options:** `--optimized-kernel-enable`; OpenCL 3.0 Intel
- **Примечание / Note:** это GPU-прогон UHD 770; CPU-бенчмарка Core i7-12700K в сообщении нет.

## Результаты / Results

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 1249.9 MH/s |
| 100 | SHA1 | 499.1 MH/s |
| 1400 | SHA2-256 | 131.3 MH/s |
| 1700 | SHA2-512 | 38937.9 kH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 21913 H/s |
| 1000 | NTLM | 2025.5 MH/s |
| 3200 | bcrypt | 1527 H/s |
