## Domotisation et amélioration du module Ikea Vindriktning

Domotisation du ikea vindriktning qui possede un sensor de particule 2.5 pem1006.  
Ajouts :
 - BME280 (temperature+humidité+pression)
 - CCS811 (eCo2+Tvoc)

### Liste des composants :

- 1x ftdi 3.3v (pour le 1er flash)
- 1x esp8266 esp01s + breakout board
- 1x convertisseur dc 5v=>3.3v (ams1117)
- 1x fusible 20x5 0.5A + porte fusible
- 1x BME280
- 1x CCS811
- 1x pcb 2.54mm, du cable, etc...

### Cablage :

GPIO 0 et 2 => i2c  
GPIO 1 => 

![links](https://github.com/NicoDupont/esp_remplissage_cuve/blob/main/img/shema.png?raw=true)

### Montage :

![pcb](https://github.com/NicoDupont/esp_remplissage_cuve/blob/main/img/pcbok.jpg?raw=true)
![integration](https://github.com/NicoDupont/esp_remplissage_cuve/blob/main/img/boxpcb.jpg?raw=true)


### HomeAssistant :

#### Entités :

![links](https://github.com/NicoDupont/esp_remplissage_cuve/blob/main/img/entite.png?raw=true)

#### Quelques liens :
- Home Assistant : [HomeAssistant](https://www.home-assistant.io/) 
- Esphome : [Esphome](https://esphome.io/index.html) 
- Esphome-flasher : [Esphome-flasher](https://github.com/esphome/esphome-flasher/releases)
    






