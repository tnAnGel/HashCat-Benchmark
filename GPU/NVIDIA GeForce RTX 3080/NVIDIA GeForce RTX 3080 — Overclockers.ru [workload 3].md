# NVIDIA GeForce RTX 3080

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 3080, 10 GB
- **Конфигурация / Setup:** 1 GPU
- **Версия hashcat / Version:** не указана
- **Источник / Source:** [Overclockers.ru — тема «Тестируем видеокарты в hashcat»](https://forums.overclockers.ru/viewtopic.php?f=31&t=626128), сообщение kapdaga от 01.12.2021
- **Параметры / Options:** `--workload-profile=3`; OpenCL 3.0 CUDA 11.5.107
- **Примечание / Note:** workload profile 3; не смешивать напрямую с результатами `-w 4`.

## Результаты / Results

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 26201.3 MH/s |
| 100 | SHA1 | 13085.4 MH/s |
| 1400 | SHA2-256 | 5967.6 MH/s |
| 1700 | SHA2-512 | 2322.4 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 924.6 kH/s |
| 1000 | NTLM | 33219.9 MH/s |
| 3200 | bcrypt | 82848 H/s |
