# AMD Radeon 760M Graphics — полный benchmark

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon 760M Graphics (RDNA 3, Phoenix iGPU; 4 MCU)
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [Hashcat Forum — AMD 760M BENCHMARK](https://hashcat.net/forum/thread-12466.html)
- **Параметры / Options:** `hashcat.exe -b -w 3`; OpenCL AMD-APP 3584.0. Автор сообщил, что `-w` здесь выключает стандартные оптимизации; это не `-O`-прогон.
- **Примечание / Note:** отдельный полный прогон той же модели. Не объединять напрямую с соседним WPA-результатом `-O` для сравнения по скорости.

## Результаты / Results

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 2010.5 MH/s |
| 100 | SHA1 | 1472.5 MH/s |
| 1400 | SHA2-256 | 736.0 MH/s |
| 1700 | SHA2-512 | 213.7 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 111.3 kH/s |
| 1000 | NTLM | 1482.6 MH/s |
| 3000 | LM | 5382.2 MH/s |
| 5500 | NetNTLMv1 / NetNTLMv1+ESS | 1415.7 MH/s |
| 5600 | NetNTLMv2 | 219.6 MH/s |
| 1500 | descrypt | 143.3 MH/s |
| 500 | md5crypt | 798.7 kH/s |
| 3200 | bcrypt | 6453 H/s |
| 1800 | sha512crypt | 11695 H/s |
| 7500 | Kerberos 5 AS-REQ | 104.7 MH/s |
| 13100 | Kerberos 5 TGS-REP | 102.6 MH/s |
| 15300 | DPAPI v1 | 20894 H/s |
| 15900 | DPAPI v2 | 8807 H/s |
| 7100 | macOS PBKDF2-SHA512 | 91709 H/s |
| 11600 | 7-Zip | 29636 H/s |
| 12500 | RAR3-hp | 5460 H/s |
| 13000 | RAR5 | 11805 H/s |
| 6211 | TrueCrypt RIPEMD160 + XTS 512 bit | 68541 H/s |
| 13400 | KeePass | 11923 H/s |
| 6800 | LastPass | 649.4 kH/s |
| 11300 | Bitcoin/Litecoin wallet.dat | 1183 H/s |

## Идентификация устройства / Device identification

```text
hashcat (v6.2.6) starting in benchmark mode
* Device #1: AMD Radeon 760M Graphics, 8480/17087 MB (3780 MB allocatable), 4MCU
Benchmark relevant options:
* --workload-profile=3
...
Started: Sun Jan 12 17:52:12 2025
Stopped: Sun Jan 12 17:54:32 2025
```
