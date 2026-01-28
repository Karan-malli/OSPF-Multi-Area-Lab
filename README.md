# Configure Multi-Area OSPF with route propagation.

Tech Stack: Cisco IOS, EVE-NG.

# Key Learnings:

**Multi-Area OSPF Architecture:** Designed a hierarchical routing domain with a Backbone (Area 0) and a Standard Area (Area 10) to optimize link-state database (LSDB) size and minimize LSA flooding.

**Route Propagation:** Configured default-information originate on the HQ router to dynamically inject a Gateway of Last Resort into the OSPF domain, simulating enterprise WAN internet access.

**Network Optimization:** Applied passive-interface commands on LAN-facing ports to prevent unnecessary OSPF Hello packets from reaching end-user devices, improving security and reducing chatter.

**LSA Analysis:** Verified routing tables to distinguish between Intra-Area (O), Inter-Area (O IA), and External Type 2 (O*E2) routes.
