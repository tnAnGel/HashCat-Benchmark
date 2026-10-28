# NVIDIA Quadro RTX 4000 — mode 22000

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Quadro RTX 4000, 8 GB
- **Конфигурация / Setup:** 1 GPU
- **Версия hashcat / Version:** v7.1.2
- **Источник / Source:** [GermanAizek gist — комментарий tuxevil от 31.05.2026](https://gist.github.com/GermanAizek/f968d0bb213b2b7c8d9b35bbc4d031e4)
- **Параметры / Options:** benchmark mode 22000; CUDA 13.3; `--backend-devices-virtmulti=1 --backend-devices-virthost=1 --optimized-kernel-enable`
- **Примечание / Note:** вывод сообщает, что оптимизированное ядро для mode 22000 недоступно, поэтому Hashcat переключился на pure kernel. Это валидный одиночный режим, не полный GPU benchmark.

## Результат / Result

```text
hashcat (v7.1.2) starting in benchmark mode
* Device #01: Quadro RTX 4000, 7695/7795 MB, 36MCU
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
Speed.#01........: 462.6 kH/s (89.10ms) @ Accel:9 Loops:1024 Thr:512 Vec:1
```
