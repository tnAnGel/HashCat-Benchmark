# AMD Radeon R9 280X

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon R9 280X (Asus Matrix Platinum; Tahiti XT / Radeon HD 7970 GHz Edition)
- **Версия / Version:** oclHashcat beta1, октябрь 2013 (исторический benchmark)
- **Источник / Source:** [Hashcat Forum — AMD Radeon R9 280X (Asus Matrix) initial benchmark](https://hashcat.net/forum/thread-2724.html)
- **Параметры / Options:** результаты скрипта epixoip; Ubuntu 12.04 LTS, Catalyst 13.11 beta1; заводская частота GPU 1100 MHz
- **Примечание / Note:** автор публикует полный набор доступных тогда режимов; `sha512crypt` и `bcrypt` первоначально показывают 0 из-за таймаута, но автор отдельно сообщает ненулевые промежуточные скорости. Это legacy `Speed.GPU.#1`, не современный `hashcat -b`.

## Ключевые результаты / Highlights

| Алгоритм | Скорость |
|----------|---------:|
| MD5 | 6.191 GH/s |
| NTLM | 9.045 GH/s |
| SHA1 | 2.468 GH/s |
| SHA256 | 1.202 GH/s |
| WPA/WPA2 | 159.6 kH/s |

## Исходные строки / Raw excerpt

```text
Hash.Type......: MD5
Speed.GPU.#1...: 6190.8 MH/s
Hash.Type......: Joomla
Speed.GPU.#1...: 5542.8 MH/s
Hash.Type......: SHA1
Speed.GPU.#1...: 2467.6 MH/s
Hash.Type......: MSSQL(2000)
Speed.GPU.#1...: 2014.3 MH/s
Hash.Type......: phpass, MD5(Wordpress), MD5(phpBB3)
Speed.GPU.#1...: 2488.5 kH/s
Hash.Type......: md5crypt, MD5(Unix), FreeBSD MD5, Cisco-IOS MD5
Speed.GPU.#1...: 4186.6 kH/s
Hash.Type......: NTLM
Speed.GPU.#1...: 9044.8 MH/s
Hash.Type......: DCC, mscash
Speed.GPU.#1...: 4570.2 MH/s
Hash.Type......: SHA256
Speed.GPU.#1...: 1202.2 MH/s
Hash.Type......: descrypt, DES(Unix), Traditional DES
Speed.GPU.#1...: 75788.6 kH/s
Hash.Type......: SHA512
Speed.GPU.#1...: 89820.5 kH/s
Hash.Type......: sha512crypt, SHA512(Unix)
Speed.GPU.#1...: 0 H/s
Hash.Type......: WPA/WPA2
Speed.GPU.#1...: 159.6 kH/s
Hash.Type......: LM
Speed.GPU.#1...: 1555.7 MH/s
Hash.Type......: Oracle 7-10g
Speed.GPU.#1...: 451.0 MH/s
Hash.Type......: bcrypt, Blowfish(OpenBSD)
Speed.GPU.#1...: 0 H/s

# Позже автор сообщил временные значения до истечения таймаута:
sha512crypt: 14864 H/s
bcrypt: 4493 H/s
```
