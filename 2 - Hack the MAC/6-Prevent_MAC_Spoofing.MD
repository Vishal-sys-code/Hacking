MAC Spoofing can be a big problem on shared segment networks. However, the current generations of Ethernet switches are offering us a basis for defeating this kind of intrusion by offering is MAC locking.
<br>

## **MAC LOCKING**
* It is possible to lock a MAC address to a specific physical port on the switch.

* When MAC-locking locks a MAC/port combination, it prevents the MAC address from being used from any other port on the segment.

* This combined with static ARP and MAC/IP filters could totally eradicate the spoofing possibilities on a shared segment network.

* Expensive, managed switches allow port locking, but the disadvantage is the overhead cost.

## **Using ARP Tables**

* The use of static ARP table in combination with the routing table could prevent most of the shared-segment spoofing possibilities.
* Most OS by default do not check if a recieved IP datagram originated from a local MAC address matches the MAC addresses in the static ARP table or if the external datagram matches the MAC address of one the known network routers that have a valid route entry in the routing table.
* Unauthorized MAC address are therefore exposed, and the decision to take defensive action can then take place.

