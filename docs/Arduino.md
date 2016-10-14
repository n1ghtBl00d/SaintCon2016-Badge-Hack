# Programming the Badge with Arduino


The ESP8266 is a fairly common SOC, and others have already done most of the work for us.


## Setting up the Arduino IDE


The ESP8266 Community made an Arduino code compiler for the ESP8266. The complete installation instructions are at <https://github.com/esp8266/Arduino>


**To Install the ESP8266 Packages for Arduino:**

>Install Arduino 1.6.8 from the Arduino website.

>Start Arduino and open Preferences window.

>Enter http://arduino.esp8266.com/stable/package_esp8266com_index.json into Additional Board Manager URLs field. You can add multiple URLs, separating them with commas.

>Open Boards Manager from Tools > Board menu and install esp8266 platform (and don't forget to select your ESP8266 board from Tools > Board menu after installation).


To prepare the Arduino IDE for uploading code to the badge, Set the board at `Tools > Board` to `Wemos D1 Mini`

Then Set the COM Port at `Tools > Port` to the COM Port of your badge. This can be found in Device Manager when the badge is plugged in.