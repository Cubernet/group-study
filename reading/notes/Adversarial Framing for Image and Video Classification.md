
**Title:** Adversarial Framing for Image and Video Classification

**Source:** AAAI2019

**Authors:** Konrad Zolna,Michal Zajac,Negar Rostamzadeh,Pedro O. Pinheiro

---

**Summary**  

This work present a simple method for attacking both image and video classifiers. 
- The method does not modify the original content of the input.
- Only adds a small border to surround it.
- The proposed attack is universal.
- While the network correctly identifies key objects for classification in unattacked images, it concentrates on the image borders when given adversarial input

The paper trains an AF framework to be used on image and video sets.

---

**Strengthens**  

- Not modify the original content of the input  
- The proposed attack is universal 

---

**Weaknesses**  

- Although the increase in the border has an obvious effect on the classifier, it will be recognized if there is manual sampling recognition

---

**Application scenario**

-Audio and video transmission that avoids sensitive detection (fidelity)

-Human machine recognition

---

**Questions**

-Why are the main points of the heat map distributed around?

-The size of the image and video has changed after adding the frame, how does the article deal with it?