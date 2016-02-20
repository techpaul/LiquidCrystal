# LiquidCrystal
## Liquid Crystal Library for Arduino higher performance

License as per standard Creative Commons for Arduino libraries

Has been submitted as Pull request on Arduino https://github.com/arduino/Arduino/pull/4550

Sorts some bugs with chip handlling, so delaying 100 us between each nibble of an 8 bit write when should be 1 us. Other fixes to get the delay times between commands to actually *NOT* block operation and reduce delays to sensible level of 40 us.

If you have a slower display there is an extra method to extend LCD command delay time to any value between 40 and 250 us.

See timings.txt which details tests and performance increase.

Some scope shot images in images folder, for differences.

## Installation

Copy LiquidCrystal.h and LiquidCrystal.cpp to your Arduino/Libraries/LiquidCrystal folder

Restart Arduino IDE and recompile your sketch and restest.
