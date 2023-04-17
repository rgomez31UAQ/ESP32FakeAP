# ESP32FakeAP

![Craiyon AI generated logo](https://github.com/TheKevinWang/ESP32FakeAP/raw/main/FakeAP/craiyon_logo.png)
Craiyon.com Ai generated picture - "A hacker is using an ESP32 to broadcast a fake wifi access point. Logo."

By hosting payloads using files instead of inside .c files like many other ESP32/ESP8266 projects, it's a lot more adaptable and usable. 

## Arduino IDE installation

Download and unzip the following into your arduino libraries directory (~/Documents/Arduino/libraries by default on windows; mkdir if not exit):

https://github.com/me-no-dev/ESPAsyncWebServer

https://github.com/me-no-dev/AsyncTCP

Then install this:

https://github.com/me-no-dev/arduino-esp32fs-plugin

Make sure to hit Tools->ESP32 Sketch Data Upload after uploading firmware to upload the static web files.

## Example

![phishing example](https://github.com/TheKevinWang/ESP32FakeAP/raw/main/FakeAP/FakeAPExample.png)

The example phishing payload is for a Broadcom firmware update based on [wifiphisher](https://github.com/wifiphisher/wifiphisher)'s fake router configuration page. Replace the "hello world" data/broadcom-wifi-3.0.12.i586.exe with your payload.

## TODO
Add deauth and evil twin AP mode
