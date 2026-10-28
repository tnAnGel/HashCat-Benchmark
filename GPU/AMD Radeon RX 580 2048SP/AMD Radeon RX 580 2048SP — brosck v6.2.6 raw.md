# AMD Radeon RX 580 2048SP — brosck, Hashcat v6.2.6

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 580 2048SP, 8 GB, 32 MCU
- **Версия Hashcat / Version:** v6.2.6
- **Тип источника / Evidence:** полный raw-вывод `hashcat -b` из GitHub Gist; это отдельный пользовательский прогон, не агрегат.
- **Источник / Source:** [brosck — rx580.txt (raw Hashcat output)](https://gist.github.com/brosck/1304acc4e1400295739b200707728fbe)
- **Backend:** OpenCL API, OpenCL 2.1 AMD-APP 3584.0. HIP runtime не инициализировался (`hiprtcCompileProgram is missing from HIPRTC shared library`).
- **Параметры / Options:** `hashcat.exe -b`; в выводе включён `--optimized-kernel-enable`.

## Результаты / Speeds

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 10,353.1 MH/s |
| 100 | SHA1 | 3,227.1 MH/s |
| 1400 | SHA2-256 | 1,355.7 MH/s |
| 1700 | SHA2-512 | 350.3 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 159.3 kH/s |
| 1000 | NTLM | 16,104.5 MH/s |
| 3000 | LM | 9,891.2 MH/s |
| 5500 | NetNTLMv1 / NetNTLMv1+ESS | 9,491.4 MH/s |
| 5600 | NetNTLMv2 | 672.1 MH/s |
| 1500 | descrypt | 379.5 MH/s |
| 500 | md5crypt | 3,916.7 kH/s |
| 3200 | bcrypt | 4,172 H/s |
| 1800 | sha512crypt | 57,675 H/s |
| 7500 | Kerberos 5 AS-REQ etype 23 | 77,798.3 kH/s |
| 13100 | Kerberos 5 TGS-REP etype 23 | 43,316.2 kH/s |
| 15300 | DPAPI masterkey v1 | 26,326 H/s |
| 15900 | DPAPI masterkey v2 | 9,612 H/s |
| 7100 | macOS PBKDF2-SHA512 | 110.4 kH/s |
| 11600 | 7-Zip | 172.8 kH/s |
| 12500 | RAR3-hp | 22,409 H/s |
| 13000 | RAR5 | 16,932 H/s |
| 6211 | TrueCrypt RIPEMD160 + XTS 512-bit | 52,777 H/s |
| 13400 | KeePass 1/2 | 36,376 H/s |
| 6800 | LastPass | 987.5 kH/s |
| 11300 | Bitcoin/Litecoin wallet.dat | 1,706 H/s |

Источник публикует весь benchmark stdout; здесь сохранены все показанные в нём режимы и скорости. Это независимый запуск и не следует сливать его показатели с другим RX 580 2048SP прогоном в соседней карточке.
