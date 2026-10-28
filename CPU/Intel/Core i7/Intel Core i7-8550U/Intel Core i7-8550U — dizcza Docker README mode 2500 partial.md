# Intel Core i7-8550U — опубликованная таблица mode 2500 (partial)

- **Процессор:** Intel Core i7-8550U CPU @ 1.80GHz (4C/8T).
- **Режим:** 2500 — WPA/WPA2 PMKID + EAPOL.
- **Команда, указанная источником:** `hashcat -m2500 -b`.
- **Версия Hashcat:** в таблице не указана.
- **Полнота:** опубликована только сравнительная таблица скоростей; raw stdout,
  настройки прогона и повторные измерения не приложены.
- **Источник:** [dizcza/docker-hashcat README, Benchmark](https://github.com/dizcza/docker-hashcat/blob/master/README.md#benchmark).

| CPU runtime | Опубликованное устройство | Скорость |
|---|---|---:|
| `intel-cpu` | Intel(R) Core(TM) i7-8550U CPU @ 1.80GHz | 11,009 H/s |
| `pocl` | pthread-Intel(R) Core(TM) i7-8550U CPU @ 1.80GHz | 7,647 H/s |

Эти числа относятся к двум backend/runtime одного процессора, а не к двум
разным моделям CPU; они остаются частичными опубликованными значениями.
