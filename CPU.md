# 🧠 Сводная таблица процессоров

Индекс всех процессоров коллекции. Файлы лежат в [`CPU/`](CPU) с разбивкой
**вендор → семейство → модель**, формат описан в [`CPU/README.md`](CPU/README.md).

**Текущее покрытие: 285 моделей процессоров** в папках с карточками. Карточки включают raw/partial/legacy-логи, per-device значения из смешанных запусков и отдельно обозначенные опубликованные сравнения; они не считаются равноценными свидетельствами и не все входят в основной ranking.

Значения — на **одно устройство** (`Speed.#N` CPU-устройства), режим
оптимизированного ядра (`-O`). Единицы: H/s → kH/s → MH/s → GH/s.
Все прогоны — CPU-only или CPU из смешанного прогона с однозначным сопоставлением.

| # | CPU | Ядра/потоки | MD5 | NTLM | SHA2-256 | SHA2-512 | WPA2 | bcrypt |
|--:|-----|-------------|----:|-----:|---------:|---------:|-----:|-------:|
| 1 | [AMD EPYC 9754](<CPU/AMD/EPYC/AMD EPYC 9754>) | 128/256 | 28.0 GH/s | 58.7 GH/s | 10.3 GH/s | 3.5 GH/s | 1.0 MH/s | 239 kH/s |
| 2 | [AMD EPYC 9654](<CPU/AMD/EPYC/AMD EPYC 9654>) | 96/192 | 23.5 GH/s | 18.3 GH/s | 7.5 GH/s | 2.4 GH/s | — | 174 kH/s |
| 3 | [AMD Ryzen Threadripper 3970X](<CPU/AMD/Ryzen Threadripper/AMD Ryzen Threadripper 3970X>) | 32/64 | 5.4 GH/s | 9.6 GH/s | 984 MH/s | 294 MH/s | 133 kH/s | 40.8 kH/s |
| 4 | [AMD Ryzen Threadripper 3960X](<CPU/AMD/Ryzen Threadripper/AMD Ryzen Threadripper 3960X>) | 24/48 | 3.8 GH/s | 6.1 GH/s | 605 MH/s | 215 MH/s | 86.7 kH/s | 23.3 kH/s |
| 5 | [AMD Ryzen 7 7700X](<CPU/AMD/Ryzen 7/AMD Ryzen 7 7700X>) | 8/16 | 3.3 GH/s | 6.2 GH/s | 762 MH/s | 261 MH/s | 64.2 kH/s | 1.0 kH/s |
| 6 | [AMD Ryzen Threadripper 1950X](<CPU/AMD/Ryzen Threadripper/AMD Ryzen Threadripper 1950X>) | 16/32 | 1.8 GH/s | 2.9 GH/s | 185 MH/s | 70.6 MH/s | 27.4 kH/s | 18.1 kH/s |
| 7 | [AMD Ryzen 7 5800X](<CPU/AMD/Ryzen 7/AMD Ryzen 7 5800X>) | 8/16 | 1.6 GH/s | 3.0 GH/s | 344 MH/s | 122 MH/s | 43.1 kH/s | 11.8 kH/s |
| 8 | [Intel Core i9-11950H](<CPU/Intel/Core i9/Intel Core i9-11950H>) | 8/16 | 1.5 GH/s | 2.6 GH/s | 350 MH/s | 109 MH/s | 27.2 kH/s | 99 H/s |
| 9 | [Intel Core i7-9700K](<CPU/Intel/Core i7/Intel Core i7-9700K>) | 8/8 | 1.0 GH/s | 1.9 GH/s | 299 MH/s | 88.9 MH/s | — | 6.0 kH/s |
| 10 | [Intel Core i7-4770](<CPU/Intel/Core i7/Intel Core i7-4770>) | 4/8 | 431 MH/s | 641 MH/s | 84.6 MH/s | 26.6 MH/s | 10.6 kH/s | 103 H/s |
| 11 | [Intel Core i3-4130](<CPU/Intel/Core i3/Intel Core i3-4130>) | 2/4 | 276 MH/s | 402 MH/s | 53.3 MH/s | 15.6 MH/s | 6.0 kH/s | 18 H/s |
| 12 | [Intel Core i5-8250U](<CPU/Intel/Core i5/Intel Core i5-8250U>) | 4/8 | 255 MH/s | 421 MH/s | 21.9 MH/s | 6.6 MH/s | — | 2.9 kH/s |
| 13 | [Intel Xeon E5-2676 v3](<CPU/Intel/Xeon/Intel Xeon E5-2676 v3>) ⚠️ | 12/24 | 135 MH/s | — | 42.8 MH/s | — | — | — |
| 14 | [AMD Ryzen 5 4600H](<CPU/AMD/Ryzen 5/AMD Ryzen 5 4600H>) ⚠️ | 6/12 | — | — | — | — | — | — |

> ⚠️ **Xeon E5-2676 v3** — вывод обрезан на 3 режимах (MD5/SHA1/SHA2-256).
> **Ryzen 5 4600H** — только один режим SHA1 (478.2 MH/s), в сводные колонки не попадает;
> подробности в файле карточки.

> Прочерк «—» означает, что режим отсутствует в исходном прогоне.
> Пометка ⚠️ у карточки — прогон неполный или с нестандартными опциями,
> подробности в шапке соответствующего файла.

## Новые частичные результаты

Эти модели подтверждены отдельными публичными Hashcat benchmark-режимами, но
пока не имеют сопоставимого набора данных для основной таблицы:

- [Intel Core i3-2330M](<CPU/Intel/Core i3/Intel Core i3-2330M>) — v5.1.0, несколько режимов.
- [Intel Core i3-2350M](<CPU/Intel/Core i3/Intel Core i3-2350M>) — v5.1.0, один MD5-режим с `--force` / PoCL.
- [Intel Core i7-3632QM](<CPU/Intel/Core i7/Intel Core i7-3632QM>) — v6.2.5, один MD5-режим.
- [Intel Core i7-6700K](<CPU/Intel/Core i7/Intel Core i7-6700K>) — v6.2.1, один SCRYPT-режим (mode 15700, `N=262144`).
- [Intel Core i7-8550U](<CPU/Intel/Core i7/Intel Core i7-8550U>) — mode 2500, Intel CPU Runtime и PoCL; опубликованная таблица без версии/raw stdout.
- [Intel Core i5-1240P](<CPU/Intel/Core i5/Intel Core i5-1240P>) — v6.2.6, один MD5-режим; скорость CPU отделена от iGPU.
- [Intel Core i7-14700K](<CPU/Intel/Core i7/Intel Core i7-14700K>) — официальные Hashcat v7.0.0 Argon2 modes 34000/70000 и v8.0.0 Python Bridge SHA-256 mode 73000; без raw stdout.
- [Intel Core i7-1165G7](<CPU/Intel/Core i7/Intel Core i7-1165G7>) — v7.1.2 CPU-only MD5 mode 0, 1647.2 MH/s, PoCL; partial raw.
- [AMD Ryzen 9 9900X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 9900X>) — официальный Hashcat v7.0.0 report: NTLM >10 GH/s и Argon2 modes 34000/70000; без raw stdout.
- [Intel Xeon E5-4640](<CPU/Intel/Xeon/Intel Xeon E5-4640>) — Hashcat Forum: 17.6433 MH/s на четырёхсокетном узле, DES-контекст, mode/version в успешной строке не указаны.
- [AMD Ryzen 9 5900X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 5900X>) — v6.2.6, один SCRYPT-режим, два профиля DDR4.
- [Intel Core i3-550](<CPU/Intel/Core i3/Intel Core i3-550>) — MD5.
- [Intel Core i5-5250U](<CPU/Intel/Core i5/Intel Core i5-5250U>) — MD5.
- [Intel Core i5-5287U](<CPU/Intel/Core i5/Intel Core i5-5287U>) — SSHA-512, явный CPU-only benchmark.
- [Intel Core i5-3470](<CPU/Intel/Core i5/Intel Core i5-3470>) — v5.1.0, шесть режимов.
- [Intel Core i7-2720QM](<CPU/Intel/Core i7/Intel Core i7-2720QM>) — oclHashcat v2.01, MD4/MD5.
- [Intel Core i7-2820QM](<CPU/Intel/Core i7/Intel Core i7-2820QM>) — v6.2.5, MD5.
- [Intel Core i7-3615QM](<CPU/Intel/Core i7/Intel Core i7-3615QM>) — oclHashcat v2.01, MD4.
- [Intel Core i9-7920X](<CPU/Intel/Core i9/Intel Core i9-7920X>) — descrypt, CPU device в смешанной системе.
- [Intel Core i9-9900KF](<CPU/Intel/Core i9/Intel Core i9-9900KF>) — v5.1.0, MD5.
- [Intel Core i5-13420H](<CPU/Intel/Core i5/Intel Core i5-13420H>) — v6.2.6, PoCL, SHA2-256.
- [Intel Xeon E5-2670 0](<CPU/Intel/Xeon/Intel Xeon E5-2670 0>) — NTLM, CPU device в многоплатформенном выводе.
- [Intel Xeon X5482](<CPU/Intel/Xeon/Intel Xeon X5482>) — v5.1.0, WPA2.
- [Intel Xeon E5-2630 v3](<CPU/Intel/Xeon/Intel Xeon E5-2630 v3>) — v3.40, MD4.
- [Intel Xeon E5-2697 v2](<CPU/Intel/Xeon/Intel Xeon E5-2697 v2>) — v3.6.0, MD4.
- [Intel Xeon E5-2620 v3](<CPU/Intel/Xeon/Intel Xeon E5-2620 v3>) — oclHashcat v2.01, NetNTLMv1.
- [Intel Core i7-4870HQ](<CPU/Intel/Core i7/Intel Core i7-4870HQ>) — oclHashcat v2.01, AzureSync PBKDF2.
- [Intel Core i7-4600U](<CPU/Intel/Core i7/Intel Core i7-4600U>) — v4.0.1 PoCL, MD4/MD5.
- [AMD Ryzen 7 1700X](<CPU/AMD/Ryzen 7/AMD Ryzen 7 1700X>) — WPA2, CPU в смешанном запуске.
- [AMD Ryzen 5 2400G](<CPU/AMD/Ryzen 5/AMD Ryzen 5 2400G>) — v5.1.0, несколько режимов.
- [AMD Ryzen 5 8600G](<CPU/AMD/Ryzen 5/AMD Ryzen 5 8600G>) — WPA-PBKDF2, CPU отдельно от Radeon 760M.
- [AMD Ryzen 7 2700](<CPU/AMD/Ryzen 7/AMD Ryzen 7 2700>) — v6.2.6, MD5, CPU в mixed run.
- [AMD Ryzen 7 3700X](<CPU/AMD/Ryzen 7/AMD Ryzen 7 3700X>) — v6.2.2, CPU-only MD5 после пропуска RX 580.
- [AMD Ryzen 7 PRO 5850U](<CPU/AMD/Ryzen 7/AMD Ryzen 7 PRO 5850U>) — mode 1400 PoCL CPU, нестандартный `-w 1`/CPU affinity.
- [Intel Core i5-10300H](<CPU/Intel/Core i5/Intel Core i5-10300H>) — v5.1.0, CPU device в mixed run, MD5.
- [AMD Ryzen 5 1500X](<CPU/AMD/Ryzen 5/AMD Ryzen 5 1500X>) — опубликованный фрагмент benchmark-вывода на рисунке; версия не указана.
- [Intel Xeon W-3223](<CPU/Intel/Xeon/Intel Xeon W-3223>) — v6.2.2-80, 23 измеренных режима в mixed run; CPU-пропуски в двух режимах.
- [Intel Xeon Silver 4116](<CPU/Intel/Xeon/Intel Xeon Silver 4116>) — KeePass mode 13400, версия в фрагменте не указана.
- [Intel Core i5-4250U](<CPU/Intel/Core i5/Intel Core i5-4250U>) — 17 CPU-режимов из частичного Gist; версия не указана, bcrypt с runtime errors.
- [Apple M1](<CPU/Apple/M Series/Apple M1>) — v6.2.5-139, CPU OpenCL `Speed.#1` в смешанном CPU+GPU raw-запуске; не CPU-isolated.
- [Intel Core i7-4770K](<CPU/Intel/Core i7/Intel Core i7-4770K>) — `oclHashcat -b`, mode 1000, Intel runtime и PoCL; частичный raw с проблемой PoCL.
- [AMD Ryzen 7 1700X](<CPU/AMD/Ryzen 7/AMD Ryzen 7 1700X>) — Hashcat v3.40, CPU-only `-D1 -b`, raw.
- [Intel Core i9-10900F](<CPU/Intel/Core i9/Intel Core i9-10900F>) — опубликованная CPU-only скорость MD4; нет raw stdout.
- [AMD Ryzen 5 1600](<CPU/AMD/Ryzen 5/AMD Ryzen 5 1600>), [Ryzen 9 9950X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 9950X>) и [Intel Core i7-11800H](<CPU/Intel/Core i7/Intel Core i7-11800H>) — iVision v7.1.2, mode 23410, опубликованные CPU/OpenCL backend-строки без raw stdout.
- [AMD Ryzen 7 4800H](<CPU/AMD/Ryzen 7/AMD Ryzen 7 4800H>), [Ryzen 7 7700](<CPU/AMD/Ryzen 7/AMD Ryzen 7 7700>) и [Pentium N3530](<CPU/Intel/Pentium/Pentium N3530>) — результаты WPA2 dictionary attack из статьи Chalyi et al.; это не `hashcat -b`.

### Legacy benchmark outputs (старые единицы words/s)

Эти записи оставлены в исходной метрике старых версий Hashcat и не включены в
современное ранжирование `H/s`.

- [Intel Core 2 Duo T7600](<CPU/Intel/Core 2/Intel Core 2 Duo T7600>) — v3.00, MD5 и WPA.
- [Intel Core i5-5300U](<CPU/Intel/Core i5/Intel Core i5-5300U>) — v2.00, MD4/MD5.
- [Intel Core i5-4200U](<CPU/Intel/Core i5/Intel Core i5-4200U>) — MD4/MD5/SHA1.
- [Intel Core i5-2450M](<CPU/Intel/Core i5/Intel Core i5-2450M>) — v0.49/v0.50, MD5.
- [Intel Core i5-4570](<CPU/Intel/Core i5/Intel Core i5-4570>) — v0.49 AVX2, MD4/MD5.
- [Intel Core i7 M 620](<CPU/Intel/Core i7/Intel Core i7 M 620>) — v0.49, MD4/MD5.
- [Intel Core i7-2670QM](<CPU/Intel/Core i7/Intel Core i7-2670QM>) — legacy MD4/MD5.
- [Intel Core i7-2600K](<CPU/Intel/Core i7/Intel Core i7-2600K>) — legacy MD4/MD5.
- [Intel Core i7-4940MX](<CPU/Intel/Core i7/Intel Core i7-4940MX>) — v0.49, MD4/MD5.
- [Intel Core i7-5960X](<CPU/Intel/Core i7/Intel Core i7-5960X>) — v0.49 AVX2, MD4/MD5.
- [Intel Xeon E7450](<CPU/Intel/Xeon/Intel Xeon E7450>) — v2.00, bcrypt.
- [Intel Xeon E7-4880 v2](<CPU/Intel/Xeon/Intel Xeon E7-4880 v2>) — v0.50, MD4/MD5/SHA1.
- [AMD FX-8350](<CPU/AMD/FX/AMD FX-8350>) — v0.49 XOP, MD4/MD5.

Новые отдельные режимы на уже заведённых моделях: Core i7-9700K (SCRYPT),
Ryzen Threadripper 3970X (SCRYPT) и Threadripper 1950X (дополнительные WPA2
backend/OS-прогоны). Они сохранены отдельными источниками и не заменяют основной набор.

## Community WPA-PBKDF2 comparison (mode 22000) — не raw

227 уникальных названий CPU из Gist GermanAizek перенесены в отдельные карточки
по папкам моделей. В таблице ниже сохранены исходное написание и скорость;
методика, версия Hashcat и raw stdout не опубликованы, поэтому значения не
смешиваются с основным ranking. Повтор Core M-5Y10c с тем же значением
объединён в одну карточку.

<!-- WPA22000_INDEX_START -->
<!-- WPA22000_INDEX_END -->

---

## Полный указатель моделей

В каталоге 285 папок моделей; строки с community/PHCS-данными не означают наличие raw.

<!-- FULL_CPU_INDEX_START -->
| CPU-модель / папка | WPA mode 22000, H/s | Другие карточки | Что есть |
|---|---:|---:|---|
| [Apple M1](<CPU/Apple/M Series/Apple M1>) | — | 1 | CPU `Speed.#1` из смешанного raw-прогона |
| [AMD A4-4000 APU](<CPU/AMD/APU/AMD A4-4000 APU>) | 1464 | 0 | community WPA22000 |
| [AMD A6-4455M APU](<CPU/AMD/APU/AMD A6-4455M APU>) | 871 | 0 | community WPA22000 |
| [AMD A6-5200 APU](<CPU/AMD/APU/AMD A6-5200 APU>) | 1914 | 0 | community WPA22000 |
| [AMD A6-5400K APU](<CPU/AMD/APU/AMD A6-5400K APU>) | 1597 | 0 | community WPA22000 |
| [AMD A8-3500M APU](<CPU/AMD/APU/AMD A8-3500M APU>) | 1872 | 0 | community WPA22000 |
| [AMD A8-4500M](<CPU/AMD/APU/AMD A8-4500M>) | 2078 | 0 | community WPA22000 |
| [AMD A8-5550M APU](<CPU/AMD/APU/AMD A8-5550M APU>) | 2276 | 0 | community WPA22000 |
| [AMD Athlon 64 X2 4600+](<CPU/AMD/Athlon/AMD Athlon 64 X2 4600+>) | 625 | 0 | community WPA22000 |
| [AMD Athlon II X2 260](<CPU/AMD/Athlon/AMD Athlon II X2 260>) | 1536 | 0 | community WPA22000 |
| [AMD Athlon II X2 270](<CPU/AMD/Athlon/AMD Athlon II X2 270>) | 1948 | 0 | community WPA22000 |
| [AMD Athlon II X4 610e](<CPU/AMD/Athlon/AMD Athlon II X4 610e>) | 2704 | 0 | community WPA22000 |
| [AMD Athlon II X4 631](<CPU/AMD/Athlon/AMD Athlon II X4 631>) | 3193 | 0 | community WPA22000 |
| [AMD Athlon II X4 640](<CPU/AMD/Athlon/AMD Athlon II X4 640>) | 3437 | 0 | community WPA22000 |
| [AMD Athlon X2 245](<CPU/AMD/Athlon/AMD Athlon X2 245>) | 1558 | 0 | community WPA22000 |
| [AMD Athlon X2 QL-64](<CPU/AMD/Athlon/AMD Athlon X2 QL-64>) | 592 | 0 | community WPA22000 |
| [AMD Athlon X4 750K](<CPU/AMD/Athlon/AMD Athlon X4 750K>) | 3379 | 0 | community WPA22000 |
| [AMD Athlon X4 860K](<CPU/AMD/Athlon/AMD Athlon X4 860K>) | 3392 | 0 | community WPA22000 |
| [AMD E-300 APU](<CPU/AMD/APU/AMD E-300 APU>) | 275 | 0 | community WPA22000 |
| [AMD E-350](<CPU/AMD/APU/AMD E-350>) | 364 | 0 | community WPA22000 |
| [AMD E1-1200 APU](<CPU/AMD/APU/AMD E1-1200 APU>) | 276 | 0 | community WPA22000 |
| [AMD E1-2100 APU](<CPU/AMD/APU/AMD E1-2100 APU>) | 459 | 0 | community WPA22000 |
| [AMD E2-3000M APU](<CPU/AMD/APU/AMD E2-3000M APU>) | 1032 | 0 | community WPA22000 |
| [AMD EPYC 9654](<CPU/AMD/EPYC/AMD EPYC 9654>) | — | 1 | 1 other card(s) |
| [AMD EPYC 9754](<CPU/AMD/EPYC/AMD EPYC 9754>) | — | 1 | 1 other card(s), PHCS summary |
| [AMD FX-4320 Quad-Core](<CPU/AMD/FX/AMD FX-4320 Quad-Core>) | 3604 | 0 | community WPA22000 |
| [AMD FX-6100](<CPU/AMD/FX/AMD FX-6100>) | 4065 | 0 | community WPA22000 |
| [AMD FX-6300](<CPU/AMD/FX/AMD FX-6300>) | 4262 | 0 | community WPA22000 |
| [AMD FX-6350](<CPU/AMD/FX/AMD FX-6350>) | 5738 | 0 | community WPA22000 |
| [AMD FX-8120](<CPU/AMD/FX/AMD FX-8120>) | 5484 | 0 | community WPA22000 |
| [AMD FX-8150 Eight-Core](<CPU/AMD/FX/AMD FX-8150 Eight-Core>) | 7087 | 0 | community WPA22000 |
| [AMD FX-8320 Eight-Core](<CPU/AMD/FX/AMD FX-8320 Eight-Core>) | 6387 | 0 | community WPA22000 |
| [AMD FX-8350](<CPU/AMD/FX/AMD FX-8350>) | 7577 | 1 | 1 other card(s), community WPA22000 |
| [AMD Phenom 8450](<CPU/AMD/Phenom/AMD Phenom 8450>) | 1597 | 0 | community WPA22000 |
| [AMD Phenom 9550](<CPU/AMD/Phenom/AMD Phenom 9550>) | 2111 | 0 | community WPA22000 |
| [AMD Phenom 9750 Quad-Core](<CPU/AMD/Phenom/AMD Phenom 9750 Quad-Core>) | 2173 | 0 | community WPA22000 |
| [AMD Phenom II N950 Quad-Core](<CPU/AMD/Phenom/AMD Phenom II N950 Quad-Core>) | 2442 | 0 | community WPA22000 |
| [AMD Phenom II X4 840](<CPU/AMD/Phenom/AMD Phenom II X4 840>) | 3638 | 0 | community WPA22000 |
| [AMD Phenom II X4 965](<CPU/AMD/Phenom/AMD Phenom II X4 965>) | 4015 | 0 | community WPA22000 |
| [AMD Phenom II X4 B50](<CPU/AMD/Phenom/AMD Phenom II X4 B50>) | 3721 | 0 | community WPA22000 |
| [AMD Phenom II X6 1055T](<CPU/AMD/Phenom/AMD Phenom II X6 1055T>) | 6445 | 0 | community WPA22000 |
| [AMD Phenom II X6 1075T](<CPU/AMD/Phenom/AMD Phenom II X6 1075T>) | 5227 | 0 | community WPA22000 |
| [AMD Ryzen 5 1500X](<CPU/AMD/Ryzen 5/AMD Ryzen 5 1500X>) | — | 1 | 1 other card(s) |
| [AMD Ryzen 5 1600](<CPU/AMD/Ryzen 5/AMD Ryzen 5 1600>) | — | 1 | iVision mode 23410 CPU backend; aggregate |
| [AMD Ryzen 5 2400G](<CPU/AMD/Ryzen 5/AMD Ryzen 5 2400G>) | 7790 | 1 | 1 other card(s), community WPA22000 |
| [AMD Ryzen 5 2600X](<CPU/AMD/Ryzen 5/AMD Ryzen 5 2600X>) | 10747 | 0 | community WPA22000 |
| [AMD Ryzen 5 3500X](<CPU/AMD/Ryzen 5/AMD Ryzen 5 3500X>) | 23952 | 0 | community WPA22000 |
| [AMD Ryzen 5 4600H](<CPU/AMD/Ryzen 5/AMD Ryzen 5 4600H>) | — | 1 | 1 other card(s) |
| [AMD Ryzen 5 8600G](<CPU/AMD/Ryzen 5/AMD Ryzen 5 8600G>) | — | 1 | 1 other card(s) |
| [AMD Ryzen 7 1700X](<CPU/AMD/Ryzen 7/AMD Ryzen 7 1700X>) | — | 2 | v3.40 raw `-D1 -b`; plus partial card |
| [AMD Ryzen 7 2700](<CPU/AMD/Ryzen 7/AMD Ryzen 7 2700>) | — | 1 | 1 other card(s) |
| [AMD Ryzen 7 3700X](<CPU/AMD/Ryzen 7/AMD Ryzen 7 3700X>) | 34817 | 1 | 1 other card(s), community WPA22000 |
| [AMD Ryzen 7 4800H](<CPU/AMD/Ryzen 7/AMD Ryzen 7 4800H>) | — | 1 | WPA2 dictionary-attack paper; not `-b` |
| [AMD Ryzen 7 5800U](<CPU/AMD/Ryzen 7/AMD Ryzen 7 5800U>) | 33162 | 0 | community WPA22000 |
| [AMD Ryzen 7 5800X](<CPU/AMD/Ryzen 7/AMD Ryzen 7 5800X>) | — | 1 | 1 other card(s) |
| [AMD Ryzen 7 7700](<CPU/AMD/Ryzen 7/AMD Ryzen 7 7700>) | — | 1 | WPA2 dictionary-attack paper; not `-b` |
| [AMD Ryzen 7 7700X](<CPU/AMD/Ryzen 7/AMD Ryzen 7 7700X>) | — | 1 | 1 other card(s) |
| [AMD Ryzen 7 PRO 5850U](<CPU/AMD/Ryzen 7/AMD Ryzen 7 PRO 5850U>) | — | 1 | 1 other card(s) |
| [AMD Ryzen 9 3900X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 3900X>) | 48838 | 0 | community WPA22000 |
| [AMD Ryzen 9 5900X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 5900X>) | 65737 | 1 | 1 other card(s), community WPA22000 |
| [AMD Ryzen 9 5950X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 5950X>) | 68376 | 0 | community WPA22000 |
| [AMD Ryzen 9 9900X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 9900X>) | — | 1 | 1 other card(s) |
| [AMD Ryzen 9 9950X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 9950X>) | — | 1 | iVision mode 23410 CPU backend; aggregate |
| [AMD Ryzen Threadripper 1950X](<CPU/AMD/Ryzen Threadripper/AMD Ryzen Threadripper 1950X>) | — | 2 | 2 other card(s) |
| [AMD Ryzen Threadripper 3960X](<CPU/AMD/Ryzen Threadripper/AMD Ryzen Threadripper 3960X>) | — | 1 | 1 other card(s) |
| [AMD Ryzen Threadripper 3970X](<CPU/AMD/Ryzen Threadripper/AMD Ryzen Threadripper 3970X>) | — | 2 | 2 other card(s) |
| [AMD Ryzen Threadripper 3990X 64-Core](<CPU/AMD/Ryzen Threadripper/AMD Ryzen Threadripper 3990X 64-Core>) | — | 0 | PHCS summary |
| [AMD Sempron 145](<CPU/AMD/Sempron/AMD Sempron 145>) | 818 | 0 | community WPA22000 |
| [AMD Sempron X2 180](<CPU/AMD/Sempron/AMD Sempron X2 180>) | 1416 | 0 | community WPA22000 |
| [AMD Sempron X2 190](<CPU/AMD/Sempron/AMD Sempron X2 190>) | 1386 | 0 | community WPA22000 |
| [AMD Turion 64 X2 TL-52](<CPU/AMD/Turion/AMD Turion 64 X2 TL-52>) | 447 | 0 | community WPA22000 |
| [AMD Turion II P560](<CPU/AMD/Turion/AMD Turion II P560>) | 1165 | 0 | community WPA22000 |
| [Celeron Dual-Core T3000](<CPU/Intel/Celeron/Celeron Dual-Core T3000>) | 1091 | 0 | community WPA22000 |
| [Intel 2140](<CPU/Intel/Other Intel/Intel 2140>) | 1362 | 0 | community WPA22000 |
| [Intel Atom D525](<CPU/Intel/Atom/Intel Atom D525>) | 804 | 0 | community WPA22000 |
| [Intel Atom N2600](<CPU/Intel/Atom/Intel Atom N2600>) | 626 | 0 | community WPA22000 |
| [Intel Atom N270](<CPU/Intel/Atom/Intel Atom N270>) | 380 | 0 | community WPA22000 |
| [Intel Atom N455](<CPU/Intel/Atom/Intel Atom N455>) | 281 | 0 | community WPA22000 |
| [Intel Atom N470](<CPU/Intel/Atom/Intel Atom N470>) | 360 | 0 | community WPA22000 |
| [Intel Atom Z3735F](<CPU/Intel/Atom/Intel Atom Z3735F>) | 975 | 0 | community WPA22000 |
| [Intel Celeron 1000M](<CPU/Intel/Celeron/Intel Celeron 1000M>) | 1472 | 0 | community WPA22000 |
| [Intel Celeron 1005M](<CPU/Intel/Celeron/Intel Celeron 1005M>) | 1471 | 0 | community WPA22000 |
| [Intel Celeron 1007U](<CPU/Intel/Celeron/Intel Celeron 1007U>) | 1190 | 0 | community WPA22000 |
| [Intel Celeron 430](<CPU/Intel/Celeron/Intel Celeron 430>) | 516 | 0 | community WPA22000 |
| [Intel Celeron 925](<CPU/Intel/Celeron/Intel Celeron 925>) | 719 | 0 | community WPA22000 |
| [Intel Celeron CPU B800](<CPU/Intel/Celeron/Intel Celeron CPU B800>) | 1127 | 0 | community WPA22000 |
| [Intel Celeron E1500](<CPU/Intel/Celeron/Intel Celeron E1500>) | 1613 | 0 | community WPA22000 |
| [Intel Celeron M](<CPU/Intel/Celeron/Intel Celeron M>) | 79 | 0 | community WPA22000 |
| [Intel Celeron M 530](<CPU/Intel/Celeron/Intel Celeron M 530>) | 573 | 0 | community WPA22000 |
| [Intel Celeron N2920](<CPU/Intel/Celeron/Intel Celeron N2920>) | 1233 | 0 | community WPA22000 |
| [Intel Core 2 Duo T6500](<CPU/Intel/Core 2/Intel Core 2 Duo T6500>) | 1482 | 0 | community WPA22000 |
| [Intel Core 2 Duo T7600](<CPU/Intel/Core 2/Intel Core 2 Duo T7600>) | — | 1 | 1 other card(s) |
| [Intel Core 2 Quad Q9550](<CPU/Intel/Core 2/Intel Core 2 Quad Q9550>) | 4119 | 0 | community WPA22000 |
| [Intel Core i3 10105](<CPU/Intel/Core i3/Intel Core i3 10105>) | 17958 | 0 | community WPA22000 |
| [Intel Core i3 12100](<CPU/Intel/Core i3/Intel Core i3 12100>) | 17756 | 0 | community WPA22000 |
| [Intel Core i3 540](<CPU/Intel/Core i3/Intel Core i3 540>) | 2153 | 0 | community WPA22000 |
| [Intel Core i3 CPU M350](<CPU/Intel/Core i3/Intel Core i3 CPU M350>) | 1003 | 0 | community WPA22000 |
| [Intel Core i3 M330](<CPU/Intel/Core i3/Intel Core i3 M330>) | 1681 | 0 | community WPA22000 |
| [Intel Core i3 M380](<CPU/Intel/Core i3/Intel Core i3 M380>) | 2017 | 0 | community WPA22000 |
| [Intel Core i3 U380](<CPU/Intel/Core i3/Intel Core i3 U380>) | 822 | 0 | community WPA22000 |
| [Intel Core i3-10100](<CPU/Intel/Core i3/Intel Core i3-10100>) | 17842 | 0 | community WPA22000 |
| [Intel Core i3-2100](<CPU/Intel/Core i3/Intel Core i3-2100>) | 2561 | 0 | community WPA22000 |
| [Intel Core i3-2120](<CPU/Intel/Core i3/Intel Core i3-2120>) | 2769 | 0 | community WPA22000 |
| [Intel Core i3-2328M](<CPU/Intel/Core i3/Intel Core i3-2328M>) | 1656 | 0 | community WPA22000 |
| [Intel Core i3-2330M](<CPU/Intel/Core i3/Intel Core i3-2330M>) | — | 1 | 1 other card(s) |
| [Intel Core i3-2348M](<CPU/Intel/Core i3/Intel Core i3-2348M>) | 1644 | 0 | community WPA22000 |
| [Intel Core i3-2350M](<CPU/Intel/Core i3/Intel Core i3-2350M>) | 1784 | 1 | 1 other card(s), community WPA22000 |
| [Intel Core i3-2367M](<CPU/Intel/Core i3/Intel Core i3-2367M>) | 923 | 0 | community WPA22000 |
| [Intel Core i3-2370M](<CPU/Intel/Core i3/Intel Core i3-2370M>) | 1977 | 0 | community WPA22000 |
| [Intel Core i3-3110M](<CPU/Intel/Core i3/Intel Core i3-3110M>) | 2151 | 0 | community WPA22000 |
| [Intel Core i3-3120M](<CPU/Intel/Core i3/Intel Core i3-3120M>) | 2289 | 0 | community WPA22000 |
| [Intel Core i3-3217U](<CPU/Intel/Core i3/Intel Core i3-3217U>) | 1458 | 0 | community WPA22000 |
| [Intel Core i3-3220](<CPU/Intel/Core i3/Intel Core i3-3220>) | 2976 | 0 | community WPA22000 |
| [Intel Core i3-3227U](<CPU/Intel/Core i3/Intel Core i3-3227U>) | 1682 | 0 | community WPA22000 |
| [Intel Core i3-3240](<CPU/Intel/Core i3/Intel Core i3-3240>) | 1552 | 0 | community WPA22000 |
| [Intel Core i3-4005U](<CPU/Intel/Core i3/Intel Core i3-4005U>) | 3454 | 0 | community WPA22000 |
| [Intel Core i3-4010U](<CPU/Intel/Core i3/Intel Core i3-4010U>) | 3477 | 0 | community WPA22000 |
| [Intel Core i3-4130](<CPU/Intel/Core i3/Intel Core i3-4130>) | 6896 | 1 | 1 other card(s), community WPA22000 |
| [Intel Core i3-4170](<CPU/Intel/Core i3/Intel Core i3-4170>) | 7154 | 0 | community WPA22000 |
| [Intel Core i3-550](<CPU/Intel/Core i3/Intel Core i3-550>) | — | 1 | 1 other card(s) |
| [Intel Core i3-6006U](<CPU/Intel/Core i3/Intel Core i3-6006U>) | 4308 | 0 | community WPA22000 |
| [Intel Core i3-7100](<CPU/Intel/Core i3/Intel Core i3-7100>) | 8526 | 0 | community WPA22000 |
| [Intel Core i3-9100F](<CPU/Intel/Core i3/Intel Core i3-9100F>) | 15870 | 0 | community WPA22000 |
| [Intel Core i5 8265U](<CPU/Intel/Core i5/Intel Core i5 8265U>) | 9328 | 0 | community WPA22000 |
| [Intel Core i5 M 480](<CPU/Intel/Core i5/Intel Core i5 M 480>) | Intel Core i5 M 480: 1011; Intel Corei5 M 480: 2139 | 0 | community WPA22000 |
| [Intel Core i5 M430](<CPU/Intel/Core i5/Intel Core i5 M430>) | 1795 | 0 | community WPA22000 |
| [Intel Core i5 M460](<CPU/Intel/Core i5/Intel Core i5 M460>) | 2068 | 0 | community WPA22000 |
| [Intel Core i5 M520](<CPU/Intel/Core i5/Intel Core i5 M520>) | 2121 | 0 | community WPA22000 |
| [Intel Core i5-10210U](<CPU/Intel/Core i5/Intel Core i5-10210U>) | 11818 | 0 | community WPA22000 |
| [Intel Core i5-10300H](<CPU/Intel/Core i5/Intel Core i5-10300H>) | — | 1 | 1 other card(s) |
| [Intel Core i5-11400H](<CPU/Intel/Core i5/Intel Core i5-11400H>) | 26951 | 0 | community WPA22000 |
| [Intel Core i5-1235U](<CPU/Intel/Core i5/Intel Core i5-1235U>) | 9615 | 0 | community WPA22000 |
| [Intel Core i5-12400F](<CPU/Intel/Core i5/Intel Core i5-12400F>) | 26424 | 0 | community WPA22000 |
| [Intel Core i5-1240P](<CPU/Intel/Core i5/Intel Core i5-1240P>) | — | 1 | 1 other card(s) |
| [Intel Core i5-13420H](<CPU/Intel/Core i5/Intel Core i5-13420H>) | — | 1 | 1 other card(s) |
| [Intel Core i5-2300](<CPU/Intel/Core i5/Intel Core i5-2300>) | 4379 | 0 | community WPA22000 |
| [Intel Core i5-2310](<CPU/Intel/Core i5/Intel Core i5-2310>) | 4739 | 0 | community WPA22000 |
| [Intel Core i5-2380P](<CPU/Intel/Core i5/Intel Core i5-2380P>) | 4636 | 0 | community WPA22000 |
| [Intel Core i5-2400](<CPU/Intel/Core i5/Intel Core i5-2400>) | 4928 | 0 | community WPA22000 |
| [Intel Core i5-2410M](<CPU/Intel/Core i5/Intel Core i5-2410M>) | 2103 | 0 | community WPA22000 |
| [Intel Core i5-2430M](<CPU/Intel/Core i5/Intel Core i5-2430M>) | 2299 | 0 | community WPA22000 |
| [Intel Core i5-2450M](<CPU/Intel/Core i5/Intel Core i5-2450M>) | 602 | 1 | 1 other card(s), community WPA22000 |
| [Intel Core i5-2520M](<CPU/Intel/Core i5/Intel Core i5-2520M>) | 2474 | 0 | community WPA22000 |
| [Intel Core i5-3210M](<CPU/Intel/Core i5/Intel Core i5-3210M>) | 2652 | 0 | community WPA22000 |
| [Intel Core i5-3230M](<CPU/Intel/Core i5/Intel Core i5-3230M>) | 1961 | 0 | community WPA22000 |
| [Intel Core i5-3337U](<CPU/Intel/Core i5/Intel Core i5-3337U>) | 2162 | 0 | community WPA22000 |
| [Intel Core i5-3470](<CPU/Intel/Core i5/Intel Core i5-3470>) | 5558 | 1 | 1 other card(s), community WPA22000 |
| [Intel Core i5-4200M](<CPU/Intel/Core i5/Intel Core i5-4200M>) | 6122 | 0 | community WPA22000 |
| [Intel Core i5-4200U](<CPU/Intel/Core i5/Intel Core i5-4200U>) | 4689 | 1 | 1 other card(s), community WPA22000 |
| [Intel Core i5-4210H](<CPU/Intel/Core i5/Intel Core i5-4210H>) | 5559 | 0 | community WPA22000 |
| [Intel Core i5-4210U](<CPU/Intel/Core i5/Intel Core i5-4210U>) | 4175 | 0 | community WPA22000 |
| [Intel Core i5-4250U](<CPU/Intel/Core i5/Intel Core i5-4250U>) | — | 1 | 1 other card(s) |
| [Intel Core i5-4300U](<CPU/Intel/Core i5/Intel Core i5-4300U>) | 5286 | 0 | community WPA22000 |
| [Intel Core i5-4430](<CPU/Intel/Core i5/Intel Core i5-4430>) | 11649 | 0 | community WPA22000 |
| [Intel Core i5-4440](<CPU/Intel/Core i5/Intel Core i5-4440>) | 11257 | 0 | community WPA22000 |
| [Intel Core i5-4570](<CPU/Intel/Core i5/Intel Core i5-4570>) | 13300 | 1 | 1 other card(s), community WPA22000 |
| [Intel Core i5-4590](<CPU/Intel/Core i5/Intel Core i5-4590>) | 13302 | 0 | community WPA22000 |
| [Intel Core i5-5250U](<CPU/Intel/Core i5/Intel Core i5-5250U>) | — | 1 | 1 other card(s) |
| [Intel Core i5-5287U](<CPU/Intel/Core i5/Intel Core i5-5287U>) | — | 1 | 1 other card(s) |
| [Intel Core i5-5300U](<CPU/Intel/Core i5/Intel Core i5-5300U>) | — | 1 | 1 other card(s) |
| [Intel Core i5-6300HQ](<CPU/Intel/Core i5/Intel Core i5-6300HQ>) | 10664 | 0 | community WPA22000 |
| [Intel Core i5-7200](<CPU/Intel/Core i5/Intel Core i5-7200>) | 5498 | 0 | community WPA22000 |
| [Intel Core i5-8250U](<CPU/Intel/Core i5/Intel Core i5-8250U>) | 7986 | 1 | 1 other card(s), community WPA22000 |
| [Intel Core i5-9400F](<CPU/Intel/Core i5/Intel Core i5-9400F>) | 20171 | 0 | community WPA22000 |
| [Intel Core i7 12700](<CPU/Intel/Core i7/Intel Core i7 12700>) | 46512 | 0 | community WPA22000 |
| [Intel Core i7 13700](<CPU/Intel/Core i7/Intel Core i7 13700>) | 57517 | 0 | community WPA22000 |
| [Intel Core i7 860](<CPU/Intel/Core i7/Intel Core i7 860>) | 4863 | 0 | community WPA22000 |
| [Intel Core i7 9700KF](<CPU/Intel/Core i7/Intel Core i7 9700KF>) | 35231 | 0 | community WPA22000 |
| [Intel Core i7 M 620](<CPU/Intel/Core i7/Intel Core i7 M 620>) | — | 1 | 1 other card(s) |
| [Intel Core i7 Q720](<CPU/Intel/Core i7/Intel Core i7 Q720>) | 1709 | 0 | community WPA22000 |
| [Intel Core i7-10700](<CPU/Intel/Core i7/Intel Core i7-10700>) | 29937 | 0 | community WPA22000 |
| [Intel Core i7-1165G7](<CPU/Intel/Core i7/Intel Core i7-1165G7>) | — | 1 | 1 other card(s) |
| [Intel Core i7-11800H](<CPU/Intel/Core i7/Intel Core i7-11800H>) | 31781 | 1 | community WPA22000; iVision mode 23410 aggregate |
| [Intel Core i7-14700K](<CPU/Intel/Core i7/Intel Core i7-14700K>) | — | 2 | 2 other card(s) |
| [Intel Core i7-2600K](<CPU/Intel/Core i7/Intel Core i7-2600K>) | 5636 | 1 | 1 other card(s), community WPA22000 |
| [Intel Core i7-2630QM](<CPU/Intel/Core i7/Intel Core i7-2630QM>) | 2953 | 0 | community WPA22000 |
| [Intel Core i7-2670QM](<CPU/Intel/Core i7/Intel Core i7-2670QM>) | 4414 | 1 | 1 other card(s), community WPA22000 |
| [Intel Core i7-2720QM](<CPU/Intel/Core i7/Intel Core i7-2720QM>) | 2705 | 1 | 1 other card(s), community WPA22000 |
| [Intel Core i7-2820QM](<CPU/Intel/Core i7/Intel Core i7-2820QM>) | — | 1 | 1 other card(s) |
| [Intel Core i7-3540M](<CPU/Intel/Core i7/Intel Core i7-3540M>) | 2633 | 0 | community WPA22000 |
| [Intel Core i7-3615QM](<CPU/Intel/Core i7/Intel Core i7-3615QM>) | — | 1 | 1 other card(s) |
| [Intel Core i7-3630QM](<CPU/Intel/Core i7/Intel Core i7-3630QM>) | 5291 | 0 | community WPA22000 |
| [Intel Core i7-3632QM](<CPU/Intel/Core i7/Intel Core i7-3632QM>) | 5232 | 1 | 1 other card(s), community WPA22000 |
| [Intel Core i7-3720QM](<CPU/Intel/Core i7/Intel Core i7-3720QM>) | 5735 | 0 | community WPA22000 |
| [Intel Core i7-3770](<CPU/Intel/Core i7/Intel Core i7-3770>) | 6821 | 0 | community WPA22000 |
| [Intel Core i7-3820](<CPU/Intel/Core i7/Intel Core i7-3820>) | 5421 | 0 | community WPA22000 |
| [Intel Core i7-3930K](<CPU/Intel/Core i7/Intel Core i7-3930K>) | 8003 | 0 | community WPA22000 |
| [Intel Core i7-4510U](<CPU/Intel/Core i7/Intel Core i7-4510U>) | 5569 | 0 | community WPA22000 |
| [Intel Core i7-4600U](<CPU/Intel/Core i7/Intel Core i7-4600U>) | — | 1 | 1 other card(s) |
| [Intel Core i7-4700HQ](<CPU/Intel/Core i7/Intel Core i7-4700HQ>) | 5993 | 0 | community WPA22000 |
| [Intel Core i7-4700MQ](<CPU/Intel/Core i7/Intel Core i7-4700MQ>) | 12813 | 0 | community WPA22000 |
| [Intel Core i7-4702MQ](<CPU/Intel/Core i7/Intel Core i7-4702MQ>) | 11658 | 0 | community WPA22000 |
| [Intel Core i7-4710HQ](<CPU/Intel/Core i7/Intel Core i7-4710HQ>) | 11160 | 0 | community WPA22000 |
| [Intel Core i7-4710MQ](<CPU/Intel/Core i7/Intel Core i7-4710MQ>) | 8010 | 0 | community WPA22000 |
| [Intel Core i7-4720HQ](<CPU/Intel/Core i7/Intel Core i7-4720HQ>) | 13764 | 0 | community WPA22000 |
| [Intel Core i7-4770](<CPU/Intel/Core i7/Intel Core i7-4770>) | — | 1 | 1 other card(s) |
| [Intel Core i7-4770K](<CPU/Intel/Core i7/Intel Core i7-4770K>) | 15425 | 1 | community WPA22000; PoCL/Intel mode 1000 partial raw |
| [Intel Core i7-4790K](<CPU/Intel/Core i7/Intel Core i7-4790K>) | 17870 | 0 | community WPA22000 |
| [Intel Core i7-4820K](<CPU/Intel/Core i7/Intel Core i7-4820K>) | 6461 | 0 | community WPA22000 |
| [Intel Core i7-4870HQ](<CPU/Intel/Core i7/Intel Core i7-4870HQ>) | — | 1 | 1 other card(s) |
| [Intel Core i7-4940MX](<CPU/Intel/Core i7/Intel Core i7-4940MX>) | — | 1 | 1 other card(s) |
| [Intel Core i7-5820K](<CPU/Intel/Core i7/Intel Core i7-5820K>) | 25451 | 0 | community WPA22000 |
| [Intel Core i7-5960X](<CPU/Intel/Core i7/Intel Core i7-5960X>) | — | 1 | 1 other card(s) |
| [Intel Core i7-6700K](<CPU/Intel/Core i7/Intel Core i7-6700K>) | 18544 | 1 | 1 other card(s), community WPA22000 |
| [Intel Core i7-7700HQ](<CPU/Intel/Core i7/Intel Core i7-7700HQ>) | 14341 | 0 | community WPA22000 |
| [Intel Core i7-7820HQ](<CPU/Intel/Core i7/Intel Core i7-7820HQ>) | 15250 | 0 | community WPA22000 |
| [Intel Core i7-8550U](<CPU/Intel/Core i7/Intel Core i7-8550U>) | — | 1 | 1 other card(s) |
| [Intel Core i7-8750H](<CPU/Intel/Core i7/Intel Core i7-8750H>) | 17685 | 0 | community WPA22000 |
| [Intel Core i7-9700K](<CPU/Intel/Core i7/Intel Core i7-9700K>) | — | 2 | 2 other card(s) |
| [Intel Core i7-9750H](<CPU/Intel/Core i7/Intel Core i7-9750H>) | 18615 | 0 | community WPA22000 |
| [Intel Core i9-10900F](<CPU/Intel/Core i9/Intel Core i9-10900F>) | — | 1 | published MD4 CPU-only speed; no raw |
| [Intel Core i9-11950H](<CPU/Intel/Core i9/Intel Core i9-11950H>) | — | 1 | 1 other card(s) |
| [Intel Core i9-7920X](<CPU/Intel/Core i9/Intel Core i9-7920X>) | — | 1 | 1 other card(s) |
| [Intel Core i9-9900KF](<CPU/Intel/Core i9/Intel Core i9-9900KF>) | — | 1 | 1 other card(s) |
| [Intel Core M-5Y10c](<CPU/Intel/Core M/Intel Core M-5Y10c>) | 4079 | 0 | community WPA22000 |
| [Intel Core2 6300](<CPU/Intel/Core 2/Intel Core2 6300>) | 1120 | 0 | community WPA22000 |
| [Intel Core2 Duo E4600](<CPU/Intel/Core 2/Intel Core2 Duo E4600>) | 1749 | 0 | community WPA22000 |
| [Intel Core2 Duo E7300](<CPU/Intel/Core 2/Intel Core2 Duo E7300>) | 1812 | 0 | community WPA22000 |
| [Intel Core2 Duo E7500](<CPU/Intel/Core 2/Intel Core2 Duo E7500>) | 2099 | 0 | community WPA22000 |
| [Intel Core2 Duo E8400](<CPU/Intel/Core 2/Intel Core2 Duo E8400>) | 1933 | 0 | community WPA22000 |
| [Intel Core2 Duo P7450](<CPU/Intel/Core 2/Intel Core2 Duo P7450>) | 1013 | 0 | community WPA22000 |
| [Intel Core2 Duo P8600](<CPU/Intel/Core 2/Intel Core2 Duo P8600>) | 1560 | 0 | community WPA22000 |
| [Intel Core2 Duo P9400](<CPU/Intel/Core 2/Intel Core2 Duo P9400>) | 1682 | 0 | community WPA22000 |
| [Intel Core2 Duo T5250](<CPU/Intel/Core 2/Intel Core2 Duo T5250>) | 1015 | 0 | community WPA22000 |
| [Intel Core2 Duo T5450](<CPU/Intel/Core 2/Intel Core2 Duo T5450>) | 1191 | 0 | community WPA22000 |
| [Intel Core2 Duo T5800](<CPU/Intel/Core 2/Intel Core2 Duo T5800>) | 1373 | 0 | community WPA22000 |
| [Intel Core2 Duo T6400](<CPU/Intel/Core 2/Intel Core2 Duo T6400>) | 1227 | 0 | community WPA22000 |
| [Intel Core2 Duo T6570](<CPU/Intel/Core 2/Intel Core2 Duo T6570>) | 1500 | 0 | community WPA22000 |
| [Intel Core2 Duo T6670](<CPU/Intel/Core 2/Intel Core2 Duo T6670>) | 1479 | 0 | community WPA22000 |
| [Intel Core2 Duo T7300](<CPU/Intel/Core 2/Intel Core2 Duo T7300>) | 1362 | 0 | community WPA22000 |
| [Intel Core2 Duo T7500](<CPU/Intel/Core 2/Intel Core2 Duo T7500>) | 1530 | 0 | community WPA22000 |
| [Intel Core2 Q9650](<CPU/Intel/Core 2/Intel Core2 Q9650>) | 4261 | 0 | community WPA22000 |
| [Intel Core2 Quad Q8300](<CPU/Intel/Core 2/Intel Core2 Quad Q8300>) | 4025 | 0 | community WPA22000 |
| [Intel Core2 Quad Q8400](<CPU/Intel/Core 2/Intel Core2 Quad Q8400>) | 3896 | 0 | community WPA22000 |
| [Intel Core2 Quad Q9400](<CPU/Intel/Core 2/Intel Core2 Quad Q9400>) | 3730 | 0 | community WPA22000 |
| [Intel Core2 Solo U3500](<CPU/Intel/Core 2/Intel Core2 Solo U3500>) | 502 | 0 | community WPA22000 |
| [Intel Core2 T5300](<CPU/Intel/Core 2/Intel Core2 T5300>) | 571 | 0 | community WPA22000 |
| [Intel Pentium 2020M](<CPU/Intel/Pentium/Intel Pentium 2020M>) | 2026 | 0 | community WPA22000 |
| [Intel Pentium 2117U](<CPU/Intel/Pentium/Intel Pentium 2117U>) | 1541 | 0 | community WPA22000 |
| [Intel Pentium 4](<CPU/Intel/Pentium/Intel Pentium 4>) | 352 | 0 | community WPA22000 |
| [Intel Pentium 4415U](<CPU/Intel/Pentium/Intel Pentium 4415U>) | 2202 | 0 | community WPA22000 |
| [Intel Pentium B950](<CPU/Intel/Pentium/Intel Pentium B950>) | 1610 | 0 | community WPA22000 |
| [Intel Pentium B960](<CPU/Intel/Pentium/Intel Pentium B960>) | 1629 | 0 | community WPA22000 |
| [Intel Pentium Dual E2160](<CPU/Intel/Pentium/Intel Pentium Dual E2160>) | 924 | 0 | community WPA22000 |
| [Intel Pentium G2030](<CPU/Intel/Pentium/Intel Pentium G2030>) | 2665 | 0 | community WPA22000 |
| [Intel Pentium G850](<CPU/Intel/Pentium/Intel Pentium G850>) | 2182 | 0 | community WPA22000 |
| [Intel Pentium M](<CPU/Intel/Pentium/Intel Pentium M>) | 92 | 0 | community WPA22000 |
| [Pentium N3530](<CPU/Intel/Pentium/Pentium N3530>) | — | 1 | WPA2 dictionary-attack paper; not `-b` |
| [Intel Pentium N3540](<CPU/Intel/Pentium/Intel Pentium N3540>) | 1673 | 0 | community WPA22000 |
| [Intel Pentium P6200](<CPU/Intel/Pentium/Intel Pentium P6200>) | 1529 | 0 | community WPA22000 |
| [Intel U7300](<CPU/Intel/Other Intel/Intel U7300>) | 958 | 0 | community WPA22000 |
| [Intel Xeon 5150](<CPU/Intel/Xeon/Intel Xeon 5150>) | 3852 | 0 | community WPA22000 |
| [Intel Xeon CPU E3-1230 v3](<CPU/Intel/Xeon/Intel Xeon CPU E3-1230 v3>) | 14397 | 0 | community WPA22000 |
| [Intel Xeon CPU E5-2650 v2](<CPU/Intel/Xeon/Intel Xeon CPU E5-2650 v2>) | 1137 | 0 | community WPA22000 |
| [Intel Xeon E3-1230 V2](<CPU/Intel/Xeon/Intel Xeon E3-1230 V2>) | 5626 | 0 | community WPA22000 |
| [Intel Xeon E3-1231 v3](<CPU/Intel/Xeon/Intel Xeon E3-1231 v3>) | 14652 | 0 | community WPA22000 |
| [Intel Xeon E3-1270 v3](<CPU/Intel/Xeon/Intel Xeon E3-1270 v3>) | 15188 | 0 | community WPA22000 |
| [Intel Xeon E3-1270 v5](<CPU/Intel/Xeon/Intel Xeon E3-1270 v5>) | — | 0 | PHCS summary |
| [Intel Xeon E3-1505M v6](<CPU/Intel/Xeon/Intel Xeon E3-1505M v6>) | 15547 | 0 | community WPA22000 |
| [Intel Xeon E5 1650 v2](<CPU/Intel/Xeon/Intel Xeon E5 1650 v2>) | 9911 | 0 | community WPA22000 |
| [Intel Xeon E5-2620 v3](<CPU/Intel/Xeon/Intel Xeon E5-2620 v3>) | — | 1 | 1 other card(s) |
| [Intel Xeon E5-2630 v3](<CPU/Intel/Xeon/Intel Xeon E5-2630 v3>) | — | 1 | 1 other card(s) |
| [Intel Xeon E5-2660](<CPU/Intel/Xeon/Intel Xeon E5-2660>) | 8798 | 0 | community WPA22000 |
| [Intel Xeon E5-2670 0](<CPU/Intel/Xeon/Intel Xeon E5-2670 0>) | — | 1 | 1 other card(s) |
| [Intel Xeon E5-2676 v3](<CPU/Intel/Xeon/Intel Xeon E5-2676 v3>) | — | 1 | 1 other card(s) |
| [Intel Xeon E5-2696 v3](<CPU/Intel/Xeon/Intel Xeon E5-2696 v3>) | 41355 | 0 | community WPA22000 |
| [Intel Xeon E5-2697 v2](<CPU/Intel/Xeon/Intel Xeon E5-2697 v2>) | — | 1 | 1 other card(s) |
| [Intel Xeon E5-4640](<CPU/Intel/Xeon/Intel Xeon E5-4640>) | — | 1 | 1 other card(s) |
| [Intel Xeon E5430](<CPU/Intel/Xeon/Intel Xeon E5430>) | 4499 | 0 | community WPA22000 |
| [Intel Xeon E7-4880 v2](<CPU/Intel/Xeon/Intel Xeon E7-4880 v2>) | — | 1 | 1 other card(s) |
| [Intel Xeon E7450](<CPU/Intel/Xeon/Intel Xeon E7450>) | — | 1 | 1 other card(s) |
| [Intel Xeon L5520](<CPU/Intel/Xeon/Intel Xeon L5520>) | 3484 | 0 | community WPA22000 |
| [Intel Xeon Platinum 8276L](<CPU/Intel/Xeon/Intel Xeon Platinum 8276L>) | 65940 | 0 | community WPA22000 |
| [Intel Xeon Silver 4116](<CPU/Intel/Xeon/Intel Xeon Silver 4116>) | — | 1 | 1 other card(s) |
| [Intel Xeon W-3223](<CPU/Intel/Xeon/Intel Xeon W-3223>) | — | 1 | 1 other card(s) |
| [Intel Xeon X5450](<CPU/Intel/Xeon/Intel Xeon X5450>) | 4382 | 0 | community WPA22000 |
| [Intel Xeon X5482](<CPU/Intel/Xeon/Intel Xeon X5482>) | — | 1 | 1 other card(s) |
| [Intel Xeon X5650](<CPU/Intel/Xeon/Intel Xeon X5650>) | 6579 | 0 | community WPA22000 |
| [Pentium Dual-Core CPU E5700](<CPU/Intel/Pentium/Pentium Dual-Core CPU E5700>) | 1981 | 0 | community WPA22000 |
| [Pentium Dual-Core E5300](<CPU/Intel/Pentium/Pentium Dual-Core E5300>) | 1899 | 0 | community WPA22000 |
| [Pentium Dual-Core E5800](<CPU/Intel/Pentium/Pentium Dual-Core E5800>) | 2346 | 0 | community WPA22000 |
| [Pentium Dual-Core E6600](<CPU/Intel/Pentium/Pentium Dual-Core E6600>) | 2226 | 0 | community WPA22000 |
| [Pentium Dual-Core T4200](<CPU/Intel/Pentium/Pentium Dual-Core T4200>) | 1408 | 0 | community WPA22000 |
| [Pentium Dual-Core T4400](<CPU/Intel/Pentium/Pentium Dual-Core T4400>) | 1545 | 0 | community WPA22000 |
| [Pentium Dual-Core T4500](<CPU/Intel/Pentium/Pentium Dual-Core T4500>) | 1462 | 0 | community WPA22000 |
<!-- FULL_CPU_INDEX_END -->

## Реестр покрытия

Полный список целей — **4240 моделей** — разобран по приоритетам в
[`CPU-ROSTER.md`](CPU-ROSTER.md). Исходный ранжированный список сохранён как есть
в [`CPU-RANKING.txt`](CPU-RANKING.txt) (`модель|ядра/потоки`, порядок = место в рейтинге).

| Тир | Кол-во | Стоит ли искать |
|---|---:|---|
| 🟢 A | 1142 | Да — EPYC, Ryzen, Xeon Scalable/6xxx/W, Core Ultra, Core 12–15 gen |
| 🟡 B | 158 | Точечно, по запросу |
| 🔴 C | 1200 | Маловероятно |
| ⚫ D | 1740 | Практически исключено |

## Важное отличие от GPU

Публичных прогонов `hashcat -b` на процессорах **существенно меньше**, чем на
видеокартах: hashcat на CPU гоняют редко и обычно попутно — когда GPU не
подхватился, — часто в одном-двух режимах. Поэтому по большому списку моделей
доля закрытых позиций будет заметно ниже, чем была по видеокартам.
Это не повод занижать планку: правило прежнее — **лучше пустая строка,
чем выдуманные цифры**.
