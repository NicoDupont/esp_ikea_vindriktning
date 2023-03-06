## Domotisation et amélioration du module Ikea Vindriktning

Domotisation du ikea vindriktning qui possede un sensor de particule 2.5 pm1006.  

Ajouts :
 - BME280 (temperature+humidité+pression) 
 - CCS811 (eCo2+Tvoc)
 - MICS-5524 (CO) formule de calcul pour le CO a confirmer
 - Esp8266 / Esp01s firmware esphome

### Liste des composants :

- 1x ftdi 3.3v (pour le 1er flash)
- 1x esp8266 esp01s + breakout board
- 1x convertisseur dc 5v=>3.3v (ams1117)
- 1x BME280 (3.3v)
- 1x CCS811 (3.3v)
- 1x ADS1115 (5v) + levelshifter (i2c 3.3v<=>5v)
- 1x MICS-5524 (5v)
### Cablage :

GPIO 0 et 2 => i2c  
GPIO 1 => pm1006 (lecture uniquement via la liaison série)  
CCS811 => baseline a renseigner. voir la [doc esphome](https://esphome.io/components/sensor/ccs811.html) 

![links](https://github.com/NicoDupont/esp_ikea_vindriktning/blob/main/img/shema.png?raw=true)

### Montage :

Prototype :  
![proto](https://github.com/NicoDupont/esp_ikea_vindriktning/blob/main/img/proto.jpg?raw=true)  
Pcb Soudé :  
![pcb](https://github.com/NicoDupont/esp_ikea_vindriktning/blob/main/img/pcbfinal.jpeg?raw=true)  
Integration dans le boitier :  
![integration](https://github.com/NicoDupont/esp_ikea_vindriktning/blob/main/img/pcbintegre.jpg?raw=true)


### HomeAssistant :

![links](https://github.com/NicoDupont/esp_ikea_vindriktning/blob/main/img/entite.png?raw=true)

#### Quelques liens :
- Home Assistant : [HomeAssistant](https://www.home-assistant.io/) 
- Esphome : [Esphome](https://esphome.io/index.html) 
- Esphome-flasher : [Esphome-flasher](https://github.com/esphome/esphome-flasher/releases)
- Lib dfrobot pour le mics5524 : [dfrobot](https://wiki.dfrobot.com/Fermion__MEMS_Gas_Sensor___MiCS-5524_SKU_SEN0440)
    






