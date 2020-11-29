
**Title:** Stealthy Adversarial Perturbations Against Real-Time Video Classification Systems

**Source:** NDSS19

**Authors:** Shasha Li, Ajaya Neupane, Sujoy Paul, Chengyu Song, Srikanth V. Krishnamurthy, Amit K. Roy Chowdhury, Ananthram Swami

---

**Summary**

The paper proposed a method of attackting Real-Time video classification system. Compared with offline adversarial attack towards video classification system, attacking a Real-Time system may be faced with following problems:  
	- The efficiency problem: perturbations need to be generated in advance
	- The boundary problem: the sliding window of perturbations may not have the same size as the classification system.  
	- Target problem: how to keep non-targets unaffected.
The paper proposed a GAN-like architecture named C-DUP to solve these problems. The discriminator is a pre-trained C3D video classifier, while the generator is used to generate perturbations rather than perturbed videos. To achieve efficiency, all the perturbations are generated off-line and added to the original frames online. To solve the boundary problem, a post-process is added before perturbations adding to the clean frames. Meanwhile, a regularization term is added to the loss function in order to  control the scope of the perturbations.  
According to several experiments, C-DUP has a better performance on success rate and imperceptibility.
---

**Strengthens**  

- Real-time attack  
- Keepnon-targets unaffected  

---

**Weaknesses**  

- Not showing the adversarial features of GAN architecture.
