# How to capture network traffic: Port mirroring

Port mirroring, also known as SPAN or roving analysis, is a method of monitoring network traffic which forwards a copy of each incoming and/or outgoing packet from one (or several) port(s) (or VLAN) of a switch to another port where the analysis device is connected.

Port mirroring can be managed locally or remotely.

To configure port mirroring, an administrator selects one or several ports from which all packets will be copied (source ports) and another port or ports where the copies of the packets will be sent (destination port).

The administrator can include either all packets in the port mirroring or only the transmitted /received packets. 

In case both transmitted and received packets are included, a packet going from a first monitored port to another monitored port will be copied twice to the destination port. 

This will have an impact on the measures and performance provided by the analysis device (e.g., retransmission rates, response times, …). 

APS captures and evaluates the data without any impact on the original traffic.

Port mirroring is the most commonly used solution for capturing traffic because it is inexpensive, flexible in terms of how much traffic can be captured at once, and remotely configurable.

Please note that port mirroring may have some drawbacks, such as:

It can consume significant CPU resources while active

There is a risk of not receiving some packets (such as media errors)

In the case of traffic congestion at the switch level, port mirroring is likely to drop some traffic (because the SPAN process does not have priority)

In some cases, a better solution for long-term monitoring may be a passive TAP or an Ethernet repeater (”hub”)

## Advantages of port mirroring

Low cost (this feature is embedded in most switches)

Can be configured remotely through IP or Console port

The only way to capture intra-switch traffic

A good way to capture traffic on several ports at once

## Drawbacks of port mirroring

Not adequate for fully utilized full-duplex links (packets may be dropped)

Filters out physical errors

Impact on the switch’s CPU

Can alter the timing of the frame (with an impact on response time analysis)

SPAN has a lesser priority than port to port data transfer

## How to capture network traffic: Network TAP

A network TAP (Terminal Access Point) is a hardware device which can passively capture traffic on a network. 

It is commonly used to monitor the traffic between two points in the network. 

If the network between these two points consists of a physical cable, a network TAP may be the best way to capture traffic.

The network TAP has at least three ports: an A port, a B port, and a monitor port. 

To place a tap between points A and B, the network cable between point A and point B is replaced with a pair of cables, one going to the TAP’s A port, the other one going to the TAP’s B port. 

The TAP passes all traffic between the two network points, so they are still connected to each other. 

The TAP also copies the traffic to its monitor port, thus enabling an analysis device to listen.

Network TAPs are commonly used by monitoring and collection devices such as APS. 

TAPs can also be used in security applications because they are non-obtrusive, are not detectable on the network, can deal with full-duplex and non-shared networks, and will usually pass-through traffic even if the tap stops working or loses power.

## Advantages of TAPs

No risk of dropped packets

Monitoring of all packets (including hardware errors (MAC & media))

Provides full visibility, including congestion situations

## Drawbacks of TAPs

The device may require two listening interfaces on the analysis device

Costly

No visibility on intra-switch traffic

Not appropriate for the observation of a narrow traffic range
