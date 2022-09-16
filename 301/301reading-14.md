# What is a Port Scanner and How Does it Work?

A port scanner is a computer program that checks network ports for one of three possible statuses – open, closed, or filtered.

Port scanners are valuable tools in diagnosing network and connectivity issues. However, attackers use port scanners to detect possible access points for infiltration and to identify what kinds of devices you are running on the network, like firewalls, proxy servers or VPN servers.How Does a Port Scanner Operate?

A port scanner sends a network request to connect to a specific TCP or UDP port on a computer and records the response.
So what a port scanner does is send a packet of network data to a port to check the current status. If you wanted to check to see if your web server was operating correctly, you would check the status of port 80 on that server to make sure it was open and listening.
The status helps network engineers diagnose network issues or application connectivity issues, or helps attackers find possible ports to use for infiltration into your network.
What is a Port?
A port is a virtual location where networking communication starts and ends (in a nutshell). For a more in-depth explanation, we need to establish a little background information. There are two kinds of network ports on each computer (65,536 of each for a total of 131,082 network ports):
TCP and UDP
Each computer has an Internet Protocol (IP) address, which is how the network knows which computer to send packets to. If you send a packet to the IP address, the computer knows what port to route the packet to based on the application or packet contents. Each service running on the computer needs to “listen” on a designated port.
The first 1023 TCP ports are the well-known ports reserved for applications like FTP(21), HTTP(80), or SSH(22) and the Internet Assigned Numbers Authority (IANA) reserves these points to keep them standardized.
TCP ports 1024 – 49151 are available for use by services or applications, and you can register them with IANA, so they are considered semi-reserved. Ports 49152 and higher are free to use.
Port Scanning Basics
A port scanner sends a TCP or UDP network packet and asks the port about their current status. The three types of responses are below:
Open, Accepted: The computer responds and asks if there is anything it can do for you.
Closed, Not Listening: The computer responds that “This port is currently in use and unavailable at this time.”
Filtered, Dropped, Blocked: The computer doesn’t even bother to respond.
Port scans generally occur early in the cyber kill chain, during reconnaissance and intrusion. Attackers use port scans to detect targets with open and unused ports that they can repurpose for infiltration, command and control, and data exfiltration or discover what applications run on that computer to exploit a vulnerability in that application.
Port Scanning Techniques

Nmap is one of the most popular open-source port scanning tools available. Nmap provides a number of different port scanning techniques for different scenarios.
Ping Scanner
The simplest port scans are ping scans. A ping is an Internet Control Message Protocol (ICMP) echo request – you are looking for any ICMP replies, which indicates that the target is alive. A ping scan is an automated blast of many ICMP echo requests to different targets to see who responds. Ping scans aren’t technically port scanning techniques, as the best you can get back is that there is a computer on the other end, but it’s related and usually the first task before you do a port scan.
Administrators usually disable ICMP (ping) either on the firewall or on the router for external traffic, and they leave it open inside the network. It’s quick and easy to turn off this functionality and make it impossible to scout the network this way. However, ping is a useful troubleshooting tool, and turning it off makes tracking down network problems a little more difficult.
TCP Half Open
One of the more common and popular port scanning techniques is the TCP half-open port scan, sometimes referred to as an SYN scan. It’s a fast and sneaky scan that tries to find potential open ports on the target computer.
SYN packets request a response from a computer, and an ACK packet is a response. In a typical TCP transaction, there is an  SYN, an ACK from the service, and a third ACK confirming message received.
This scan is fast and hard to detect because it never completes the full TCP 3 way-handshake. The scanner sends an SYN message and just notes the SYN-ACK responses. The scanner doesn’t complete the connection by sending the final ACK: it leaves the target hanging.
Any SYN-ACK responses are possibly open ports. An RST(reset) response means the port is closed, but there is a live computer here. No responses indicate SYN is filtered on the network. An ICMP (or ping) no response also counts as a filtered response.
TCP half-open scans are the default scan in NMAP.
TCP Connect
This port scanning technique is basically the same as the TCP Half-Open scan, but instead of leaving the target hanging, the port scanner completes the TCP connection.
It’s not as popular a technique as the TCP half-open. First, you have to send one more packet per scan, which increases the amount of noise you are making on the network. Second, since you complete the target’s connection, you might trip an alarm that the half-open scan wouldn’t.
Target systems are more likely to log a full TCP connection, and intrusion detection systems (IDS) are similarly more likely to trigger alarms on several TCP connections from the same host.
The advantage of the TCP connect scan is that a user doesn’t need the same level of privileges to run as they do to run the Half-open scan. TCP connect scans use the connection protocols any user needs to have to connect to other systems.
UDP
UDP scans are slower than TCP scans, but there are plenty of exploitable UDP services that attackers can use, DNS exfiltration, for example. Defenders need to protect their UDP ports with the same voracity as their TCP ports.
UDP scans work best when you send a specific payload to the target. For example, if you want to know if a DNS server is up, you would send a DNS request. For other UDP ports, the packet is sent empty. An ICMP unreachable response means the port is closed or filtered. If there is a service running, you might get a UDP response, which means the port is open. No response could mean that the port is open or filtered.
One more logical use of a UDP scan is to send a DNS request to UDP port 53 and see if you get a DNS reply. If you do get a response, you know that there is a DNS server on that computer. A UDP scan can be useful to scout for active services that way, and the Nmap port scanner is preconfigured to send requests for many standard services.
Difference Between TCP and UDP
TCP and UDP are the two most common protocols in use for Internet Protocol (IP) networks. Transmission Control Protocol (TCP) is a nice orderly transaction protocol: TCP sends each packet in order, complete with error checking, verification, and a 3-way handshake to confirm each packet is successful.
UDP doesn’t have any error checking but tends to be faster. Live streaming and online video games often use UDP for this reason. UDP is a connectionless protocol, so programs that use UDP just send the data – and if you miss a packet, you will never get it again.
Stealth Scanning
Some port scans are easier to detect than others, so defenders need to know about these  TCP flags that allow attackers to make their port scans difficult to detect.
When you send a port scan with a packet and the FIN flag, you send the packet and not expecting a response. If you do get an RST, you can assume that the port is closed. If you get nothing back, that indicates the port is open. Firewalls are looking for SYN packets, so FIN packets slip through undetected.
The X-MAS scan sends a packet with the FIN, URG, and PUSH flags and expects an RST or no response, just like the FIN scan. There isn’t much practical use for this scan, but it does make the packet resemble a Christmas tree, so there is that.
You can also send packets with no flags, called a NULL packet, and the response is either an RST or nothing.
The good thing – for the hacker – about these scans is that they don’t usually show up in logs. More recent Intrusion Detection Software (IDS) and, of course, WireShark will catch these scans. The bad news is that if the target is a Microsoft OS, you will only see closed ports – but if you do find an open port, you can assume that it’s not a Windows machine. The most significant advantage of using these flags is that they can slip past firewalls, which makes the results more reliable.
Additional Scanning Techniques
The scans we discussed are the most common, but this is not an exhaustive list. Here are some more scans and the reasons to run them:
TCP ACK scan: to map firewall rulesets
TCP Window scan: can differentiate open ports from closed ports but only works on a minority of systems
–scanflags: for the advanced user that wants to send their custom TCP flags in a scan, you can do that in Nmap
Port Scanning Tools
Nmap
Solarwinds Port Scanner
Netcat
Advanced Port Scanner
NetScan Tools
How to Detect a Port Scan?

There are a few different techniques to detect port scans, which could be attempts to scan your network for vulnerabilities.
One is a dedicated port scan detector software application, like PortSentry or Scanlogd.
Netcat includes port scanning functionality as well as the ability to create a simple chat server or program different packets for testing purposes.
Intrusion detection systems (IDS) are another way to detect port scans. Look for an IDS that uses a wide variety of rules to detect the various kinds of port scans that aren’t merely threshold-based.
Why Should You Run a Port Scan?
You should run port scans proactively to detect and close all possible vulnerabilities that attackers might exploit.
Proactive port scanning is a good habit that you should repeat on a regular schedule. Also, review and audit all open ports to verify they are being used correctly and that any applications that do use open ports are secure and protected from known vulnerabilities.
Implications of Running a Port Scan
Here are some caveats to running port scans. Some services or computers might fail from a port scan. This is for internal systems more so than internet-facing systems, but it can happen.
Running port scans without authorization can be considered an aggressive action, and if you are on a shared network, you might scan a system that isn’t under your control, which isn’t good.
Port scans are a critical part of building a good defense from cyberattacks. Attackers are using port scans, as well. You need to beat them to the punch and close down possible attack vectors and make their lives as difficult as possible.
Protecting the perimeter is only part of the battle, however. You need to protect and monitor your data with the same vigilance you protect and monitor your ports. Varonis Data Security Platform helps you protect your data by building internal barriers to your most sensitive data and then monitoring all activity that could impact that data.
Check out our Live Cyber Attack lab to see how Varonis protects data from different attacks.
 

