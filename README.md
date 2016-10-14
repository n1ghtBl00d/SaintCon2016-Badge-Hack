# SaintCon2016-Badge-Hack
My guide to hacking the 2016 SaintCon Badge

## The 2016 SaintCon Badge
<!-- Insert Image-->
[Official Badge Assembly Instructions](saintcon.gitlab.io/SaintCon2016Badge/assembly)
[Official Programming Instuctions](saintcon.gitlab.io/SaintCon2016Badge/flashing)


### Hardware Overview


The controller board is a [Wemos D1 mini](https://www.wemos.cc/product/d1-mini.html). It uses the [ESP8266](http://www.esp8266.com/) SOC.
The ESP8266 runs at 3.3v, but also has 5v output. It has 11 digital I/O pins and 1 analog input pin. It has integrated wifi.


The badge has 2 7-segment, 4-digit led displays.
All 8 digits are controlled with a MAX7291 IC. It communicates with the ESP8266 over SPI protocol.

The badge is powered by a rechargeable 2000mAh USB power bank.
