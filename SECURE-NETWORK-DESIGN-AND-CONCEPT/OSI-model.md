# OSI

Demonstrates how commincation works in terms of layers

* Physical layer
* Data Link
* Network
* Transport
* Session
* Presentation
* Application

The OSI shows what happens to data as it is communcated to another device. I want to send something to a friend, the order is in reverse - app, pre, ses, tra, net, dat, phy - and when he recieves it, the normal order
is in play as it reconstructs my message

## Application Layer
This is the UI where i can directly interact with the data. This can be in the form of a software such as outlook which uses SMTP ( simple mail transfer ). I write my message and it moves to the next stage

## Presentation -> Session
Formats the data in the email. Encryption and compression occur here if configured
Session establishes a connection between outlook and the mail server, establishing connection, maintaining and terminating

## Transport
For example UDP and TCP are protocols used here for transport. Data will be broken down into segments in this section preparing it for transport

## Network
Routing and IP assigning takes place here determining the best path to take to get the message to the destination

## Data link
Takes the segments/packets and frames them. These frames contain mac addresses. This layer ensures data moves correctly on the LAN, say if the data needs to go to your own router first


## Physical Layer
Cables, switches, ethernet, wifi, repeaters
Data is transferred in binary bits. Raw bits are moved over a physical medium. 

in a wired connection, say through an ethernet, data will have a binary value. This binary value will be communcated through electrical signals, representing either 0 or 1. So a high voltage would mean 1 and a lower
would mean 0.
so:
Ethernet - Electrical signal/voltage
Fiber Optic - Light signals

For a wireless connection such as WiFi or bluetooth it works similarly. This is called modulation.
AM ( amplitude modulation ) - strength variation of waves dictate 1 or 0
Frequency modulation -  frequency of waves dictates 1 or 0

You may see Wi-Fi and think ' how does that come under physical?'. Wi-Fi uses radio waves to communcate between devices, and these radiowaves exist in the physical world although we cannot see or touch them


So physical layer facilitates physical connection and data transmission


