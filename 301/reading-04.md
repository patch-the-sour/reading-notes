# What is Group Policy (GPO) and What Role Does It Play in Data Security
 
First things first, what is Group Policy? 

Group Policy is a feature of Windows that facilitates a wide variety of advanced settings that network administrators can use to control the working environment of users and computer accounts in Active Directory. 

It essentially provides a centralized place for administrators to manage and configure operating systems, applications and users’ settings.

Group Policies, when used correctly, can enable you to increase the security of user’s computers and help defend against both insider threats and external attacks.

In this blog, we will go through a detailed explanation of what Group Policies and GPOs are, and how system administrators can use them to help prevent data breaches.

What is a Group Policy Object (GPO)?

A Group Policy Object (GPO) is a group of settings that are created using the Microsoft Management Console (MMC) Group Policy Editor. 

GPOs can be associated with a single or numerous Active Directory containers, including sites, domains, or organizational units (OUs). 

The MMC allows users to create GPOs that define registry-based policies, security options, software installation and much more.

Active Directory applies GPOs in the same, logical order; local policies, site policies, domain policies and OU policies.

Note: GPOs that are in nested OUs work from the OU closest to the root first and outwards from there.

## Examples of GPOs

Group Policy Objects can be used in a number of ways that benefit security, many of which will be mentioned throughout this article. 

Below are a few more specific examples:

A Group Policy Object could be used to determine the home page that a user sees when they launch their internet browser after logging onto the domain.

Administrators can use GPOs to define which network connected printers appear on the list of available printers after a user in a specific Active Directory OU logs onto the domain.

Admins can also use GPOs to tweak a number of security protocols and practices, such as restricting internet connection options, programs and even screen time.

## How Are Group Policy Objects Processed?

The order at which GPOs are processed affects what settings are applied to the computer and user. 

The order that GPOs are processed is known as LSDOU, which stands for local, site, domain, organizational unit. 

The local computer policy is the first to be processed, followed by the site level to domain AD policies, then finally into organization units. 

If there happen to be conflicting policies in LSDOU, the last applied policies wins out.

## Should You Use Group Policy?

The short answer is yes. If you want to ensure that your data and your core IT infrastructure is set up in a secure way, then you probably need to understand how to properly use Group Policy.

It might surprise you to learn that Windows straight out-of-the-box isn’t exactly secure. 

There are numerous gaps in security, most of which can be addressed using GPOs. Without plugging these gaps, you leave yourself exposed to a plethora of security threats.

GPOs, for example, can help you implement a policy of least privilege where your users only have the permissions they require to do their job. 

They can do this through disabling Local Administrator rights globally in your network and grant admin privileges to individuals or groups based on their roles.

Group Policies can be used in numerous ways to bolster security, including disabling outdated protocols, preventing users from making certain changes and more. 

Let’s take a look at some of the benefits of Group Policy.

## The Benefits of Group Policy for Data Security

The benefits of Group Policy are not limited solely to security, there are a number of other advantages that are worth mentioning.

Password Policy: Many organizations are operating with relaxed password policies, with many users often having passwords set to never expire. 

Passwords that aren’t regularly rotated, are too simple or use common passphrases are at risk of being hacked through brute force. 

GPOs can be used to establish password length, complexity and other requirements.

Systems Management: GPOs can be used to simplify tasks that are at best mundane and at worst critically time consuming. 

You can save yourself hours and hours of time configuring the environment of new users and computers joining your domain by using GPOs to apply a standardized, universal one.

Health Checking: GPOs can be used to deploy software updates and system patches to ensure your environment is healthy and up to date against the latest security threats.

# What Is Active Directory and How Does It Work?

## The Limitations of Group Policy

There are a number of limitations that you need to be aware of before you start implementing them.

Firstly, the GPO editor isn’t the most user-friendly console that you’re likely to come across. 

A deep understanding of PowerShell will help make it easier to do all the GPO updates.

Speaking of GPO updates, they are undertaken randomly every 90 to 120 minutes whenever the computer gets rebooted. 

You can be specific with an update rate from 0 minutes up to 45 days. 

However, if you do specify 0 minutes, then by default the GPOs will attempt to update every 7 seconds, which is likely to choke your network with traffic.

GPOs are also not immune to cyberattacks. 

If an attacker wanted to change local GPOs on a computer in order to move laterally across the network, it would be very difficult to detect this without a Group Policy auditing and monitoring solution in place.

## How Lepide Helps

The Lepide’s Group Policy Auditing solution (part of Lepide Data Security Platform) will help you to get more visibility over the changes being made to your Group Policy Objects. 

Every time a critical change is made, Lepide will send the admin a real time alert and provide the option to roll back unwanted changes to their previous state, allowing admins to maintain a policy of least privilege and ensure the security policies of the organization remain intact.



