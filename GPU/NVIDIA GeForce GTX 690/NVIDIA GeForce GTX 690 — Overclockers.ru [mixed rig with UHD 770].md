# NVIDIA GeForce GTX 690 + Intel UHD Graphics 770 (mixed rig)

- **Вендор / Vendor:** NVIDIA
- **Видеокарты / GPUs:** NVIDIA GeForce GTX 690 плюс Intel UHD Graphics 770
- **Конфигурация / Setup:** смешанный стенд; одна GTX 690 определяется как два GPU-устройства (#1/#2), UHD 770 — устройство #3
- **Версия hashcat / Version:** не указана
- **Источник / Source:** [Overclockers.ru — тема «Тестируем видеокарты в hashcat»](https://forums.overclockers.ru/viewtopic.php?f=31&t=626128), сообщение Litium от 19.10.2022
- **Параметры / Options:** `--optimized-kernel-enable`; CUDA/OpenCL 11.3–11.4
- **Примечание / Note:** `Speed.#*` суммирует разные GPU, поэтому не является скоростью GTX 690. Ниже сохранены отдельные строки устройств.

## Результаты / Results

| Mode | GTX 690 GPU #1 | GTX 690 GPU #2 | UHD 770 #3 | Суммарно |
|-----:|-----------:|-----------:|-----------:|---------:|
| 0 (MD5) | 3383.6 MH/s | 3393.5 MH/s | 1253.3 MH/s | 8030.4 MH/s |
| 100 (SHA1) | 1002.3 MH/s | 1006.0 MH/s | 501.0 MH/s | 2509.3 MH/s |
| 1400 (SHA2-256) | 466.7 MH/s | 466.6 MH/s | 133.9 MH/s | 1067.2 MH/s |
| 1700 (SHA2-512) | 107.4 MH/s | 107.3 MH/s | 39485.6 kH/s | 254.1 MH/s |
| 22000 (WPA-PBKDF2) | 56417 H/s | 56667 H/s | 22010 H/s | 135.1 kH/s |
| 1000 (NTLM) | 5656.5 MH/s | 5655.3 MH/s | 2036.1 MH/s | 13347.9 MH/s |
