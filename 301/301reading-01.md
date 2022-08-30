# What’s the Difference Between Windows and Windows Server? 

Microsoft offers desktop and server versions of Windows. 

At first glance Windows 10 and Windows Server 2016 look similar, but each has different uses. 

Windows 10 excels at everyday use, while Windows Server manages many computers, files, and services.

## Windows 10 and Windows Server Share Similar Code

If you load up a clean copy of Windows 10 and Windows Server 2016, it would be easy to confuse the two at first. 

They can have the same desktop, same start button, and even the same task view button. 

They use the same kernel and can feasibly run the same software. You can, for instance, install Google Chrome or Microsoft Office on both.

But the similarities stop there. 

Microsoft designed Windows 10 for use as a desktop you sit in front of, and Windows Server as a server (it’s right there in the name) that runs services people access across a network. 

While Windows Server does have a desktop option, Microsoft recommends installing Windows Server without a Graphical User Interface (or removing it), leaving just a command line to work which reduces the overhead needed to run the server. 

This includes a push to choose Nano Server, which drops the GUI and local login capabilities in exchange for using far less space than the standard Server install.
 
## Windows Server Includes Server Software

If you have the GUI enabled, moments after Windows Server loads, a Server Manager program launches showing the first distinct difference in the two Operating Systems. Here you can add on server-specific features like Windows Deployment services, DHCP services, and Active Directory Domain Services. 

These features allow deployment of an OS remotely to other machines, the creation of static IP addresses for client machines, control of a network domain for joining other computers to a domain, and creating domain users. 

Features like these aren’t available for Windows 10 natively, although you could install third-party software like the Apache web server.

Also, Windows Server supports features like SMB Direct for faster file sharing, greater support for Resilient File System, the only way to get similar features without Server is to use Windows 10 Pro for Workstations.

Servers are designed to work in conjunction as well, so you may have one server fulfilling one or two of the roles above, and another server taking on other roles to spread the work.

Windows Server Supports Higher-End Hardware

Windows Server also supports more powerful hardware. 

While Windows 10 Pro has a max limit of 2 TB of RAM, Windows Server allows for 24 TB. 

A desktop user is unlikely even to consider such a large amount of RAM, but servers can make good use of their greater RAM capacity, between managing many users, computers, and potential VMs through Hyper-V. 

Windows 10 has a limit on processors as well. 

The Windows 10 Home edition only supports one physical CPU, while Windows 10 Pro supports two. 

Server 2016 supports up to 64 sockets. Similarly, a 32-bit copy of Windows 10 only supports 32 cores, and the 64-bit version supports 256 cores, but Windows Server has no limit for cores. 

To get something closer to these capabilities, you would have to use Windows 10 Pro for Workstations, which supports 4 CPUs and 6 TB of RAM.
 
## Windows Server is Locked Down

Much like the LTSB branch of Windows 10, Windows Server has several features removed. 

You won’t find Cortana, the Microsoft Store, Edge, or Timeline. 

Instead of Edge, Windows Server is still using Internet Explorer, and it is locked down to hinder normal web browsing. 

When downloading Google Chrome, we had to add exceptions for all of Google’s URLs to complete the download. 

Windows Server’s extra security makes its presence known at nearly any website visited through Internet Explorer. 

Windows Server doesn’t support signing in with a Microsoft account, so you can’t bring your settings to it from another PC. 

Instead, you’ll need to either sign in with a local account or a domain account. 

While Windows 10 Home is finally getting a pause updates feature, Windows Server can disable updates entirely through group policy (as can Windows 10 Enterprise and Windows LTSB).
 
## Windows 10 Is the Familiar Desktop Experience

While Windows 10 lacks server-specific features, it makes up for it in other areas. 

Windows 10 updates arrive faster and more often, it has capabilities like Timeline and Cortana that are missing on Windows Server, and it isn’t as locked down. 

Installing new software, especially downloaded from the internet, requires few hoops to jump through, and your preferences come with you from one machine to another if you sign in with a Microsoft Account.  

Additionally, Windows 10 has other features like Your Phone, Progressive Web Apps, and the Windows Subsystem for Linux. 

Some of these features rely on the Microsoft Store, which Windows Server does not have access to. 

And if you prefer, you can change Windows 10 to suit your needs and act more like Windows 7.

Windows Server is More Expensive, Too

And if you have Windows 7, 8, or 8.1 keys, you can install Windows 10 for free. 

Windows Server 2016 licenses aren’t easy to buy (they’re meant for business after all), and they’re expensive. 

If you are a business, depending on your size and needs a single license can cost between $500 and $6200. 

Most purchasers use a Volume License route instead. Windows Server is made primarily for businesses, so it is priced accordingly. 

If you’re considering a Windows OS for your personal computer, your best choice is Windows 10. 

It’s still possible to use Windows 7, 8, or 8.1 keys to activate it, and the features are tailor-made for home use. 

But if you want a Windows OS to manage other computers, at home or work, provide a File Server or a web server, then Windows Server is the obvious choice.
