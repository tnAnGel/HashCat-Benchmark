# NVIDIA GeForce GTX 965M

- **Видеокарта / GPU:** NVIDIA GeForce GTX 965M
- **Статус коллекции:** ⬜ стандартный benchmark `hashcat -b` не подтверждён
- **Источник устройства:** [hashcat forum — GTX 965M обнаружена, запуск завершился ошибкой OpenCL](https://hashcat.net/forum/thread-5881.html)
- **Внешний ориентир:** [таблица Hashcat-ng](https://gist.github.com/GermanAizek/f968d0bb213b2b7c8d9b35bbc4d031e4) приводит значение `93515`.
- **Ограничение:** таблица относится к Hashcat-ng, проприетарному форку для WPA-PBKDF2-PMKID+EAPOL; единица и методика этого значения в источнике не описаны. Оно не записывается как скорость официального hashcat.

Форумный вывод показывает GTX 965M в списке устройств, однако `clCreateContext()` завершился ошибкой до измерения скорости.
