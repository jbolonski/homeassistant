# Home Assistant Configuration

https://home-assistant.io/

## Integrations

* Alexa
* MQTT
* ZigBee
* Z-Wave
* DD-WRT
* Honeywell

## Device Tracking

# Removed due to unreliability
# * DD-WRT
# * Owntracks

## Lights

* LimitlessLED Lights - Dimmable, Color Temp, RGB
   * through LimitLessLED Wifi Bridge
* Flux LED Light (Magic Home)
* Hue Lights & Bridge
   * Light Bulb
   * Hue Play Lights

## Sensors

* Ecolink Z-Wave PIR Motion Detector, Pet Immune (PIRZWAVE2-ECO)
* Octoprint
* MQTT
* Aeotec Water Sensor, Z-Wave Flood & Leak Sensor
   * Needed to use OZWCP to set 'Report Type to Send' to 17 instead of the default of 256
   * In order to successfully set 'Report Type to Send'
      * Pull Battery
      * Replace Battery
      * Press Zwave Button
      * Click "Submit" in OZWCP

## Binary Sensors

* Octoprint - currently disabled

## Switched Outlets

* Leviton DZPA1-1BW
    * warning: These let low voltage through when off and can cause issues with things like LED lights.
* TP-Link Wi-Fi Smart Plug HS100
* Wemo Mini Smart Plug 

## Switches
* Broadlink RM Switch

## Cameras

* Octoprint mjpeg streamer - enabled but not displayed in the UI

## Locks

* Schlage BE469NXCEN Touchscreen
	* If this stops working the zwcfg_###.xml might have gotten messed up.
	* If the lock works from ozwcp but not hass then compare the diff between the zwcfg_###.xml from the ozwcp directory and the file from the hass .home directory

## Removed Devices

* OSRAM Lightify Light - Dimmable (replaced by Hue bulb)
