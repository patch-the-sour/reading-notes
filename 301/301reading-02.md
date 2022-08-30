# Domain Controller

Windows domains are typically used on large networks — corporate networks, school networks, and government networks. 

They aren’t something you’ll encounter at home unless you have a laptop provided by your employer or school.

A typical home computer is an isolated entity. 

You control the settings and user accounts on the computer.

A computer joined to a domain is different — these settings are controlled on a domain controller.

## What is a Domain?

Windows domains provide network administrators with a way to manage a large number of PCs and control them from one place. 

One or more servers — known as domain controllers — have control over the domain and the computers on it.

Domains are generally made up of computers on the same local network. 

However, computers joined to a domain can continue communicating with their domain controller over VPN or Internet connection. 

This allows businesses and schools to remotely manage laptops they provide to their employees and students.

When a computer is joined to a domain, it doesn’t use its own local user accounts. 

User accounts and passwords are managed on the domain controller. 

When you log into a computer on that domain, the computer authenticates your user account name and password with the domain controller. 

This means you can log in with the same username and password on any computer joined to the domain.

Network administrators can change group policy settings on the domain controller. 

Each computer on the domain will get these settings from the domain controller and they’ll override any local settings users specify on their PCs. 

All the settings are controlled from a single place. 

This also “locks down” the computers. 

You probably won’t be allowed to change many system settings on a computer joined to a domain.
 

## Is My Computer Part of a Domain?

You could set up a domain controller at home, but there’s no reason to do this unless you really want the experience. 

A computer at work or school, there’s a good chance your computer is part of a domain. 

A laptop provided to you by your work or school, it may also be part of a domain.

You can quickly check whether your computer is part of a domain or not. 

Open the Control Panel, click the System and Security category, and click System. 

Look under “Computer name, domain and workgroup settings” here. 

If you see “Domain”: followed by the name of a domain, your computer is joined to a domain.


## Workgroups vs. Domains

Every Windows computer not joined to a domain is part of a workgroup. 

A workgroup is a group of computers on the same local network. 

Unlike on a domain, no computer on a workgroup has control over any other computer — they’re all joined together as equals. 

A workgroup doesn’t require a password, either.

Workgroups were previously used for home file and printer sharing on previous versions of Windows. 

You can now use a homegroup to easily share files and printers between PCs at home. 

Workgroups have now been pushed to the background, so you shouldn’t need to worry about them.

Just leave the default workgroup name of WORKGROUP and set up homegroup file sharing.


## Joining or Leaving a Domain

If your computer is part of a domain, joining or leaving the domain won’t generally be your job. 

If your computer needs to be on a domain, it will already be on a domain when it’s handed to you. 

You’ll usually need the domain administrator’s permission to leave a domain, so people who sit down to use a domain-joined PC can’t just leave the domain. 

However, you can leave a domain if you have local administrator access on your PC. 

You won’t have administrator access if you’re using a locked-down PC, of course.

Click the Change Settings link next to “Computer name, domain and workgroup settings” in the System information window to access the System Properties window, which allows you to join or leave a domain.
