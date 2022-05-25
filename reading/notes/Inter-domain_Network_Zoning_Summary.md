**Title**: Comprehensive Inter-domain Network Zoning Architecture

**Source:** NDSS '21

**Authors:** Jonghoon Kwon, Claude Hähni, Patrick Bamert, Adrian Perrig

---

**Summary**

* MONDRIAN: all new network zoning architecture that ensures security of inter-domain communication on layer 3.

* Supporting heterogeneous layer 2 architectures and scalable cryptographic-key management and flexible security policy enforcement.

* Architecture
  
  * MONDRIAN flattens the current hierarchically-complex network zone topology into a collection of horizontal zones connected to a unified security gateway, called Zone Translation Point (TP), thus simplifying large enterprise networks.
  * Zones communicates with each other by TPs.
  * TPs are entry points for different network zones, enables some capabilities such as source identification and authorization and unauthorized access filter.

---

**Ideas**

* This network zoning architecture could be applied to military-industrial networks with some add-ons that implements classified management and zone-level network situation awareness(to prevent offensive lateral movement implemented by APTs)
