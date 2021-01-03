# Home Assistant Config

**This Page is a work in progress.**  
_TODO:_  
- _Fill the structure_
- _Links_
- _Screenshots_

This repository hosts my [Home Assistant](https://home-assistant.io) configuration files.

## Structure
You'll be unable to reproduce my own Home Assistant instance using these files directly. However, you are welcome to use this repo as inspiration for your own instance.  
Note that it is recommended that you install the included custom components and python scripts directly from their source (rather than this repository).

The main Home Assistant configuration file is configuration.yaml. Most of my configuration is located within the yaml folder.
My Lovelace UI configuration can be seen in the storage folder.

## Cool Automations

## My Hardware

Raspberry Pi 4, (SSD), BroadLink IR Blaster, Sonoff iFan03 flashed with Tasmota, Shelly 2.5, Yeelight Color, IOTLink for Windows, Google Home Mini.

## Plugins
In order to expand the experience and capabilities that are supplied by Home Assistant from the box, I use the following additional

### Android App
I'm using the companion app to display the frontend on my phone. I also created multiple widgets that are displayed on my launcher home screen.  
It's a great app that also provides an incredible amount of sensors that allow monitoring the phone's state over Home Assistant. Even as a data lover (and hoarder), I decided to disable some sensors that I had no current use for.

### Custom Components (Integrations)

**Hacs**  
**Blitzortung**  
**Places**  
**SmartIR**  
**Shellies Discovery**  

### Frontend Cards
I use the following cards to extend the lovelace UI

**Atomic Calendar Revive** - displays a nice customizable calendar.  
**auto-entities** - I use it to create a card of active automations and another card of inactive ones.  
**Bar Card** - provides nice display for my printer ink supply.  
**Compass Card** - used to display latest lightning strike's direction and distance.  
**fold-entity-row** - collapses many rows of my phone's sensors into a single row.  
**hui-element**  - it's kind of a cheat card, allowing me to display the _Restriction Card_ as a row instead of a full card.  
**Lovelace Swipe Navigation** - allows swiping between views on mobile.  
**Mini Graph Card** - a highly customizable history graph card.  
**Mni Media Player** - a highly customizable media player card.  
**Restriction Card** - protects me from accidental touches by adding a "lock" that can be dismissed either by an additional tap or after confirming an alert that I set up.  
**slider-entity-row** - an easy to use slider for my cover and AC temperature setting.  
**Swipe Card** - I use it for my weather entities cards (now, today, tomorrow) - each has many rows. Only the first card is displayed and the rest are accessible by swiping it.  
**Transmission Card** - designed to display info and control Transmission torrent client.  
**TV Remote Card** - displays a gigantic remote that I set up to control my streamer.  

### Home Assistant Supervised Add-ons
Home Assistant Supervised environment (formerly called Hassio) allows running Docker based add-ons on the same machine.

**AdGuard Home**  
**Assistant Relay**   
**chrony**   
**File Editor**  
**Grafana**  
**Grocy**  
**Grocy's Barcode Buddy**  
**Home Assistant Google Drive Backup**  
**InfluxDB**  
**Jackett**  
**jellyfin**  
**MariaDB**  
**Mosquitto broker**  
**NGINX Home Assistant SSL proxy**  
**Portainer**  
**Radarr**  
**roombapw Docker Image**  
**Samba share**  
**Sonarr**  
**Terminal & SSH**  
**Transmission**  
**WireGuard**  