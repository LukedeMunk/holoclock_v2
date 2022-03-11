# HoloClock v2
[English](README.md)

Een op ESP32 gebaseerde, verbeterde versie van het HoloClock project van [ekaggrat](https://www.thingiverse.com/thing:570797). Deze code kan worden gebruikt voort de [HoloClock v2](https://technicbuilds.munkservices.com/) bouwset. Alles wat je nodig hebt zit bij de bouwset, dus het wordt aanbevolen om die te kopen. Als je de klok zelf wil bouwen zonder bouwset, heb je een 3D printer en hardware componenten nodig. De componenten zijn te vinden onder het kopje `Hardware`. De code is grotendeels verklaard met comments, maar er is ook een document [hier](docs/code_documentation) te vinden. Je kan je eigen code testen en deze code gebruiken als backup. De software is getest op de volgende borden:

* ESP32 DEVKIT V1

## Hardware

### Elektronica

Hieronder is een lijst van de benodigde elektronische componenten te vinden. Het circuit kan gevonden worden in de `docs` map.

* 1x ESP32 DEVKIT V1
* 1x A4988 motorboard
* 1x 28BYJ-48 12V motor
* 1x 12V 2A adapter (3.5mm/1mm DC plug)
* 1x 12V to 5V step down converter (LM7805)
* 1x PCB
* 1x DC022B Panel Mount Connector

### 3D objecten

Hieronder is een lijst van de benodigde 3D objecten te vinden. De printer die gebruikt is, is de Creality CR-10S Pro V2. Ultimaker Cura v4.12.1 is gebruikt voor het slice van de objecten. In de `hardware/3D models` map kan je de modellen vinden.

* 1x `base_1`
* 1x `base_2`
* 2x `big_ring`
* 1x `frame_l`
* 1x `frame_r`
* 1x `gear_center`
* 1x `gear_hour`
* 1x `gear_motor`
* 2x `gear_side`
* 1x `joiner_7mm`
* 1x `joiner_10mm`
* 3x `joiner_13mm`
* 1x `needle_hour`
* 1x `needle_minute`
* 1x `PCB_helper` (Optioneel)
* 2x `roller_1`
* 2x `roller_2`
* 2x `roller_stopper`
* 2x `spacer_10mm`
* 2x `spacer_14mm`
* 2x `spacer_30mm`
* 2x `spacer_middle`
* 3x `wheel_1`
* 1x `wheel_2`

### Bouten en inserted threads

Hieronder is een lijst van de benodigde bouten en inserted threads te vinden.

* 2x `M3 screw 5mm`
* 1x `M3 screw 25mm`
* 2x `M3 screw 30mm`
* 6x `M3 screw 40mm`
* 19x `M3 4mmx5mm inserted thread`

## Software

### Inleiding

De software is geschreven, gecompileerd en geüploaded met de Arduino IDE (v1.8.13). Je zou de online Arduino IDE of andere software kunnen gebruiken, maar het wordt aanbevolen om [deze](https://www.arduino.cc/en/software) versie te gebruiken.

### Installeren

Clone de repository, ga naar de map `holoclock_v2/HoloClock`  en open `holoClock.ino`. Upload naar de ESP32. Een uitgebreide tutorial is [hier](https://randomnerdtutorials.com/installing-the-esp32-board-in-arduino-ide-windows-instructions/) te vinden.

Gebruik dan [deze tool](https://randomnerdtutorials.com/install-esp32-filesystem-uploader-arduino-ide/) om de webserver bestanden (.html, .css, etc.) te uploaden naar de ESP32.

Verbind met het `Configure clock` netwerk en vul het wachtwoord `clock1234` in. Ga naar een browser en typ in de urlbalk `192.168.4.1` (of `http://clock`) en verbind met een wifi netwerk.
Na een herstart, ga naar een (mobiele) browser en typ in de urlbalk `http://clock`. Hier kan je de klok bedienen.

## Vragen of feedback?

Je kan een issue aanmaken als je vragen of feedback hebt voor deze repository. Als je geïnteresseerd bent in meer projecten van mij, check mijn [GitHub profiel](https://github.com/LukedeMunk). Als je geïnteresseerd bent om mij in te huren, check mijn [LinkedIn](https://www.linkedin.com/in/luke-de-munk/) of [website](https://www.munkservices.com). Dit product kopen? Bezoek de [TechnicBuilds](https://technicbuilds.munkservices.com/) website.

## Authors

* **Luke de Munk** - *Hoofdauteur van de software* - [LinkedIn](https://www.linkedin.com/in/luke-de-munk/)
* **ekaggrat** - *Maker van het originele project* - [ekaggrat](https://www.thingiverse.com/thing:570797)

<!-- ## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details -->