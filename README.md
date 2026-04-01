# Wireless-Connections-with-Access-Point-in-Cisco-Packet-Tracer

## Overview 

In this lab, I configured Wireless local area networks (WLAN) using Cisco Packet Tracer, which I'm able to simulate tools to build and test networks without physical hardware. The goal is to set up a secure wireless access point to connect multiple devices. In this example, I will use an access point, computer, laptop, and smartphone, and then test to see if the network is successful.

# Steps Taken 


1. I will drag and drop an Access Point, a PC, a Laptop, and a Smartphone in our logical dashboard to get started. 

<img width="1638" height="876" alt="image" src="https://github.com/user-attachments/assets/d08dfed3-0cb9-46f5-8a1a-cb955331136d" />

<img width="690" height="762" alt="image" src="https://github.com/user-attachments/assets/ecf37449-3ed9-4761-a622-de515f1d1a05" />

2. I then need to set our SSID and password for our access point. Once I click on the access point --> Config --> Port 1, I can rename our SSID from Default to "JoseCyber."

Port 0 is for wired connections
Port 1 is for Wireless connections

<img width="1174" height="504" alt="image" src="https://github.com/user-attachments/assets/3db56ef6-537e-4020-a006-3643730e1123" />


3. For Authentication or password, I will click on WPA2-PSK. 

WPA2-PSK is the standard security protocol that is used to protect most modern home or small office wireless networks. PSK is the password or passphrase that you create for your router and type onto your phone or computer to connect. 

I will create a random password. If this Ire a real-life environment, I would suggest special characters and a long password of 12 to 16 characters in order to secure our network from threat actors.

SIPt@tGamE6!*

<img width="700" height="360" alt="image" src="https://github.com/user-attachments/assets/bd5c1bf4-fa4c-4999-940a-8db92d758441" />

4. The next step is to connect the PC, which is PC0, to the access point. I will have to remove the wired connection at the bottom and connect the WMP300N module, which will provide a 2.4 gigahertz wireless connection. 

Basically, this PC needs a wireless antenna to connect to the access point

<img width="846" height="688" alt="image" src="https://github.com/user-attachments/assets/255b6c28-0cf6-4fdc-88fb-ce1d71a08147" />


5. I will now have to connect the PC to the access point by going to the desktop tab and clicking on PC wireless. 

<img width="744" height="634" alt="image" src="https://github.com/user-attachments/assets/3bf22d50-0a35-48b9-b127-36547e4177bc" />


I clicked on the connect tab for the wireless adapter configuration utility and refreshed to see and locate any nearby wireless networks that the antenna picked up. I was able to see my wireless access point, JoseCyber, with a signal of 39%. I then clicked on connect and entered the password.

<img width="774" height="626" alt="image" src="https://github.com/user-attachments/assets/26271cb3-9e9a-49e2-bf9b-ae3fe8364839" />

<img width="550" height="392" alt="image" src="https://github.com/user-attachments/assets/84907790-2cbb-4396-8a20-ff7b8d12a5d8" />

I can now see from the logical POV on the dashboard that the PC is connected to the access point.

6. Now I will connect the laptop to the access point.
I first had to turn off the laptop and then remove the wired connection module. Then I equipped it with a wireless module. 

<img width="694" height="426" alt="image" src="https://github.com/user-attachments/assets/eb32c332-d5f3-4ae6-ab3e-4bd65719640f" />


<img width="612" height="452" alt="image" src="https://github.com/user-attachments/assets/cec97f25-b5fe-49a0-a6b5-7d6d3738bafd" />


Next, I turned on the laptop, clicked on the desktop tab, clicked on PC wireless, and looked for my access point. Then I clicked on connect and was able to input the password and connect the device.

<img width="712" height="628" alt="image" src="https://github.com/user-attachments/assets/23b097e7-9011-4134-981f-cd19452efa59" />

<img width="718" height="760" alt="image" src="https://github.com/user-attachments/assets/d1d97128-6a2e-4196-ad22-4590c9ebd1c8" />

<img width="1220" height="702" alt="image" src="https://github.com/user-attachments/assets/1eefa096-0bf4-4a5f-93ac-c79c7c1802cb" />


7. Now I can connect the smartphone. I clicked on the Smartphone and Int to the Config Tab. From there, on the left-hand side, I clicked on the tab Wireless0. I then input the SSID: JoseCyber and selected WPA2-PSK and added the password. 

<img width="756" height="476" alt="image" src="https://github.com/user-attachments/assets/6e42bab5-f76a-46f0-9c6e-32a2f71d6ff8" />


8. I would like to simulate a test to see if I can ping the PC0 to the smartphone, so I will have to add a static IP address.

I assign static IP addresses to each device. In production environments, a DHCP server typically handles this automatically, but I will use static IPs, which are useful in labs and for servers or printers that need a permanent address. All devices are placed in the 192.168.1.0/24 subnet. 

IPv4 Address PC0: 192.168.1.10
IPv4 Address Laptop: 192.168.1.11
IPv4 Address Smartphone: 192.168.1.12



PC0
<img width="1102" height="596" alt="image" src="https://github.com/user-attachments/assets/163b9310-e05c-4788-abe5-0acd18c949fa" />



Laptop
<img width="1236" height="570" alt="image" src="https://github.com/user-attachments/assets/fd9bbf57-63b5-482b-8c1b-336e8311beb7" />


Smartphone
<img width="1178" height="478" alt="image" src="https://github.com/user-attachments/assets/4b43932c-2cd7-4ff4-92c4-3bc6da4b8b8d" />



9. I will now show the simulation to test the ping and watch the traffic

<img width="768" height="398" alt="image" src="https://github.com/user-attachments/assets/60afa681-c653-452e-8896-19ca34a4bce6" />



<img width="680" height="406" alt="image" src="https://github.com/user-attachments/assets/6e474da2-1306-47eb-82e6-27af5f77c5a9" />

After the access points, it asks everybody in the network, "Hey, are you so and so's IP address?" I notice on the smartphone, it is actually checking to see and will respond, "Yes, I am the address that you are looking for." It will relay the message back to the access point and back to PC0.


<img width="730" height="374" alt="image" src="https://github.com/user-attachments/assets/fb18df5f-587c-4be0-951f-04351d134d5b" />


<img width="754" height="344" alt="image" src="https://github.com/user-attachments/assets/167adae9-d231-4900-9d02-12f17f3a4a37" />



## What I learned

I use the 192.168.1.0/24 subnet with a subnet mask of 255.255.255.0. The /24 notation means that the 1st 24 bits identify the network, leaving 8 bits for device addressing, giving us 254 usable IP addresses on this network.

Why I keep using static IPS instead of DHCP. The way I think about it is kind of like a hotel versus only night condo. When I stay at a hotel, the front desk assigns me a room every time I check in or someone else checks in. It might be 204 today, and the room might be 310 the next time period. I don't pick it, but the hotel handles it automatically; that's basically DHCP. So my device will get assigned to an address automatically every time I connect to the network.

When I own my own condo or house, my condo or house address will always stay the same. It is attained to me, so that is an IP address. This address is permanent and manually set.


Something I forgot to mention, I showed that my PC had a 39% signal strength. I went to the physical dashboard and then moved the computer, smartphone, and laptop right next to the access point, which increased the signal strength to 100. In an office setting, no one is going to be sitting right next to the access point in the server room period that's why there are going to be many access points in a corporate environment in different places. An IT professional might have to do a wireless site survey to map out weak signal strengths throughout the building or environment and would have to add an access point to increase better coverage.

It was received. 
<img width="824" height="470" alt="image" src="https://github.com/user-attachments/assets/b14d77f0-4752-4d97-a37d-060d934bba15" />
