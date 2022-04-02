**Title:**  Ripple A Programmable, Decentralized Link-Flooding Defense Against Adaptive Adversaries

**Source:**  Usenix Security '21

**Authors:**  Jiarong Xing, Wenqing Wu, Ang Chen

---

**Summary**

* Aiming at **Mitigating link-flooding attacks**: an enhanced version of traditional DDoS attacks, **creating congestions on critical links**.
  * (Attackers) Construct topology and identify critical links
  * Find a set of public servers (aka “decoy”) sharing the critical links
  * Flood the critical links by sending traffic to decoy servers
* Challenge -- Adaptive attacks: Change attack strategies dynamically to evade the deployed defense
* Shortages of SDN-based defense-- Cannot handle fast adaptive attacks
  * The SDN feedback loops require several RTTs
  * Adaptive adversaries can change attacks very fast
  * Software computation (e.g., for traffic engineering via ILP) is slow
* Solution: Decentralized construction of “panoramic” views
* Panorama:  Defines the global threat signals needed for the defense
* Different attacks require different panoramic views -- Solution: A language to specify needed panoramic views

---

**Strengthens**  

* Decentralized defenses in programmable switches
  * Significantly tighten the feedback loop
  * Inspect every packet, no need to sample traffic
  * Operate at hardware speeds, faster than SDN controllers
* Panorama: Defines the global threat signals needed for the defense
  * defense different link-flooding attacks
  * Panoramic view reconstruction proceeds in round
* Faster than centralized SDN-controller

---

**Weaknesses**  

* Reliability of spanning-tree protocol for local view exchange -- what if the switches cannot combine panorama?  
* Time consumption in the process of reconstruct panorama -- is it that fast, the whole process can be done in 0.5 ~ 1 RTT?

---

**Comments**  

assistant prof. Ang Chen has significant works in distributed systems and networks, the reconstruction of panorama depends on his early work listed below.

 *HULA: Scalable Load Balancing Using Programmable Data Planes*

*Contra: A Programmable System for Performance-aware Routing*
