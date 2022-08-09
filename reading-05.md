# How Does the SMB Protocol Work?
“SMB works through a client-server approach, where a client makes specific requests and the server responds accordingly. This is known as a response-request protocol. This protocol facilitates file shares between networked computers.”

In other words I can share my files on my lab PC  from my personal computer if I'm running both on the same network.

Important SMB implementations include:

SMB 1.0 (1984)
‍ Created by IBM for file sharing in DOS. It introduced opportunistic locking as a client-side caching mechanism designed to reduce network traffic.

Samba (1992)
‍Samba is an open-source implementation of the SMB protocol and Microsoft Active Directory for Unix systems and Linux distributions that supports file sharing and print services, authentication and authorization, name resolution, and service announcements between Linux/Unix servers and Windows clients.

CIFS (1996)
‍Microsoft-developed SMB dialect that debuted in Windows 95 and added support for larger file sizes, transport directly over TCP/IP, symbolic links, and hard links.

NQ (1998)
‍NQ is a family of portable SMB client and server implementations developed by Visuality Systems. NQ is portable to non-Windows platforms such as Linux, iOS, and Android and supports SMB 3.1.1 dialect.

Netsmb (2004)
‍Netsmb is a family of in-kernel SMB client and server implementations in BSD operating systems.

SMB 2.0 (2006)
‍Released with Windows Vista and Windows Server 2008, it reduced chattiness to improve performance, enhance scalability and resiliency, and added support for WAN acceleration.

Tuxera SMB (2009)
‍Tuxera is also a proprietary SMB implementation that runs in either kernel or user-space.

Likewise (2009)
‍Likewise developed a CIFS/SMB implementation that provided a multiprotocol, identity-aware platform for network access to files in OEM storage products built on Linux/Unix based platforms.

SMB 2.1 (2010)
‍Introduced with Windows Server 2008 R2 and Windows 7. The client oplock leasing model replaced opportunistic locking to enhance caching and improve performance. It also introduced large maximum transmission unit (MTU) support and improved energy efficiency, enabling clients to open files from an SMB server to enter sleep mode.

SMB 3.0 (2012)
‍Debuted in Windows 8 and Windows Server 2012. It introduced several significant improvements to availability, performance, backup, security, and management.

MoSMB (2012)
‍MoSMB is a proprietary SMB implementation for Linux and other Unix-like systems, developed by Ryussi Technologies. It supports only SMB 2.x and SMB 3.x.‍

SMB 3.02 (2014)
‍Introduced in Windows 8.1 and Windows Server 2012 R2 and included performance updates and the ability to disable CIFS/SMB 1.0 support, including the removal of related binaries.

SMB 3.1.1 (2015)
‍ Released with Windows 10 and Windows Server 2016 and added support for advanced encryption, preauthentication integrity to prevent man-in-the-middle attacks and cluster dialect fencing.
 
## Are ports dangerous?

Typical Port numbers are 139 and 445

These 2 ports are not known for being dangerous but there are some known issues with exposing them. 

The most dangerous open ports are called wormable ports

SMB uses this type 

Opened by default 

Early versions of the SMB protocol were exploited during the WannaCry ransomware attack through a zero-day exploit called EternalBlue.

Use Upguard to protect your s***!!!!!
 
 
 
 
 

