# Testing Applications using MQTT over WebSocket

## Introduction
The goal of this document is to explain how to design scenarios in NeoLoad using MQTT over WebSocket.

### Supported versions

MQTT 3 and MQTT 3.1.  
The MQTT websocket module has been tested with NeoLoad 5.4.0.

## Requirements

* **NeoLoad** - First of all you need to download NeoLoad and install it on your machine. 
http://www.neotys.com/support/download-neoload.html

* **Neoload MQTT WebSocket’s Data Format Extension** - Download [the latest release](https://github.com/cmarton/test/releases/latest).   
*This extension needs to be added on each new NeoLoad  project using MQTT over WebSocket.*

* **MQTT Framework** - To design your scenario, you need to configure MQTT technical parameters as well as parameters related to your functional use case.
In order to respect the messaging workflow related to MQTT, it is recommended to add the MQTT framework into Neoload.
NeoLoad will manage all ”synchronous messages with the help of the Neoload Mqtt framework. Download [the latest release](https://github.com/cmarton/test/releases/latest).

## Create a new Neoload project with the MQTT module

### Create a new project

1. Create a new NeoLoad project from the NeoLoad main menu.

### Change the settings of the new project

1. Open the Preferences screen (Edit/Preferences)
1. Select the Project settings tab. On the left panel, select the Modules Manager section.
1. Select the Extensions tab. Add a new extension by selecting the mqttwebsocket.jar.

# MQTT messaging workflow

The [Protocol specification](http://public.dhe.ibm.com/software/dw/webservices/ws-mqtt/mqtt-v3r1.html) of MQTT describes 
the following workflow between the different messages:




