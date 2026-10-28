# NVIDIA GeForce GTX 765M

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** GeForce GTX 765M, 2048 MB, 862 MHz, 4 MCU
- **Версия / Version:** cudaHashcat-lite v0.15
- **Источник / Source:** [Hashcat Forum — GTX 765M benchmark](https://hashcat.net/forum/thread-2617.html)
- **Тип данных / Evidence:** raw partial benchmark-mode excerpt; timed runs were aborted by runtime limit

## Опубликованные строки

| Тип хеша в исходнике | Алгоритм | Скорость |
|---|---|---:|
| MD5 | MD5 | 1428.6 M/s |
| md5($pass.$salt) | salted MD5 | 1428.4 M/s |
| (форумный фрагмент, тип не сохранился) | — | 13,562.7 k/s |
| SHA512 | SHA-512 | 44,090.0 k/s |
| sha512($pass.$salt) | salted SHA-512 | 44,085.9 k/s |
| Cisco-PIX MD5 | Cisco-PIX MD5 | 879.6 M/s |
| Double MD5 | double MD5 | 408.6 M/s |
| vBulletin < v3.8.5 | vBulletin | 408.7 M/s |
| vBulletin > v3.8.5 | vBulletin | 265.8 M/s |
| IPB2+, MyBB1.2+ | forum hash | 268.8 M/s |
| LM | LM | 70,609.9 k/s |
| Oracle 7–10g | Oracle | 50,452.4 k/s |
| SHA-3 (Keccak) | SHA-3 | 27,024.0 k/s |
| Half MD5 | Half MD5 | 637.0 M/s |
| NetNTLMv1-VANILLA / +ESS | NetNTLMv1 | 1052.4 M/s |
| NetNTLMv2 | NetNTLMv2 | 97,301.5 k/s |
| Cisco-IOS SHA256 | SHA-256 | 158.9 M/s |

Часть источника после NetNTLMv2 сохранена на странице форума; этот документ
фиксирует только строки, явно прочитанные в опубликованном фрагменте.
