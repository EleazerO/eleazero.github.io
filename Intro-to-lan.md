---
layout: post
tags: [lan]
title: "Intro to Lan"
permalink: /intro_to_lan
---

## Task 1 - Local Area Network (LAN) Topologies ##

LAN stands for Local Area network and is a type of network that covers a small geographic location for example a house or office building  

Topology is another name for the format or structure of something in this case we would be referring to a network

### Types of Topology ##

**Star Topology**<br>
![Startopo](startopt.png)
Star topologies are devices that are individually connected through a **switch** or **hub** usually through a **router**


## What are they? ##


## Hubs ##
![hubs](hub.jpg)
Hub : Basic networking device that broadcasts internet and data to every computer or device it is connected to.


Think of a hub like a speakerphone in a conference call. When someone talks, everyone can hear it, whether it’s meant for them or not.
This means that all devices on the hub get the same data at the same time, and it slows things down if too many people (devices) are trying to talk


### Switches ##
![switch](switch.jpg)
Switch: A switch is also a networking device that has a similar functionality to a hub in that it connects multiple devices within a network. However, unlike a hub, a switch receives internet and data and sends it only to the specific device that requested or is the intended recipient, based on the device's MAC address.




A switch is more like a personal call. It knows exactly who the message is for and sends it directly to that person (device), instead of shouting it to everyone.
This makes things much faster and more efficient because it only sends the data where it needs to go, without bothering other devices.



**Router**
![router](router.jpg)
<br>
A router is a network device that sends internet to devices that are connected to it







<br>
<br>
<br>

**Bus topology**<br>
![bus](bustopt.png)
A bus topology operates by having a main cable (backbone cable/ethernet cable) that connects all devices in the network. When data is sent by a device, it travels along the main cable, and each device checks to see if the data is meant for it. If the data is addressed to a particular device, that device receives it. If it’s not, the other devices ignore the data. All devices share the same communication path, and only one device can send data at a time.

Imagine you have several houses on a street, and each house has a mailbox. Instead of each house having its own mailman, there’s one mailman who drives down the street with one big road connecting all the houses. When the mailman has a letter for someone, he drives along the road and stops at each house to check if the letter is for them


**Ring Topology**
![ring](ringtopt.png)
In a ring topology, every device (like computers or other hardware) is connected in a circle, forming a closed loop. Data travels around the ring in one direction (or sometimes both directions in some advanced versions). Each device in the network passes the data to the next one until it reaches its destination. There’s no central hub, and each device acts like a checkpoint that helps pass the data along.

Imagine a group of people sitting in a circle, passing a message or item hand to hand. If person A wants to send a note to person D, the note will go from A to B, then from B to C, and finally from C to D. Each person in the circle checks if the note is for them, and if not, they simply pass it along to the next person


## Practicals ##


**Question**<br>
What does LAN stand for


<details>
  <summary><strong>Click to see Answer</strong></summary>
  Local Area network
</details>

<br>
<br>

**Question**<br>
What is the verb given to the job routers perform (hint:This is the term given to deciding what route packets should take)


<details>
  <summary><strong>Click to see Answer</strong></summary>
  Routing
</details>


<br>
<br>



**Question**<br>
What device is used to centrally connect multiple devices on the local network and transmit data to the **correct location**?(hint: Something smarter than a hub/repeater.)

<details>
  <summary><strong>Click to see Answer</strong></summary>
  Switch
</details>

<br>
<br>

**Question**<br>
What topology is cost efficient to set up (hint:*** Topology)

<details>
  <summary><strong>Click to see Answer</strong></summary>
  Bus Topology
</details>

<br>
<br>

**Question**<br>
What topology is expensive to set up and maintain (hint**** Topology:)


<details><br>
  <summary><strong>Click to see Answer</strong></summary>
  Star topology
</details>

<br>
<br>

**Question**
Complete the interactive lab attached to this task. What is the flag given at the end?


![ring](ring1lab.png)
<br>
![ring](ring2lab.png)
<br>
![ring](ringlabc.png)
<br>
![ring](ring3lab.png)
<br>
![ring](buslab1.png)
<br>
![ring](buslab2.png)
<br>
![ring](buslab3.png)
<br>
![ring](buslab4.png)
<br>
![ring](buslab5.png)
<br>
![ring](buslab6.png)
<br>
![ring](buslab7.png)
<br>
![ring](starlab1.png)
<br>
![ring](starlab2.png)


<details><br>
  <summary><strong>Click to see Answer</strong></summary>
  THM{TOPOLOGY_FLAWS}
</details>



## Task 2 - A Primer on Subnetting  ##
![subnet](subnetting.png)
A ***subnet***  is the term given to splitting up a network into smaller, miniature networks within itself.

Imagine you live in a big apartment building. The entire building has one main address, but within that building, each apartment has its own  specific number. That apartment number helps mail carriers deliver packages to the right place.


So, if the main network is a large office building, a subnet might be a specific floor or department that handles its own internet traffic separately from other departments. This helps keep things organized and efficient.

 The name of this feature is called a  ***subnet mask***  that   helps define which part of an IP address is the network portion  and which part is the individual device - This organization makes it simpler to route data within networks and between different networks.

Subnet masks are used for 3 separate functions.

1. Network Address
2. Host address
3. Defult gateway  

Their Definitions in detail:
![si](subnetfeatues.png)




**Questions**
What is the technical term for dividing a network into smaller piece?



<details><br>
  <summary><strong>Click to see Answer</strong></summary>
  subnetting
</details>

<br>
<br>


**Questions**
How many bits are in a subnet mask(hint:his can be converted into 4 bytes)



<details><br>
  <summary><strong>Click to see Answer</strong></summary>
  32
</details>
<br>
<br>


**Questions**
What is the range of the section(octet) of a subnet mask?(hint:Smallest to largest)

<details><br>
  <summary><strong>Click to see Answer</strong></summary>
  0-255
</details>


<br>
<br>


**Questions**
What is adress is used to identify the start of a network (hint:******* Address)


<details><br>
  <summary><strong>Click to see Answer</strong></summary>
  Network adress
</details>

<br>
<br>


**Questions**
What is address is used to identify devices withing a network (hint:**** Address)


<details><br>
  <summary><strong>Click to see Answer</strong></summary>
  Host Address
</details>

<br>
<br>

**Questions**
What is the name used to identify the device responsible for sending data to another network?

<details><br>
  <summary><strong>Click to see Answer</strong></summary>
  Defult Gateway
</details>

<br>
<br>

##Task 3 ## The ARP protocol is used to make a device identifiable on a local network. It works by sending an ARP request to find out which device (IP address) has a specific MAC address. The device with the matching IP address responds with an ARP reply, stating that it has that corresponding MAC address. The result is stored in an ARP cache, which is used for future communications between devices on the local network. This allows devices to send and receive information accurately within the local network.



**Question**<br>
What does address resolution stand for


<details>
  <summary><strong>Click to see Answer</strong></summary>
  Addres Resolution Protocol
</details>

<br>
<br>





**Question**<br>
What category of ARP Packet asks for a device wether or not it has a specific IP address


<details>
  <summary><strong>Click to see Answer</strong></summary>
  Request
</details>

<br>
<br>


**Question**<br>
What category of ARP Packet asks a device whether or not it has a specific IP address?

<details>
  <summary><strong>Click to see Answer</strong></summary>
  MAC Address
</details>

<br>
<br>



**Question**<br>
What address is used as a logical identifier for a device on a network?

<details>
  <summary><strong>Click to see Answer</strong></summary>
  IP Address
</details>

<br>
<br>





## TASK 4 - The DHCP Protocol ##

![dhcp](DHCP Request.png)

In a nutshell this is used for assigning Public and private IP addresses temporarily to communicate  to a computer.  When a device connects to a network, if it has not already been manually assigned an IP address, it sends out a request ***(DHCP Discover)***
To see if any DHCP servers are on the network. The DHCP server then replies back with an IP address the device could uses ***(DHCP Offer)***.

The device then sends a reply confirming it wants the offered IP Address ***(DHCP Request)***, and then lastly, the DHCP server sends a reply acknowledging this has been completed, and the device can start using the IP Address ***(DHCP ACK)***.




**Question**<br>
What type of DHCP packet is used by a device to retrieve an IP address?(hint:DHCP ********)

<details>
  <summary><strong>Click to see Answer</strong></summary>
  DHCP Discover
</details>

<br>
<br>

**Question**<br>
What type of DHCP packet does a device send once it has been offered an IP address by the DHCP server0 ?(hint:DHCP Request)

<details>
  <summary><strong>Click to see Answer</strong></summary>
  DHCP Discover
</details>

<br>
<br>



**Question**<br>
Finally, what is the last DHCP packet that is sent to a device from a DHCP server?

<details>
  <summary><strong>Click to see Answer</strong></summary>
  DHCP ACK
</details>

<br>
<br>



## TASK 5 - Continue your learning to OSI Model ##