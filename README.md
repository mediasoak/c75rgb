I cannot get this keyboard's LEDs to produce anything other than blinding white light.
The source files the manufacturer gave me use RGBLIGHT in keyboard.json instead of RGB_MATRIX, but even using RGBLIGHT myself I only get white light.
I think I'm missing information on the WS2812 driver. I have the pins correctly configured, but what if the driver is also using PWN or STI?
Or the problem could be something else entirely; I'm only a novice, after all.

Thu 2 Jul 2026
The following troubleshooting changes have been made:
added "driver": "pwm" under "ws2812" in keyboard.json
added a keyboard level config.h file containing zvecr's configs
added today's QMK MSYS error output
