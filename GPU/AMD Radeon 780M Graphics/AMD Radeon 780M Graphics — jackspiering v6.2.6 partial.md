# AMD Radeon 780M Graphics

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon 780M Graphics (6 MCU)
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [публичный gist jackspiering — Hashcat benchmark output](https://gist.github.com/jackspiering/fa5b3942f0e766f7b935f7cd898a0e04)
- **Параметры / Options:** `--optimized-kernel-enable`
- **Статус / Status:** частичный прогон — опубликованы шесть режимов; это не полный `--benchmark-all`.

В gist также указаны Windows 11 Pro 23H2, OpenCL 2.1 / AMD-APP 3617.0 и 4116 MB доступной памяти.

## Опубликованные результаты / Published results

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 7371.0 MH/s |
| 100 | SHA1 | 2993.0 MH/s |
| 1400 | SHA-256 | 1259.4 MH/s |
| 1700 | SHA-512 | 292.5 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 143.3 kH/s |
| 1000 | NTLM | 13336.9 MH/s |

## Фрагмент сведений об устройстве / Device excerpt

```text
AMD Radeon 780M Graphics
6 MCU
4116 MB allocatable
OpenCL 2.1 AMD-APP (3617.0)
```
