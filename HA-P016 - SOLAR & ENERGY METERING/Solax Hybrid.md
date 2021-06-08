# SOLAX HYBRID INVERTER - MODBUS TCP - HOME ASSISTANT (without Pocket wifi)

## References:

[https://community.home-assistant.io/t/solax-inverter-by-modbus-no-pocket-wifi/140143](https://community.home-assistant.io/t/solax-inverter-by-modbus-no-pocket-wifi/140143)

## Description

We don't need the Solax Pocket WiFi dongle, because we can use the Inverter's built in LAN connection. It can connect to the Cloud through theLAN port.

After performing an Intense Nmap scan we found that port 502 is open. It's a Modbus TCP port.

The Modbus registers are in Hex and they need to be converted to decimal to use with HA built in Modbus Integration 105 as the Integration Supports serial this will possibly work connected to the RS485 port if your Inverter does not have built in LAN?

As you are directly talking to the inverter you can update values as quick or slow as you want.  
I am only reading values at the moment, but you can program the Inverter / Battery over Modbus.

On the new Hybrids we have an Ethernet port (RJ45) on the inverter Motherboard it’s self, this is under the front cover. As well as terminals and an RJ45 for RS485 (ModBus).
