# Computer Network | AAA (Authentication, Authorization and Accounting)

The administrator can take access to a router or a device through a console but it is very inconvenient if he is sitting far from the place of that device. So, eventually, he has to take remote access to that device. 

But as remote access will be available by using an IP address, therefore, it is possible that an unauthorized user can take access using that same IP address therefore for security measures, we have to put authentication. Also, the packets exchanged between the device should be encrypted so that any other person should not be able to capture that sensitive information. 

Therefore, a framework called AAA is used to provide that extra level of security. 

## AAA (Authentication, Authorization, Accounting) – 
AAA is a standard-based framework used to control who is permitted to use network resources (through authentication), what they are authorized to do (through authorization), and capture the actions performed while accessing the network (through accounting). 

 ## Authentication – 

The process by which it can be identified that the user, which wants to access the network resources, valid or not by asking some credentials such as username and password. Common methods are to put authentication on console port, AUX port, or vty lines. 

As network administrators, we can control how a user is authenticated if someone wants to access the network. 

Some of these methods include using the local database of that device (router) or sending authentication requests to an external server like the ACS server. 

To specify the method to be used for authentication, a default or customized authentication method list is used. 

 ## Authorization – 

It provides capabilities to enforce policies on network resources after the user has gained access to the network resources through authentication.

After the authentication is successful, authorization can be used to determine what resources is the user allowed to access and the operations that can be performed. 

For example, if a junior network engineer (who should not access all the resources) wants to access the device then the administrator can create a view that will allow particular commands only to be executed by the usehe commands that are allowed in the method list). 

The administrator can use the authorization method list to specify how the user is authorized to network resources i.e through a local database or ACS server. 

 ## Accounting – 
It provides means of monitoring and capturing the events done by the user while accessing the network resources. 

It even monitors how long the user has access to the network.

The administrator can create an accounting method list to specify what should be accounted for and to whom the accounting records should be sent. 
 
AAA implementation: AAA can be implemented by using the local database of the device or by using an external ACS server. 

 local database – If we want to use the local running configuration of the router or switch to implement AAA, we should create users first for authentication and provide privilege levels to users for Authorization. 
 
## ACS server – This is the common method used. 

An external ACS server is used (can be ACS device or software installed on Vmware) for AAA on which configuration on both router and ACS is required. 

The configuration includes creating a user, separate customized method list for authentication, Authorization, and Accounting. 

The client or Network Access Server (NAS) sends authentication requests to the ACS server and the server takes the decision to allow the user to access the network resource or not according to the credentials provided by the user. 
 
Note – If the ACS server fails to authenticate, the administrator should mention using the local database of the device as a backup, in the method list, to implement AAA.

thing because you didn't give it a useful "known good" password . So the server has no choice but to reject the request. The MSCHAP data might be correct, but the server has no way to know that. So it replies with a reject.
