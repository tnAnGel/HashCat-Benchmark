# 🧠 Реестр процессоров — 4240 моделей

Полный ранжированный список из внешнего рейтинга (PassMark-подобный),
сохранён как есть в [`CPU-RANKING.txt`](CPU-RANKING.txt) — формат `модель|ядра/потоки`,
порядок = место в рейтинге. Этот файл — разбор того же списка по приоритетам поиска
публичного вывода `hashcat -b`.

**Всего моделей: 4240** · Intel: 2754 · AMD: 1486

Статус покрытия: ✅ в `CPU/` есть опубликованный raw-фрагмент; ⚠️ есть отдельная
карточка с публичным агрегатом, community comparison или официальным обработанным
отчётом без raw stdout. Community-таблицы без метода/версии — поисковая зацепка,
не независимая верификация;
⬜ подтверждённый бенчмарк пока не найден. Полнота и ограничения конкретного
прогона указаны в `CPU.md`, карточке или [`PUBLIC-AGGREGATES.md`](PUBLIC-AGGREGATES.md).

## Легенда приоритетов

| Тир | Кол-во | Что это | Стоит ли искать |
|---|---:|---|---|
| 🟢 A | 1142 | Топ рейтинга + все современные семейства (EPYC, Ryzen, Xeon Scalable/6xxx/W, Core Ultra, Core 12-15 gen) | **Да** — серверы часто без GPU, прогоны попадаются |
| 🟡 B | 158 | Прочее из верхней трети рейтинга, до ~2017 года | Точечно, по запросу |
| 🔴 C | 1200 | Средний слой: Core 2/i-1xx–i-4xxx, Phenom, FX, старые Xeon E5 v1–v2 | Маловероятно |
| ⚫ D | 1740 | Хвост: Pentium 4/III/II, K5–K6, Athlon 64, Atom, Celeron, Duron | Практически исключено |

**Почему хвост отсечён.** Дело не в возрасте, а в инструкциях: современный hashcat
собирается под SSE4.2/AVX и не запускается на до-Nehalem x86. Плюс CPU-прогоны в
принципе редки — hashcat на процессоре гоняют попутно, а не специально. Реальный фронт —
тир A (1142 моделей), и даже там ожидаемая доля находок невысока.

---

## 🟢 Тир A — искать — 1142 моделей

### AMD — 482

- ⬜ AMD Ryzen Threadripper PRO 9995WX · 96/192 · #1
- ⬜ AMD EPYC 9755 · 128/256 · #2
- ⬜ AMD EPYC 9965 · 192/384 · #3
- ⬜ AMD EPYC 9655P · 96/192 · #4
- ⬜ AMD EPYC 9655 · 96/192 · #5
- ⬜ AMD Ryzen Threadripper PRO 9985WX · 64/128 · #6
- ⬜ AMD EPYC 9845 · 160/320 · #7
- ⬜ AMD EPYC 9575F · 64/128 · #8
- ⬜ AMD Ryzen Threadripper 9980X · 64/128 · #9
- ⬜ AMD Ryzen Threadripper PRO 7995WX · 96/192 · #10
- ⬜ AMD EPYC 9555P · 64/128 · #11
- ⬜ AMD Ryzen Threadripper 7980X · 64/128 · #12
- ⬜ AMD EPYC 9565 · 72/144 · #13
- ⬜ AMD EPYC 9555 · 64/128 · #15
- ⬜ AMD Ryzen Threadripper PRO 7985WX · 64/128 · #16
- ⬜ AMD EPYC 9745 · 128/256 · #17
- ⬜ AMD EPYC 9J14 · 96/192 · #18
- ⬜ AMD EPYC 9B14 · 96/192 · #19
- ⬜ AMD EPYC 9475F · 48/96 · #20
- ⬜ AMD EPYC 9684X · 96/192 · #21
- ✅ AMD EPYC 9654 · 96/192 · #23
- ⬜ AMD EPYC 9V74 · 80/160 · #24
- ⬜ AMD EPYC 9654P · 96/192 · #25
- ⬜ AMD EPYC 9455P · 48/96 · #26
- ⬜ AMD EPYC 9D25 · 128/256 · #27
- ⬜ AMD EPYC 9455 · 48/96 · #28
- ⬜ AMD EPYC 9634 · 84/168 · #29
- ⬜ AMD Ryzen Threadripper 9970X · 32/64 · #30
- ⬜ AMD Ryzen Threadripper PRO 9975WX · 32/64 · #31
- ⬜ AMD EPYC 9554P · 64/128 · #33
- ⬜ AMD EPYC 9554 · 64/128 · #35
- ⬜ AMD EPYC 9734 · 112/224 · #36
- ⬜ AMD EPYC 9474F · 48/96 · #37
- ⬜ AMD Ryzen Threadripper 7970X · 32/64 · #39
- ✅ AMD EPYC 9754 · 128/256 · #40
- ⬜ AMD EPYC 9355P · 32/64 · #41
- ⬜ AMD Ryzen Threadripper PRO 7975WX · 32/64 · #43
- ⬜ AMD EPYC 9375F · 32/64 · #44
- ⬜ AMD Ryzen Threadripper PRO 5995WX · 64/128 · #45
- ⬜ AMD EPYC 9454P · 48/96 · #46
- ⬜ AMD Ryzen Threadripper PRO 9965WX · 24/48 · #49
- ⬜ AMD Ryzen Threadripper 9960X · 24/48 · #50
- ⬜ AMD EPYC 7773X · 64/128 · #52
- ⬜ AMD EPYC 9534 · 64/128 · #54
- ⬜ AMD EPYC 9454 · 48/96 · #56
- ⬜ AMD EPYC 9275F · 24/48 · #60
- ⬜ AMD EPYC 7763 · 64/128 · #61
- ⚠️ AMD Ryzen Threadripper 3990X · 64/128 · #62 (PHCS mode-0 MD5 summary; no local raw log)
- ⬜ AMD Ryzen Threadripper 7960X · 24/48 · #63
- ⬜ AMD Ryzen Threadripper PRO 3995WX · 64/128 · #64
- ⬜ AMD Ryzen Threadripper PRO 7965WX · 24/48 · #67
- ⬜ AMD EPYC 9374F · 32/64 · #68
- ⬜ AMD EPYC 7663 · 56/112 · #69
- ⬜ AMD EPYC 7V13 · 64/128 · #70
- ⬜ AMD EPYC 7713P · 64/128 · #71
- ⬜ AMD EPYC 7643P · 48/96 · #75
- ⬜ AMD EPYC 7643 · 48/96 · #77
- ⬜ AMD EPYC 7C13 · 64/128 · #78
- ⬜ AMD EPYC 9255 · 24/48 · #80
- ⬜ AMD Ryzen Threadripper PRO 5975WX · 32/64 · #81
- ⬜ AMD EPYC 9354P · 32/64 · #82
- ⬜ AMD EPYC 9274F · 24/48 · #83
- ⬜ AMD EPYC 9354 · 32/64 · #84
- ⬜ AMD EPYC 7662 · 64/128 · #87
- ⬜ AMD EPYC 9384X · 32/64 · #88
- ⬜ AMD EPYC 8534P · 64/128 · #89
- ⬜ AMD EPYC 7V12 · 64/128 · #91
- ⬜ AMD EPYC 7713 · 64/128 · #92
- ⬜ AMD Ryzen 9 9950X3D · 16/32 · #93
- ⬜ AMD EPYC 7H12 · 64/128 · #96
- ⬜ AMD EPYC 7573X · 32/64 · #97
- ⬜ AMD EPYC 4585PX · 16/32 · #98
- ⬜ AMD Ryzen Threadripper PRO 9955WX · 16/32 · #100
- ⬜ AMD Ryzen Threadripper PRO 5965WX · 24/48 · #104
- ⬜ AMD EPYC 7543P · 32/64 · #105
- ⬜ AMD EPYC 8434P · 48/96 · #106
- ⬜ AMD EPYC 9175F · 16/32 · #108
- ⚠️ [AMD Ryzen 9 9950X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 9950X>) · 16/32 · #109 — iVision v7.1.2 mode 23410 CPU/OpenCL aggregate, no raw stdout
- ⬜ AMD EPYC 9334 · 32/64 · #110
- ✅ AMD Ryzen Threadripper 3970X · 32/64 · #112
- ⬜ AMD Ryzen Threadripper PRO 3975WX · 32/64 · #113
- ⬜ AMD EPYC 75F3 · 32/64 · #114
- ⬜ AMD EPYC 4564P · 16/32 · #116
- ⬜ AMD EPYC 4565P · 16/32 · #118
- ⬜ AMD EPYC 9254 · 24/48 · #120
- ⬜ AMD Ryzen 9 9955HX3D · 16/32 · #128
- ⬜ AMD EPYC 7543 · 32/64 · #129
- ⬜ AMD EPYC 74F3 · 24/48 · #132
- ⬜ AMD EPYC 7742 · 64/128 · #139
- ⬜ AMD Ryzen Threadripper PRO 7955WX · 16/32 · #141
- ⬜ AMD EPYC 4584PX · 16/32 · #142
- ⬜ AMD EPYC 7702 · 64/128 · #143
- ⬜ AMD Ryzen 9 7950X · 16/32 · #146
- ⬜ AMD EPYC 7642 · 48/96 · #148
- ⬜ AMD EPYC 7473X · 24/48 · #149
- ⬜ AMD Ryzen 9 7950X3D · 16/32 · #154
- ⬜ AMD EPYC 7513 · 32/64 · #155
- ⬜ AMD Ryzen 9 7945X3D · 16/32 · #157
- ⬜ AMD Ryzen 9 7945HX3D · 16/32 · #160
- ⬜ AMD EPYC 9135 · 16/32 · #161
- ⬜ AMD EPYC 7552 · 48/96 · #162
- ⬜ AMD EPYC 8324P · 32/64 · #163
- ⬜ AMD EPYC 7443P · 24/48 · #165
- ⬜ AMD EPYC 7443 · 24/48 · #166
- ⬜ AMD Ryzen Threadripper PRO 9945WX · 12/24 · #168
- ⬜ AMD Ryzen 9 9900X3D · 12/24 · #170
- ⬜ AMD Ryzen 9 9955HX · 16/32 · #172
- ⬜ AMD Ryzen AI Max+ 395 · 16/32 · #173
- ⬜ AMD EPYC 7702P · 64/128 · #178
- ⚠️ [AMD Ryzen 9 9900X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 9900X>) · 12/24 · #179 — официальный Hashcat v7.0.0 NTLM >10 GH/s + Argon2 report, без raw stdout
- ⬜ AMD EPYC 4545P · 16/32 · #180
- ⬜ AMD Ryzen 9 7945HX · 16/32 · #184
- ⬜ AMD Ryzen 9 7940HX · 16/32 · #186
- ✅ AMD Ryzen Threadripper 3960X · 24/48 · #189
- ⬜ AMD EPYC 9174F · 16/32 · #191
- ⬜ AMD EPYC 7F72 · 24/48 · #192
- ⬜ AMD EPYC 7502 · 32/64 · #194
- ⬜ AMD Ryzen 9 8945HX · 16/32 · #195
- ⬜ AMD Ryzen 9 9850HX · 12/24 · #198
- ⬜ AMD Ryzen AI Max+ Pro 395 · 16/32 · #199
- ⬜ AMD EPYC 7502P · 32/64 · #201
- ⬜ AMD EPYC 7532 · 32/64 · #206
- ⬜ AMD EPYC 7413 · 24/48 · #207
- ⬜ AMD Ryzen 9 8940HX · 16/32 · #209
- ⬜ AMD EPYC 4484PX · 12/24 · #211
- ⬜ AMD Ryzen 9 7900X3D · 12/24 · #214
- ⬜ AMD EPYC 4465P · 12/24 · #215
- ⬜ AMD Ryzen Threadripper PRO 7945WX · 12/24 · #217
- ⬜ AMD EPYC 9224 · 24/48 · #219
- ⬜ AMD Ryzen Threadripper PRO 5955WX · 16/32 · #220
- ⬜ AMD Ryzen 9 PRO 9945 · 12/24 · #224
- ⬜ AMD EPYC 9115 · 16/32 · #225
- ⬜ AMD EPYC 7453 · 28/56 · #226
- ⬜ AMD Ryzen 9 7900 · 12/24 · #229
- ⬜ AMD EPYC 9184X · 16/32 · #230
- ⬜ AMD EPYC 4464P · 12/24 · #233
- ⬜ AMD Ryzen 9 PRO 7945 · 12/24 · #239
- ⬜ AMD Ryzen 9 7900X · 12/24 · #244
- ⬜ AMD EPYC 73F3 · 16/32 · #246
- ⬜ AMD EPYC 7402 · 24/48 · #247
- ⬜ AMD EPYC 7452 · 32/64 · #249
- ⬜ AMD EPYC 8224P · 24/48 · #250
- ⬜ AMD Ryzen 9 7845HX · 12/24 · #254
- ⚠️ AMD Ryzen 9 5900XT · 16/32 · #258
- ⚠️ AMD Ryzen 9 5950X · 16/32 · #260
- ⬜ AMD EPYC 9124 · 16/32 · #261
- ⬜ AMD EPYC 7343 · 16/32 · #262
- ⬜ AMD Ryzen 7 8840HX · 12/24 · #266
- ⬜ AMD Ryzen AI Max Pro 390 · 12/24 · #268
- ⬜ AMD Ryzen 7 7840HX · 12/24 · #270
- ⬜ AMD EPYC 7D12 · 32/64 · #274
- ⬜ AMD Ryzen AI Max 390 · 12/24 · #284
- ⬜ AMD EPYC 7F52 · 16/32 · #287
- ⬜ AMD EPYC 7313P · 16/32 · #293
- ⬜ AMD Ryzen Threadripper PRO 5945WX · 12/24 · #294
- ⬜ AMD Ryzen 7 9800X3D · 8/16 · #295
- ⬜ AMD Ryzen Threadripper PRO 3955WX · 16/32 · #296
- ⬜ AMD EPYC 7402P · 24/48 · #303
- ⬜ AMD EPYC 7542 · 32/64 · #305
- ⬜ AMD EPYC 7313 · 16/32 · #308
- ✅ AMD Ryzen 9 5900X · 12/24 · #322 (partial mode 15700)
- ⬜ AMD Ryzen 7 9700X · 8/16 · #325
- ⬜ AMD Ryzen 7 PRO 9745 · 8/16 · #326
- ⬜ AMD EPYC 7303P · 16/32 · #332
- ⬜ AMD EPYC 4345P · 8/16 · #333
- ⬜ AMD Ryzen 9 3950X · 16/32 · #334
- ⬜ AMD EPYC 8124P · 16/32 · #335
- ⬜ AMD Ryzen AI 9 HX 470 · 12/24 · #337
- ✅ AMD Ryzen 7 7700X · 8/16 · #342
- ⬜ AMD EPYC 7352 · 24/48 · #347
- ⬜ AMD Ryzen AI 9 HX 370 · 12/24 · #349
- ⬜ AMD EPYC 7601 · 32/64 · #350
- ⬜ AMD Ryzen AI 9 HX 375 · 12/24 · #352
- ⬜ AMD Ryzen 7 PRO 7745 · 8/16 · #355
- ⬜ AMD Ryzen 9 PRO 5945 · 12/24 · #359
- ⚠️ [AMD Ryzen 7 7700](<CPU/AMD/Ryzen 7/AMD Ryzen 7 7700>) · 8/16 · #362 — WPA2 dictionary-attack publication; not `hashcat -b`
- ⬜ AMD Ryzen 7 7800X3D · 8/16 · #364
- ⬜ AMD EPYC 4364P · 8/16 · #369
- ⬜ AMD Ryzen 9 5900 · 12/24 · #371
- ⬜ AMD EPYC 7302 · 16/32 · #375
- ⬜ AMD Ryzen Threadripper PRO 3945WX · 12/24 · #377
- ⬜ AMD EPYC 7551P · 32/64 · #378
- ⬜ AMD EPYC 4344P · 8/16 · #381
- ⬜ AMD Ryzen AI Max 385 · 8/16 · #384
- ⬜ AMD Ryzen Threadripper 2990WX · 32/64 · #386
- ⬜ AMD Ryzen 7 7745HX · 8/16 · #392
- ⬜ AMD Ryzen AI Max+ 388 · 8/16 · #403
- ⬜ AMD Ryzen 7 8700G · 8/16 · #405
- ⚠️ AMD Ryzen 9 3900XT · 12/24 · #407
- ⬜ AMD Ryzen 7 8745HX · 8/16 · #409
- ⬜ AMD Ryzen AI Max Pro 385 · 8/16 · #410
- ⬜ AMD Ryzen 5 PRO 9645 · 6/12 · #412
- ⬜ AMD Ryzen 9 PRO 3900 · 12/24 · #421
- ⬜ AMD EPYC 4245P · 6/12 · #423
- ⬜ AMD Ryzen 7 8700F · 8/16 · #424
- ⬜ AMD Ryzen 7 PRO 8700G · 8/16 · #425
- ⬜ AMD Ryzen Threadripper 2970WX · 24/48 · #430
- ⬜ AMD Ryzen 9 3900 · 12/24 · #432
- ⬜ AMD EPYC 9015 · 8/16 · #435
- ⬜ AMD Ryzen AI 9 365 · 10/20 · #437
- ⬜ AMD EPYC 7282 · 16/32 · #440
- ⬜ AMD Ryzen 9 8945H · 8/16 · #441
- ⬜ AMD Ryzen 5 9600X · 6/12 · #448
- ⬜ AMD EPYC 7302P · 16/32 · #449
- ⬜ AMD Ryzen 9 7940HS · 8/16 · #450
- ⬜ AMD Ryzen 9 8945HS · 8/16 · #457
- ⬜ AMD Ryzen 9 270 · 8/16 · #461
- ⬜ AMD Ryzen 7 8745H · 8/16 · #462
- ⬜ AMD Ryzen 5 9600 · 6/12 · #463
- ⬜ AMD Ryzen 9 7940H · 8/16 · #467
- ⬜ AMD Ryzen 7 8745HS · 8/16 · #474
- ⬜ AMD Ryzen Threadripper 2950X · 16/32 · #481
- ⬜ AMD EPYC 7571 · 32/64 · #482
- ⬜ AMD EPYC 7303 · 16/32 · #483
- ⚠️ AMD Ryzen 9 3900X · 12/24 · #484
- ⬜ AMD Ryzen 5 9500F · 6/12 · #486
- ⬜ AMD Ryzen 7 7840HS · 8/16 · #488
- ⬜ AMD Ryzen 7 8845HS · 8/16 · #490
- ⬜ AMD Ryzen 7 PRO 8700GE · 8/16 · #495
- ⬜ AMD Ryzen 5 7600X · 6/12 · #497
- ⬜ AMD Ryzen 7 5800X3D · 8/16 · #498
- ⬜ AMD Ryzen 7 260 · 8/16 · #501
- ⬜ AMD Ryzen 7 5800XT · 8/16 · #506
- ⬜ AMD Ryzen 7 PRO 8840H · 8/16 · #508
- ⬜ AMD EPYC 7401P · 24/48 · #514
- ⬜ AMD Ryzen 7 7840H · 8/16 · #515
- ⬜ AMD Ryzen 5 PRO 7645 · 6/12 · #522
- ⬜ AMD EPYC 7371 · 16/32 · #527
- ⬜ AMD Ryzen 9 PRO 7940HS · 8/16 · #528
- ⬜ AMD EPYC 72F3 · 8/16 · #531
- ⬜ AMD EPYC 4244P · 6/12 · #535
- ⬜ AMD Ryzen 5 7600 · 6/12 · #537
- ⬜ AMD Ryzen 7 8845H · 8/16 · #540
- ✅ AMD Ryzen Threadripper 1950X · 16/32 · #541
- ⬜ AMD Ryzen 7 PRO 8840HS · 8/16 · #544
- ✅ AMD Ryzen 7 5800X · 8/16 · #549
- ⬜ AMD Ryzen 5 7500F · 6/12 · #550
- ⬜ AMD Ryzen 7 5700X · 8/16 · #551
- ⬜ AMD Ryzen 7 5700X3D · 8/16 · #558
- ⬜ AMD Ryzen Z2 · 8/16 · #559
- ⬜ AMD Ryzen AI 7 PRO 450 · 8/16 · #563
- ⬜ AMD Ryzen 5 7645HX · 6/12 · #564
- ⬜ AMD Ryzen 7 PRO 5845 · 8/16 · #566
- ⬜ AMD EPYC 7551 · 32/64 · #568
- ⬜ AMD Ryzen 5 7600X3D · 6/12 · #570
- ⬜ AMD Ryzen 7 5800 · 8/16 · #572
- ⬜ AMD Ryzen 7 250 · 8/16 · #575
- ⬜ AMD Ryzen 5 7400F · 6/12 · #578
- ⬜ AMD Ryzen 5 PRO 8600G · 6/12 · #585
- ✅ AMD Ryzen 5 8600G · 6/12 · #587
- ⬜ AMD EPYC 7272 · 12/24 · #589
- ⬜ AMD Ryzen 5 7500X3D · 6/12 · #591
- ⬜ AMD Ryzen 7 8840HS · 8/16 · #592
- ⬜ AMD EPYC 7501 · 32/64 · #594
- ⬜ AMD Ryzen AI 7 350 · 8/16 · #595
- ⬜ AMD Ryzen Z2 Extreme · 8/16 · #597
- ⬜ AMD Ryzen Z1 Extreme · 8/16 · #603
- ⬜ AMD Ryzen 7 7840U · 8/16 · #609
- ⬜ AMD Ryzen 5 8400F · 6/12 · #610
- ⬜ AMD Ryzen 7 PRO 7840U · 8/16 · #612
- ⬜ AMD Ryzen AI Max Pro 380 · 6/12 · #613
- ⬜ AMD Ryzen 7 5700G · 8/16 · #619
- ⬜ AMD Ryzen Threadripper 2920X · 12/24 · #620
- ⬜ AMD Ryzen 9 6900HX · 8/16 · #626
- ⬜ AMD Ryzen 7 PRO 5750G · 8/16 · #627
- ⬜ AMD Ryzen 7 PRO 5755G · 8/16 · #628
- ⬜ AMD Ryzen 9 PRO 6950H · 8/16 · #629
- ⬜ AMD Ryzen 5 PRO 8600GE · 6/12 · #630
- ⬜ AMD Ryzen 7 7735H · 8/16 · #638
- ⬜ AMD Ryzen 7 8840U · 8/16 · #641
- ⬜ AMD Ryzen 7 PRO 6850H · 8/16 · #643
- ⬜ AMD EPYC 7451 · 24/48 · #646
- ⬜ AMD Ryzen 7 7840S · 8/16 · #648
- ⬜ AMD Ryzen 5 PRO 8645HS · 6/12 · #650
- ⬜ AMD Ryzen 9 5980HX · 8/16 · #652
- ⬜ AMD Ryzen 7 7435HS · 8/16 · #656
- ⬜ AMD Ryzen 5 240 · 6/12 · #657
- ⬜ AMD Ryzen 7 6800H · 8/16 · #659
- ⬜ AMD Ryzen 5 7640HS · 6/12 · #661
- ⬜ AMD Ryzen 5 PRO 7445 · 6/12 · #663
- ⬜ AMD Ryzen 7 7735HS · 8/16 · #666
- ⬜ AMD Ryzen 9 PRO 6950HS · 8/16 · #669
- ⬜ AMD EPYC 7351P · 16/32 · #670
- ⬜ AMD Ryzen 7 6800HS · 8/16 · #671
- ⬜ AMD Ryzen 7 3800XT · 8/16 · #673
- ⬜ AMD Ryzen AI Z2 Extreme · 8/16 · #679
- ⬜ AMD Ryzen Threadripper 1920X · 12/24 · #680
- ⬜ AMD Ryzen 7 3800X · 8/16 · #681
- ⬜ AMD Ryzen 7 PRO 6850HS · 8/16 · #686
- ⬜ AMD Ryzen 5 5600XT · 6/12 · #687
- ⬜ AMD Ryzen 5 8645HS · 6/12 · #690
- ⬜ AMD Ryzen 5 PRO 7640HS · 6/12 · #692
- ⬜ AMD Ryzen 9 5900HX · 8/16 · #694
- ⬜ AMD Ryzen AI 7 PRO 360 · 8/16 · #699
- ⬜ AMD EPYC 7203P · 8/16 · #701
- ⬜ AMD Ryzen 5 PRO 8500G · 6/12 · #702
- ⬜ AMD Ryzen 5 5600T · 6/12 · #705
- ⬜ AMD Ryzen 5 PRO 5645 · 6/12 · #706
- ⬜ AMD Ryzen 5 5600X3D · 6/12 · #709
- ⬜ AMD Ryzen 7 7736U · 8/16 · #712
- ✅ AMD Ryzen 7 3700X · 8/16 · #713
- ⬜ AMD Ryzen 5 PRO 8500GE · 6/12 · #716
- ⬜ AMD Ryzen 5 5600 · 6/12 · #717
- ⬜ AMD Ryzen 7 5700GE · 8/16 · #722
- ⬜ AMD Ryzen 5 8500G · 6/12 · #724
- ⬜ AMD Ryzen 7 PRO 250 · 8/16 · #727
- ⬜ AMD Ryzen 5 PRO 7640U · 6/12 · #736
- ⬜ AMD EPYC 7351 · 16/32 · #740
- ⬜ AMD Ryzen 5 8500GE · 6/12 · #742
- ⬜ AMD Ryzen 7 PRO 5750GE · 8/16 · #748
- ⬜ AMD Ryzen 5 5600X · 6/12 · #756
- ⬜ AMD Ryzen 7 PRO 5755GE · 8/16 · #758
- ⬜ AMD Ryzen 9 6900HS · 8/16 · #759
- ⬜ AMD Ryzen AI 7 455 · 6/12 · #763
- ⬜ AMD Ryzen 7 6800U · 8/16 · #764
- ⬜ AMD Ryzen 5 7640U · 6/12 · #766
- ⬜ AMD EPYC 7F32 · 8/16 · #767
- ⬜ AMD Ryzen 5 7400 · 6/12 · #775
- ⬜ AMD Ryzen 7 7735U · 8/16 · #777
- ⬜ AMD Ryzen 7 PRO 6850U · 8/16 · #778
- ⬜ AMD Ryzen 5 PRO 5650G · 6/12 · #780
- ⬜ AMD Ryzen 5 5500X3D · 6/12 · #781
- ⬜ AMD EPYC 8024P · 8/16 · #782
- ⬜ AMD Ryzen 5 5600GT · 6/12 · #786
- ⬜ AMD Ryzen 9 5980HS · 8/16 · #788
- ⬜ AMD Ryzen 5 7545U · 6/12 · #789
- ⬜ AMD Ryzen 7 4700G · 8/16 · #790
- ⬜ AMD Ryzen Embedded V3C48 · 8/16 · #793
- ⬜ AMD Ryzen 7 PRO 6860Z · 8/16 · #798
- ⬜ AMD Ryzen 5 8640U · 6/12 · #803
- ⬜ AMD Ryzen 5 230 · 6/12 · #805
- ⬜ AMD Ryzen 5 8640HS · 6/12 · #806
- ⬜ AMD Ryzen 5 PRO 220 · 6/12 · #807
- ⬜ AMD Ryzen 7 PRO 3700 · 8/16 · #812
- ⬜ AMD Ryzen 5 PRO 5655G · 6/12 · #815
- ⬜ AMD Ryzen 7 PRO 4700G · 8/16 · #817
- ⬜ AMD Ryzen 5 5600G · 6/12 · #818
- ⬜ AMD Ryzen 7 4700GE · 8/16 · #819
- ⬜ AMD Ryzen AI 5 340 · 6/12 · #820
- ⬜ AMD Ryzen 5 PRO 230 · 6/12 · #822
- ⬜ AMD Ryzen 7 PRO 4750G · 8/16 · #824
- ⬜ AMD EPYC 3451 · 16/32 · #827
- ⬜ AMD Ryzen 7 5800HS · 8/16 · #829
- ⬜ AMD Ryzen AI 5 PRO 340 · 6/12 · #832
- ⬜ AMD EPYC 7281 · 16/32 · #842
- ⬜ AMD Ryzen 7 5800H · 8/16 · #846
- ⬜ AMD Ryzen 9 5900HS · 8/16 · #849
- ⬜ AMD Ryzen 7 7445HS · 6/12 · #852
- ⬜ AMD Ryzen 5 5500GT · 6/12 · #860
- ⬜ AMD EPYC 7262 · 8/16 · #864
- ⬜ AMD Ryzen 9 4900H · 8/16 · #868
- ⬜ AMD Ryzen 5 PRO 7545U · 6/12 · #869
- ⬜ AMD Ryzen 5 220 · 6/12 · #870
- ⬜ AMD Ryzen 5 5600F · 6/12 · #871
- ⬜ AMD Ryzen 5 7540U · 6/12 · #873
- ⬜ AMD EPYC 7252 · 8/16 · #876
- ⬜ AMD Ryzen 7 Pro 7735U · 8/16 · #879
- ⬜ AMD Ryzen 5 6600H · 6/12 · #880
- ⬜ AMD Ryzen Embedded V2748 · 8/16 · #883
- ⬜ AMD Ryzen 5 5500 · 6/12 · #884
- ⬜ AMD Ryzen 7 PRO 4750GE · 8/16 · #886
- ⬜ AMD Ryzen 5 8540U · 6/12 · #887
- ⬜ AMD Ryzen 5 PRO 6650H · 6/12 · #890
- ⬜ AMD EPYC 4124P · 4/8 · #892
- ⬜ AMD Ryzen 7 PRO 7730U · 8/16 · #893
- ⬜ AMD Ryzen 5 PRO 5650GE · 6/12 · #895
- ⬜ AMD Ryzen 5 PRO 5655GE · 6/12 · #899
- ⬜ AMD Ryzen 5 5600GE · 6/12 · #902
- ⬜ AMD Ryzen 9 4900HS · 8/16 · #904
- ⬜ AMD Ryzen 5 PRO 215 · 6/12 · #906
- ⬜ AMD Ryzen 5 7535HS · 6/12 · #916
- ⬜ AMD Ryzen 5 3600XT · 6/12 · #917
- ⬜ AMD EPYC 7203 · 8/16 · #919
- ⬜ AMD EPYC 7232P · 8/16 · #920
- ⬜ AMD Ryzen 5 6600HS · 6/12 · #921
- ⚠️ [AMD Ryzen 7 4800H](<CPU/AMD/Ryzen 7/AMD Ryzen 7 4800H>) · 8/16 · #923 — WPA2 dictionary-attack publication; not `hashcat -b`
- ⬜ AMD Ryzen 5 PRO 7540U · 6/12 · #931
- ⬜ AMD Ryzen 5 3600X · 6/12 · #932
- ⬜ AMD Ryzen 7 4800HS · 8/16 · #939
- ⚠️ AMD Ryzen 7 5800U · 8/16 · #940
- ⬜ AMD Ryzen 5 4400G · 6/12 · #942
- ⬜ AMD Ryzen 7 4850U · 8/16 · #945
- ⬜ AMD Ryzen 7 2700X · 8/16 · #946
- ⬜ AMD Ryzen 7 PRO 2700X · 8/16 · #951
- ⬜ AMD Ryzen 5 6600U · 6/12 · #953
- ⬜ AMD Ryzen 5 7535U · 6/12 · #957
- ✅ AMD Ryzen 7 PRO 5850U · 8/16 · #960
- ⬜ AMD Ryzen 7 5825U · 8/16 · #969
- ⬜ AMD Ryzen 7 4800U · 8/16 · #977
- ⬜ AMD Ryzen Threadripper 1900X · 8/16 · #981
- ⬜ AMD Ryzen 7 7730U · 8/16 · #982
- ⬜ AMD Ryzen 7 Extreme Edition · 8/16 · #983
- ⬜ AMD Ryzen 5 PRO 6650U · 6/12 · #986
- ⬜ AMD Ryzen 5 PRO 4655G · 6/12 · #989
- ⬜ AMD Ryzen 5 Pro 7535U · 6/12 · #994
- ⬜ AMD Ryzen 5 PRO 4650G · 6/12 · #997
- ⬜ AMD Ryzen 5 4500 · 6/12 · #999
- ⬜ AMD Ryzen 5 4600G · 6/12 · #1001
- ⬜ AMD Ryzen 5 3600 · 6/12 · #1004
- ⬜ AMD Ryzen 5 4600GE · 6/12 · #1011
- ⬜ AMD Ryzen 5 7430U · 6/12 · #1012
- ⬜ AMD Ryzen Embedded V2718 · 8/16 · #1015
- ⬜ AMD Ryzen 7 PRO 5875U · 8/16 · #1026
- ⬜ AMD Ryzen 5 PRO 4650GE · 6/12 · #1033
- ⬜ AMD Ryzen 5 7530U · 6/12 · #1034
- ⬜ AMD Ryzen 5 7533HS · 6/12 · #1035
- ✅ AMD Ryzen 7 2700 · 8/16 · #1037
- ⬜ AMD Ryzen 5 5560U · 6/12 · #1038
- ⬜ AMD Ryzen 5 5600H · 6/12 · #1042
- ⬜ AMD Ryzen 7 5700U · 8/16 · #1045
- ⬜ AMD Ryzen 7 PRO 1700X · 8/16 · #1047
- ⬜ AMD Ryzen 5 PRO 4400GE · 6/12 · #1052
- ⬜ AMD Ryzen 7 1800X · 8/16 · #1053
- ⬜ AMD Ryzen 7 PRO 4750U · 8/16 · #1055
- ⬜ AMD Ryzen 7 2700E · 8/16 · #1059
- ⬜ AMD Ryzen 5 5625U · 6/12 · #1061
- ⬜ AMD Ryzen 7 5825C · 8/16 · #1066
- ⬜ AMD Ryzen 3 PRO 8300G · 4/8 · #1069
- ⬜ AMD Ryzen 3 PRO 8300GE · 4/8 · #1071
- ⬜ AMD Ryzen 5 4600HS · 6/12 · #1078
- ⬜ AMD Ryzen 5 5600U · 6/12 · #1081
- ✅ [AMD Ryzen 7 1700X](<CPU/AMD/Ryzen 7/AMD Ryzen 7 1700X>) · 8/16 · #1082 — CPU-only v3.40 raw `-D1 -b` added
- ⬜ AMD Ryzen 5 PRO 5650U · 6/12 · #1087
- ⬜ AMD Ryzen 5 PRO 5675U · 6/12 · #1089
- ⬜ AMD EPYC 7251 · 8/16 · #1090
- ⬜ AMD Ryzen 3 8300G · 4/8 · #1097
- ⬜ AMD Ryzen 5 7535H · 6/12 · #1098
- ⬜ AMD Ryzen 3 PRO 5355G · 4/8 · #1101
- ⬜ AMD Ryzen 5 PRO 7530U · 6/12 · #1102
- ⬜ AMD Ryzen 5 PRO 4655GE · 6/12 · #1103
- ⬜ AMD EPYC 7301 · 16/32 · #1104
- ⬜ AMD Ryzen AI 5 430 · 4/8 · #1111
- ⬜ AMD Ryzen Embedded V3C18I · 8/16 · #1114
- ⬜ AMD Ryzen 7 PRO 1700 · 8/16 · #1115
- ⬜ AMD Ryzen 3 PRO 5350G · 4/8 · #1116
- ✅ AMD Ryzen 5 4600H · 6/12 · #1120
- ⬜ AMD EPYC 3251 · 8/16 · #1123
- ⬜ AMD Ryzen 7 PRO 2700 · 8/16 · #1129
- ⬜ AMD Ryzen 3 8300GE · 4/8 · #1137
- ⬜ AMD Ryzen 9 5900H · 8/16 · #1143
- ⬜ AMD Ryzen 3 210 · 4/8 · #1144
- ⬜ AMD Ryzen 5 PRO 2600 · 6/12 · #1152
- ⬜ AMD Ryzen 7 1700 · 8/16 · #1157
- ⬜ AMD Ryzen Embedded V2516 · 6/12 · #1163
- ⚠️ AMD Ryzen 5 3500X · 6/6 · #1165
- ⬜ AMD Ryzen 3 7440U · 4/8 · #1170
- ⬜ AMD Ryzen 3 5300G · 4/8 · #1171
- ⬜ AMD Ryzen 5 4600U · 6/12 · #1172
- ⚠️ AMD Ryzen 5 2600X · 6/12 · #1173
- ⬜ AMD Ryzen 3 5300GE · 4/8 · #1183
- ⬜ AMD Ryzen 5 3500 · 6/6 · #1188
- ⬜ AMD Ryzen 3 PRO 5355GE · 4/8 · #1189
- ⬜ AMD Ryzen AI 5 330 · 4/8 · #1190
- ⬜ AMD Ryzen 5 2600 · 6/12 · #1191
- ⬜ AMD Ryzen 5 1600X · 6/12 · #1195
- ⬜ AMD Ryzen 7 4700U · 8/8 · #1198
- ⬜ AMD Ryzen 3 PRO 5350GE · 4/8 · #1199
- ⬜ AMD Ryzen 3 7335U · 4/8 · #1205
- ⬜ AMD Ryzen 3 PRO 7330U · 4/8 · #1209
- ⬜ AMD Ryzen 5 7235HS · 4/8 · #1210
- ⬜ AMD Ryzen 5 2600E · 6/12 · #1212
- ⬜ AMD Ryzen 5 5500U · 6/12 · #1213
- ⬜ AMD Ryzen 3 Pro 7335U · 4/8 · #1215
- ⬜ AMD Ryzen 3 PRO 210 · 4/8 · #1223
- ⬜ AMD Ryzen 5 PRO 4650U · 6/12 · #1228
- ⬜ AMD Ryzen 3 8440U · 4/8 · #1234
- ⬜ AMD Ryzen Embedded V3C14 · 4/8 · #1242
- ⬜ AMD Ryzen 3 3300X · 4/8 · #1243
- ⬜ AMD Ryzen Z2 Go · 4/8 · #1246
- ⬜ AMD Ryzen Embedded V2546 · 6/12 · #1251
- ⬜ AMD Ryzen 5 5500H · 4/8 · #1260
- ⬜ AMD Ryzen 5 PRO 1600 · 6/12 · #1267
- ⬜ AMD Ryzen 3 5425U · 4/8 · #1270
- ⬜ AMD Ryzen 3 4300GE · 4/8 · #1272
- ⚠️ [AMD Ryzen 5 1600](<CPU/AMD/Ryzen 5/AMD Ryzen 5 1600>) · 6/12 · #1277 — iVision v7.1.2 mode 23410 CPU/OpenCL aggregate, no raw stdout
- ⬜ AMD EPYC 7261 · 8/16 · #1282
- ⬜ AMD Ryzen 3 PRO 5475U · 4/8 · #1283
- ⬜ AMD Ryzen 3 4100 · 4/8 · #1286
- ⬜ AMD Ryzen 3 5400U · 4/8 · #1289
- ⬜ AMD Ryzen 3 PRO 4350GE · 4/8 · #1291
- ⬜ AMD Ryzen 3 PRO 4200GE · 4/8 · #1292
- ⬜ AMD Ryzen 3 PRO 4200G · 4/8 · #1299

### Intel — 660

- ⬜ Intel Xeon 6960P · 72/144 · #14
- ⬜ Intel Xeon 6781P · 80/160 · #22
- ⬜ Intel Xeon 6747P · 48/96 · #32
- ⬜ Intel Xeon 6741P · 48/96 · #34
- ⬜ Intel Xeon w9-3595X · 60/120 · #38
- ⬜ Intel Xeon Platinum 8570 · 56/112 · #42
- ⬜ Intel Xeon 6740P · 48/96 · #47
- ⬜ Intel Xeon Platinum 8470 · 52/104 · #48
- ⬜ Intel Xeon Platinum 8488C · 56/112 · #51
- ⬜ Intel Xeon 6780E · 144/144 · #53
- ⬜ Intel Xeon w9-3575X · 44/88 · #55
- ⬜ Intel Xeon Platinum 8592+ · 64/128 · #57
- ⬜ Intel Xeon Max 9480 · 56/112 · #58
- ⬜ Intel Xeon w9-3495X · 56/112 · #59
- ⬜ Intel Xeon Platinum 8568Y+ · 48/96 · #65
- ⬜ Intel Xeon 6737P · 32/64 · #66
- ⬜ Intel Xeon 6740E · 96/96 · #72
- ⬜ Intel Xeon Platinum 8461V · 48/96 · #73
- ⬜ Intel Xeon 6732P · 32/64 · #74
- ⬜ Intel Xeon 6730P · 32/64 · #76
- ⬜ Intel Xeon Gold 6548Y+ · 32/64 · #79
- ⬜ Intel Xeon w7-3565X · 32/64 · #85
- ⬜ Intel Xeon Gold 6448H · 32/64 · #86
- ⬜ Intel Xeon Platinum 8571N · 52/104 · #90
- ⬜ Intel Xeon w7-3555 · 28/56 · #94
- ⬜ Intel Core Ultra 9 285K · 24/24 · #95
- ⬜ Intel Xeon w7-2595X · 26/52 · #99
- ⬜ Intel Xeon w9-3475X · 36/72 · #101
- ⬜ Intel Xeon 6521P · 24/48 · #102
- ⬜ Intel Xeon Platinum 8469C · 48/96 · #103
- ⬜ Intel Xeon 6520P · 24/48 · #107
- ⬜ Intel Xeon Gold 6438Y+ · 32/64 · #111
- ⬜ Intel Xeon Platinum 8454H · 32/64 · #115
- ⬜ Intel Xeon Platinum 8380 · 40/80 · #117
- ⬜ Intel Xeon w7-3465X · 28/56 · #119
- ⬜ Intel Xeon 6710E · 64/64 · #121
- ⬜ Intel Xeon Gold 5520+ · 28/56 · #122
- ⬜ Intel Core i9-13900KS · 24/32 · #123
- ⬜ Intel Xeon Gold 6448Y · 32/64 · #124
- ⬜ Intel Xeon Gold 5512U · 28/56 · #125
- ⬜ Intel Core i9-14900KS · 24/32 · #126
- ⬜ Intel Xeon Gold 6542Y · 24/48 · #127
- ⬜ Intel Xeon W-3375 · 38/76 · #130
- ⬜ Intel Core Ultra 7 265K · 20/20 · #131
- ⬜ Intel Core Ultra 7 265KF · 20/20 · #133
- ⬜ Intel Xeon Gold 6442Y · 24/48 · #134
- ⬜ Intel Core i9-14900K · 24/32 · #135
- ⬜ Intel Xeon w7-3545 · 24/48 · #136
- ⬜ Intel Core i9-14900KF · 24/32 · #137
- ⬜ Intel Core i9-13900K · 24/32 · #138
- ⬜ Intel Xeon Gold 5420+ · 28/56 · #140
- ⬜ Intel Core i9-13900KF · 24/32 · #144
- ⬜ Intel Core Ultra 9 285HX · 24/24 · #145
- ⬜ Intel Xeon Gold 6423N · 28/56 · #147
- ⬜ Intel Core Ultra 9 285 · 24/24 · #150
- ⬜ Intel Xeon W-3365 · 32/64 · #151
- ⬜ Intel Xeon w7-2495X · 24/48 · #152
- ⬜ Intel Xeon Gold 6414U · 32/64 · #153
- ⬜ Intel Xeon Platinum 8362 · 32/64 · #156
- ⬜ Intel Xeon Platinum 8375C · 32/64 · #158
- ⬜ Intel Core Ultra 9 275HX · 24/24 · #159
- ⬜ Intel Xeon w7-3455 · 24/48 · #164
- ⬜ Intel Xeon w5-3535X · 20/40 · #167
- ⬜ Intel Xeon Platinum 8358 · 32/64 · #169
- ⬜ Intel Xeon Platinum 8360Y · 36/72 · #171
- ⬜ Intel Xeon w7-2475X · 20/40 · #174
- ⬜ Intel Xeon Gold 6430 · 32/64 · #175
- ⬜ Intel Xeon w7-2575X · 22/44 · #176
- ⬜ Intel Xeon Gold 6438N · 32/64 · #177
- ⬜ Intel Xeon w5-2565X · 18/36 · #181
- ⬜ Intel Core i7-14700KF · 20/28 · #182
- ⚠️ [Intel Core i7-14700K](<CPU/Intel/Core i7/Intel Core i7-14700K>) · 20/28 · #183 — Hashcat v7.0.0 Argon2 и v8.0.0 Python Bridge SHA-256; без raw stdout
- ⬜ Intel Xeon Gold 6348 · 28/56 · #185
- ⬜ Intel Xeon Gold 6418H · 24/48 · #187
- ⬜ Intel Xeon Gold 5412U · 24/48 · #188
- ⬜ Intel Xeon Gold 6544Y · 16/32 · #190
- ⬜ Intel Xeon Gold 6554S · 36/72 · #193
- ⬜ Intel Xeon Platinum 8562Y+ · 32/64 · #196
- ⬜ Intel Xeon 6736P · 36/72 · #197
- ⬜ Intel Core Ultra 7 265 · 20/20 · #200
- ⬜ Intel Core Ultra 7 265F · 20/20 · #202
- ⬜ Intel Xeon Platinum 8347C · 36/72 · #203
- ⬜ Intel Core Ultra 7 255HX · 20/20 · #204
- ⬜ Intel Xeon w5-3525 · 16/32 · #205
- ⬜ Intel Xeon w7-3445 · 20/40 · #208
- ⬜ Intel Xeon Gold 6314U · 32/64 · #210
- ⬜ Intel Core Ultra 7 265HX · 20/20 · #212
- ⬜ Intel Core i9-13900F · 24/32 · #213
- ⬜ Intel Xeon W-3345 · 24/48 · #216
- ⬜ Intel Xeon w5-2555X · 14/28 · #218
- ⬜ Intel Xeon 6517P · 16/32 · #221
- ⬜ Intel Xeon Gold 6444Y · 16/32 · #222
- ⬜ Intel Xeon Gold 6342 · 24/48 · #223
- ⬜ Intel Core i9-14900F · 24/32 · #227
- ⬜ Intel Xeon Platinum 8368Q · 38/76 · #228
- ⬜ Intel Xeon Gold 6530 · 32/64 · #231
- ⬜ Intel Core i9-13980HX · 24/32 · #232
- ⚠️ Intel Core i7-13700K · 16/24 · #234
- ⚠️ Intel Core i7-13700KF · 16/24 · #235
- ⬜ Intel Xeon 6511P · 16/32 · #236
- ⬜ Intel Xeon Gold 5418Y · 24/48 · #237
- ⬜ Intel Xeon Gold 6336Y · 24/48 · #238
- ⬜ Intel Xeon w5-2465X · 16/32 · #240
- ⬜ Intel Core i9-14900 · 24/32 · #241
- ⬜ Intel Core i9-13900 · 24/32 · #242
- ⬜ Intel Xeon Gold 6538N · 32/64 · #243
- ⬜ Intel Xeon w5-3435X · 16/32 · #245
- ⬜ Intel Core i9-14900HX · 24/32 · #248
- ⬜ Intel Xeon Silver 4416+ · 20/40 · #251
- ⬜ Intel Core i9-12900KS · 16/24 · #252
- ⬜ Intel Core Ultra 5 245K · 14/14 · #253
- ⬜ Intel Core Ultra 5 245KF · 14/14 · #255
- ⬜ Intel Xeon Gold 6526Y · 16/32 · #256
- ⬜ Intel Xeon W-3175X · 28/56 · #257
- ⬜ Intel Core i9-13900T · 24/32 · #259
- ⬜ Intel Core i7-13790F · 16/24 · #263
- ⬜ Intel Xeon Gold 6338N · 32/64 · #264
- ⬜ Intel Xeon Gold 6330 · 28/56 · #265
- ⬜ Intel Xeon Gold 6312U · 18/36 · #267
- ⬜ Intel Core i7-14700F · 20/28 · #269
- ⬜ Intel Core i9-12900K · 16/24 · #271
- ⬜ Intel Core i7-14790F · 16/24 · #272
- ⬜ Intel Core i9-13950HX · 24/32 · #273
- ⬜ Intel Core i7-14700 · 20/28 · #275
- ⬜ Intel Xeon Platinum 8275CL · 24/48 · #276
- ⬜ Intel Xeon w5-2545 · 12/24 · #277
- ⬜ Intel Core i9-12900KF · 16/24 · #278
- ⬜ Intel Xeon 6515P · 16/32 · #279
- ⬜ Intel Xeon Gold 6416H · 18/36 · #280
- ⬜ Intel Core i9-13900E · 24/32 · #281
- ⬜ Intel Core Ultra 5 245HX · 14/14 · #282
- ⬜ Intel Xeon Gold 6338 · 32/64 · #283
- ⬜ Intel Core Ultra 5 235HX · 14/14 · #285
- ⬜ Intel Core Ultra 5 235 · 14/14 · #286
- ⬜ Intel Core Ultra 7 265T · 20/20 · #288
- ⬜ Intel Core Ultra 5 245 · 14/14 · #289
- ⬜ Intel Xeon W-3275 · 28/56 · #290
- ⬜ Intel Xeon 6505P · 12/24 · #291
- ⬜ Intel Xeon W-3335 · 38/76 · #292
- ⬜ Intel Core i5-14600KF · 14/20 · #297
- ⬜ Intel Core i5-14600K · 14/20 · #298
- ⬜ Intel Core i9-14900T · 24/32 · #299
- ⬜ Intel Core i9-13900HX · 24/32 · #300
- ⬜ Intel Xeon Gold 6354 · 18/36 · #301
- ⚠️ Intel Core i7-13700F · 16/24 · #302
- ⬜ Intel Core Ultra X9 388H · 16/16 · #304
- ⬜ Intel Xeon Gold 6258R · 28/56 · #306
- ⬜ Intel Xeon Gold 6346 · 16/32 · #307
- ⬜ Intel Xeon Platinum 8280M · 28/56 · #309
- ⬜ Intel Core i5-13600K · 14/20 · #310
- ⬜ Intel Xeon Gold 5320 · 26/52 · #311
- ⬜ Intel Core i5-13600KF · 14/20 · #312
- ⬜ Intel Xeon Platinum 8273CL · 28/56 · #313
- ⬜ Intel Xeon W-3275M · 28/56 · #314
- ⬜ Intel Xeon w5-2455X · 12/24 · #315
- ⬜ Intel Core i7-14700HX · 20/28 · #316
- ⬜ Intel Xeon Platinum 8280 · 28/56 · #317
- ⬜ Intel Core i7-13850HX · 20/28 · #318
- ⬜ Intel Core Ultra 9 285T · 24/24 · #319
- ⬜ Intel Xeon Gold 6330N · 28/56 · #320
- ⬜ Intel Xeon w5-3425 · 12/24 · #321
- ⚠️ Intel Core i7-13700 · 16/24 · #323
- ⬜ Intel Xeon Gold 6242R · 20/40 · #324
- ⬜ Intel Core i9-12900F · 16/24 · #327
- ⬜ Intel Xeon Gold 6338T · 24/48 · #328
- ⬜ Intel Xeon Platinum 8268 · 24/48 · #329
- ⬜ Intel Xeon Gold 5416S · 16/32 · #330
- ⬜ Intel Xeon Gold 6248R · 24/48 · #331
- ⬜ Intel Core Ultra 7 356H · 16/16 · #336
- ⬜ Intel Xeon Gold 6238R · 28/56 · #338
- ⬜ Intel Core Ultra 7 265H · 16/16 · #339
- ⬜ Intel Xeon Platinum 8260M · 24/48 · #340
- ⬜ Intel Xeon Gold 6268CL · 24/48 · #341
- ⬜ Intel Core Ultra 9 285H · 16/16 · #343
- ⬜ Intel Core Ultra 7 366H · 16/16 · #344
- ⚠️ Intel Core i7-12700K · 12/20 · #345
- ⬜ Intel Core i7-14650HX · 16/24 · #346
- ⚠️ Intel Core i7-12700KF · 12/20 · #348
- ⚠️ Intel Core i7-13700E · 16/24 · #351
- ⬜ Intel Xeon D-2799 · 20/40 · #353
- ⬜ Intel Xeon Gold 6326 · 16/32 · #354
- ⬜ Intel Core i9-12900 · 16/24 · #356
- ⬜ Intel Xeon Platinum 8270 · 26/52 · #357
- ⬜ Intel Xeon Platinum 8180 · 28/56 · #358
- ⬜ Intel Xeon w3-2535 · 10/20 · #360
- ⬜ Intel Xeon Gold 6240R · 24/48 · #361
- ⬜ Intel Core Ultra 5 230F · 10/10 · #363
- ⬜ Intel Xeon Gold 5318Y · 24/48 · #365
- ⬜ Intel Xeon W-3265M · 24/48 · #366
- ⬜ Intel Xeon w5-3433 · 16/32 · #367
- ⬜ Intel Core i9-12900HX · 16/24 · #368
- ⬜ Intel Xeon Platinum 8180M · 28/56 · #370
- ⬜ Intel Xeon Gold 6278C · 26/58 · #372
- ⬜ Intel Xeon Gold 6230R · 26/52 · #373
- ⬜ Intel Xeon Gold 6254 · 18/36 · #374
- ⬜ Intel Core Ultra X7 368H · 16/16 · #376
- ⬜ Intel Core i5-14600 · 14/20 · #379
- ⬜ Intel Xeon Silver 4510 · 12/24 · #380
- ⬜ Intel Xeon w5-2445 · 10/20 · #382
- ⬜ Intel Core Ultra 5 235T · 14/14 · #383
- ⚠️ Intel Core i7-13700HX · 16/24 · #385
- ⬜ Intel Xeon Gold 5320H · 20/40 · #387
- ⬜ Intel Core Ultra X7 358H · 16/16 · #388
- ⬜ Intel Core i9-10980XE · 18/36 · #389
- ⬜ Intel Xeon E-2488 · 8/16 · #390
- ⬜ Intel Core i5-13600 · 14/20 · #391
- ⬜ Intel Core i7-14700T · 20/28 · #393
- ⬜ Intel Core Ultra 5 225F · 10/10 · #394
- ⬜ Intel Core i9-12950HX · 16/24 · #395
- ⬜ Intel Xeon 6507P · 8/16 · #396
- ⬜ Intel Core i7-12800HX · 16/24 · #397
- ⬜ Intel Core i5-14500 · 14/20 · #398
- ⬜ Intel Core i5-13500 · 14/20 · #399
- ⬜ Intel Core Ultra 5 245T · 14/14 · #400
- ⬜ Intel Xeon Platinum 8168 · 24/48 · #401
- ⬜ Intel Core Ultra 7 255H · 16/16 · #402
- ⬜ Intel Core i7-12850HX · 16/24 · #408
- ⬜ Intel Core Ultra 5 338H · 12/12 · #411
- ⬜ Intel Xeon Gold 6246R · 16/32 · #413
- ⬜ Intel Xeon Platinum 8260 · 24/48 · #414
- ⬜ Intel Xeon 6357P · 8/16 · #415
- ⬜ Intel Core Ultra 5 225 · 10/10 · #416
- ⬜ Intel Xeon Gold 5220R · 24/48 · #417
- ⚠️ Intel Core i7-12700F · 12/20 · #418
- ⬜ Intel Core i9-14901E · 8/16 · #419
- ⬜ Intel Xeon Gold 5320T · 20/40 · #420
- ⬜ Intel Xeon 6369P · 8/16 · #422
- ⬜ Intel Xeon W-3265 · 24/48 · #426
- ⚠️ Intel Core i7-12700 · 12/20 · #427
- ⬜ Intel Xeon Silver 4316 · 20/40 · #428
- ⬜ Intel Xeon Gold 6534 · 8/16 · #429
- ⬜ Intel Core i9-13905H · 14/20 · #431
- ⬜ Intel Xeon Platinum 8171M · 26/52 · #433
- ⬜ Intel Xeon Gold 6248 · 20/40 · #434
- ⬜ Intel Core Ultra 5 235H · 14/14 · #436
- ⬜ Intel Core Ultra 9 185H · 16/22 · #438
- ⬜ Intel Xeon Gold 5318H · 18/36 · #439
- ⬜ Intel Core i9-12900T · 16/24 · #442
- ⬜ Intel Xeon Silver 4510T · 12/24 · #443
- ⬜ Intel Xeon Gold 6238 · 22/44 · #444
- ⬜ Intel Core 7 251TE · 24/32 · #445
- ⬜ Intel Xeon Gold 6266C · 22/44 · #446
- ⬜ Intel Xeon W-2295 · 18/36 · #447
- ⬜ Intel Xeon Silver 4314 · 16/32 · #451
- ⬜ Intel Xeon W-3245 · 16/32 · #453
- ⬜ Intel Core 9 270H · 14/20 · #454
- ⬜ Intel Core Ultra 5 225H · 14/14 · #456
- ⬜ Intel Xeon Gold 6253CL · 18/36 · #458
- ⬜ Intel Xeon w3-2525 · 8/16 · #459
- ⬜ Intel Xeon D-2795NT · 20/40 · #460
- ⬜ Intel Core i5-14500HX · 14/20 · #464
- ⚠️ Intel Core i7-12700E · 12/20 · #465
- ⬜ Intel Xeon Platinum 8175M · 24/48 · #466
- ⬜ Intel Xeon w5-3423 · 12/24 · #468
- ⬜ Intel Core i9-12900E · 16/24 · #469
- ⬜ Intel Xeon Platinum 8252C · 12/24 · #470
- ⬜ Intel Core i5-13600T · 14/20 · #471
- ⬜ Intel Xeon Gold 6434 · 8/16 · #472
- ⬜ Intel Xeon Platinum 8160 · 24/48 · #473
- ⬜ Intel Xeon Platinum 8173M · 28/56 · #475
- ⬜ Intel Xeon W-2195 · 18/36 · #476
- ⬜ Intel Xeon W-3323 · 12/24 · #477
- ⬜ Intel Xeon E-2478 · 8/16 · #478
- ⚠️ Intel Core i7-13700T · 16/24 · #479
- ⬜ Intel Core i5-14450HX · 10/16 · #480
- ⬜ Intel Core i5-12600K · 10/16 · #487
- ⬜ Intel Core i5-12600KF · 10/16 · #489
- ⬜ Intel Core i7-14701TE · 8/16 · #491
- ⬜ Intel Xeon Gold 5317 · 12/24 · #492
- ⬜ Intel Xeon Gold 6212U · 24/48 · #493
- ⬜ Intel Core i5-13600HX · 14/20 · #494
- ⬜ Intel Core i9-10940X · 14/28 · #496
- ⬜ Intel Core i9-13900H · 14/20 · #499
- ⬜ Intel Xeon D-2775TE · 16/32 · #500
- ⬜ Intel Xeon Silver 4410T · 10/20 · #502
- ⬜ Intel Core i5-14600T · 14/20 · #503
- ⬜ Intel Xeon Gold 6252 · 24/48 · #504
- ⬜ Intel Xeon Gold 6148 · 20/40 · #505
- ⬜ Intel Core i7-13650HX · 14/20 · #507
- ⬜ Intel Xeon W-2275 · 14/28 · #509
- ⬜ Intel Core i5-13400E · 10/16 · #511
- ⬜ Intel Core i9-13900HK · 14/20 · #512
- ⬜ Intel Core i9-12900H · 14/20 · #513
- ⬜ Intel Core i5-13400EF · 10/16 · #516
- ⬜ Intel Xeon Gold 6150 · 18/36 · #517
- ⬜ Intel Core i5-14490F · 10/16 · #519
- ⬜ Intel Xeon Gold 6210U · 20/40 · #521
- ⬜ Intel Xeon W-3245M · 16/32 · #523
- ⬜ Intel Xeon E-2468 · 8/16 · #524
- ⬜ Intel Core i5-13490F · 10/16 · #525
- ⬜ Intel Xeon W-2191B · 18/36 · #526
- ⬜ Intel Xeon 6353P · 8/16 · #529
- ⬜ Intel Core i7-13800H · 14/20 · #530
- ⬜ Intel Xeon Gold 6226R · 16/32 · #532
- ⬜ Intel Xeon D-2796TE · 20/40 · #533
- ⬜ Intel Core Ultra 5 225T · 10/10 · #534
- ⬜ Intel Core i5-13500HX · 14/20 · #536
- ⚠️ Intel Core i7-13700H · 14/20 · #538
- ⬜ Intel Core i7-12800HE · 14/20 · #539
- ⬜ Intel Core i7-14701E · 8/16 · #542
- ⬜ Intel Xeon w3-2435 · 8/16 · #543
- ⬜ Intel Xeon 6349P · 6/12 · #545
- ⬜ Intel Xeon Gold 6240 · 18/36 · #546
- ⬜ Intel Core Ultra 7 165H · 16/22 · #547
- ⬜ Intel Xeon Gold 6154 · 18/36 · #548
- ⬜ Intel Core i5-13500E · 14/20 · #552
- ⬜ Intel Core 7 250H · 14/20 · #553
- ⬜ Intel Core i7-13705H · 14/20 · #554
- ⬜ Intel Core i5-14400F · 10/16 · #555
- ⬜ Intel Xeon W-3235 · 12/24 · #557
- ⬜ Intel Xeon Gold 6152 · 22/44 · #560
- ⬜ Intel Xeon Gold 6256 · 12/24 · #561
- ⚠️ Intel Core i7-12700H · 14/20 · #562
- ⬜ Intel Core i5-14400 · 10/16 · #565
- ⬜ Intel Core i5-13400F · 10/16 · #567
- ⬜ Intel Xeon Silver 4410Y · 12/24 · #569
- ⬜ Intel Xeon W-2265 · 12/24 · #571
- ⬜ Intel Core i5-13450HX · 10/16 · #574
- ⬜ Intel Xeon Gold 6143 · 16/32 · #576
- ⬜ Intel Xeon Platinum 8167M · 26/52 · #577
- ⬜ Intel Core i9-10920X · 12/24 · #579
- ⬜ Intel Core 7 240H · 10/16 · #580
- ⬜ Intel Xeon Gold 6138 · 20/40 · #582
- ⬜ Intel Xeon Gold 5220 · 18/36 · #583
- ⬜ Intel Xeon Gold 6208U · 16/32 · #584
- ⬜ Intel Xeon W-2170B · 14/28 · #586
- ⬜ Intel Xeon Gold 6140 · 18/36 · #588
- ⬜ Intel Xeon Gold 6222V · 20/40 · #590
- ⬜ Intel Core i5-12600HX · 12/16 · #593
- ⬜ Intel Core i9-12900TE · 16/24 · #596
- ⬜ Intel Xeon D-2766NT · 14/28 · #598
- ⬜ Intel Core i9-11900K · 8/16 · #599
- ⬜ Intel Core 5 211EF · 10/16 · #600
- ⬜ Intel Core i7-12800H · 14/20 · #601
- ⬜ Intel Xeon Gold 6230 · 20/40 · #604
- ⬜ Intel Core i5-13400 · 10/16 · #605
- ⬜ Intel Xeon Gold 6122 · 20/40 · #606
- ⬜ Intel Core i7-11700K · 8/16 · #607
- ⬜ Intel Core i7-13620H · 10/16 · #614
- ⬜ Intel Core i5-12600HL · 12/16 · #615
- ⬜ Intel Xeon E-2486 · 6/12 · #616
- ⬜ Intel Xeon Platinum 8176 · 28/56 · #617
- ⬜ Intel Xeon E-2388G · 8/16 · #618
- ⬜ Intel Core i5-13600HE · 12/16 · #622
- ⬜ Intel Core i9-11900KF · 8/16 · #623
- ⬜ Intel Core i5-12500HL · 12/16 · #624
- ⬜ Intel Core i9-12900HK · 14/20 · #625
- ⬜ Intel Core i5-13600H · 12/16 · #631
- ⬜ Intel Core i5-14500T · 14/20 · #634
- ⬜ Intel Xeon Gold 5218R · 20/40 · #635
- ⬜ Intel Core i7-12650HX · 14/20 · #636
- ⬜ Intel Core i5-12600HE · 12/16 · #637
- ⬜ Intel Core i9-11900KB · 8/16 · #639
- ⬜ Intel Xeon Platinum 8124M · 18/36 · #640
- ⬜ Intel Xeon Gold 6142 · 16/32 · #642
- ⬜ Intel Core i5-13500T · 14/20 · #644
- ⬜ Intel Core i7-11700KF · 8/16 · #645
- ⬜ Intel Xeon Gold 6242 · 16/32 · #649
- ⬜ Intel Core i9-11900 · 8/16 · #651
- ⬜ Intel Xeon Gold 6138T · 20/40 · #654
- ⬜ Intel Core Ultra 7 365 · 8/8 · #655
- ⬜ Intel Core i9-10900K · 10/20 · #658
- ⬜ Intel Xeon Platinum P-8124 · 18/36 · #660
- ⬜ Intel Core Ultra 5 135H · 14/18 · #662
- ⚠️ Intel Core i7-13700TE · 16/24 · #664
- ⬜ Intel Xeon Silver 4310 · 12/24 · #668
- ⬜ Intel Xeon Gold 6262 · 24/48 · #672
- ⬜ Intel Core i9-10850K · 10/20 · #674
- ⬜ Intel Xeon W-2175 · 14/28 · #675
- ⬜ Intel Xeon E-2436 · 6/12 · #676
- ⬜ Intel Core i9-10900X · 10/20 · #677
- ⬜ Intel Core i7-12650H · 10/16 · #678
- ⬜ Intel Core 5 120 · 6/12 · #682
- ⬜ Intel Core 5 220H · 12/16 · #685
- ⬜ Intel Core i7-11700B · 8/16 · #688
- ⬜ Intel Xeon W-2255 · 10/20 · #689
- ⬜ Intel Core 5 120F · 6/12 · #691
- ⬜ Intel Xeon Gold 5218T · 16/32 · #693
- ⬜ Intel Core i9-10910 · 10/20 · #695
- ⬜ Intel Core i5-12600 · 6/12 · #696
- ⬜ Intel Xeon Gold 6146 · 12/24 · #697
- ⬜ Intel Core i7-11850HE · 8/16 · #698
- ⬜ Intel Xeon Gold 6246 · 12/24 · #700
- ⬜ Intel Core i5-13500TE · 14/20 · #703
- ⚠️ Intel Core i7-12700T · 12/20 · #704
- ⬜ Intel Xeon E-2378G · 8/16 · #707
- ⬜ Intel Xeon Gold 6130 · 16/32 · #708
- ⬜ Intel Core i5-13500H · 12/16 · #710
- ⬜ Intel Core i9-11980HK · 8/16 · #714
- ⬜ Intel Xeon 6337P · 6/12 · #715
- ⬜ Intel Xeon Gold 6132 · 14/28 · #718
- ⬜ Intel Xeon Gold 6126T · 12/24 · #719
- ⬜ Intel Core i5-14400T · 10/16 · #720
- ⬜ Intel Core i9-10900KF · 10/20 · #721
- ⬜ Intel Core i5-12600H · 12/16 · #723
- ⬜ Intel Xeon E-2456 · 6/12 · #726
- ⬜ Intel Core Ultra 5 125H · 14/18 · #728
- ⬜ Intel Xeon 6333P · 6/12 · #729
- ⬜ Intel Xeon Gold 5218 · 16/32 · #730
- ⬜ Intel Core i7-11700 · 8/16 · #731
- ⬜ Intel Xeon Silver 4310T · 10/20 · #732
- ⬜ Intel Xeon D-2753NT · 12/24 · #733
- ⬜ Intel Xeon Gold 6226 · 12/24 · #734
- ⬜ Intel Core i5-12650HX · 14/20 · #735
- ✅ Intel Core i9-11950H · 8/16 · #737
- ⬜ Intel Xeon Gold 6250 · 8/16 · #738
- ⬜ Intel Xeon Gold 6334 · 8/16 · #739
- ⬜ Intel Xeon Gold 5315Y · 8/16 · #741
- ⬜ Intel Core i9-11900F · 8/16 · #743
- ⬜ Intel Core i5-12500H · 12/16 · #745
- ⬜ Intel Core i5-12500E · 6/12 · #746
- ⬜ Intel Core i5-12490F · 6/12 · #747
- ⬜ Intel Core i3-12300HE · 8/12 · #751
- ⬜ Intel Core i3-12300HL · 8/12 · #752
- ⬜ Intel Core i5-13400T · 10/16 · #754
- ⬜ Intel Xeon D-1747NTE · 10/20 · #755
- ⬜ Intel Xeon Gold 6130T · 16/32 · #757
- ⬜ Intel Core Ultra 9 288V · 8/8 · #760
- ⬜ Intel Core i7-1280P · 14/20 · #762
- ⬜ Intel Core i7-1370P · 14/20 · #768
- ⬜ Intel Xeon W-2155B · 10/20 · #769
- ⬜ Intel Core i5-1350PRE · 12/16 · #770
- ⬜ Intel Core i9-11900H · 8/16 · #771
- ⬜ Intel Core i9-10900 · 10/20 · #772
- ⬜ Intel Core i7-13800HRE · 14/20 · #773
- ⬜ Intel Xeon Gold 6136 · 12/24 · #774
- ⬜ Intel Core i7-11850H · 8/16 · #776
- ⚠️ Intel Core i7-12700TE · 12/20 · #779
- ⬜ Intel Core i5-12500 · 6/12 · #783
- ⬜ Intel Core i7-11700F · 8/16 · #784
- ⬜ Intel Core Ultra 7 256V · 8/8 · #785
- ⚠️ Intel Core i5-12400F · 6/12 · #791
- ⬜ Intel Core Ultra 7 268V · 8/8 · #792
- ⬜ Intel Core i5-11600K · 6/12 · #794
- ⬜ Intel Core Ultra 5 335 · 8/8 · #795
- ⬜ Intel Xeon E-2386G · 6/12 · #796
- ⬜ Intel Core i5-11600KF · 6/12 · #797
- ⬜ Intel Xeon D-2183IT · 16/32 · #801
- ⬜ Intel Xeon Gold 6137 · 8/16 · #802
- ⬜ Intel Core Ultra 7 266V · 8/8 · #804
- ⬜ Intel Core i7-1370PRE · 14/20 · #809
- ⚠️ [Intel Core i9-10900F](<CPU/Intel/Core i9/Intel Core i9-10900F>) · 10/20 · #810 — published CPU-only MD4 speed, no raw stdout
- ⬜ Intel Xeon W-2155 · 10/20 · #811
- ⬜ Intel Core i9-10900E · 10/20 · #813
- ⬜ Intel Core i5-1250P · 12/16 · #814
- ⬜ Intel Xeon D-2752TER · 12/24 · #816
- ⬜ Intel Core Ultra 7 258V · 8/8 · #821
- ⬜ Intel Xeon W-2150B · 10/20 · #823
- ⚠️ Intel Core i7-10700KF · 8/16 · #825
- ⬜ Intel Xeon w3-2425 · 6/12 · #826
- ⚠️ [Intel Core i7-11800H](<CPU/Intel/Core i7/Intel Core i7-11800H>) · 8/16 · #830 — community WPA22000 + iVision mode 23410 aggregate
- ⬜ Intel Xeon Gold 6244 · 8/16 · #831
- ⬜ Intel Core i7-1360P · 12/16 · #833
- ⬜ Intel Core i5-12400 · 6/12 · #834
- ⬜ Intel Xeon Silver 4309Y · 8/16 · #835
- ⬜ Intel Core i5-1350P · 12/16 · #838
- ⬜ Intel Core i9-11900T · 8/16 · #840
- ⬜ Intel Core 5 210H · 8/12 · #845
- ⬜ Intel Core i5-1340PE · 12/16 · #847
- ⚠️ Intel Core i7-10700K · 8/16 · #850
- ⬜ Intel Xeon E-2356G · 6/12 · #851
- ⬜ Intel Xeon W-2245 · 8/16 · #853
- ⬜ Intel Xeon Silver 4216 · 16/32 · #854
- ⬜ Intel Core Ultra 5 225U · 12/14 · #855
- ⬜ Intel Core i5-1250PE · 12/16 · #856
- ⬜ Intel Xeon Silver 4509Y · 8/16 · #858
- ⬜ Intel Core Ultra 5 236V · 8/8 · #859
- ⬜ Intel Core Ultra 5 238V · 8/8 · #861
- ⬜ Intel Core i7-1265UL · 10/12 · #862
- ⬜ Intel Xeon W-3225 · 8/16 · #863
- ⬜ Intel Core Ultra 5 226V · 8/8 · #866
- ⬜ Intel Xeon D-2187NT · 16/32 · #872
- ⬜ Intel Core i5-11600 · 6/12 · #874
- ⬜ Intel Core i5-12450HX · 8/12 · #875
- ⬜ Intel Core i5-1340P · 12/16 · #878
- ⬜ Intel Core Ultra 7 255U · 12/14 · #881
- ⬜ Intel Core Ultra 7 265U · 12/14 · #882
- ⬜ Intel Xeon D-1736NT · 8/16 · #885
- ⬜ Intel Core i3-1320PRE · 8/12 · #889
- ⬜ Intel Core 3 100HL · 8/12 · #891
- ⬜ Intel Xeon Silver 4214R · 12/24 · #897
- ⬜ Intel Core i5-12600T · 6/12 · #903
- ⬜ Intel Core Ultra 5 228V · 8/8 · #905
- ⬜ Intel Core i7-1370PE · 14/20 · #907
- ⬜ Intel Core Ultra 5 235U · 12/14 · #908
- ⬜ Intel Xeon Gold 5120T · 14/28 · #910
- ⬜ Intel Xeon Gold 6234 · 8/16 · #913
- ⬜ Intel Xeon Gold 5120 · 14/28 · #914
- ⬜ Intel Xeon E-2378 · 8/16 · #918
- ✅ Intel Core i5-13420H · 8/12 · #922
- ⬜ Intel Core i5-11500B · 6/12 · #924
- ⬜ Intel Core i5-11500 · 6/12 · #925
- ⬜ Intel Core Ultra 5 125U · 12/14 · #926
- ⬜ Intel Xeon Gold 6126 · 12/24 · #928
- ⬜ Intel Xeon D-1848TER · 10/20 · #929
- ⬜ Intel Xeon E-2278G · 8/16 · #933
- ⬜ Intel Core Ultra 7 165U · 12/14 · #934
- ⬜ Intel Core Ultra 5 135U · 12/14 · #935
- ⬜ Intel Xeon W-2145 · 8/16 · #936
- ⬜ Intel Xeon Gold 6144 · 8/16 · #937
- ⬜ Intel Core i7-1270PE · 12/16 · #938
- ⬜ Intel Core i7-1270P · 12/16 · #941
- ⬜ Intel Core i7-1260P · 12/16 · #943
- ⬜ Intel Xeon E-2288G · 8/16 · #947
- ⚠️ Intel Core i7-10700 · 8/16 · #949
- ⬜ Intel Xeon Silver 4214Y · 12/24 · #950
- ⬜ Intel Xeon Silver 4214 · 12/24 · #952
- ✅ Intel Core i5-1240P · 12/16 · #954
- ⬜ Intel Xeon 6325P · 4/8 · #955
- ⬜ Intel Core i5-12500T · 6/12 · #956
- ⬜ Intel Xeon Gold 5215 · 10/20 · #958
- ⬜ Intel Xeon E-2336 · 6/12 · #962
- ⬜ Intel Xeon D-2733NT · 8/16 · #963
- ⬜ Intel Xeon W-2140B · 8/16 · #964
- ⬜ Intel Core i3-1220PE · 8/12 · #966
- ⬜ Intel Xeon Gold 5117 · 14/28 · #967
- ⚠️ Intel Core i7-10700E · 8/16 · #968
- ⬜ Intel Core i5-12450H · 8/12 · #970
- ⬜ Intel Core i5-11400F · 6/12 · #971
- ⬜ Intel Core 5 120U · 10/12 · #973
- ⬜ Intel Xeon E-2278GE · 8/16 · #975
- ⬜ Intel Xeon Gold 5118 · 12/24 · #978
- ✅ Intel Xeon W-3223 · 8/16 · #979
- ⬜ Intel Xeon w3-2423 · 6/12 · #980
- ⬜ Intel Xeon Silver 5217 · 8/16 · #984
- ⬜ Intel Xeon D-1746TER · 10/20 · #987
- ⬜ Intel Core Ultra 7 155U · 12/14 · #988
- ⬜ Intel Core i9-10900T · 10/20 · #990
- ⬜ Intel Core i5-11400 · 6/12 · #991
- ⬜ Intel Core i5-11500H · 6/12 · #992
- ⬜ Intel Core i5-12400T · 6/12 · #993
- ⚠️ Intel Core i7-10700F · 8/16 · #995
- ⬜ Intel Xeon D-1726 · 6/12 · #998
- ⬜ Intel Core Ultra 5 332 · 6/6 · #1000
- ⬜ Intel Core i7-11600H · 6/12 · #1002
- ⬜ Intel Core i5-12500TE · 6/12 · #1003
- ⬜ Intel Xeon Gold 5217 · 8/16 · #1005
- ⬜ Intel Xeon Gold 6134 · 8/16 · #1006
- ⬜ Intel Core i5-11260H · 6/12 · #1007
- ⬜ Intel Core i3-14100F · 4/8 · #1008
- ⬜ Intel Core i9-10980HK · 8/16 · #1009
- ⬜ Intel Core i5-1245UL · 10/12 · #1013
- ⬜ Intel Core i7-11700T · 8/16 · #1014
- ⚠️ Intel Core i5-11400H · 6/12 · #1016
- ⬜ Intel Xeon Silver 4210R · 10/20 · #1017
- ⬜ Intel Xeon Silver 4116T · 12/24 · #1018
- ⬜ Intel Core i3-14100 · 4/8 · #1019
- ⬜ Intel Xeon E-2286M · 8/16 · #1020
- ⬜ Intel Xeon D-2166NT · 12/24 · #1021
- ⬜ Intel Core 7 250U · 10/12 · #1022
- ⬜ Intel Xeon E-2434 · 4/8 · #1023
- ⬜ Intel Xeon Gold 5115 · 10/20 · #1024
- ✅ Intel Xeon Silver 4116 · 12/24 · #1027
- ⬜ Intel Core 7 150U · 10/12 · #1029
- ⬜ Intel Xeon D-1733NT · 8/16 · #1031
- ⬜ Intel Core i3-13100F · 4/8 · #1039
- ⬜ Intel Core i3-1220P · 10/12 · #1044
- ⬜ Intel Core i3-12300 · 4/8 · #1046
- ⬜ Intel Core i5-11600T · 6/12 · #1048
- ⬜ Intel Core 3 201E · 4/8 · #1049
- ⬜ Intel Core i7-10875H · 8/16 · #1054
- ⬜ Intel Core 5 220U · 10/12 · #1057
- ⬜ Intel Core i5-1345U · 10/12 · #1058
- ⬜ Intel Xeon D-1732TE · 8/16 · #1060
- ⬜ Intel Core i9-10900TE · 10/20 · #1062
- ⬜ Intel Core i7-1355U · 10/12 · #1065
- ⬜ Intel Core i3-13100 · 4/8 · #1068
- ⬜ Intel Core i7-10870H · 8/16 · #1070
- ⬜ Intel Core i9-10885H · 8/16 · #1072
- ⬜ Intel Core i5-1335U · 10/12 · #1073
- ⬜ Intel Core i5-10600K · 6/12 · #1074
- ⚠️ Intel Core i3-12100F · 4/8 · #1075
- ⬜ Intel Core i9-10880H · 8/16 · #1077
- ⬜ Intel Core i5-10600KF · 6/12 · #1079
- ⬜ Intel Core i7-1365U · 10/12 · #1080
- ⬜ Intel Core i5-1240U · 10/12 · #1083
- ⬜ Intel Xeon W-2235 · 6/12 · #1084
- ⬜ Intel Core i3-13100E · 4/8 · #1085
- ⬜ Intel Xeon E-2374G · 4/8 · #1086
- ⬜ Intel Xeon D-1823NT · 6/12 · #1093
- ⬜ Intel Core i3-14100T · 4/8 · #1096
- ⬜ Intel Xeon Silver 4215 · 8/16 · #1099
- ⚠️ Intel Core i3-12100E · 4/8 · #1106
- ⬜ Intel Xeon Silver 4210 · 10/20 · #1107
- ⬜ Intel Xeon W-2135 · 6/12 · #1108
- ⚠️ Intel Core i7-10700TE · 8/16 · #1110
- ⬜ Intel Xeon E-2286G · 6/12 · #1112
- ⬜ Intel Xeon Silver 4123 · 8/16 · #1113
- ⬜ Intel Xeon E-2276G · 6/12 · #1119
- ⬜ Intel Core i7-1260U · 10/12 · #1121
- ⬜ Intel Core i7-1265U · 10/12 · #1124
- ⬜ Intel Core i5-1334U · 10/12 · #1125
- ⬜ Intel Xeon E-2246G · 6/12 · #1126
- ⬜ Intel Core i5-10600 · 6/12 · #1128
- ⬜ Intel Xeon D-1581 · 16/32 · #1130
- ⬜ Intel Xeon Silver 4215R · 8/16 · #1132
- ⬜ Intel Xeon E-2236 · 6/12 · #1133
- ⬜ Intel Core Ultra 5 134U · 12/14 · #1136
- ⬜ Intel Core i5-10500 · 6/12 · #1138
- ⬜ Intel Core i5-11400T · 6/12 · #1142
- ⬜ Intel Core i3-12300T · 4/8 · #1145
- ⬜ Intel Core 3 100U · 6/8 · #1148
- ⬜ Intel Core i5-1245U · 10/12 · #1150
- ⚠️ Intel Core i7-10700T · 8/16 · #1151
- ⬜ Intel Xeon E-2176G · 6/12 · #1154
- ⬜ Intel Xeon E-2186G · 6/12 · #1155
- ⬜ Intel Xeon D-1587 · 16/32 · #1158
- ⬜ Intel Core Ultra 5 115U · 8/10 · #1161
- ⬜ Intel Core i5-11500T · 6/12 · #1164
- ⬜ Intel Core i3-13100T · 4/8 · #1166
- ⬜ Intel Core Ultra 7 164U · 12/14 · #1168
- ⚠️ Intel Core i5-1235U · 10/12 · #1169
- ⬜ Intel Xeon E-2146G · 6/12 · #1175
- ⬜ Intel Core i7-1255U · 10/12 · #1178
- ⬜ Intel Xeon Silver 4114 · 10/20 · #1181
- ⬜ Intel Xeon E-2136 · 6/12 · #1182
- ⚠️ Intel Core i3-12100T · 4/8 · #1184
- ⚠️ Intel Core i3-12100 · 4/8 · #1187
- ⬜ Intel Xeon E-2334 · 4/8 · #1202
- ⬜ Intel Xeon Gold 6128 · 6/12 · #1203
- ⬜ Intel Xeon D-2143IT · 8/16 · #1204
- ⬜ Intel Xeon E-2278GEL · 8/16 · #1207
- ⬜ Intel Core i5-10505 · 6/12 · #1208
- ⬜ Intel Xeon E-2414 · 4/4 · #1211
- ⬜ Intel Xeon D-2141I · 8/16 · #1214
- ⬜ Intel Core i5-1335UE · 10/12 · #1216
- ⬜ Intel Xeon W-2133 · 6/12 · #1217
- ⬜ Intel Core i3-1320PE · 8/12 · #1218
- ⬜ Intel Core i5-10400 · 6/12 · #1219
- ⬜ Intel Core i3-11100HE · 4/8 · #1221
- ⬜ Intel Core i5-10400F · 6/12 · #1224
- ⬜ Intel Xeon 6315P · 4/4 · #1225
- ⬜ Intel Core 5 211TE · 10/16 · #1227
- ⬜ Intel Core i5-10600T · 6/12 · #1232
- ⬜ Intel Core i7-10850H · 6/12 · #1235
- ⬜ Intel Core i7-11370H · 4/8 · #1236
- ⬜ Intel Core i5-10500E · 6/12 · #1244
- ⬜ Intel Core i3-11100B · 4/8 · #1245
- ⬜ Intel Core i5-1345URE · 10/12 · #1247
- ⬜ Intel Xeon E-2276M · 6/12 · #1248
- ⬜ Intel Core i7-1250U · 10/12 · #1249
- ⬜ Intel Core i7-1365URE · 10/12 · #1250
- ⬜ Intel Core i3-13100TE · 4/8 · #1253
- ⬜ Intel Core i3-1315U · 6/8 · #1257
- ⬜ Intel Xeon Silver 4209T · 8/16 · #1259
- ⬜ Intel Core i5-1230U · 10/12 · #1261
- ⬜ Intel Core 7 160UL · 10/12 · #1262
- ⬜ Intel Core i7-10750H · 6/12 · #1264
- ⬜ Intel Xeon Silver 4208 · 8/16 · #1265
- ⬜ Intel Core i7-11375H · 4/8 · #1268
- ⬜ Intel Core i5-11320H · 4/8 · #1275
- ⬜ Intel Core i7-1365UE · 10/12 · #1276
- ⬜ Intel Xeon D-2146NT · 8/16 · #1278
- ⬜ Intel Xeon E-2176M · 6/12 · #1279
- ⬜ Intel Xeon E-2226G · 6/6 · #1280
- ⬜ Intel Xeon E-2186M · 6/12 · #1281
- ⬜ Intel Xeon D-1577 · 16/32 · #1284
- ⬜ Intel Core 5 120UL · 10/12 · #1293
- ⚠️ Intel Core i3-12100TE · 4/8 · #1297
- ⬜ Intel Core 3 N355 · 8/8 · #1298

## 🟡 Тир B — точечно — 158 моделей

### Intel — 158

- ⬜ Intel Core i9-9980XE · 18/36 · #404
- ⬜ Intel Xeon 4514Y · 16/32 · #406
- ⬜ Intel Core i9-7980XE · 18/36 · #452
- ⬜ Intel Core i9-9990XE · 14/28 · #455
- ⬜ Intel Core i9-9960X · 16/32 · #485
- ⬜ Intel Core i9-7960X · 16/32 · #510
- ⬜ Intel Xeon E5-2699A v4 · 22/44 · #518
- ⬜ Intel Core i9-9940X · 14/28 · #520
- ⬜ Intel Xeon E5-2698R v4 · 20/40 · #556
- ⬜ Intel Xeon W-1390P · 8/16 · #573
- ⬜ Intel Core i9-7940X · 14/28 · #581
- ⬜ Intel Xeon W-1390 · 8/16 · #602
- ⬜ Intel Xeon E5-2699 v4 · 22/44 · #608
- ⬜ Intel Core i9-9920X · 12/24 · #611
- ⬜ Intel Xeon W-1370P · 8/16 · #621
- ⬜ Intel Xeon E5-2696 v4 · 22/44 · #632
- ⬜ Intel Xeon W-1370 · 8/16 · #633
- ✅ Intel Core i9-7920X · 12/24 · #647
- ⬜ Intel Xeon W-1290P · 10/20 · #653
- ⬜ Intel Xeon E5-2679 v4 · 20/40 · #665
- ⬜ Intel Xeon E5-2698 v4 · 20/40 · #667
- ⬜ Intel Xeon E7-8891 v3 · 10/20 · #683
- ⬜ Intel Xeon W-11955M · 8/16 · #684
- ⚠️ Intel Xeon E5-2696 v3 · 18/36 · #711
- ⬜ Intel Xeon E5-4669 v4 · 22/44 · #725
- ⬜ Intel Xeon E5-2697A v4 · 16/32 · #744
- ⬜ Intel Core i9-9900X · 10/20 · #749
- ⬜ Intel Xeon E5-2697 v4 · 18/36 · #750
- ⬜ Intel Xeon E5-4667 v4 · 18/36 · #753
- ⬜ Intel Xeon W-1290 · 10/20 · #761
- ⬜ Intel Xeon E5-2699 v3 · 18/36 · #765
- ⬜ Intel Xeon W-1350P · 6/12 · #787
- ⬜ Intel Xeon W-1290E · 10/20 · #799
- ⬜ Intel Xeon E5-2673 v4 · 20/40 · #800
- ⬜ Intel Core i9-9820X · 10/20 · #808
- ⬜ Intel Core i9-9900KS · 8/16 · #828
- ⬜ Intel Core i9-7900X · 10/20 · #836
- ⬜ Intel Xeon W-1350 · 6/12 · #837
- ⬜ Intel Xeon W-1270E · 8/16 · #839
- ⬜ Intel Xeon E5-2690 v4 · 14/28 · #841
- ⬜ Intel Xeon E5-2698 v3 · 16/32 · #843
- ⬜ Intel Xeon W-11865MRE · 8/16 · #844
- ⬜ Intel Xeon E5-2682 v4 · 16/32 · #848
- ⬜ Intel Xeon W-1270P · 8/16 · #857
- ⬜ Intel Xeon E7-8880 v3 · 18/36 · #865
- ⬜ Intel Xeon E5-2686 v4 · 18/36 · #867
- ⬜ Intel Xeon E5-2697 v3 · 14/28 · #877
- ✅ Intel Core i9-9900KF · 8/16 · #888
- ⬜ Intel Xeon E5-2695 v4 · 18/36 · #894
- ⬜ Intel Xeon W-1270 · 8/16 · #896
- ⬜ Intel Xeon W-11555MRE · 6/12 · #898
- ⬜ Intel Core i7-9800X · 8/16 · #900
- ⬜ Intel Xeon W-11855M · 6/12 · #901
- ⬜ Intel Xeon E5-2686 v3 · 18/36 · #909
- ⬜ Intel Xeon W-1290T · 10/20 · #911
- ⬜ Intel Atom P5362 · 24/24 · #912
- ⬜ Intel Xeon E5-2687W v4 · 12/24 · #915
- ⬜ Intel Xeon E5-2683 v4 · 16/32 · #927
- ⬜ Intel Core i7-7820X · 8/16 · #930
- ⬜ Intel Core i9-9900K · 8/16 · #944
- ⬜ Intel Xeon E7-4809 v2 · 6/12 · #948
- ⬜ Intel Xeon E5-2695 v3 · 14/28 · #959
- ⬜ Intel Xeon E5-4650 v4 · 14/28 · #961
- ⬜ Intel Xeon E5-4669 v3 · 18/36 · #965
- ⬜ Intel Xeon E5-2689 v4 · 10/20 · #972
- ⬜ Intel Core i7-6950X · 10/20 · #974
- ⬜ Intel Xeon W-11865MLE · 8/16 · #976
- ⬜ Intel Xeon E5-2690 v3 · 12/24 · #985
- ⬜ Intel Xeon W-10885M · 8/16 · #996
- ⬜ Intel Xeon E5-4660 v4 · 16/32 · #1010
- ⚠️ Intel Xeon E5-2660 v4 · 14/28 · #1025
- ⬜ Intel Core i9-9900 · 8/16 · #1028
- ⬜ Intel Xeon E5-2680 v4 · 14/28 · #1030
- ⬜ Intel Xeon E5-1681 v3 · 10/20 · #1032
- ⬜ Intel Xeon E5-2683 v3 · 14/28 · #1036
- ⬜ Intel Xeon E5-2680 v3 · 12/24 · #1040
- ⬜ Intel Core i7-6900K · 8/16 · #1041
- ⬜ Intel Xeon W-1290TE · 10/20 · #1043
- ⬜ Intel Xeon E5-2678 v3 · 12/24 · #1050
- ⬜ Intel Core i9-9980HK · 8/16 · #1051
- ⬜ Intel Xeon E5-2687W v3 · 10/20 · #1056
- ✅ Intel Core i7-9700K · 8/8 · #1063
- ⬜ Intel Xeon E5-4667 v3 · 16/32 · #1064
- ⚠️ Intel Core i7-9700KF · 8/8 · #1067
- ⬜ Intel Core i7-8086K · 6/12 · #1076
- ⬜ Intel Xeon E5-2666 v3 · 10/20 · #1088
- ⬜ Intel Xeon W-1250P · 6/12 · #1091
- ⬜ Intel Xeon E5-4660 v3 · 14/28 · #1092
- ⬜ Intel Xeon W-1250 · 6/12 · #1094
- ⬜ Intel Xeon E5-2658A v3 · 12/24 · #1095
- ⬜ Intel Xeon E5-2658 v4 · 14/28 · #1100
- ⬜ Intel Xeon W-1270TE · 8/16 · #1105
- ⬜ Intel Xeon E5-1680 v4 · 8/16 · #1109
- ⬜ Intel Xeon E5-2658 v3 · 12/24 · #1117
- ⬜ Intel Xeon E5-2670 v3 · 12/24 · #1118
- ⬜ Intel Xeon E5-1680 v3 · 8/16 · #1122
- ⬜ Intel Xeon E5-2667 v4 · 8/16 · #1127
- ⬜ Intel Xeon E5-2696 v2 · 12/24 · #1131
- ⬜ Intel Core i7-9700F · 8/8 · #1134
- ⬜ Intel Xeon E5-2673 v3 · 12/24 · #1135
- ⬜ Intel Core i7-9700 · 8/8 · #1139
- ⬜ Intel Atom P5342 · 16/16 · #1140
- ⬜ Intel Xeon E5-2650 v4 · 12/24 · #1141
- ✅ Intel Xeon E5-2697 v2 · 12/24 · #1146
- ⬜ Intel Xeon E5-4627 v4 · 10/10 · #1147
- ⬜ Intel Core i9-9880H · 8/16 · #1149
- ⬜ Intel Xeon E5-2690 v2 · 10/20 · #1153
- ⬜ Intel Xeon E5-2650L v4 · 12/24 · #1156
- ⚠️ Intel Xeon E5-2660 v3 · 10/20 · #1159
- ⬜ Intel Core i7-8700K · 6/12 · #1160
- ⬜ Intel Core i9-9900T · 8/16 · #1162
- ⬜ Intel Core i7-7800X · 6/12 · #1167
- ✅ Intel Core i7-5960X · 8/16 · #1174
- ⬜ Intel Xeon E5-1660 v4 · 8/16 · #1176
- ⬜ Intel Xeon W-1250E · 6/12 · #1177
- ⬜ Intel Core i7-9700E · 8/8 · #1179
- ⬜ Intel Xeon E5-2695 v2 · 12/24 · #1180
- ✅ Intel Xeon E5-2676 v3 · 12/24 · #1185
- ⬜ Intel Xeon E5-1660 v3 · 8/16 · #1186
- ⬜ Intel Xeon E5-2673 v2 · 8/16 · #1192
- ⬜ Intel Xeon E5-2675 v3 · 16/32 · #1193
- ⬜ Intel Xeon E5-2640 v4 · 10/20 · #1194
- ⬜ Intel Xeon E5-1680 v2 · 8/16 · #1196
- ⬜ Intel Xeon W-10855M · 6/12 · #1197
- ⬜ Intel Xeon E5-2667 v3 · 8/16 · #1200
- ⬜ Intel Xeon E5-2680 v2 · 10/20 · #1201
- ⬜ Intel Xeon E5-2685 v3 · 12/12 · #1206
- ⬜ Intel Xeon E5-2618L v4 · 10/20 · #1220
- ⬜ Intel Xeon E5-2663 v3 · 10/10 · #1222
- ⬜ Intel Xeon E5-2687W v2 · 8/16 · #1226
- ⬜ Intel Xeon E5-2649 v3 · 10/20 · #1229
- ⬜ Intel Core i7-8700 · 6/12 · #1230
- ⬜ Intel Core i7-8700B · 6/12 · #1231
- ⬜ Intel Xeon E5-2667 v2 · 8/16 · #1233
- ⬜ Intel Xeon E5-2650L v3 · 12/24 · #1237
- ⬜ Intel Xeon E5-2650 v3 · 10/20 · #1238
- ⬜ Intel Xeon E5-4628L v4 · 14/28 · #1239
- ⬜ Intel Xeon W-11555MLE · 6/12 · #1240
- ⬜ Intel Xeon E5-2692 v2 · 12/24 · #1241
- ⬜ Intel Xeon E7-4870 v2 · 15/30 · #1252
- ⬜ Intel Xeon Bronze 3508U · 8/8 · #1254
- ⬜ Intel Core i7-6850K · 6/12 · #1255
- ⬜ Intel Xeon E5-2630 v4 · 10/20 · #1256
- ⬜ Intel Xeon E5-2648L v4 · 14/28 · #1258
- ⬜ Intel Xeon E5-2618L v3 · 8/16 · #1263
- ⬜ Intel Xeon E5-4650 v2 · 10/20 · #1266
- ⬜ Intel Xeon E5-4655 v4 · 8/16 · #1269
- ⬜ Intel Xeon E5-1650 v4 · 6/12 · #1271
- ⬜ Intel Xeon E5-4627 v3 · 10/10 · #1273
- ⬜ Intel Core i7-9850H · 6/12 · #1274
- ⬜ Intel Core i5-9600KF · 6/6 · #1285
- ⬜ Intel Xeon E5-4657L v2 · 12/24 · #1287
- ⬜ Intel Xeon E5-2670 v2 · 10/20 · #1288
- ⬜ Intel Core i7-6800K · 6/12 · #1290
- ⬜ Intel Xeon E5-4650 v3 · 12/24 · #1294
- ⬜ Intel Xeon E5-2643 v4 · 6/12 · #1295
- ⬜ Intel Xeon E5-2640 v3 · 8/16 · #1296
- ⬜ Intel Xeon E5-2628L v4 · 12/24 · #1300

## 🔴 Тир C — маловероятно — 1200 моделей

Список целиком — в [`CPU-RANKING.txt`](CPU-RANKING.txt), строки 1301–2500. Здесь не дублируется: по этим моделям поиск не планируется.

## ⚫ Тир D — практически исключено — 1740 моделей

Список целиком — в [`CPU-RANKING.txt`](CPU-RANKING.txt), строки 2501–4240. Здесь не дублируется: по этим моделям поиск не планируется.

## Дополнительные результаты и найденные модели

### Community WPA-PBKDF2 comparison (mode 22000)

В Gist опубликованы значения для 227 уникальных названий CPU. Это не raw и не
полный `hashcat -b`; для каждого значения заведена карточка по пути
`CPU/<вендор>/<семейство>/<модель>/`. Повтор строки Core M-5Y10c в исходнике
не дублирован. Полный индекс со скоростями и ссылками — в [`CPU.md`](CPU.md).

<!-- WPA22000_ROSTER_START -->
| Модель в источнике | Mode 22000, H/s | Папка |
|---|---:|---|
| AMD A4-4000 APU | 1464 | [AMD A4-4000 APU](<CPU/AMD/APU/AMD A4-4000 APU>) |
| AMD A6-4455M APU | 871 | [AMD A6-4455M APU](<CPU/AMD/APU/AMD A6-4455M APU>) |
| AMD A6-5200 APU | 1914 | [AMD A6-5200 APU](<CPU/AMD/APU/AMD A6-5200 APU>) |
| AMD A6-5400K APU | 1597 | [AMD A6-5400K APU](<CPU/AMD/APU/AMD A6-5400K APU>) |
| AMD A8-3500M APU | 1872 | [AMD A8-3500M APU](<CPU/AMD/APU/AMD A8-3500M APU>) |
| AMD A8-4500M | 2078 | [AMD A8-4500M](<CPU/AMD/APU/AMD A8-4500M>) |
| AMD A8-5550M APU | 2276 | [AMD A8-5550M APU](<CPU/AMD/APU/AMD A8-5550M APU>) |
| AMD Athlon 64 X2 4600+ | 625 | [AMD Athlon 64 X2 4600+](<CPU/AMD/Athlon/AMD Athlon 64 X2 4600+>) |
| AMD Athlon II X2 260 | 1536 | [AMD Athlon II X2 260](<CPU/AMD/Athlon/AMD Athlon II X2 260>) |
| AMD Athlon II X2 270 | 1948 | [AMD Athlon II X2 270](<CPU/AMD/Athlon/AMD Athlon II X2 270>) |
| AMD Athlon II X4 610e | 2704 | [AMD Athlon II X4 610e](<CPU/AMD/Athlon/AMD Athlon II X4 610e>) |
| AMD Athlon II X4 631 | 3193 | [AMD Athlon II X4 631](<CPU/AMD/Athlon/AMD Athlon II X4 631>) |
| AMD Athlon II X4 640 | 3437 | [AMD Athlon II X4 640](<CPU/AMD/Athlon/AMD Athlon II X4 640>) |
| AMD Athlon X2 245 | 1558 | [AMD Athlon X2 245](<CPU/AMD/Athlon/AMD Athlon X2 245>) |
| AMD Athlon X2 QL-64 | 592 | [AMD Athlon X2 QL-64](<CPU/AMD/Athlon/AMD Athlon X2 QL-64>) |
| AMD Athlon X4 750K | 3379 | [AMD Athlon X4 750K](<CPU/AMD/Athlon/AMD Athlon X4 750K>) |
| AMD Athlon X4 860K | 3392 | [AMD Athlon X4 860K](<CPU/AMD/Athlon/AMD Athlon X4 860K>) |
| AMD E-300 APU | 275 | [AMD E-300 APU](<CPU/AMD/APU/AMD E-300 APU>) |
| AMD E-350 | 364 | [AMD E-350](<CPU/AMD/APU/AMD E-350>) |
| AMD E1-1200 APU | 276 | [AMD E1-1200 APU](<CPU/AMD/APU/AMD E1-1200 APU>) |
| AMD E1-2100 APU | 459 | [AMD E1-2100 APU](<CPU/AMD/APU/AMD E1-2100 APU>) |
| AMD E2-3000M APU | 1032 | [AMD E2-3000M APU](<CPU/AMD/APU/AMD E2-3000M APU>) |
| AMD FX-4320 Quad-Core | 3604 | [AMD FX-4320 Quad-Core](<CPU/AMD/FX/AMD FX-4320 Quad-Core>) |
| AMD FX-6100 | 4065 | [AMD FX-6100](<CPU/AMD/FX/AMD FX-6100>) |
| AMD FX-6300 | 4262 | [AMD FX-6300](<CPU/AMD/FX/AMD FX-6300>) |
| AMD FX-6350 | 5738 | [AMD FX-6350](<CPU/AMD/FX/AMD FX-6350>) |
| AMD FX-8120 | 5484 | [AMD FX-8120](<CPU/AMD/FX/AMD FX-8120>) |
| AMD FX-8150 Eight-Core | 7087 | [AMD FX-8150 Eight-Core](<CPU/AMD/FX/AMD FX-8150 Eight-Core>) |
| AMD FX-8320 Eight-Core | 6387 | [AMD FX-8320 Eight-Core](<CPU/AMD/FX/AMD FX-8320 Eight-Core>) |
| AMD FX-8350 | 7577 | [AMD FX-8350](<CPU/AMD/FX/AMD FX-8350>) |
| AMD Phenom 8450 | 1597 | [AMD Phenom 8450](<CPU/AMD/Phenom/AMD Phenom 8450>) |
| AMD Phenom 9550 | 2111 | [AMD Phenom 9550](<CPU/AMD/Phenom/AMD Phenom 9550>) |
| AMD Phenom 9750 Quad-Core | 2173 | [AMD Phenom 9750 Quad-Core](<CPU/AMD/Phenom/AMD Phenom 9750 Quad-Core>) |
| AMD Phenom II N950 Quad-Core | 2442 | [AMD Phenom II N950 Quad-Core](<CPU/AMD/Phenom/AMD Phenom II N950 Quad-Core>) |
| AMD Phenom II X4 840 | 3638 | [AMD Phenom II X4 840](<CPU/AMD/Phenom/AMD Phenom II X4 840>) |
| AMD Phenom II X4 965 | 4015 | [AMD Phenom II X4 965](<CPU/AMD/Phenom/AMD Phenom II X4 965>) |
| AMD Phenom II X4 B50 | 3721 | [AMD Phenom II X4 B50](<CPU/AMD/Phenom/AMD Phenom II X4 B50>) |
| AMD Phenom II X6 1055T | 6445 | [AMD Phenom II X6 1055T](<CPU/AMD/Phenom/AMD Phenom II X6 1055T>) |
| AMD Phenom II X6 1075T | 5227 | [AMD Phenom II X6 1075T](<CPU/AMD/Phenom/AMD Phenom II X6 1075T>) |
| AMD Ryzen 5 2400G | 7790 | [AMD Ryzen 5 2400G](<CPU/AMD/Ryzen 5/AMD Ryzen 5 2400G>) |
| AMD Ryzen 5 2600X | 10747 | [AMD Ryzen 5 2600X](<CPU/AMD/Ryzen 5/AMD Ryzen 5 2600X>) |
| AMD Ryzen 5 3500X | 23952 | [AMD Ryzen 5 3500X](<CPU/AMD/Ryzen 5/AMD Ryzen 5 3500X>) |
| AMD Ryzen 7 3700X | 34817 | [AMD Ryzen 7 3700X](<CPU/AMD/Ryzen 7/AMD Ryzen 7 3700X>) |
| AMD Ryzen 7 5800U | 33162 | [AMD Ryzen 7 5800U](<CPU/AMD/Ryzen 7/AMD Ryzen 7 5800U>) |
| AMD Ryzen 9 3900X | 48838 | [AMD Ryzen 9 3900X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 3900X>) |
| AMD Ryzen 9 5900X | 65737 | [AMD Ryzen 9 5900X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 5900X>) |
| AMD Ryzen 9 5950X | 68376 | [AMD Ryzen 9 5950X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 5950X>) |
| AMD Sempron 145 | 818 | [AMD Sempron 145](<CPU/AMD/Sempron/AMD Sempron 145>) |
| AMD Sempron X2 180 | 1416 | [AMD Sempron X2 180](<CPU/AMD/Sempron/AMD Sempron X2 180>) |
| AMD Sempron X2 190 | 1386 | [AMD Sempron X2 190](<CPU/AMD/Sempron/AMD Sempron X2 190>) |
| AMD Turion 64 X2 TL-52 | 447 | [AMD Turion 64 X2 TL-52](<CPU/AMD/Turion/AMD Turion 64 X2 TL-52>) |
| AMD Turion II P560 | 1165 | [AMD Turion II P560](<CPU/AMD/Turion/AMD Turion II P560>) |
| Celeron Dual-Core T3000 | 1091 | [Celeron Dual-Core T3000](<CPU/Intel/Celeron/Celeron Dual-Core T3000>) |
| Intel 2140 | 1362 | [Intel 2140](<CPU/Intel/Other Intel/Intel 2140>) |
| Intel Atom D525 | 804 | [Intel Atom D525](<CPU/Intel/Atom/Intel Atom D525>) |
| Intel Atom N2600 | 626 | [Intel Atom N2600](<CPU/Intel/Atom/Intel Atom N2600>) |
| Intel Atom N270 | 380 | [Intel Atom N270](<CPU/Intel/Atom/Intel Atom N270>) |
| Intel Atom N455 | 281 | [Intel Atom N455](<CPU/Intel/Atom/Intel Atom N455>) |
| Intel Atom N470 | 360 | [Intel Atom N470](<CPU/Intel/Atom/Intel Atom N470>) |
| Intel Atom Z3735F | 975 | [Intel Atom Z3735F](<CPU/Intel/Atom/Intel Atom Z3735F>) |
| Intel Celeron 1000M | 1472 | [Intel Celeron 1000M](<CPU/Intel/Celeron/Intel Celeron 1000M>) |
| Intel Celeron 1005M | 1471 | [Intel Celeron 1005M](<CPU/Intel/Celeron/Intel Celeron 1005M>) |
| Intel Celeron 1007U | 1190 | [Intel Celeron 1007U](<CPU/Intel/Celeron/Intel Celeron 1007U>) |
| Intel Celeron 430 | 516 | [Intel Celeron 430](<CPU/Intel/Celeron/Intel Celeron 430>) |
| Intel Celeron 925 | 719 | [Intel Celeron 925](<CPU/Intel/Celeron/Intel Celeron 925>) |
| Intel Celeron CPU B800 | 1127 | [Intel Celeron CPU B800](<CPU/Intel/Celeron/Intel Celeron CPU B800>) |
| Intel Celeron E1500 | 1613 | [Intel Celeron E1500](<CPU/Intel/Celeron/Intel Celeron E1500>) |
| Intel Celeron M | 79 | [Intel Celeron M](<CPU/Intel/Celeron/Intel Celeron M>) |
| Intel Celeron M 530 | 573 | [Intel Celeron M 530](<CPU/Intel/Celeron/Intel Celeron M 530>) |
| Intel Celeron N2920 | 1233 | [Intel Celeron N2920](<CPU/Intel/Celeron/Intel Celeron N2920>) |
| Intel Core 2 Duo T6500 | 1482 | [Intel Core 2 Duo T6500](<CPU/Intel/Core 2/Intel Core 2 Duo T6500>) |
| Intel Core 2 Quad Q9550 | 4119 | [Intel Core 2 Quad Q9550](<CPU/Intel/Core 2/Intel Core 2 Quad Q9550>) |
| Intel Core i3 10105 | 17958 | [Intel Core i3 10105](<CPU/Intel/Core i3/Intel Core i3 10105>) |
| Intel Core i3 12100 | 17756 | [Intel Core i3 12100](<CPU/Intel/Core i3/Intel Core i3 12100>) |
| Intel Core i3 540 | 2153 | [Intel Core i3 540](<CPU/Intel/Core i3/Intel Core i3 540>) |
| Intel Core i3 CPU M350 | 1003 | [Intel Core i3 CPU M350](<CPU/Intel/Core i3/Intel Core i3 CPU M350>) |
| Intel Core i3 M330 | 1681 | [Intel Core i3 M330](<CPU/Intel/Core i3/Intel Core i3 M330>) |
| Intel Core i3 M380 | 2017 | [Intel Core i3 M380](<CPU/Intel/Core i3/Intel Core i3 M380>) |
| Intel Core i3 U380 | 822 | [Intel Core i3 U380](<CPU/Intel/Core i3/Intel Core i3 U380>) |
| Intel Core i3-10100 | 17842 | [Intel Core i3-10100](<CPU/Intel/Core i3/Intel Core i3-10100>) |
| Intel Core i3-2100 | 2561 | [Intel Core i3-2100](<CPU/Intel/Core i3/Intel Core i3-2100>) |
| Intel Core i3-2120 | 2769 | [Intel Core i3-2120](<CPU/Intel/Core i3/Intel Core i3-2120>) |
| Intel Core i3-2328M | 1656 | [Intel Core i3-2328M](<CPU/Intel/Core i3/Intel Core i3-2328M>) |
| Intel Core i3-2348M | 1644 | [Intel Core i3-2348M](<CPU/Intel/Core i3/Intel Core i3-2348M>) |
| Intel Core i3-2350M | 1784 | [Intel Core i3-2350M](<CPU/Intel/Core i3/Intel Core i3-2350M>) |
| Intel Core i3-2367M | 923 | [Intel Core i3-2367M](<CPU/Intel/Core i3/Intel Core i3-2367M>) |
| Intel Core i3-2370M | 1977 | [Intel Core i3-2370M](<CPU/Intel/Core i3/Intel Core i3-2370M>) |
| Intel Core i3-3110M | 2151 | [Intel Core i3-3110M](<CPU/Intel/Core i3/Intel Core i3-3110M>) |
| Intel Core i3-3120M | 2289 | [Intel Core i3-3120M](<CPU/Intel/Core i3/Intel Core i3-3120M>) |
| Intel Core i3-3217U | 1458 | [Intel Core i3-3217U](<CPU/Intel/Core i3/Intel Core i3-3217U>) |
| Intel Core i3-3220 | 2976 | [Intel Core i3-3220](<CPU/Intel/Core i3/Intel Core i3-3220>) |
| Intel Core i3-3227U | 1682 | [Intel Core i3-3227U](<CPU/Intel/Core i3/Intel Core i3-3227U>) |
| Intel Core i3-3240 | 1552 | [Intel Core i3-3240](<CPU/Intel/Core i3/Intel Core i3-3240>) |
| Intel Core i3-4005U | 3454 | [Intel Core i3-4005U](<CPU/Intel/Core i3/Intel Core i3-4005U>) |
| Intel Core i3-4010U | 3477 | [Intel Core i3-4010U](<CPU/Intel/Core i3/Intel Core i3-4010U>) |
| Intel Core i3-4130 | 6896 | [Intel Core i3-4130](<CPU/Intel/Core i3/Intel Core i3-4130>) |
| Intel Core i3-4170 | 7154 | [Intel Core i3-4170](<CPU/Intel/Core i3/Intel Core i3-4170>) |
| Intel Core i3-6006U | 4308 | [Intel Core i3-6006U](<CPU/Intel/Core i3/Intel Core i3-6006U>) |
| Intel Core i3-7100 | 8526 | [Intel Core i3-7100](<CPU/Intel/Core i3/Intel Core i3-7100>) |
| Intel Core i3-9100F | 15870 | [Intel Core i3-9100F](<CPU/Intel/Core i3/Intel Core i3-9100F>) |
| Intel Core i5 8265U | 9328 | [Intel Core i5 8265U](<CPU/Intel/Core i5/Intel Core i5 8265U>) |
| Intel Core i5 M 480 | 1011 | [Intel Core i5 M 480](<CPU/Intel/Core i5/Intel Core i5 M 480>) |
| Intel Core i5 M430 | 1795 | [Intel Core i5 M430](<CPU/Intel/Core i5/Intel Core i5 M430>) |
| Intel Core i5 M460 | 2068 | [Intel Core i5 M460](<CPU/Intel/Core i5/Intel Core i5 M460>) |
| Intel Core i5 M520 | 2121 | [Intel Core i5 M520](<CPU/Intel/Core i5/Intel Core i5 M520>) |
| Intel Core i5-10210U | 11818 | [Intel Core i5-10210U](<CPU/Intel/Core i5/Intel Core i5-10210U>) |
| Intel Core i5-11400H | 26951 | [Intel Core i5-11400H](<CPU/Intel/Core i5/Intel Core i5-11400H>) |
| Intel Core i5-1235U | 9615 | [Intel Core i5-1235U](<CPU/Intel/Core i5/Intel Core i5-1235U>) |
| Intel Core i5-12400F | 26424 | [Intel Core i5-12400F](<CPU/Intel/Core i5/Intel Core i5-12400F>) |
| Intel Core i5-2300 | 4379 | [Intel Core i5-2300](<CPU/Intel/Core i5/Intel Core i5-2300>) |
| Intel Core i5-2310 | 4739 | [Intel Core i5-2310](<CPU/Intel/Core i5/Intel Core i5-2310>) |
| Intel Core i5-2380P | 4636 | [Intel Core i5-2380P](<CPU/Intel/Core i5/Intel Core i5-2380P>) |
| Intel Core i5-2400 | 4928 | [Intel Core i5-2400](<CPU/Intel/Core i5/Intel Core i5-2400>) |
| Intel Core i5-2410M | 2103 | [Intel Core i5-2410M](<CPU/Intel/Core i5/Intel Core i5-2410M>) |
| Intel Core i5-2430M | 2299 | [Intel Core i5-2430M](<CPU/Intel/Core i5/Intel Core i5-2430M>) |
| Intel Core i5-2450M | 602 | [Intel Core i5-2450M](<CPU/Intel/Core i5/Intel Core i5-2450M>) |
| Intel Core i5-2520M | 2474 | [Intel Core i5-2520M](<CPU/Intel/Core i5/Intel Core i5-2520M>) |
| Intel Core i5-3210M | 2652 | [Intel Core i5-3210M](<CPU/Intel/Core i5/Intel Core i5-3210M>) |
| Intel Core i5-3230M | 1961 | [Intel Core i5-3230M](<CPU/Intel/Core i5/Intel Core i5-3230M>) |
| Intel Core i5-3337U | 2162 | [Intel Core i5-3337U](<CPU/Intel/Core i5/Intel Core i5-3337U>) |
| Intel Core i5-3470 | 5558 | [Intel Core i5-3470](<CPU/Intel/Core i5/Intel Core i5-3470>) |
| Intel Core i5-4200M | 6122 | [Intel Core i5-4200M](<CPU/Intel/Core i5/Intel Core i5-4200M>) |
| Intel Core i5-4200U | 4689 | [Intel Core i5-4200U](<CPU/Intel/Core i5/Intel Core i5-4200U>) |
| Intel Core i5-4210H | 5559 | [Intel Core i5-4210H](<CPU/Intel/Core i5/Intel Core i5-4210H>) |
| Intel Core i5-4210U | 4175 | [Intel Core i5-4210U](<CPU/Intel/Core i5/Intel Core i5-4210U>) |
| Intel Core i5-4300U | 5286 | [Intel Core i5-4300U](<CPU/Intel/Core i5/Intel Core i5-4300U>) |
| Intel Core i5-4430 | 11649 | [Intel Core i5-4430](<CPU/Intel/Core i5/Intel Core i5-4430>) |
| Intel Core i5-4440 | 11257 | [Intel Core i5-4440](<CPU/Intel/Core i5/Intel Core i5-4440>) |
| Intel Core i5-4570 | 13300 | [Intel Core i5-4570](<CPU/Intel/Core i5/Intel Core i5-4570>) |
| Intel Core i5-4590 | 13302 | [Intel Core i5-4590](<CPU/Intel/Core i5/Intel Core i5-4590>) |
| Intel Core i5-6300HQ | 10664 | [Intel Core i5-6300HQ](<CPU/Intel/Core i5/Intel Core i5-6300HQ>) |
| Intel Core i5-7200 | 5498 | [Intel Core i5-7200](<CPU/Intel/Core i5/Intel Core i5-7200>) |
| Intel Core i5-8250U | 7986 | [Intel Core i5-8250U](<CPU/Intel/Core i5/Intel Core i5-8250U>) |
| Intel Core i5-9400F | 20171 | [Intel Core i5-9400F](<CPU/Intel/Core i5/Intel Core i5-9400F>) |
| Intel Core i7 12700 | 46512 | [Intel Core i7 12700](<CPU/Intel/Core i7/Intel Core i7 12700>) |
| Intel Core i7 13700 | 57517 | [Intel Core i7 13700](<CPU/Intel/Core i7/Intel Core i7 13700>) |
| Intel Core i7 860 | 4863 | [Intel Core i7 860](<CPU/Intel/Core i7/Intel Core i7 860>) |
| Intel Core i7 9700KF | 35231 | [Intel Core i7 9700KF](<CPU/Intel/Core i7/Intel Core i7 9700KF>) |
| Intel Core i7 Q720 | 1709 | [Intel Core i7 Q720](<CPU/Intel/Core i7/Intel Core i7 Q720>) |
| Intel Core i7-10700 | 29937 | [Intel Core i7-10700](<CPU/Intel/Core i7/Intel Core i7-10700>) |
| Intel Core i7-11800H | 31781 | [Intel Core i7-11800H](<CPU/Intel/Core i7/Intel Core i7-11800H>) |
| Intel Core i7-2600K | 5636 | [Intel Core i7-2600K](<CPU/Intel/Core i7/Intel Core i7-2600K>) |
| Intel Core i7-2630QM | 2953 | [Intel Core i7-2630QM](<CPU/Intel/Core i7/Intel Core i7-2630QM>) |
| Intel Core i7-2670QM | 4414 | [Intel Core i7-2670QM](<CPU/Intel/Core i7/Intel Core i7-2670QM>) |
| Intel Core i7-2720QM | 2705 | [Intel Core i7-2720QM](<CPU/Intel/Core i7/Intel Core i7-2720QM>) |
| Intel Core i7-3540M | 2633 | [Intel Core i7-3540M](<CPU/Intel/Core i7/Intel Core i7-3540M>) |
| Intel Core i7-3630QM | 5291 | [Intel Core i7-3630QM](<CPU/Intel/Core i7/Intel Core i7-3630QM>) |
| Intel Core i7-3632QM | 5232 | [Intel Core i7-3632QM](<CPU/Intel/Core i7/Intel Core i7-3632QM>) |
| Intel Core i7-3720QM | 5735 | [Intel Core i7-3720QM](<CPU/Intel/Core i7/Intel Core i7-3720QM>) |
| Intel Core i7-3770 | 6821 | [Intel Core i7-3770](<CPU/Intel/Core i7/Intel Core i7-3770>) |
| Intel Core i7-3820 | 5421 | [Intel Core i7-3820](<CPU/Intel/Core i7/Intel Core i7-3820>) |
| Intel Core i7-3930K | 8003 | [Intel Core i7-3930K](<CPU/Intel/Core i7/Intel Core i7-3930K>) |
| Intel Core i7-4510U | 5569 | [Intel Core i7-4510U](<CPU/Intel/Core i7/Intel Core i7-4510U>) |
| Intel Core i7-4700HQ | 5993 | [Intel Core i7-4700HQ](<CPU/Intel/Core i7/Intel Core i7-4700HQ>) |
| Intel Core i7-4700MQ | 12813 | [Intel Core i7-4700MQ](<CPU/Intel/Core i7/Intel Core i7-4700MQ>) |
| Intel Core i7-4702MQ | 11658 | [Intel Core i7-4702MQ](<CPU/Intel/Core i7/Intel Core i7-4702MQ>) |
| Intel Core i7-4710HQ | 11160 | [Intel Core i7-4710HQ](<CPU/Intel/Core i7/Intel Core i7-4710HQ>) |
| Intel Core i7-4710MQ | 8010 | [Intel Core i7-4710MQ](<CPU/Intel/Core i7/Intel Core i7-4710MQ>) |
| Intel Core i7-4720HQ | 13764 | [Intel Core i7-4720HQ](<CPU/Intel/Core i7/Intel Core i7-4720HQ>) |
| Intel Core i7-4770K | 15425 | [Intel Core i7-4770K](<CPU/Intel/Core i7/Intel Core i7-4770K>) |
| Intel Core i7-4790K | 17870 | [Intel Core i7-4790K](<CPU/Intel/Core i7/Intel Core i7-4790K>) |
| Intel Core i7-4820K | 6461 | [Intel Core i7-4820K](<CPU/Intel/Core i7/Intel Core i7-4820K>) |
| Intel Core i7-5820K | 25451 | [Intel Core i7-5820K](<CPU/Intel/Core i7/Intel Core i7-5820K>) |
| Intel Core i7-6700K | 18544 | [Intel Core i7-6700K](<CPU/Intel/Core i7/Intel Core i7-6700K>) |
| Intel Core i7-7700HQ | 14341 | [Intel Core i7-7700HQ](<CPU/Intel/Core i7/Intel Core i7-7700HQ>) |
| Intel Core i7-7820HQ | 15250 | [Intel Core i7-7820HQ](<CPU/Intel/Core i7/Intel Core i7-7820HQ>) |
| Intel Core i7-8750H | 17685 | [Intel Core i7-8750H](<CPU/Intel/Core i7/Intel Core i7-8750H>) |
| Intel Core i7-9750H | 18615 | [Intel Core i7-9750H](<CPU/Intel/Core i7/Intel Core i7-9750H>) |
| Intel Core M-5Y10c | 4079 | [Intel Core M-5Y10c](<CPU/Intel/Core M/Intel Core M-5Y10c>) |
| Intel Core2 6300 | 1120 | [Intel Core2 6300](<CPU/Intel/Core 2/Intel Core2 6300>) |
| Intel Core2 Duo E4600 | 1749 | [Intel Core2 Duo E4600](<CPU/Intel/Core 2/Intel Core2 Duo E4600>) |
| Intel Core2 Duo E7300 | 1812 | [Intel Core2 Duo E7300](<CPU/Intel/Core 2/Intel Core2 Duo E7300>) |
| Intel Core2 Duo E7500 | 2099 | [Intel Core2 Duo E7500](<CPU/Intel/Core 2/Intel Core2 Duo E7500>) |
| Intel Core2 Duo E8400 | 1933 | [Intel Core2 Duo E8400](<CPU/Intel/Core 2/Intel Core2 Duo E8400>) |
| Intel Core2 Duo P7450 | 1013 | [Intel Core2 Duo P7450](<CPU/Intel/Core 2/Intel Core2 Duo P7450>) |
| Intel Core2 Duo P8600 | 1560 | [Intel Core2 Duo P8600](<CPU/Intel/Core 2/Intel Core2 Duo P8600>) |
| Intel Core2 Duo P9400 | 1682 | [Intel Core2 Duo P9400](<CPU/Intel/Core 2/Intel Core2 Duo P9400>) |
| Intel Core2 Duo T5250 | 1015 | [Intel Core2 Duo T5250](<CPU/Intel/Core 2/Intel Core2 Duo T5250>) |
| Intel Core2 Duo T5450 | 1191 | [Intel Core2 Duo T5450](<CPU/Intel/Core 2/Intel Core2 Duo T5450>) |
| Intel Core2 Duo T5800 | 1373 | [Intel Core2 Duo T5800](<CPU/Intel/Core 2/Intel Core2 Duo T5800>) |
| Intel Core2 Duo T6400 | 1227 | [Intel Core2 Duo T6400](<CPU/Intel/Core 2/Intel Core2 Duo T6400>) |
| Intel Core2 Duo T6570 | 1500 | [Intel Core2 Duo T6570](<CPU/Intel/Core 2/Intel Core2 Duo T6570>) |
| Intel Core2 Duo T6670 | 1479 | [Intel Core2 Duo T6670](<CPU/Intel/Core 2/Intel Core2 Duo T6670>) |
| Intel Core2 Duo T7300 | 1362 | [Intel Core2 Duo T7300](<CPU/Intel/Core 2/Intel Core2 Duo T7300>) |
| Intel Core2 Duo T7500 | 1530 | [Intel Core2 Duo T7500](<CPU/Intel/Core 2/Intel Core2 Duo T7500>) |
| Intel Core2 Q9650 | 4261 | [Intel Core2 Q9650](<CPU/Intel/Core 2/Intel Core2 Q9650>) |
| Intel Core2 Quad Q8300 | 4025 | [Intel Core2 Quad Q8300](<CPU/Intel/Core 2/Intel Core2 Quad Q8300>) |
| Intel Core2 Quad Q8400 | 3896 | [Intel Core2 Quad Q8400](<CPU/Intel/Core 2/Intel Core2 Quad Q8400>) |
| Intel Core2 Quad Q9400 | 3730 | [Intel Core2 Quad Q9400](<CPU/Intel/Core 2/Intel Core2 Quad Q9400>) |
| Intel Core2 Solo U3500 | 502 | [Intel Core2 Solo U3500](<CPU/Intel/Core 2/Intel Core2 Solo U3500>) |
| Intel Core2 T5300 | 571 | [Intel Core2 T5300](<CPU/Intel/Core 2/Intel Core2 T5300>) |
| Intel Corei5 M 480 | 2139 | [Intel Corei5 M 480](<CPU/Intel/Core i5/Intel Core i5 M 480>) |
| Intel Pentium 2020M | 2026 | [Intel Pentium 2020M](<CPU/Intel/Pentium/Intel Pentium 2020M>) |
| Intel Pentium 2117U | 1541 | [Intel Pentium 2117U](<CPU/Intel/Pentium/Intel Pentium 2117U>) |
| Intel Pentium 4 | 352 | [Intel Pentium 4](<CPU/Intel/Pentium/Intel Pentium 4>) |
| Intel Pentium 4415U | 2202 | [Intel Pentium 4415U](<CPU/Intel/Pentium/Intel Pentium 4415U>) |
| Intel Pentium B950 | 1610 | [Intel Pentium B950](<CPU/Intel/Pentium/Intel Pentium B950>) |
| Intel Pentium B960 | 1629 | [Intel Pentium B960](<CPU/Intel/Pentium/Intel Pentium B960>) |
| Intel Pentium Dual E2160 | 924 | [Intel Pentium Dual E2160](<CPU/Intel/Pentium/Intel Pentium Dual E2160>) |
| Intel Pentium G2030 | 2665 | [Intel Pentium G2030](<CPU/Intel/Pentium/Intel Pentium G2030>) |
| Intel Pentium G850 | 2182 | [Intel Pentium G850](<CPU/Intel/Pentium/Intel Pentium G850>) |
| Intel Pentium M | 92 | [Intel Pentium M](<CPU/Intel/Pentium/Intel Pentium M>) |
| Intel Pentium N3540 | 1673 | [Intel Pentium N3540](<CPU/Intel/Pentium/Intel Pentium N3540>) |
| Intel Pentium P6200 | 1529 | [Intel Pentium P6200](<CPU/Intel/Pentium/Intel Pentium P6200>) |
| Intel U7300 | 958 | [Intel U7300](<CPU/Intel/Other Intel/Intel U7300>) |
| Intel Xeon 5150 | 3852 | [Intel Xeon 5150](<CPU/Intel/Xeon/Intel Xeon 5150>) |
| Intel Xeon CPU E3-1230 v3 | 14397 | [Intel Xeon CPU E3-1230 v3](<CPU/Intel/Xeon/Intel Xeon CPU E3-1230 v3>) |
| Intel Xeon CPU E5-2650 v2 | 1137 | [Intel Xeon CPU E5-2650 v2](<CPU/Intel/Xeon/Intel Xeon CPU E5-2650 v2>) |
| Intel Xeon E3-1230 V2 | 5626 | [Intel Xeon E3-1230 V2](<CPU/Intel/Xeon/Intel Xeon E3-1230 V2>) |
| Intel Xeon E3-1231 v3 | 14652 | [Intel Xeon E3-1231 v3](<CPU/Intel/Xeon/Intel Xeon E3-1231 v3>) |
| Intel Xeon E3-1270 v3 | 15188 | [Intel Xeon E3-1270 v3](<CPU/Intel/Xeon/Intel Xeon E3-1270 v3>) |
| Intel Xeon E3-1505M v6 | 15547 | [Intel Xeon E3-1505M v6](<CPU/Intel/Xeon/Intel Xeon E3-1505M v6>) |
| Intel Xeon E5 1650 v2 | 9911 | [Intel Xeon E5 1650 v2](<CPU/Intel/Xeon/Intel Xeon E5 1650 v2>) |
| Intel Xeon E5-2660 | 8798 | [Intel Xeon E5-2660](<CPU/Intel/Xeon/Intel Xeon E5-2660>) |
| Intel Xeon E5-2696 v3 | 41355 | [Intel Xeon E5-2696 v3](<CPU/Intel/Xeon/Intel Xeon E5-2696 v3>) |
| Intel Xeon E5430 | 4499 | [Intel Xeon E5430](<CPU/Intel/Xeon/Intel Xeon E5430>) |
| Intel Xeon L5520 | 3484 | [Intel Xeon L5520](<CPU/Intel/Xeon/Intel Xeon L5520>) |
| Intel Xeon Platinum 8276L | 65940 | [Intel Xeon Platinum 8276L](<CPU/Intel/Xeon/Intel Xeon Platinum 8276L>) |
| Intel Xeon X5450 | 4382 | [Intel Xeon X5450](<CPU/Intel/Xeon/Intel Xeon X5450>) |
| Intel Xeon X5650 | 6579 | [Intel Xeon X5650](<CPU/Intel/Xeon/Intel Xeon X5650>) |
| Pentium Dual-Core CPU E5700 | 1981 | [Pentium Dual-Core CPU E5700](<CPU/Intel/Pentium/Pentium Dual-Core CPU E5700>) |
| Pentium Dual-Core E5300 | 1899 | [Pentium Dual-Core E5300](<CPU/Intel/Pentium/Pentium Dual-Core E5300>) |
| Pentium Dual-Core E5800 | 2346 | [Pentium Dual-Core E5800](<CPU/Intel/Pentium/Pentium Dual-Core E5800>) |
| Pentium Dual-Core E6600 | 2226 | [Pentium Dual-Core E6600](<CPU/Intel/Pentium/Pentium Dual-Core E6600>) |
| Pentium Dual-Core T4200 | 1408 | [Pentium Dual-Core T4200](<CPU/Intel/Pentium/Pentium Dual-Core T4200>) |
| Pentium Dual-Core T4400 | 1545 | [Pentium Dual-Core T4400](<CPU/Intel/Pentium/Pentium Dual-Core T4400>) |
| Pentium Dual-Core T4500 | 1462 | [Pentium Dual-Core T4500](<CPU/Intel/Pentium/Pentium Dual-Core T4500>) |
<!-- WPA22000_ROSTER_END -->

- ⚠️ Intel Xeon E3-1270 v5 · #1489 — PHCS mode-0 MD5 comparison, 550.6 MH/s;
  опубликован агрегат без локального raw-лога ([подробности](PUBLIC-AGGREGATES.md)).
- ✅ Intel Core i7-6700K · #1446 — Hashcat Forum, v6.2.1, CPU-only mode 15700 SCRYPT;
  один raw-режим ([карточка](CPU/Intel/Core%20i7/Intel%20Core%20i7-6700K)).
- ⚠️ Intel Core i7-8550U · #1819 — mode 2500 в двух CPU runtime, опубликована только
  сравнительная таблица без версии и raw stdout ([карточка](CPU/Intel/Core%20i7/Intel%20Core%20i7-8550U)).
- ⚠️ Intel Xeon E5-4640 · #1631 — 17.6433 MH/s на четырёхсокетной системе; Hashcat Forum, DES-контекст, mode/version не указаны ([карточка](CPU/Intel/Xeon/Intel%20Xeon%20E5-4640)).
- ⚠️ Intel Core i7-1165G7 · #1411 — v7.1.2, CPU device PoCL, MD5 mode 0: 1647.2 MH/s ([карточка](CPU/Intel/Core%20i7/Intel%20Core%20i7-1165G7)).
