# AMD Radeon RX 5500 XT

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** Radeon RX 5500 XT, 8 GB
- **Конфигурация / Setup:** 1 GPU
- **Версия hashcat / Version:** не указана
- **Источник / Source:** [Overclockers.ru — тема «Тестируем видеокарты в hashcat»](https://forums.overclockers.ru/viewtopic.php?f=31&t=626128), сообщение Junior от 01.12.2021
- **Параметры / Options:** `--optimized-kernel-enable`; OpenCL 2.1 AMD-APP 3240.6
- **Примечание / Note:** для mode 0 опубликованный вывод сначала сообщает `Insufficient memory available`, а затем показывает скорость; предупреждение сохранено, результат требует осторожной интерпретации.

## Результаты / Results

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 13302.8 MH/s (предупреждение о нехватке памяти) |
| 100 | SHA1 | 5201.8 MH/s |
| 1400 | SHA2-256 | 2194.6 MH/s |
| 1700 | SHA2-512 | 588.8 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 261.9 kH/s |
| 1000 | NTLM | 21533.8 MH/s |
| 3200 | bcrypt | 13527 H/s |
