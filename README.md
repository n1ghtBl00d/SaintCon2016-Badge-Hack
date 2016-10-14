# SaintCon2016-Badge-Hack
My guide to hacking the 2016 SaintCon Badge


<br />


## The 2016 SaintCon Badge

![Saintcon Badge](https://saintcon.gitlab.io/SaintCon2016Badge/img/IMG_20160929_213212.jpg) 

[Official Badge Assembly Instructions](saintcon.gitlab.io/SaintCon2016Badge/assembly)

[Official Programming Instuctions](saintcon.gitlab.io/SaintCon2016Badge/flashing)


<br />


### Hardware Overview


The controller board is a [Wemos D1 mini](https://www.wemos.cc/product/d1-mini.html). It uses the [ESP8266](http://www.esp8266.com/) SOC.
The ESP8266 runs at 3.3v, but also has 5v output. It has 11 digital I/O pins and 1 analog input pin. It has integrated wifi.


The badge has 2 [7-segment, 4-digit led displays](https://www.sparkfun.com/datasheets/Components/LED/7-Segment/YSD-439AB4B-35.pdf).
All 8 digits are controlled with a [MAX7291](http://www.datasheetarchive.com/MAX7291-datasheet.html) IC. It communicates with the ESP8266 over SPI protocol.

The badge is powered by a rechargeable 2000mAh USB power bank.


<br /><br /> 


### Software Overview


The stock SaintCon program is written in Lua on the NodeMCU platform.

The [Official Programming Instuctions](saintcon.gitlab.io/SaintCon2016Badge/flashing) has a list of tools that can be used to communicate with the ESP8266.

[nodemcu-uploader.py](https://github.com/kmpm/nodemcu-uploader) does not work on Windows, so I used [ESPlorer](https://github.com/4refr0nt/ESPlorer).


ESPlorer can be used to download the .lua files from the badge for inspection and modification.


<!-- insert link to Lua hacking docs. -->


#### Programming with Arduino


Alternatively, the ESP8266 can be programmed with the Arduino IDE with native Arduino code. I was familiar with Arduino programming, so this is the route that I eventually chose.

<!-- insert link to arduino hacking docs.-->
