# Network Traffic Analysis with Wireshark

The Open Systems Interconnection (OSI) model is a series of layers through which computer systems use to communicate. 

There are seven layers, and the networking layer would be layer 3. 

The network layer is responsible for packet forwarding, including routing through intermediate routers. 

However, when it comes to understanding network data delivery, we need to get through layer 2 before we can move on to layer 3.

The data link layer, or layer 2, is the protocol layer that transfers data between nodes on a network segment across the physical layer, or what is commonly known as a host’s physical address. 

Layer 2 is divided into two parts, consisting of the MAC and data link sublayers, detailing addressing and the layout of data frames, and Layer 3 includes a host’s logical address. 
 
## What Are the Seven Layers of the OSI Model?

The OSI model was developed by the International Organization for Standardization (ISO). 

It describes the layers that computer systems use to communicate over a network and was the first standard model for network communications adopted by all major computer and telecommunication companies in the early 1980s.
 
## The OSI model has seven layers:
 
Physical

Data Link

Network

Transport

Session

Presentation

Application
 
## What Is Wireshark?

Wireshark is a network protocol analyzer, or an application that captures packets from a network connection, such as from your computer to your home office or the internet. 

Packet is the name given to a discrete unit of data in a typical Ethernet network.

Wireshark is the most often-used packet sniffer in the world. Like any other packet sniffer, Wireshark does three things:

Packet Capture: Wireshark listens to a network connection in real time and then grabs entire streams of traffic – quite possibly tens of thousands of packets at a time.

Filtering: Wireshark is capable of slicing and dicing all of this random live data using filters. By applying a filter, you can obtain just the information you need to see.

Visualization: Wireshark, like any good packet sniffer, allows you to dive right into the very middle of a network packet. 

It also allows you to visualize entire conversations and network streams.
