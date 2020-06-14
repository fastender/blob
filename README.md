
<h1 align="center">
  <a name="logo" href="https://github.com/fastender/homeassistant"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/the%20blob.gif" alt="The Blob" width="200"></a>
  <br>
  The Blob - I Am Your House<br></br>
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
* [Home Assistant](#home-assistant)
  * [Lovelace](#lovelace)
  * [Automations](#automations)
* [To-Do-List](#To-Do-List)


<!-- HARDWARE -->
## Hardware
My priority when selecting the hardware was a power-saving system. Usually a combination of a small motherboard with a relatively weak but power saving processor still outperforms the usual ready to use NAS devices. 

Look to the sexy Inter-Tech X-608 Infinity Mirror RGB PC Case, with a "Black Hole" on the front and awesome RGB lighting effects. [See it in the Dark](https://www.youtube.com/watch?v=olyw9uxEDu8).

<p align="center">
  <a name="case" href="https://github.com/fastender/homeassistant"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/case.gif" alt="Inter-Tech X-608 Mid Tower Case" width="200"></a>
  <br>
</p>

As a suitable mainboard/CPU combination I decided for the [ASRock J5005-ITX](https://www.amazon.de/Asrock-J5005-MB-Intel-Gemini-Lake/dp/B079G91MQ1/ref=cm_cr_arp_d_product_top?ie=UTF8) with current Intel Gemini Lake architecture. The board has four SATA connectors. Currently one SSD and two hard disks are connected. The maximum power consumption of the board is 10 Watt.

Connected are beside the [SanDisk Cruzer Fit Z33 16GB USB stick](https://www.amazon.de/SanDisk-Cruzer-16GB-USB-Stick-schwarz/dp/B005FYNSZA) with 2x [Seagate SkyHawk 10 TB](https://www.amazon.de/Seagate-ST10000VX0004-SkyHawk-interne-Festplatte/dp/B01IAY6AC4). 2x8 GB RAM from [Crucial](https://www.amazon.de/Crucial-CT8G4SFS824A-Speicher-PC4-19200-260-Pin/dp/B01BIWKP58/ref=sr_1_3?__mk_de_DE=ÅMÅŽÕÑ&dchild=1&keywords=Crucial+CT8G4SFS824A&qid=1590216768&s=computers&sr=1-3) and an SSD from [Samsung 850 EVO](https://www.amazon.de/Samsung-MZ-75E500B-EU-interne-schwarz/dp/B00P73B1E4/ref=sr_1_3?__mk_de_DE=ÅMÅŽÕÑ&dchild=1&keywords=850+evo+500&qid=1590216809&s=computers&sr=1-3) are used.

My current system consumes about 26 watts when idle and with rotating hard drives. If the device is in continuous operation, the electricity costs amount to approx. 5.30€/month or 64€/year at an electricity price of 0.28€/kWh. So you don't become poor with the electricity costs, especially since the system replaces many different services that are subject to charges.


<!-- SOFTWARE -->
## Software
As operating system I use the Linux distribution [unRAID](https://unraid.net).

unRAID is in my opinion the best NAS operating system (apart from the finished NAS systems) I have come across so far, if you are looking for an easy and uncomplicated use. Similar to Apple's motto "it simply works", you don't have to deal with the terminal or anything like that. For everything there is a simple and clear UI. If you ever need help or a feature is missing, the community is very helpful, whether via the App Store or simply with advice.

<p align="center">
  <a name="logo" href="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/unraid-1.png"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/unraid-1.png" alt="unRAID - Dashboard" width="200"></a>
  <br>
  unRAID - Dashboard<br>
</p>

unRaid provides network storage for the media, which also allows streaming to 1-3 devices simultaneously. The system is low-maintenance and no exaggerated previous knowledge is necessary.

<p align="center">
  <a name="logo" href="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/unraid-2.png"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/unraid-2.png" alt="unRAID - Main" width="200"></a>
  <br>
  unRAID - Main<br>
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

<!-- LOVELACE -->
## Lovelace
When designing, it was very important for me to use a simple, minimalist system. It should not be overloaded and should be understandable.

<p align="center">
  <a name="Mattias Persson" href="https://github.com/matt8707/hass-config"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/Mattias Persson.png" alt="Mattias Persson" width="200"></a>
    <a name="Thomas Lovén" href="https://github.com/thomasloven"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/Thomas Lovén.png" alt="Thomas Lovén" width="200"></a>
    <a name="Custom cards for Home Assistant" href="https://github.com/custom-cards"><img src="https://raw.githubusercontent.com/fastender/homeassistant/master/logos/Custom cards for Home Assistant.png" alt="Custom cards for Home Assistant" width="200"></a>
</p>

I was very much inspired by [Mattias Persson](https://github.com/matt8707/hass-config) when designing the Lovelace. I would also like to say that without the really very helpful integrations of the ingenious [Thomas Lovén](https://github.com/thomasloven) and [Custom cards for Home Assistant](https://github.com/custom-cards)
my design could never be realized. Many thanks!

The [Lovelace YAML-Modus](https://www.home-assistant.io/lovelace/yaml-mode/) is used and the codes are [splitted](https://www.home-assistant.io/docs/configuration/splitting_configuration/) with [!includes](https://www.youtube.com/watch?v=Ili8B4hgQ-g), [Lovelace Decluttering Card](https://github.com/custom-cards/decluttering-card) and [templates](https://github.com/custom-cards/button-card#configuration-templates).

<p align="center">
    <a name="Pic 1" href="https://raw.githubusercontent.com/fastender/blob/master/logos/blob-1.png"><img src="https://raw.githubusercontent.com/fastender/blob/master/logos/blob-1.png" alt="1" width="200"></a>
    <a name="Pic 2" href="https://raw.githubusercontent.com/fastender/blob/master/logos/blob-2.png"><img src="https://raw.githubusercontent.com/fastender/blob/master/logos/blob-2.png" alt="2" width="200"></a>
    <a name="Pic 3" href="https://raw.githubusercontent.com/fastender/blob/master/logos/blob-3.png"><img src="https://raw.githubusercontent.com/fastender/blob/master/logos/blob-3.png" alt="3" width="200"></a>
    <a name="Pic 4" href="https://raw.githubusercontent.com/fastender/blob/master/logos/blob-4.png"><img src="https://raw.githubusercontent.com/fastender/blob/master/logos/blob-4.png" alt="4" width="200"></a>
    <a name="Pic 5" href="https://raw.githubusercontent.com/fastender/blob/master/logos/blob-5.png"><img src="https://raw.githubusercontent.com/fastender/blob/master/logos/blob-5.png" alt="5" width="200"></a>
</p>

[Video](https://raw.githubusercontent.com/fastender/blob/master/logos/blob-video.mp4)

<!-- AUTOMATIONS -->
## Automations

I love NodeRed and use it for virtually all of my automations.  Node-Red is the perfect complement to Home Assistant, allowing for very complicated logic to be constructed visually through a simple “flow” interface and it integrates seamlessly with Home Assistant. 

It's a visual automation editor that I find much easier to use than the YAML-based automation system in HomeAssistant. I also much prefer the easy debugging my automations that was difficult to do in HomeAssistant.

There are a lot of palettes out there that let you do all sorts of crazy things. I use: node-red-contrib-schedex, node-red-contrib-time-range-switch and node-red-contrib-weekday.

This automations are largely guaranteed by NodeRed. There will be the possibility to switch them off manually via the view of the respective rooms in the settings.

1. SONOS in Living Room and Childrenroom is controlled by a Hue Dimmer Switch. Playlist selection and device control is enabled with this script: [Media](https://github.com/fastender/blob/blob/master/automations/media.json)


More coming soon! See examples...

Temperature notification by the sensor when nobody is at home and the temperature in certain rooms is above a certain temperature at a certain time. Only then should the air conditioner start.

Daily automatic cleaning of certain areas at a certain time by the vacuum cleaner when nobody is at home.

Automatic locking of the entrance door after a certain period of time.

Automatic switching on of the entrance light when the entrance door is opened and switching off after a certain period of time.

Light control of the Media Player in the living room (keyword: Movie), dimming of the lights during playback and brightening of the lights during pause/stop.

Monitoring of washing machines and reminders
https://philhawthorne.com/making-dumb-dishwashers-and-washing-machines-smart-alerts-when-the-dishes-and-clothes-are-cleaned/

To use as few switches for the lights as possible, using sensors in each room for light control. Possibility of interrupting this automation when using Hue Switch Dimmer switch.

No more water leaks by monitoring with the water sensor and notification.

An image is displayed of the person entering the house when no person is at home.

Greeting of the person when entering the house by analysing the presence with Bluetooth.

Notification when the entrance door is not closed.

Shutters control themselves at certain times. When no person is at home or after a certain time.

All lights are controlled randomly in the house and give the impression that people are still at home. This is very efficient in deterring criminals.

A dog barking scares off people who might ring your doorbell to check if you are at home. Simple and practical.

Easier waking up with the sunlight and also playlist.
https://www.wouterbulten.nl/blog/tech/custom-wake-up-light-with-node-red/

Notification when letter is inserted.

Monitoring of sleep quality and weight and other health data (heart, etc.). Notification when anomalies occur.

Alexa reminds for sleep time. Prayer time. Dinner time. Homework time.









![Screenshot of Home Assistant Header](https://i.imgur.com/vjDH1LJ.png)

<!-- TODO-LIST -->
## To-Do-List

Control garage and Apple TV with RM Link

Better allocation of lights and control with Hue Dimmer Switches

Automation of the shower. When humidity is high, the window is opened and vice versa. Scenes for shower.

In the corridor area a tablet in which the Home Assistant is displayed.

Alarm system is set autonomously.

A charger is invisibly installed in the bedroom chest of drawers.

More coming soon!
