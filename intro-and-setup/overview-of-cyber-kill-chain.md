# Overview of Cyber Kill Chain

A framework developed by Lockheed Martin and great example of how to plan an attack as an ethical hacker. There is many ways to approach this framework.

- A framework of best practices for planning your countermeasures.
- Industry standard among security practitioners.

They have sound documentations and many examples on how it can be sed.

## Overview of framework

1. Reconnaissance:

- Who and where
- Harvesting emails, social sites, etc.

2. Weaponisation:

- Tool for the attack.

3. Delivery:

- How and where the bad code will be delivered.
- Email is typically the delivery mechanism.

4. Exploitation:

- Exploit the vulnerability found.

5. Installation:

- Tool installs what it needs to control the system.
- Malware is often used.

6. Control:

- The tool takes over part or the entire system.

7. Action:

- The hacker now has full control over the resources.
- Typically uses ransom strategies or pulls data.

Any attack starts with reconnaissance, figuring out who or where we could plan an attack. Example via emails, social sites where attacker can exploit vulnabilities in an app, system or network. Then attacker moves to weaponisation, building the tool or a code that will exploit the vulnerability and to be delivered to the resources we have gathered in the reconnaissance step. Next is the delivery step where an attcker will send a Trojan, virus, or whatever eapon he has programmed through emails, social communication channels, texts, etc. In the next steps, the attacker exploits the vulnerability he found in the reconnaissance stage through the communication channels. In step 5, the tool is installing malware or code in to the system, app or network to be able to exploit these resources. This is where user may have clicked on the link and a tool installed itself. Then the tool install would eventually take over and command a resource in question. A good example is how a hacker is able to control the tempature levels and the server environment and overheat the entire room, which eventually shut down the server hardware. Finally, once the resources control by the hacker, they take over and pulls whatever data they are after and holds ransom over the resources for thier own benefits. The goal of this framework is to determine what proper steps need to taken on a resources under threat at any of these stages, but also how the prevent the attacker
