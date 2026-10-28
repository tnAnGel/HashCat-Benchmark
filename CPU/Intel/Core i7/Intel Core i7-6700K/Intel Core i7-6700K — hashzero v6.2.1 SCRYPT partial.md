# Intel Core i7-6700K — Hashcat v6.2.1 SCRYPT partial

- **Процессор:** Intel Core i7-6700K CPU @ 4.00GHz (4C/8T, Skylake).
- **Версия:** Hashcat v6.2.1.
- **Режим:** 15700 — Ethereum Wallet / SCRYPT, `N=262144`.
- **Запуск:** `hashcat.exe -b -m 15700 -D 1 -d 2`.
- **Устройство:** CPU Device #2; Intel HD Graphics 530 (Device #1) пропущена.
- **Результат:** `Speed.#2 10 H/s`.
- **Полнота:** один режим; исходное сообщение содержит опубликованный фрагмент raw stdout.
- **Источник:** [Hashcat Forum — hashcat v6.2.0 SCRYPT](https://hashcat.net/forum/showthread.php?mode=threaded&pid=52797&tid=10141).

```text
OpenCL API (OpenCL 2.1 WINDOWS) - Platform #2 [Intel(R) Corporation]
* Device #2: Intel(R) Core(TM) i7-6700K CPU @ 4.00GHz,
  48765/48829 MB (12207 MB allocatable), 8MCU
* --backend-devices=2
* --opencl-device-types=1
* --optimized-kernel-enable
Hashmode: 15700 - Ethereum Wallet, SCRYPT (Iterations: 262144)
Speed.#2.........: 10 H/s (1.65ms) @ Accel:8 Loops:1024 Thr:1 Vec:1
```

В том же сообщении есть v6.1.1, но с `Iterations: 1`; его скорость не
сопоставима с `N=262144`, поэтому сюда не перенесена.
