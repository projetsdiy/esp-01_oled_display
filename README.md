# Comment relier un écran OLED I2C et un ESP-01 (ESP8266)
Tutoriel rapide pour apprendre comment relier un mini écran OLED (SSD1306) sur un module ESP8266 ESP-01.
Lire l'article complet sur Projets DIY http://www.projetsdiy.fr/scanner-wifi-ecran-oled-i2c-ssd1306-esp01-esp8266/
<h2>Matériel nécessaire </h2>
Pour réaliser ce projet vous aurez besoin des éléments suivants :
- <a href="http://geni.us/3GoD" target="_blank" rel="nofollow" data-mce-href="http://geni.us/3GoD">Un module ESP-01</a>
- <a href="http://geni.us/pyN" target="_blank" rel="nofollow" data-mce-href="http://geni.us/pyN">Un module FTDI</a>
- <a href="http://geni.us/1VsC" target="_blank" rel="nofollow" data-mce-href="http://geni.us/1VsC">Un Ecran OLED I2C 0.96'' monochrome (basé sur le chipset SSD1306)</a>
- Des Jumpers Dupont
- Un bouton poussoir (Reset optionnel)
- Une résistance 220 ohms (optionnel)
<h2>Circuit pour téléverser le programme </h2>
La programmation de l'ESP-01 se déroule en deux temps. Branchez tout d'abord votre ESP comme ceci pour que l'ESP-01 démarre en mode bootload. Avant de téléverser le programme, modifiez les variables ssid et password de votre réseau.

<h2>Brancher l'écran OLED</h2>
Maintenant que le code a été téléversé dans l'ESP-01, on peut brancher l'écran OLED sur l'ESP-01 comme ceci
- SDA <--> GPIO0
- SCK <--> GPIO2
- GND <--> GND
- VCC <--> 3.3V
A la mise sous tension de l'ESP, le programme de scanner WiFi démarre et affiche après quelques secondes le réseau sur lequel l'ESP-01 est connecté, l'adresse ip de ce dernier ainsi que la force du signal.
