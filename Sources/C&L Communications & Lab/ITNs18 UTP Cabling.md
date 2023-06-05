---
title: Introduction to Networking
date: 07/03/2023
source: lesson 4.4
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs18 UTP Cabling

## **Reference**
Introduction to Networking, Cisco; Lesson 3.2.

## **Quote**
> ## Properties of UTP Cabling
> When used as a networking medium, UTP cabling consists of four pairs of color-coded copper wires that have been twisted together and then encased in a flexible plastic sheath. Its small size can be advantageous during installation.
> 
> UTP cable does not use shielding to counter the effects of EMI and RFI. Instead, cable designers have discovered other ways that they can limit the negative effect of crosstalk:
> 
> -   **Cancellation -** Designers now pair wires in a circuit. When two wires in an electrical circuit are placed close together, their magnetic fields are the exact opposite of each other. Therefore, the two magnetic fields cancel each other and also cancel out any outside EMI and RFI signals.
> -   **Varying the number of twists per wire pair -** To further enhance the cancellation effect of paired circuit wires, designers vary the number of twists of each wire pair in a cable. UTP cable must follow precise specifications governing how many twists or braids are permitted per meter (3.28 feet) of cable. Notice in the figure that the orange/orange white pair is twisted less than the blue/blue white pair. Each colored pair is twisted a different number of times.
> 
> UTP cable relies solely on the cancellation effect produced by the twisted wire pairs to limit signal degradation and effectively provide self-shielding for wire pairs within the network media.
> 
> ## UTP Cabling Standards and Connectors
> UTP cabling conforms to the standards established jointly by the TIA/EIA. Specifically, TIA/EIA-568 stipulates the commercial cabling standards for LAN installations and is the standard most commonly used in LAN cabling environments. Some of the elements defined are as follows:
> 
> -   Cable types
> -   Cable lengths
> -   Connectors
> -   Cable termination
> -   Methods of testing cable
> 
> The electrical characteristics of copper cabling are defined by the Institute of Electrical and Electronics Engineers (IEEE). IEEE rates UTP cabling according to its performance. Cables are placed into categories based on their ability to carry higher bandwidth rates. For example, Category 5 cable is used commonly in 100BASE-TX Fast Ethernet installations. Other categories include Enhanced Category 5 cable, Category 6, and Category 6a.
> 
> Cables in higher categories are designed and constructed to support higher data rates. As new gigabit speed Ethernet technologies are being developed and adopted, Category 5e is now the minimally acceptable cable type, with Category 6 being the recommended type for new building installations.
> 
> The figure shows three categories of UTP cable:
> 
> -   Category 3 was originally used for voice communication over voice lines, but later used for data transmission.
> -   Category 5 and 5e is used for data transmission. Category 5 supports 100Mbps and Category 5e supports 1000 Mbps
> -   Category 6 has an added separator between each wire pair to support higher speeds. Category 6 supports up to 10 Gbps.
> -   Category 7 also supports 10 Gbps.
> -   Category 8 supports 40 Gbps.
> 
> Some manufacturers are making cables exceeding the TIA/EIA Category 6a specifications and refer to these as Category 7.
> 
> ## Straight-through and Crossover UTP Cables
> Different situations may require UTP cables to be wired according to different wiring conventions. This means that the individual wires in the cable have to be connected in different orders to different sets of pins in the RJ-45 connectors.
> 
> The following are the main cable types that are obtained by using specific wiring conventions:
> 
> -   **Ethernet Straight-through -** The most common type of networking cable. It is commonly used to interconnect a host to a switch and a switch to a router.
> -   **Ethernet Crossover -** A cable used to interconnect similar devices. For example, to connect a switch to a switch, a host to a host, or a router to a router. However, crossover cables are now considered legacy as NICs use medium-dependent interface crossover (auto-MDIX) to automatically detect the cable type and make the internal connection.
> 
> **Note**: Another type of cable is a rollover cable, which is Cisco proprietary. It is used to connect a workstation to a router or switch console port.
> 
> Using a crossover or straight-through cable incorrectly between devices may not damage the devices, but connectivity and communication between the devices will not take place. This is a common error and checking that the device connections are correct should be the first troubleshooting action if connectivity is not achieved.
> 
> The figure identifies the individual wire pairs for the T568A and T568B standards.
> 
> ![[Pasted image 20230319120905.png]]

## **Summary**
UTP Cabling:
- Consist of four pairs of color-coded copper wires.
- The twisted pairs not only cancel the crosstalk, also cancel EMI and RFI signals.
- UTP cabling conforms to the standards established jointly by the TIA/EIA.
- UTP cables have been placed into categories based on their ability to carry higher bandwidth rates. For example, category 5 and 5e supports 100 Mbps and category 8 supports 40 Gbps.
- There are two types of UTP cables, Straight-through and Crossover.
- Straight-through is the most common type of networking cable and is used to connect different types of devices.
- Crossover is used to interconnect similar devices.