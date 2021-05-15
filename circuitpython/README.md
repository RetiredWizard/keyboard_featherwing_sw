# Keyboard FeatherWing CircuitPython Code

This folder contains example CircuitPython code for the Keyboard FeatherWing

Here are the libraries needed for the code to work properly:

==== BASE ====
| Functionality  | Name                      | Source |
|----------------------|---------------------------|--------|
| Common         | `adafruit_bus_device`     | https://github.com/adafruit/Adafruit_CircuitPython_BusDevice |
| Keyboard       | `bbq10keyboard`           | https://github.com/arturo182/arturo182_CircuitPython_BBQ10Keyboard |
| LCD            | `adafruit_ili9341`        | https://github.com/adafruit/Adafruit_ILI9341 |
| Neopixel       | `neopixel`                | https://github.com/adafruit/Adafruit_CircuitPython_Neopixel |
| SD Card        | `adafruit_sdcard`         | https://github.com/adafruit/Adafruit_CircuitPython_SD |
| Touch Display Rev 1  | `adafruit_stmpe610`       | https://github.com/adafruit/Adafruit_CircuitPython_STMPE610 |
| Touch Driver Rev 2   | `tsc2004`                 | https://github.com/solderparty/arturo182_CircuitPython_tsc2004 |
| Graphic Label  | `adafruit_display_text`   | https://github.com/adafruit/Adafruit_CircuitPython_Display_Text |
| Graphic Shapes       | `adafruit_display_shapes` | https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes |

The `factory_test.py` file also has an optional dependency to `adafruit_pct2075` from https://github.com/adafruit/Adafruit_CircuitPython_PCT2075

Files in this folder:
 - `factory_test.py` - The test used to check all peripherals on the board, works for Rev 1 and Rev 2
 - `uart_demo.py` - A simple UART demo, you can send text over UART using the keyboard and see what is received
 - `kfw_pico_board.py` - A compability layer for the Raspberry Pi Pico Adapter board. Import this as `board` and you can use the standard Feather pin names.

All the code has been tested with CircuitPython 6.0 on the Adafruit Feather M4 Express and the Solder Party Raspberry Pi Pico KFW Adapter.