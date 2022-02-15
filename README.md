# Domoticz-Tasmota-Smartplug
Domoticz plugin to integrate a smartplug running Tasmota firmware

Tested with Python version 3.8, Domoticz version 2020.2

## Prerequisites

Smartplug running Tasmota firmware. Tested with Athom TP29 and PG01 smartplugs from AliExpress.

## Installation

Assuming that domoticz directory is installed in your home directory.

```bash
cd ~/domoticz/plugins
git clone https://github.com/mvdklip/Domoticz-Tasmota-Smartplug
# restart domoticz:
sudo /etc/init.d/domoticz.sh restart
```
In the web UI, navigate to the Hardware page and add an entry of type "Tasmota Smartplug".

Make sure to (temporarily) enable 'Accept new Hardware Devices' in System Settings so that the plugin can add devices.

Afterwards navigate to the Devices page and enable the newly created devices.

## Updating

Like other plugins, in the Domoticz-Tasmota-Smartplug directory:
```bash
git pull
sudo /etc/init.d/domoticz.sh restart
```

## Parameters

| Parameter | Value |
| :--- | :--- |
| **IP address** | IP of the smartplug eg. 192.168.1.231 |
| **Port** | Port of the smartplug web interface eg. 80 |
| **Username** | Username for the smartplug web interface |
| **Password** | Password for the smartplug web interface |
| **Query interval** | how often is data retrieved |
| **Debug** | show debug logging |
