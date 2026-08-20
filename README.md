# esp32s3-I2S-Audio-player-from-SD-and-USB
esp32s3 I2S Audio player from SD and USB
При первом запуске:
1. ESP32 создаёт сеть ESP-Player-Setup.
2. Телефон подключается к ней.
3. Открывается страница настройки со сканированием доступных Wi‑Fi.
4. Выбираете свою сеть и вводите пароль.
5. Настройки сохраняются во flash.
6. В дальнейшем устройство подключается автоматически.
Страница плеера будет доступна по адресу:
http://esp-player.local/


bootloader.bin   → 0x0000

partitions.bin   → 0x8000

firmware.bin     → 0x10000

Pins:

-SD-

#define SD_CS 39

#define SD_SCK 41

#define SD_MOSI 40

#define SD_MISO 42


-Audio-

#define AUDIO_I2S_BCLK  16

#define AUDIO_I2S_DOUT  17

#define AUDIO_I2S_LRCLK 18


-USB-

D- 19

D+ 20
