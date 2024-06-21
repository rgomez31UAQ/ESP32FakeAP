# ESP32FakeAP
<p align="center">
<img width="399" alt="immagine" src="https://raw.githubusercontent.com/TheKevinWang/ESP32FakeAP/main/FakeAP/esp32_fakeap_bing3.jpg">
<br>
Imagen generada por Bing Ai - "Un hacker utiliza un ESP32 para difundir un falso punto de acceso wifi. Logotipo"</p>

Al alojar cargas útiles utilizando archivos en lugar de dentro de archivos .c como muchos otros proyectos ESP32/ESP8266, es mucho más adaptable y utilizable. 
## Instalación de Arduino IDE
Descarga y descomprime lo siguiente en tu directorio de librerías de arduino (~/Documents/Arduino/libraries por defecto en windows; mkdir si no sales):
https://github.com/me-no-dev/ESPAsyncWebServer

https://github.com/me-no-dev/AsyncTCP

Entonces instala esto:
https://github.com/me-no-dev/arduino-esp32fs-plugin

Asegúrese de pulsar Herramientas->ESP32 Sketch Data Upload después de cargar el firmware para cargar los archivos web estáticos.
## Ejemplo
Por defecto, el SSID wifi es "Free Guest Wifi" y es un AP abierto. Todas las peticiones dns se redirigen al servidor web local. 
![phishing example](https://github.com/TheKevinWang/ESP32FakeAP/raw/main/FakeAP/FakeAPExample.png)

El payload de phishing de ejemplo es para una actualización del firmware de Broadcom basada en la falsa página de configuración del router de [wifiphisher](https://github.com/wifiphisher/wifiphisher). Sustituye el "hola mundo" data/broadcom-wifi-3.0.12.i586.exe por tu payload.
## TODO
Añadir phishing de credenciales
Añadir modo deauth y evil twin AP
## Disclaimer

Utilícelo sólo para pruebas de seguridad con permiso. 
