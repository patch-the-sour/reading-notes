# VirtualBox Network Settings
Networking is a crucial component of interactive computer operations.

One of the central focal ideas behind hardware virtualization is the possibility to use virtual machines in nearly all cases where physical computers can also be used. 

Virtual machines running on VirtualBox can be connected to different networks. 

VirtualBox provides multiple network modes for virtual machines.

## Virtual Network Adapters
Each VirtualBox VM can use up to eight virtual network adapters, each of which in turn is referred to as a network interface controller (NIC). 

Four virtual network adapters can be configured in the VirtualBox GUI (graphical user interface). 

VBoxManage is a command line management tool of VirtualBox that can be used for configuring all VirtualBox settings including VirtualBox network settings.

## Types of Virtual Network Adapters in VirtualBox

A virtual network adapter is a software-emulated physical device. 

There are six virtual adapter types that can be virtualized by VirtualBox.

AMD PCnet-PCI II (Am79C970A). 

This network adapter is based on AMD chip and can be used in many situations. 

As for Windows guests, this network adapter can be used for older Windows versions (such as Windows 2000) because newer Windows versions such as Windows 7, 8 and 10 do not contain a built-in driver for this adapter. 

Originally, the

Am79C970A

PCI device contained a single chip 10-Mbit controller and the DMA engine was integrated. 

This network adapter also supports AMD’s Magic Packet technology for remote wake-up.

AMD PCnet-FAST III (Am79C973). This virtualized network adapter is supported by almost all guest operating systems that can run on VirtualBox.

GRUB (the boot loader) can use this adapter for network boot. Similarly to the previous network adapter, this one is based AMD chip.

Intel PRO/1000 MT Desktop (82540EM). This adapter works perfectly with Windows Vista and newer Windows versions. 

The most of Linux distributions support this adapter as well.

Intel PRO/1000 T Server (82543GC). Windows XP recognizes this adapter without installing additional drivers.

Intel PRO/1000 MT Server (82545EM). This adapter model is useful to import OVF templates from other platforms and can facilitate import process.

Paravirtualized Network Adapter (virtio-net) is a special case. 

Instead of virtualizing networking hardware that is supported by most operating systems, a guest operating system must provide a special software interface for virtualized environments. 

This approach allows you to avoid the complexity of networking hardware emulating and, as a result, can improve network performance.

The industry standard virtIO networking drivers are supported by VirtualBox. 

VirtIO networking drivers are a part of the KVM project and are open-source. 

These drivers are available for Linux with kernel 2.6.25 or later, and Windows including older versions such as Windows 2000, XP and Vista.

## Jumbo frames support

VirtualBox provides limited support for jumbo frames (Ethernet frames that can carry packets which size is more than 1,500 bytes). 

If you need to use jumbo frames, select an Intel virtualized network adapter, and configure that adapter to work in bridged mode. 

AMD-based virtual networks adapters don’t support jumbo frames. 

If you try to enable jumbo frames for AMD-based virtual network adapters, jumbo frames will be dropped silently for input and output traffic. 

Jumbo frames are disabled by default.

## VirtualBox Network Modes

VirtualBox provides a long list of network modes, which is one of the most interesting features of VirtualBox network settings. 

Each virtual network adapter can be separately configured to operate in a different network mode. 

For example, you can set the NAT mode for the adapter 1 and the Host-only mode for the adapter 2. 

You can select the network mode in the Attached to drop-down menu.
