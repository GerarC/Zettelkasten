---
title: Introduction to Networking
date: 07/03/2023
source: lesson 4.3
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs17 Copper Cable

## **Reference**
Introduction to Networking, Cisco; Lesson 3.2.

## **Quote**
> ## Characteristics of Copper Cabling
> Copper cabling is the most common type of cabling used in networks today. In fact, copper cabling is not just one type of cable. There are three different types of copper cabling that are each used in specific situations.
> 
> Networks use copper media because it is inexpensive, easy to install, and has low resistance to electrical current. However, copper media is limited by distance and signal interference.
> 
> Data is transmitted on copper cables as electrical pulses. A detector in the network interface of a destination device must receive a signal that can be successfully decoded to match the signal sent. However, the farther the signal travels, the more it deteriorates. This is referred to as signal attenuation. For this reason, all copper media must follow strict distance limitations as specified by the guiding standards.
> 
> The timing and voltage values of the electrical pulses are also susceptible to interference from two sources:
> 
> -   **Electromagnetic interference (EMI) or radio frequency interference (RFI) -** EMI and RFI signals can distort and corrupt the data signals being carried by copper media. Potential sources of EMI and RFI include radio waves and electromagnetic devices, such as fluorescent lights or electric motors.
> -   **Crosstalk** - Crosstalk is a disturbance caused by the electric or magnetic fields of a signal on one wire to the signal in an adjacent wire. In telephone circuits, crosstalk can result in hearing part of another voice conversation from an adjacent circuit. Specifically, when an electrical current flows through a wire, it creates a small, circular magnetic field around the wire, which can be picked up by an adjacent wire.
> 
> To counter the negative effects of EMI and RFI, some types of copper cables are wrapped in metallic shielding and require proper grounding connections.
> 
> To counter the negative effects of crosstalk, some types of copper cables have opposing circuit wire pairs twisted together, which effectively cancels the crosstalk.
> 
> The susceptibility of copper cables to electronic noise can also be limited using these recommendations:
> 
> -   Selecting the cable type or category most suited to a given networking environment
> -   Designing a cable infrastructure to avoid known and potential sources of interference in the building structure
> -   Using cabling techniques that include the proper handling and termination of the cables
> 
> ## Types of Copper Cabling
> ![[Pasted image 20230319115716.png]]
> 
> ## Unshielded twisted-pair (UTP)
> Unshielded twisted-pair (UTP) cabling is the most common networking media. UTP cabling, terminated with RJ-45 connectors, is used for interconnecting network hosts with intermediary networking devices, such as switches and routers.
> 
> In LANs, UTP cable consists of four pairs of color-coded wires that have been twisted together and then encased in a flexible plastic sheath that protects from minor physical damage. The twisting of wires helps protect against signal interference from other wires.
> 
> ## Shielded twisted-pair (STP)
> Shielded twisted-pair (STP) provides better noise protection than UTP cabling. However, compared to UTP cable, STP cable is significantly more expensive and difficult to install. Like UTP cable, STP uses an RJ-45 connector.
> 
> STP cables combine the techniques of shielding to counter EMI and RFI, and wire twisting to counter crosstalk. To gain the full benefit of the shielding, STP cables are terminated with special shielded STP data connectors. If the cable is improperly grounded, the shield may act as an antenna and pick up unwanted signals.
> 
> ## Coaxial cable
> Coaxial cable, or coax for short, gets its name from the fact that there are two conductors that share the same axis. As shown in the figure, coaxial cable consists of the following:
> 
> -   A copper conductor is used to transmit the electronic signals.
> -   A layer of flexible plastic insulation surrounds a copper conductor.
> -   The insulating material is surrounded in a woven copper braid, or metallic foil, that acts as the second wire in the circuit and as a shield for the inner conductor. This second layer, or shield, also reduces the amount of outside electromagnetic interference.
> -   The entire cable is covered with a cable jacket to prevent minor physical damage.
> 
> There are different types of connectors used with coax cable. The Bayonet Neill–Concelman (BNC), N type, and F type connectors are shown in the figure.
> 
> Although UTP cable has essentially replaced coaxial cable in modern Ethernet installations, the coaxial cable design is used in the following situations:
> 
> -   **Wireless installations** - Coaxial cables attach antennas to wireless devices. The coaxial cable carries radio frequency (RF) energy between the antennas and the radio equipment.
> -   **Cable internet installations** - Cable service providers provide internet connectivity to their customers by replacing portions of the coaxial cable and supporting amplification elements with fiber-optic cable. However, the wiring inside the customer's premises is still coax cable.

## **Summary**
Copper Cable:
- Is the most common type of cabling used in networks.
- There are three types of copper cable.
- It's commonly used because is cheaper, easy to setup and has low resistance to electrical current.
- Is limited by the distance and signal interference though.
- Destination device must receive a signal that can be decoded, but the farther the signal travels, the more it deteriorates, this is more known as signal attenuation.
- The timing and the voltage values of the pulses are also susceptible to: EMI and RFI, Crosstalk
- To counter EMI and RFI some types of copper cables are wrapped in metallic shielding.
- To counter crosstalk some types of copper cables have opposing circuit wire pairs twisted together which cancels it.
- The types of copper cables are: Unshielded twisted-pair (UTP), Shielded twited-pair (STP) and the coaxial cable.

Crosstalk:
- Is an interference created by the electromagnetic field of a wire over other wire.
