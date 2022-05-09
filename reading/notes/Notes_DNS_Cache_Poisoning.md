**Title**: DNS Cache Poisoning Attack Reloaded: Revolutions with Side Channels

**Source:** CCS '20

**Authors**: Keyu Man, Zhiyun Qian, Zhongjie Wang, Xiaofeng Zheng, Youjun Huang, Haixin Duan

---

**Summary**

* An interaction between application level behavior and operating system level behavior, that is, Global rate limit for ICMP messages, may be abused to probe open UDP ports
* Develop novel methods to extend the attack window significantly, one of them again leveraging the rate limiting feature

**Method**

* An attacker triggers a request to DNS resolver and tries to prevent the resolver from receiving a legal response

* Probe the UDP port used by the resolver by side-channel, global rate limit for ICMP messages

* Simply injects a large number of spoofed DNS replies bruteforcing the TxIDs  

**Defense**

* Setting the timeout of DNS queries more aggressively

* A randomized ICMP global rate limit

* Additional randomness in both request and response

----

**Ideas**

* Network Infrastructure Defense (DNS, PKI, Switches, Routers, Data Center...)

* Cache(All kinds) check

* Security operation, Threats detection, Log analysis...
