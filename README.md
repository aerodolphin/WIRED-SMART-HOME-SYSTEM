# WIRED SMART HOME SYSTEM


## Why a Smart Home System

When considering the integration of new technology into our lives, it is crucial to contemplate the advantages it brings. This typically revolves around the following inquiries:

1. Does it save time?
2. Does it improve my experience?

If not, does it enable me to accomplish something substantial that I was not able to achieve before?

The goal is to improve the human experience in the system in some way or at least to help us to save energy.

It looks cool to showing off to our friends that we can turn on and off some lights with a phone but in a daylife world we just want to turn the light on with a simple wall switch. In my opinion, a good smart home light control system is the one capable of turning on and off the lights with a reliable occupancy detection system.


## Motivation

My main motivation is from my love of technology and creating things that could improve our lives in someway. Combining with the fact I'm building a new home, It's the perfect time to implement a smart home system capable of saving some time and improving my family experience. I hope this subject is of interest to some people so that we can create an online community for sharing experience and knowledge. With a smart system we can save energy, reduce costs, create automations, create an alarm system, simplify daily routines, customize things, etc.


## The Smart Home System

After try some open source smart home softwares (openHAB, Home Assistant and Domoticz) I choose the Home Assistant platform.

Regarding to the network topology the ideal was the star topology where the hub acts as a central point of communication, and data flows between devices and the hub. This topology offers high reliability and ease of management, but it requires more cabling compared to other topologies. Because of that disadvantage I choosed what I called of an hybrid solution where we have some micro hub's connected to a central hub where we have the Home Assistant and connected to these micro hub's we also have some devices connected in a bus topology (I2C protocol).

For me it's very important to have the majority of the devices connected by wire and running locally (independently of clouds and Internet). 

![Smart Home System Hybrid Topology](https://drive.google.com/uc?id=1DeBX2HS4ZQM6OJaZdMSIzAMpnMHtWVtp)


## Why a Wired Smart Home System

A wired smart home system offers several advantages over a wireless system. That's why I would like to focus on that. I quickly discovered that there are not many wired systems and devices available on the market. That's why I decided to develop some and share.

Here is a list of advantages of a wired smart home system compared to a wireless one:

* **Reliability:** Wired smart home systems are known for their reliability. Since they rely on physical cables to connect devices and sensors throughout the home, they tend to be more stable and less prone to interference compared to wireless systems [2]. Wired connections provide a consistent and uninterrupted connection, reducing the chances of signal dropouts or connectivity issues.

* **Security:** Wired smart home systems are generally more secure than wireless systems. Since the data transmitted through wired connections travels over physical cables, it is less susceptible to hacking or unauthorized access compared to wireless signals that can be intercepted. This can be particularly important when it comes to sensitive data or home security systems.

* **Latency:** Wired connections offer lower latency compared to wireless connections. Latency refers to the time it takes for data to travel between devices. Wired connections have a direct and dedicated pathway, resulting in faster response times. This can be beneficial for devices that require real-time interaction, such as streaming media or gaming devices.

* **Bandwidth** Wired connections generally provide higher bandwidth compared to wireless connections. This means that wired smart home systems can handle larger amounts of data at a faster rate. It can be advantageous for bandwidth-intensive tasks like streaming high-definition video, transferring large files, or using multiple devices simultaneously.

* **Interferences:** Unlike wireless signals, wired connections are not susceptible to signal interference from other electronic devices or physical obstacles. Wireless signals can be affected by factors such as distance, walls, and other devices operating on the same frequency, potentially leading to reduced signal strength or disruptions. With a wired smart home system, you can minimize these interference issues.

* **Limitations:** Wired smart home systems are not subject to the limitations of Wi-Fi networks. Wireless networks may have limitations on the number of devices they can support simultaneously. In contrast, a wired system can handle a larger number of devices without experiencing congestion or reduced performance.

* **No Batteries:** No batteries to deal with. Wireless devices require constant battery supervision and often need frequent battery replacements.

These advantages make wired smart home systems an attractive option for those seeking reliability, security, low latency, high bandwidth, and freedom from wireless limitations and interference. However, it's essential to consider the specific needs of your smart home setup.



## Devices under development

* ESP32-ETH - ESP32 with Ethernet
* WIO-HUB - Wired Input/Output Hub
* WOD - Wired Occupancy Detector
* WIC - Wired Irrigation Controller
* WAIRQ - Wired Air Quality Sensor

The device names can be changed. I'm accepting suggestions for the names and references.

