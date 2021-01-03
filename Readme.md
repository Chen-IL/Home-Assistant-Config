# Home Assistant Config

**This Page is a work in progress.**  
_TODO:_  
- _Provide missing content (automations, hardware, add-ons description)_
- _Screenshots_

This repository hosts my [Home Assistant](https://home-assistant.io) configuration files.

## Structure
You'll be unable to reproduce my own Home Assistant instance using these files directly. However, you are welcome to use this repo as inspiration for your own instance.  
Note that it is recommended that you install the included custom components and python scripts directly from their source (rather than this repository).

The main Home Assistant configuration file is configuration.yaml. Most of my configuration is located within the yaml folder.
My Lovelace UI configuration can be seen in the storage folder.

## Cool Automations

## My Hardware

Raspberry Pi 4, (SSD), BroadLink IR Controller, Sonoff iFan03 flashed with Tasmota, Shelly 2.5, Yeelight Color, IOTLink for Windows, Google Home Mini.

## Plugins
In order to expand the experience and capabilities that are supplied by Home Assistant from the box, I use the following additional plugins:

### Android App
I'm using the [Home Assistant Companion](https://companion.home-assistant.io/) app to display the frontend on my phone. I also created multiple widgets that are displayed on my launcher home screen.  
It's a great app that also provides an incredible amount of sensors that allow monitoring the phone's state over Home Assistant. Even as a data lover (and hoarder), I decided to disable some sensors that I had no current use for.

### Custom Components (Integrations)

[HACS](https://hacs.xyz/) - Custom Components, Cards, Themes and more can be installed using HACS.  
[Blitzortung](https://github.com/mrk-its/homeassistant-blitzortung) via HACS - tracks lightning strikes nearby. Offering sensors and displays strikes on the map component.  
[Places](https://github.com/custom-components/places) via HACS - reverse geocoding (device_tracker -> meaningful location string) using OpenStreetMap. My version is modified to support language choice and build the resulting string differently.  
[SmartIR](https://github.com/smartHomeHub/SmartIR) via HACS - using an IR controller to create climate devices, media players and fans.  
[Shellies Discovery](https://github.com/bieniu/ha-shellies-discovery) via HACS Automations - MQTT discovery support for Shelly devices.  

### Frontend Cards
I use the following cards to extend the lovelace UI. All of the following are installed using HACS.

[Atomic Calendar Revive](https://github.com/marksie1988/atomic-calendar-revive) - displays a nice customizable calendar.  
[auto-entities](https://github.com/thomasloven/lovelace-auto-entities) - I use it to create a card of active automations and another card of inactive ones.  
[Bar Card](https://github.com/custom-cards/bar-card) - provides nice display for my printer ink supply.  
[Compass Card](https://github.com/tomvanswam/compass-card) - used to display latest lightning strike's direction and distance.  
[fold-entity-row](https://github.com/thomasloven/lovelace-fold-entity-row) - collapses many rows of my phone's sensors into a single row.  
[hui-element](https://github.com/thomasloven/lovelace-hui-element)  - it's kind of a cheat card, allowing me to display the _Restriction Card_ as a row instead of a full card.  
[Lovelace Swipe Navigation](https://github.com/maykar/lovelace-swipe-navigation) - allows swiping between views on mobile.  
[Mini Graph Card](https://github.com/kalkih/mini-graph-card) - a highly customizable history graph card.  
[Mini Media Player](https://github.com/kalkih/mini-media-player) - a highly customizable media player card.  
[Restriction Card](https://github.com/iantrich/restriction-card) - protects me from accidental touches by adding a "lock" that can be dismissed either by an additional tap or after confirming an alert that I set up.  
[slider-entity-row](https://github.com/thomasloven/lovelace-slider-entity-row) - an easy to use slider for my cover and AC temperature setting.  
[Swipe Card](https://github.com/bramkragten/swipe-card) - I use it for my weather entities cards (now, today, tomorrow) - each has many rows. Only the first card is displayed and the rest are accessible by swiping it.  
[Transmission Card](https://github.com/amaximus/transmission-card) - designed to display info and control Transmission torrent client.  
[TV Remote Card](https://github.com/marrobHD/tv-card) - displays a gigantic remote that I set up to control my streamer.  

### Home Assistant Supervised Add-ons
Home Assistant Supervised environment (formerly called Hassio) allows running Docker based add-ons on the same machine. Some Add-ons are available within the default repository. Others require adding custom repositories.

[AdGuard Home](https://github.com/hassio-addons/addon-adguard-home)  
[Assistant Relay](https://github.com/Apipa169/Assistant-Relay-for-Hassio)   
[chrony](https://github.com/hassio-addons/addon-chrony)   
[File Editor](https://github.com/home-assistant/hassio-addons/tree/master/configurator)  
[Grafana](https://github.com/hassio-addons/addon-grafana)  
[Grocy](https://github.com/hassio-addons/addon-grocy)  
[Grocy's Barcode Buddy](https://github.com/Forceu/barcodebuddy)  
[Home Assistant Google Drive Backup](https://github.com/sabeechen/hassio-google-drive-backup)  
[InfluxDB](https://github.com/hassio-addons/addon-influxdb)  
[Jackett](https://github.com/haberda/hassio_addons/tree/master/jackett)  
[jellyfin](https://github.com/petersendev/hassio-addons/tree/master/jellyfin)  
[MariaDB](https://github.com/home-assistant/hassio-addons/tree/master/mariadb)  
[Mosquitto broker](https://home-assistant.io/addons/mosquitto/)  
[NGINX Home Assistant SSL proxy](https://github.com/home-assistant/hassio-addons/tree/master/nginx_proxy)  
[Portainer](https://github.com/hassio-addons/addon-portainer)  
[Radarr](https://github.com/petersendev/hassio-addons/tree/master/radarr)  
[roombapw Docker Image](https://github.com/jeremywillans/hass-addons/tree/master/roombapw)  
[Samba share](https://github.com/home-assistant/hassio-addons/tree/master/samba)  
[Sonarr](https://github.com/petersendev/hassio-addons/tree/master/sonarr)  
[Terminal & SSH](https://github.com/home-assistant/hassio-addons/tree/master/ssh)  
[Transmission](https://github.com/pierrickrouxel/hassio-addon-transmission)  
[WireGuard](https://github.com/hassio-addons/addon-wireguard)  