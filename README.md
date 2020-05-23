
<h1 align="center">
  <a name="logo" href="https://github.com/fastender/homeassistant"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/the%20blob.gif" alt="The Blob" width="200"></a>
  <br>
  The Blob<br></br>
</h1>


<h3 align="center"><font size="8">
As a home server, the Blob <br>is the on-board computer for the intelligent building.</h3>
  
<h4 align="center">
  <img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/case.jpg" alt="The Blob" width="200">
</h4>

<p align="center"><font size="4">The Blob connects the electrical installation of the house with the computer network and the Internet. In this way it enables central control of intelligent building technology via a large number of operating devices - regardless of location. In addition, numerous other technologies such as door intercoms, cameras and audio systems as well as third-party systems for the sanitary, kitchen and entertainment areas can be seamlessly integrated into the building control system.<br></br>The Blob is designed to provide numerous advantages such as the benefits of mobile technology control, as well as the full experience with maximum convenience, security and energy efficiency. At the same time, the sexy Home Assistant interface makes the control of intelligent technology a pleasure by allowing complex systems to be controlled easily - with just one finger.</p>





<!-- TABLE OF CONTENTS -->
## Table of Contents

* [Hardware](#hardware)
* [Software](#software)
* [Devices](#devices)
* [Todo List](#todo-list)
* [Home Assistant](#home-assistant)
  * [Lovelace](#lovelace)
  * [Automations](#automations)




<!-- HARDWARE -->
## Hardware
My priority when selecting the hardware was a power-saving system. Usually a combination of a small motherboard with a relatively weak but power saving processor still outperforms the usual ready to use NAS devices. 

Look to the sexy Inter-Tech X-608 Infinity Mirror RGB PC Case, with a "Black Hole" on the front and awesome RGB lighting effects. [See it in the Dark](https://www.youtube.com/watch?v=olyw9uxEDu8)

<p align="center">
  <a name="case" href="https://github.com/fastender/homeassistant"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/case.gif" alt="Inter-Tech X-608 Mid Tower Case" width="200"></a>
  <br>
</p>

As a suitable mainboard/CPU combination I decided for the [ASRock J5005-ITX](https://www.amazon.de/Asrock-J5005-MB-Intel-Gemini-Lake/dp/B079G91MQ1/ref=cm_cr_arp_d_product_top?ie=UTF8) with current Intel Gemini Lake architecture. The board has four SATA connectors. Currently one SSD and two hard disks are connected. The maximum power consumption of the board is 10 Watt.

Connected are beside the [SanDisk Cruzer Fit Z33 16GB USB stick](https://www.amazon.de/SanDisk-Cruzer-16GB-USB-Stick-schwarz/dp/B005FYNSZA) with 2x [Seagate SkyHawk 10 TB](https://www.amazon.de/Seagate-ST10000VX0004-SkyHawk-interne-Festplatte/dp/B01IAY6AC4). 2x8 GB RAM from [Crucial](https://www.amazon.de/Crucial-CT8G4SFS824A-Speicher-PC4-19200-260-Pin/dp/B01BIWKP58/ref=sr_1_3?__mk_de_DE=ÅMÅŽÕÑ&dchild=1&keywords=Crucial+CT8G4SFS824A&qid=1590216768&s=computers&sr=1-3) and an SSD from [Samsung 850 EVO](https://www.amazon.de/Samsung-MZ-75E500B-EU-interne-schwarz/dp/B00P73B1E4/ref=sr_1_3?__mk_de_DE=ÅMÅŽÕÑ&dchild=1&keywords=850+evo+500&qid=1590216809&s=computers&sr=1-3) are used.

My current system consumes about 26 watts when idle and with rotating hard drives. If the device is in continuous operation, the electricity costs amount to approx. 5.30€/month or 64€/year at an electricity price of 0.28€/kWh. So you don't become poor with the electricity costs, especially since the system replaces many different services that are subject to charges.


<!-- SOFTWARE -->
## Software
As operating system I use the Linux distribution [unRaid](https://unraid.net).

unRAID is in my opinion the best NAS operating system (apart from the finished NAS systems) I have come across so far, if you are looking for an easy and uncomplicated use. Similar to Apple's motto "it simply works", you don't have to deal with the terminal or anything like that. For everything there is a simple and clear UI. If you ever need help or a feature is missing, the community is very helpful, whether via the App Store or simply with advice.

<p align="center">
  <a name="logo" href="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/unraid-1.png"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/unraid-1.png" alt="Unraid - Dashboard" width="200"></a>
  <br>
  Unraid - Dashboard<br>
</p>

unRaid provides network storage for the media, which also allows streaming to 1-3 devices simultaneously. The system is low-maintenance and no exaggerated previous knowledge is necessary.

<p align="center">
  <a name="logo" href="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/unraid-2.png"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/unraid-2.png" alt="Unraid - Main" width="200"></a>
  <br>
  Unraid - Main<br>
</p>

For the OS the USB stick is used, the SSD serves as a cache and hosts the data of dockers and VMs. The hard drives contain the data used by the Plex, for example.

<!-- DEVICES -->
## Devices
I have invested a lot in the past few years to buy the equipment at home.

For me it was important from the beginning that all electrical devices can be operated by one system: Voice Control and Home Assistant. 

[Alexa Echo Dot](https://www.amazon.de/Echo-Dot-3-Gen-Intelligenter-Lautsprecher-mit-Alexa-Anthrazit-Stoff/dp/B07PHPXHQS) is used for voice control, but Siri can also be used at any time. 

2x [SONOS Play 3](https://www.sonos.com/de-de/products/wireless-speakers) are used as speakers, which are connected to the [Apple TV](https://www.apple.com/de/shop/buy-tv/apple-tv-hd/32-gb). For security 3x [Arlo Ultra 4k](https://www.arlo.com/de/products/arlo-ultra/default.aspx) cameras are used. The CO monitoring is done by three [Nest](https://store.google.com/de/product/nest_protect_2nd_gendevices). The alarm is secured via [Somfy](https://www.somfy.de/produkte/sicherheit/vernetzte-sicherheitslosungen-fur-ihr-zuhause).

In addition to over 50 [Philips Hue](https://www2.meethue.com/de-de/product-overview) and [Ikea lamps](https://www.ikea.com/de/de/p/tradfri-led-leuchtmittel-e27-600-lm-kabellos-dimmbar-farb-und-weissspektrum-farb-und-weissspektrum-rund-opalweiss-00408612/), various sensors for movement, water monitoring, door and window monitoring of the brand [Aqara](https://www.aqara.com/us/home.html), as well as smart sockets from [OSRAM](https://www.amazon.de/Osram-schaltbare-fernbedienbar-Lichtsteuerung-kompatibel/dp/B074PZLX2Pare) used. [EVE Aqua](https://www.evehome.com/de/eve-aqua) is used for watering the garden.

Smart [Ikea roller blinds](https://www.ikea.com/de/de/p/kadrilj-rollo-kabellos-batteriebetrieben-grau-80408123/) are used. Older electric roller blinds are made smart via [SwitchBot](https://www.switch-bot.com).
<hr>

#### <a name="Hardware"></a>The smarthome is actually mainly controlled by these main actors in terms of hardware:
* [ConBee II](https://www.amazon.de/ConBee-das-universelle-Zigbee-USB-Gateway/dp/B07PZ7ZHG5) - For the control of the SmartHome devices ConBee II is used as Zigbee USB gateway . It combines manufacturer-independent all the used Philips Hue, IKEA Trådfri, OSRAM Lightify, Xiaomi Aqara and many other Zigbee products.

* [VERA Plus Smart Home Controller](https://www.amazon.de/Vera-Smart-Gateway-Überwachungstechnik-MCVEVERA_Plus/dp/B01BVLVGZY) is used to control the Z-Wave devices, especially for the [FIBARO Roller Shutter 3 control](https://www.amazon.de/FIBARO-FIBEFGR-223-Roller-Shutter-3/dp/B07L5S38RN/ref=sr_1_1_sspa?__mk_de_DE=ÅMÅŽÕÑ&dchild=1&keywords=roller+shutter+3&qid=1590218162&quartzVehicle=72-820&replacementKeywords=roller+shutter&sr=8-1-spons&psc=1&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUEyWTBLN1NOVk9DQjJUJmVuY3J5cHRlZElkPUEwOTUxNjQzMUI1QkFTRkVSVDdPMiZlbmNyeXB0ZWRBZElkPUEwMjA2MTMwMzRWMU1YSVFNNjc3OSZ3aWRnZXROYW1lPXNwX2F0ZiZhY3Rpb249Y2xpY2tSZWRpcmVjdCZkb05vdExvZ0NsaWNrPXRydWU=).

<!-- HOME ASSISTANT -->
## Home-Assistant
Hass.io was installed on a virtual [Ubuntu Server 18.04](https://ubuntu.com/download/server) according to these [instructions](https://www.juanmtech.com/set-up-hassio-in-docker-and-in-an-ubuntu-server/). The ConBee II USB stick is attached to the Hass.io VM using Unraid USB pass-through.

Look to the sexy Inter-Tech X-608 Infinity Mirror RGB PC Case, with a "Black Hole" on the front and awesome RGB lighting effects. [See it in the Dark](https://www.youtube.com/watch?v=olyw9uxEDu8).

<p align="center">
  <a name="case" href="https://github.com/fastender/homeassistant"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/case.gif" alt="Inter-Tech X-608 Mid Tower Case" width="200"></a>
  <br>
</p>

<!-- LOVELACE -->
## Lovelace
When designing the operation, it was very important for me to use a simple, minimalist system. It should not be overloaded and understandable.

I was very much inspired by [Mattias Persson](https://github.com/matt8707/hass-config) when designing the Lovelace. I would also like to say that without the really very helpful integrations of and 
my design could never be realized. 

<p align="center">
  <a name="case" href="https://github.com/matt8707/hass-config"><img src="https://raw.githubusercontent.com/matt8707/hass-config/master/www/img/s_main.png" alt="Inter-Tech X-608 Mid Tower Case" width="200"></a>
    <a name="case" href="https://github.com/matt8707/hass-config"><img src="https://raw.githubusercontent.com/matt8707/hass-config/master/www/img/s_main.png" alt="Inter-Tech X-608 Mid Tower Case" width="200"></a>
    <a name="case" href="https://github.com/matt8707/hass-config"><img src="https://raw.githubusercontent.com/matt8707/hass-config/master/www/img/s_main.png" alt="Inter-Tech X-608 Mid Tower Case" width="200"></a>
  <br>
</p>

<!-- AUTOMATIONS -->
## Automations
My priority when selecting the hardware was a power-saving system. Usually a combination of a small motherboard with a relatively weak but power saving processor still outperforms the usual ready to use NAS devices. 

![Screenshot of Home Assistant Header](https://i.imgur.com/vjDH1LJ.png)

Look to the sexy Inter-Tech X-608 Infinity Mirror RGB PC Case, with a "Black Hole" on the front and awesome RGB lighting effects. [See it in the Dark](https://www.youtube.com/watch?v=olyw9uxEDu8)

<p align="center">
  <a name="case" href="https://github.com/fastender/homeassistant"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/case.gif" alt="Inter-Tech X-608 Mid Tower Case" width="200"></a>
  <br>
</p>


