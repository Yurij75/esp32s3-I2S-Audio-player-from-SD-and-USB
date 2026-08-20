# esp32s3-I2S-Audio-player-from-SD-and-USB
esp32s3 I2S Audio player from SD and USB
1. При отсутствии сохранённой сети создаётся Wi‑Fi:
ESP-Player-Setup
2. Страница настройки:
http://192.168.4.1/
3. Сети сканируются на самой странице.
4. Введённые SSID и пароль сохраняются во flash.
5. После перезапуска ESP32 подключается автоматически.
6. Адрес плеера выводится в Serial Monitor:
WiFi OK, открой в браузере: http://192.168.0.xxx/


bootloader.bin   → 0x0000

partitions.bin   → 0x8000

firmware.bin     → 0x10000

Pins:

*SD*

#define SD_CS 39

#define SD_SCK 41

#define SD_MOSI 40

#define SD_MISO 42


*Audio*

#define AUDIO_I2S_BCLK  16

#define AUDIO_I2S_DOUT  17

#define AUDIO_I2S_LRCLK 18


*USB*

D- 19

D+ 20

Также подключить питание ко всем устройствам в зависимости от модификации. USB подать 5 волбт.
