# CIDR

CIDR notation is a way of representing a CIDR block, which is simply a range of IP addresses. 

When you create a network, the aim is to make sure there are enough available IP addresses for your use case, without making the CIDR block too large and wasteful.

An IPv4 (version 4 of IP) address is usually represented as four 8-bit decimal numbers or octets separated by dots, for example 127.0.0.1 (localhost on most systems). 

An 8-bit number when represented in the decimal system as opposed to binary has a range of 0–255.

So all four octets together add up to 32 bits, for a range of 0.0.0.0–255.255.255.255. 

In CIDR notation, this full range would be represented as 0.0.0.0/0. The final digit after the “/” represents how many bits make up the mask.
 
Say we have the CIDR block 10.0.0.0/16. What this effectively means is that half of the available bits for the mask are being used (32 x .5 = 16). 

Since masking is left-aligned, this gives us the range 10.0.0.0–10.0.255.255. 

As you can see, the first two octets (adding up to 16 bits) are masked and therefore do not change.

So this particular CIDR block gives us a range of 65,536 (or 2¹⁶) IP addresses.
 
If we wanted a smaller range (say half of the example just given) we would write 10.0.0.0/17, which would give us a range of 32,768 (or 2¹⁵) IP addresses.
 
As you can see, the larger the mask, the smaller the range. 

So 10.0.0.0/24 will give us a range of 10.0.0.0–10.0.0.255, which is just 256 (or 2⁸) IP addresses.
 
To get some practice playing around with these numbers and ranges, you can try this online CIDR calculator.
 
 
## What Is Network Segmentation and Why It Matters?

Locked doors behind locked doors discourage lazy threat actors and force them to look elsewhere. Therefore, there is no substitute for network segmentation when it comes to protecting your data.
 
Before we dive into what parts of the network to segment and how to do it, let’s level set with a definition.
 
## What Is Network Segmentation?

Network segmentation is when different parts of a computer network, or network zones, are separated by devices like bridges, switches and routers.

Network segmentation is a discipline and a framework that can be applied in the data center and on premises at your facilities.
 
Following are a few key benefits of network segmentation:
 
Limiting access privileges to those who truly need it

Protecting the network from widespread cyberattacks

Boosting network performance by reducing the number of users in specific zones

## Why Is Network Segmentation Important?

Firewalls have to do far too much these days: From real-time learning behavioral analytics all the way down to allowing necessary cookies for user experience.

Firewalls are very strict and follow established firewall rules, but they don’t do everything to protect your digital assets. 

What’s more, they can quickly become an outdated generation firewall. 

Your static IP addresses deserve to be protected, and they need backup beyond the front lines.
 
What happens when a threat actor penetrates the firewall via a phishing attempt, for example? Systems and services need to be isolated from one another to prevent a small breach from becoming a massive incident that leads to a data breach.
 
It’s one thing to have your smart lighting system compromised, but it’s another to have your customer data stolen. These are both virtualized functions for many businesses, but they are not nearly the same in terms of risk and liability.
 
If the business in the above example practices proper network segmentation and is hacked via their smart lighting system (this isn’t uncommon), the threat actor will find another obstacle.

Basically, it’s like turning a corner within a hedge maze to find a dead end: the threat actor will have to work their way backward and attempt to find other access points to the systems and data they are attempting to compromise. 

At this point, most cybercriminals are going to get discouraged and look for an easier target.
 
Whether you are running a virtual local area network (LAN) in the cloud or running an SDN-powered architecture, network segmentation will protect your assets.
 
## Types of Network Segmentation

So how do you know what network zones your organization needs? 

Think about the different types of users and data you have and who needs access to what.
 
Here are some examples of the types of network zones you may want to establish:
 
Users: Users are a network in and of themselves. Make sure you have correct access control on your users in your active directory.

Who needs the least privilege on your network? 

Privilege levels should be based on the user’s role in switching administration.

## How many admins have full access rights?

Make sure you have less than a handful. 

Access control lists are typically already a part of your active directory server.

The idea here is you are extending that practice to more components of your network.

Screened Subnet: This includes the subnetworks that expose externally facing systems – where the handshakes take place on your network. 

For example, it may include public-facing websites or other resources accessible via the internet.

You want to separate things that the public can access from your local area network (LAN) and internal data that needs to be protected.

## Guest Network: Guest Wi-Fi should be separate from the corporate Wi-Fi. 

This may seem like a no brainer, but I find a lot of smaller businesses never bother to set it up.

Even residential routers include this feature – you can easily set up a guest Wi-Fi in your home!

IT Workstations: This is the dev network zone for IT. 

It’s where your IT staff does non-administrative work, and it should be segmented for testing. 

I would also recommend giving IT a dedicated internet circuit for testing.

This can be a best effort, cheaper connection.

Don’t let anyone else in the company have network access to it aside from IT.

Servers by Department: Do department servers need to talk to one another? 

Create a public drive and a private drive, and then segment access on the private drives to those within each team or department.

This can limit the crawl of malware.

VoIP/Communications: Placing communications systems on their own network zone boosts performance and enhances quality. 

But in terms of network security, as communications move toward more APIs unique to your most used software as a service (SaaS) platforms, this network will become a more common attack surface.

Traditional Physical Security: Cameras, ID card scanners, etc., should be in their own network zone. 

This is not to be taken lightly, as the risk of a physical breach can be more harmful than a digital one. 

There are a number of real-world examples of this, including in 2017, the closed-circuit camera network in Washington, D.C., was hacked, leaving police cameras unable to function for three days.

Industrial Control Systems: HVAC, for example, like the non-segmented network compromised in the Target breach, should have two-factor authentication and be segmented.

Customer Databases: Due to compliance requirements, customer databases need to be secured more intently than, for instance, your print server. 

PCI-DSS, HIPAA, HiTRUST, FINRA, GDPR and other pieces of data legislation will determine the level of segmentation and cybersecurity that would be best practice in terms of implementation.

I would suggest configuring your intrusion detection and intrusion prevention system (IDS/IPS) tools to monitor your internal segmented network zones, just as you would set them to monitor your public-facing networks. Make sure to review your logs or work with an IT partner that will double your vigilance and act as an extra set of eyes.
 
Moving to the cloud is a legitimate strategy for network segmentation, but as I have written before, it doesn’t mean it’s easier or more secure.

Learn more on why your cloud solutions deserve zero-trust networking.
 
## Who Needs Network Segmentation?

Everyone running internal systems, whether physical or virtualized, to meet business needs network security.

The more complicated the architecture, the more important the need for segmentation. 

The only users who won’t need network segmentation are businesses that rely 100% on software as a service (SaaS) solutions or alternatively a business that operates offline/without IT services.
 
If you’re running a flat network to simplify the number of switches, you’re going to be an ideal target for a threat actor. 

While a flat network may save you time and money in the initial setup, you are leaving yourself open to being burned on the back end. 

That type of easy, lateral movement across the entire network will allow the bad guys to get wherever they want to go with little to no resistance.
 
Each customer will require a different level of segmentation.
 
There is no substitute for network segmentation. 

Micro-segmentation requires some time to initially set up, but the benefits highly outweigh the upfront time cost.
 
## Benefits of Network Segmentation

While safety and security are critical benefits unto themselves, the following are also excellent advantages when it comes to network segmentation:
 
Damage control and limitation in case of an incident via the smaller attack surface

Improved access control for external and internal network security

Reducing the attack plane and scope of compliance requirements related auditing

Improved performance with less congestion on network traffic

Better analytics around network monitoring, network access and network devices

Endpoint device protection, especially important as IoT devices become more common

Network segmentation can boost your overall security policy by limiting access privileges to those who need it, protecting the network from widespread cyberattacks and enabling better network performance by reducing the number of users in specific zones. 

