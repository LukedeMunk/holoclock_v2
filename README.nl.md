# HoloClock v2

[English](https://github.com/LukedeMunk/holoclock_v2/blob/master/README.md)

Code for an ESP32 based improved version of the HoloClock project of [ekaggrat](https://www.thingiverse.com/thing:570797). This code can be used for the [HoloClock v2](https://www.munkservices.com) DIY kit. Everything what you need is in the DIY kit, so it is recommended to buy. If you want to make it without the kit, you need a 3D printer and hardware components. The components needed is listed under `Hardware`. The code is mainly explained in the comments. You can test your own code and use these files as a backup. The software is tested on the following boards:

* ESP32 DEVKIT V1

## Hardware

### Electronics

A list of hardware components is given below. The circuit can be found in the 'docs' folder.

* 1x ESP32 DEVKIT V1
* 1x A4988 Motorboard
* 1x 12V xxA adapter (3.5mm/1mm DC plug)
* 1x 12V to 5V step down converter (LM7805)
* 1x PCB
* 1x DC022B Panel Mount Connector

### 3D models

A list of 3D models is given below. The printer which is used to print, is the Creality CR-10S Pro V2. Ultimaker Cura v4.12.1 is used to slice the objects. In the `hardware/3D models` folder, you can find the models. The `300x300mm_plan.stl` file can be used to print all the needed models in one batch.

* 1x `base_2`
* 1x `base_3`
* 2x `big_ring`
* 1x `frame_l`
* 1x `frame_r`
* 1x `gear_center`
* 1x `gear_hour`
* 1x `gear_motor`
* 1x `gear_side`
* 1x `needle_hour`
* 1x `needle_minute`
* 2x `roller_1`
* 2x `roller_2`
* 2x `roller_stopper`
* 4x `spacer`
* 3x `wheel_1`
* 1x `wheel_2`

### Screws and nuts

A list of the screws and nuts is given below.

* 6x `M3 screw 40mm`
* 2x `M3 screw 35mm`
* 1x `M3 screw 25mm`
* 19x `M3 4mmx5mm inserted thread`

## Software

### Prerequisites

The software is written, compiled and uploaded using the Arduino IDE (v1.8.13). You could use the online Arduino IDE or other software, but I recommend using the version you can download on [this page](https://www.arduino.cc/en/software).

### Deployment

Clone the repository, navigate to "holoclock_v2/HoloClock" folder and open "holoClock.ino". Upload to the ESP32.

Then use [this tool](https://randomnerdtutorials.com/install-esp32-filesystem-uploader-arduino-ide/) to upload the webserver files (.html, .css, etc.) to the ESP32.

Connect to the `Configureer klok` network and fill in the password `clock1234`. Go to a browser and search for `192.168.4.1` and connect to a wifi network.
After a reboot, go to a (mobile) browser and search `http://clock`. Here you can control the clock.

## Questions or feedback?

You can submit an issue if you have questions or feedback for this repository. If you are interested in more of my projects, checkout my [GitHub profile](https://github.com/LukedeMunk). If you are interested in hiring me, checkout my [LinkedIn](https://www.linkedin.com/in/luke-de-munk/) or [website](https://www.munkservices.com).

## Authors

* **Luke de Munk** - *Head author of software* - [LinkedIn](https://www.linkedin.com/in/luke-de-munk/)
* **ekaggrat** - *Creator of original project* - [ekaggrat](https://www.thingiverse.com/thing:570797)

<!-- ## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details -->