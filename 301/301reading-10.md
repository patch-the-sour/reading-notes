# What Is a p2p(peer to peer) VPN
## Site-to-Site VPN Defined
A site-to-site virtual private network (VPN) refers to a connection set up between multiple networks. This could be a corporate network where multiple offices work in conjunction with each other or a branch office network with a central office and multiple branch locations. 

Site-to-site VPNs are useful for companies that prioritize private, protected traffic and are particularly helpful for organizations with more than one office spread out over large geographical locations. These businesses often have to access resources housed on a primary network, which could include servers that facilitate email or store data. In some instances, a server may be the operational hub of an application essential to the company’s business. A site-to-site VPN can, in that case, give all sites full access to the application—as if it were housed within their physical facility.

The history of site-to-site VPNs intersects, in many ways, with the history of the internet itself. Site-to-site VPNs were a forbearer of what we now know as the internet. They were first made possible through the use of the original packet switching network named Advanced Research Projects Agency Network (ARPANET), as well as the initial uses of Transmission Control Protocol/Internet Protocol (TCP/IP). 

TCP/IP outlines how data is organized according to packets, given addresses, transmitted, and received across different computers on the internet. Before the internet was launched as we know it today, computers were connected between sites through a private network and TCP/IP. In this way, site-to-site networks predated the internet, forming the foundation for what we have today.

The modern iteration of a VPN gained popularity because of people wanting to mask their IP addresses and surf the internet more safely. A hidden IP address gives you the freedom to download torrents without revealing who you are. You can also gain access to geo-blocked content, regardless of your location. In addition, on a public network, you have to deal with a constant barrage of cyberattacks, but with a VPN, you can enjoy a more secure, encrypted connection. These attributes made private VPNs a top choice among individual users.

However, VPNs designed for one—or a few—users at a time do not have the capabilities to serve the needs of a large organization. In many cases, big companies must send many terabytes of data between locations, quickly and safely, and the kind of VPN sufficient for a normal torrent user or web surfer would not be able to handle the workload.

## Understanding VPN and Its Types
There are a few different types of SSL VPNs, and each comes with its own benefits. Depending on the needs of your organization, one type may better fit your objectives than others.

## Remote Access VPNs
A remote access VPN refers to a temporary connection set up between two or more users and a central location. In most cases, a remote access VPN is used to give each location access to a data center. In some situations, a connection that makes use of Internet Protocol security (IPsec) is sufficient. However, it is also common for an organization to utilize a VPN, which avails them of the security positioned at the gateways at each end of the VPN.

A remote access VPN is a useful tool for companies with remote workers either on the road or in their homes. If these workers need to access private or sensitive information housed in the company’s servers, they can connect to a remote access VPN. In this way, each employee is able to gain access to the resources they need to do their jobs.

This VPN type can be used to provide workers in different locations with an experience similar to that of those in the main office who can connect to the server at their desks using an Ethernet cable. In a sense, the remote access VPN extends a cable across many miles—and even international borders—right into each employee’s workstation, which includes desktops, laptops, and mobile devices.

## Intranet-based Site-to-Site
An intranet-based site-to-site VPN connects more than one local-area network (LAN) to form a wide-area network (WAN). A company may also use this kind of setup to incorporate software-defined WAN (SD-WAN). Intranet-based site-to-site VPNs are useful tools for combining resources housed in disparate offices securely, as if they were all in the same physical location.

An intranet-based site-to-site VPN is particularly helpful if each site either develops its own resources or houses unique processes that the entire company would benefit from having access to. For example, if each office had design schematics that were constantly being updated and adjusted for clients, an intranet-based site-to-site VPN would give decision-makers in a number of offices secure access to everything produced—regardless of their physical location.

## Extranet-based Site-to-Site
Extranet-based site-to-site VPNs are often used by two or more different companies that want to share certain resources but keep others private. With an extranet-based site-to-site VPN, each entity connects to the VPN and chooses what they want to make available to the other companies. In this way, they can collaborate and share without exposing proprietary data.

## What are the three types of SSL VPNs?
How to Create a Site-to-Site VPN
Creating a site-to-site VPN involves determining how you want the data to be transferred from one site to the next and choosing a way to make sure it is secure from intruders. This can be done with an internet-based site-to-site VPN or a multiprotocol label switching (MPLS) site-to-site VPN.

## Creating an Internet-based Site-to-Site VPN
An internet-based site-to-site VPN uses the existing network of an organization in combination with the public internet. To set up an internet-based site-to-site VPN, you need a VPN gateway that secures the data traveling back and forth.

To create an internet-based site-to-site VPN, you make a tunnel that connects two networks, for which you need three components:

A base network in one location
A satellite network in another location
A tunnel with security gateways on each end
The tunnel “burrows through” or sits on top of a physical internet connection. However, the tunnel protects the traffic flowing through it from being accessed by people using the physical network. To set it up, you need to set up a gateway at each site. The first gateway the data meets as it enters the tunnel will encrypt the data. The encryption keeps each data packet safe from users, devices, and malware that could seek to corrupt, steal, or compromise it in some way. 

As the data arrives at its destination, it meets the other gateway. This decrypts the data so the network on the other side can read it. Entities in the physical internet the data has to travel through while encrypted will not be able to read it. The data will remain unreadable without a second gateway to decrypt it for the receiving network.

The gateway may incorporate a network access server and a secure access service edge (SASE), which requires the user to enter credentials before they gain access to the VPN.

You can also use a firewall, which furnishes a powerful barrier that sits between the organization’s private network and the surrounding internet. The firewalls can restrict the kind of traffic allowed to go through them.

## Creating an MPLS Site-to-Site VPN
MPLS can be a useful tool for organizations wanting to send data between two locations. An MPLS site-to-site VPN depends on infrastructure made available by the VPN provider, as opposed to the company that uses the VPN. The configuration of an MPLS VPN involves creating VPN connections between the primary site and the satellite sites.

MPLS works through labels that route data packets to where they need to go instead of using IP addresses. Nodes are designed to interpret the labels and send the data packets directly to the next destination. This enables you to make direct links between the nodes. If you are setting up an MPLS site-to-site VPN, you can use MPLS to route the data directly from location A to location B. In a normal exchange of data using IP addresses, the information may go all over the country before it finally reaches its destination. 

For example, data could go from Los Angeles to Utah to Las Vegas instead of straight from L.A. to Vegas. MPLS avoids the extra routing.

To create an MPLS site-to-site VPN, you first have to set up a broadband IP network, which will serve as the backbone for the MPLS network. The organization then has to equip each site with an MPLS-suitable switch that connects to a router. This allows the data that passes through the switch to be sent using MPLS. As a data packet at location A hits the switch, it gets encoded using MPLS. Then, it passes to location A’s router and straight to location B’s router and switch.

## Why Implement a Site-to-Site VPN
There are several factors to consider when figuring out whether to implement site-to-site VPN services. In some cases, typical IPsec is sufficient for communication between two or more locations. However, there are a few considerations that may drive a company to use VPN connections instead:

The number of locations
Business size
The distance between each location
The resources the locations have to share with each other
In most cases, a site-to-site VPN is a good solution if your business consists of several locations, each with employees that need to share resources provided by the main office. If you use a site-to-site VPN in this kind of situation, you can ensure that all employees have secure access to the same resources.

For example, suppose you have a company based in New York, but it has several branch offices, one in Shanghai, one in France, and another in Switzerland. Each location has between 15 and 20 employees. The company’s email system is housed on a central server. You also have a data server that holds important marketing collateral and proprietary information. 

If you use a site-to-site VPN, not only can every employee access the same resources but the data is also encrypted, keeping it safe from attackers who may want to exploit it.

## 5 Key Components of a Site-to-Site VPN
### Watertight Security
The VPN your company chooses must be protected by stringent security measures. The data that travels back and forth must be secure, both as it moves from point to point and while at rest in each location. This involves adequate authorization, authentication, and administration. It is also important for all practices to support the security policies of the organization, including any established best practices that have been developed by the various IT staff in each location.

A VPN with properly programmed gateways will only let data through if it has the appropriate authentication. Otherwise, it is discarded, which, in many cases, keeps the network safe.

## Ease of Operations
If a VPN is difficult to use, it can cause more frustration than convenience. Users should have the freedom to access the VPN using a web browser. While it is important to ensure ease of access, this should not result in lax security practices. If users have to take an extra step to get into the VPN, the extra security may be worth the additional few moments it takes to gain entry.

This does not mean access has to be cumbersome. In the majority of cases, employees should be able to get into the VPN using mobile devices like laptops, tablets, or smartphones.

With a VPN, you can also make network administration easier. You can manage remote locations from a central office and exercise complete control over the entire network. This gives you the flexibility to upgrade your security measures, including installing new features or updating existing software—all from one location.

## Simple and Secure Scalability
It is easy to scale a VPN. You can add a new site, user, office, or partner organization in minutes. If you do not have to put additional VPN clients at each new location, it is quick and inexpensive to incorporate additional connections. Also, in case you need to relocate a satellite office, it is easy to set up another location.

## Business Continuity
In the event of a disaster, whether naturally caused or due to an infrastructural issue, it is important to minimize business interruption and get back up and running as soon as possible. A site-to-site VPN lets you leverage remote access immediately after an emergency has been identified. 

If, for example, an office is affected by a disaster, employees do not have to stop all production until things are back up and running. They can each be granted access to the site-to-site VPN, connect to the resources at headquarters, and work from home. With a VPN, you can minimize downtime and reduce the financial effects of a disaster.

## Flexible Deployment
With a VPN, you have the power to deploy a new solution across a broad network of devices at various physical locations. You can choose which sites to provide the new solution to first, second, and so forth. This could give you the flexibility to offer training or support in controllable phases instead of tackling it all at once and potentially overwhelming your IT team.

## The Benefits of Managed VPN Services
The implementation of a site-to-site VPN for an organization is often a challenge. Maintaining the operation and security of the VPN can consume valuable resources. But using managed VPN services can allow you to focus on the most important aspects of your business, as the managed service provider makes sure connectivity is maintained to keep the business running smoothly. 

Also, with managed services, you have a scalable solution that lets you add locations anywhere in the world. Everything, from setup to upgrading to modifying the system, is handled by the service provider.

## How Fortinet Can Help
The security of your VPN cannot be left to chance. High-performance encryption and decryption is necessary on both ends of your site-to-site VPN. Because large volumes of information must be transported securely, you also need a system that can process data quickly without sacrificing the safety of the network. With new threats emerging daily, you need a solution that can adequately protect data while in transit and within each location. This is where the FortiGate high-performance crypto VPN can be a powerful resource.

The FortiGate unified threat management (UTM) solution and the FortiClient endpoint security applications can keep your VPN secure. The FortiGate unit can be installed on a private network where it examines the data that flows in. If the data is safe, it is allowed to pass. In this way, FortiGate keeps your network safe.

Then, FortiClient can be installed on the user’s computer. FortiClient uses real-time scanning to inspect endpoints for vulnerabilities. Also, with FortiClient installed, you have the ability to not only protect each endpoint from malware but you can also use sandbox threat intelligence to identify and block zero-day threats. With FortiGate protecting your networks and FortiClient protecting the endpoints connected to it, your site-to-site VPN solution is secure from all angles.
